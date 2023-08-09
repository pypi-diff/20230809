# Comparing `tmp/flax-0.7.1.tar.gz` & `tmp/flax-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flax-0.7.1.tar", last modified: Tue Aug  1 01:59:13 2023, max compression
+gzip compressed data, was "flax-0.7.2.tar", last modified: Wed Aug  9 01:43:46 2023, max compression
```

## Comparing `flax-0.7.1.tar` & `flax-0.7.2.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.620033 flax-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 01:58:55.000000 flax-0.7.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.556033 flax-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.556033 flax-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-01 01:58:55.000000 flax-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.556033 flax-0.7.1/.github/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-01 01:58:55.000000 flax-0.7.1/.github/analytics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-08-01 01:58:55.000000 flax-0.7.1/.github/analytics/get_repo_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-01 01:58:55.000000 flax-0.7.1/.github/analytics/issue_activity_since_date.gql
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-01 01:58:55.000000 flax-0.7.1/.github/analytics/pr_data_query.gql
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 01:58:55.000000 flax-0.7.1/.github/analytics/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-01 01:58:55.000000 flax-0.7.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.556033 flax-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-01 01:58:55.000000 flax-0.7.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-01 01:58:55.000000 flax-0.7.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-01 01:58:55.000000 flax-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-01 01:58:55.000000 flax-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-01 01:58:55.000000 flax-0.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-01 01:58:55.000000 flax-0.7.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    20706 2023-08-01 01:58:55.000000 flax-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-08-01 01:58:55.000000 flax-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-01 01:59:13.620033 flax-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-08-01 01:58:55.000000 flax-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 01:58:55.000000 flax-0.7.1/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.556033 flax-0.7.1/dev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.556033 flax-0.7.1/dev/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-01 01:58:55.000000 flax-0.7.1/dev/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 01:58:55.000000 flax-0.7.1/dev/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-01 01:58:55.000000 flax-0.7.1/dev/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-01 01:58:55.000000 flax-0.7.1/dev/update_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.560033 flax-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 01:58:55.000000 flax-0.7.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 01:58:55.000000 flax-0.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-01 01:58:55.000000 flax-0.7.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.564033 flax-0.7.1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-01 01:58:55.000000 flax-0.7.1/docs/_ext/codediff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-01 01:58:55.000000 flax-0.7.1/docs/_ext/codediff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-01 01:58:55.000000 flax-0.7.1/docs/_ext/flax_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.552033 flax-0.7.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.564033 flax-0.7.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-01 01:58:55.000000 flax-0.7.1/docs/_static/css/flax_theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.552033 flax-0.7.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.564033 flax-0.7.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 01:58:55.000000 flax-0.7.1/docs/_templates/autosummary/flax_module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.564033 flax-0.7.1/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.core.frozen_dict.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.jax_utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.568033 flax-0.7.1/docs/api_reference/flax.linen/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/activation_functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/init_apply.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/initializers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/layers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/profiling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/spmd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/transformations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.linen/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.serialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.struct.rst
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.traceback_util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.training.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/flax.traverse_util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 01:58:55.000000 flax-0.7.1/docs/api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-01 01:58:55.000000 flax-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-08-01 01:58:55.000000 flax-0.7.1/docs/conf_sphinx_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-08-01 01:58:55.000000 flax-0.7.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.568033 flax-0.7.1/docs/developer_notes/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 01:58:55.000000 flax-0.7.1/docs/developer_notes/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-08-01 01:58:55.000000 flax-0.7.1/docs/developer_notes/lift.md
--rw-r--r--   0 runner    (1001) docker     (123)    22018 2023-08-01 01:58:55.000000 flax-0.7.1/docs/developer_notes/module_lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-01 01:58:55.000000 flax-0.7.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-08-01 01:58:55.000000 flax-0.7.1/docs/examples_community_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-01 01:58:55.000000 flax-0.7.1/docs/examples_core_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22579 2023-08-01 01:58:55.000000 flax-0.7.1/docs/examples_google_research_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 01:58:55.000000 flax-0.7.1/docs/examples_repositories_that_use_flax.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flax.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.568033 flax-0.7.1/docs/flip/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flip/0000-template.md
--rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flip/1009-optimizer-api.md
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flip/1777-default-dtype.md
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flip/2434-general-metadata.md
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flip/2974-kw-only-dataclasses.md
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-01 01:58:55.000000 flax-0.7.1/docs/flip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   102681 2023-08-01 01:58:55.000000 flax-0.7.1/docs/getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-08-01 01:58:55.000000 flax-0.7.1/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-08-01 01:58:55.000000 flax-0.7.1/docs/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.576033 flax-0.7.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/arguments.md
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/batch_norm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/convert_pytorch_to_flax.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/dropout.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/ensembling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/extracting_intermediates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39480 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/flax_basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/flax_basics.md
--rw-r--r--   0 runner    (1001) docker     (123)    63884 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/flax_on_pjit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/flax_on_pjit.md
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/full_eval.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/haiku_migration_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index_converting_and_upgrading.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index_data_preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index_flax_fundamentals.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index_model_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index_parallel_training.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/index_training_techniques.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38261 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/jax_for_the_impatient.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/jax_for_the_impatient.md
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/linen_upgrade_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/lr_schedule.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/model_surgery.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/model_surgery.md
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/optax_update_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/orbax_upgrade_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/regular_dict_upgrade_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/rnncell_upgrade_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/setup_or_nncompact.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/state_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/transfer_learning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/transfer_learning.md
--rw-r--r--   0 runner    (1001) docker     (123)    52447 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/use_checkpointing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-08-01 01:58:55.000000 flax-0.7.1/docs/guides/use_checkpointing.md
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-01 01:58:55.000000 flax-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-08-01 01:58:55.000000 flax-0.7.1/docs/mission.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.576033 flax-0.7.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/flax_sharp_bits.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/flax_sharp_bits.md
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/full_eval.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/full_eval.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/linen_intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/linen_intro.md
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/optax_update_guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/optax_update_guide.md
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/orbax_upgrade_guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/orbax_upgrade_guide.md
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/state_params.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-08-01 01:58:55.000000 flax-0.7.1/docs/notebooks/state_params.md
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-01 01:58:55.000000 flax-0.7.1/docs/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-08-01 01:58:55.000000 flax-0.7.1/docs/philosophy.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 01:58:55.000000 flax-0.7.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.576033 flax-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 01:58:55.000000 flax-0.7.1/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.576033 flax-0.7.1/examples/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-08-01 01:58:55.000000 flax-0.7.1/examples/cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-01 01:58:55.000000 flax-0.7.1/examples/cloud/launch_gce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-01 01:58:55.000000 flax-0.7.1/examples/cloud/startup_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.580033 flax-0.7.1/examples/imagenet/
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.580033 flax-0.7.1/examples/imagenet/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/configs/fake_data_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/configs/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/configs/v100_x8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/configs/v100_x8_mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)   294627 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/imagenet.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/imagenet_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/imagenet_fake_data_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-01 01:58:55.000000 flax-0.7.1/examples/imagenet/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.580033 flax-0.7.1/examples/linen_design_test/
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/attention_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/mlp_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/mlp_inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/mlp_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/tied_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-01 01:58:55.000000 flax-0.7.1/examples/linen_design_test/weight_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.584033 flax-0.7.1/examples/lm1b/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.584033 flax-0.7.1/examples/lm1b/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/input_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/temperature_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/temperature_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-01 01:58:55.000000 flax-0.7.1/examples/lm1b/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.584033 flax-0.7.1/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.584033 flax-0.7.1/examples/mnist/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    99011 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/mnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/mnist_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-01 01:58:55.000000 flax-0.7.1/examples/mnist/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.588033 flax-0.7.1/examples/nlp_seq/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-01 01:58:55.000000 flax-0.7.1/examples/nlp_seq/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-01 01:58:55.000000 flax-0.7.1/examples/nlp_seq/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-01 01:58:55.000000 flax-0.7.1/examples/nlp_seq/input_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-01 01:58:55.000000 flax-0.7.1/examples/nlp_seq/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 01:58:55.000000 flax-0.7.1/examples/nlp_seq/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-08-01 01:58:55.000000 flax-0.7.1/examples/nlp_seq/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.588033 flax-0.7.1/examples/ogbg_molpcba/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.592033 flax-0.7.1/examples/ogbg_molpcba/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/configs/default_graph_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/configs/hparam_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/configs/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/input_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)  1111228 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/ogbg_molpcba.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/ogbg_molpcba_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ogbg_molpcba/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.592033 flax-0.7.1/examples/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.592033 flax-0.7.1/examples/ppo/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/ppo_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/ppo_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/ppo_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/seed_rl_atari_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-01 01:58:55.000000 flax-0.7.1/examples/ppo/test_episodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.592033 flax-0.7.1/examples/seq2seq/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/seq2seq.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-01 01:58:55.000000 flax-0.7.1/examples/seq2seq/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.596033 flax-0.7.1/examples/sst2/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/build_vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.596033 flax-0.7.1/examples/sst2/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/configs/default.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9834 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/input_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/sst2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/train_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   117898 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/vocab.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4407 2023-08-01 01:58:55.000000 flax-0.7.1/examples/sst2/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.596033 flax-0.7.1/examples/vae/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/reconstruction.png
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.596033 flax-0.7.1/examples/vae/results/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/results/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    43139 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/sample.png
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-01 01:58:55.000000 flax-0.7.1/examples/vae/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.600033 flax-0.7.1/examples/wmt/
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/bleu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.600033 flax-0.7.1/examples/wmt/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/input_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23417 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-01 01:58:55.000000 flax-0.7.1/examples/wmt/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.600033 flax-0.7.1/flax/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 01:58:55.000000 flax-0.7.1/flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-01 01:58:55.000000 flax-0.7.1/flax/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.604033 flax-0.7.1/flax/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/axes_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/flax_functional_engine.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/frozen_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    55971 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/lift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.604033 flax-0.7.1/flax/core/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/nn/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/nn/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/nn/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/partial_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    35668 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/tracers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-01 01:58:55.000000 flax-0.7.1/flax/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-08-01 01:58:55.000000 flax-0.7.1/flax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-01 01:58:55.000000 flax-0.7.1/flax/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-08-01 01:58:55.000000 flax-0.7.1/flax/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-08-01 01:58:55.000000 flax-0.7.1/flax/jax_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.608033 flax-0.7.1/flax/linen/
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.608033 flax-0.7.1/flax/linen/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/experimental/layers_with_named_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/kw_only_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    33001 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    88743 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    19344 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/partitioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    20309 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    59542 2023-08-01 01:58:55.000000 flax-0.7.1/flax/linen/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.608033 flax-0.7.1/flax/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-01 01:58:55.000000 flax-0.7.1/flax/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-08-01 01:58:55.000000 flax-0.7.1/flax/metrics/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.608033 flax-0.7.1/flax/oss/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 01:58:55.000000 flax-0.7.1/flax/oss/ .git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 01:58:55.000000 flax-0.7.1/flax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-08-01 01:58:55.000000 flax-0.7.1/flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-08-01 01:58:55.000000 flax-0.7.1/flax/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.608033 flax-0.7.1/flax/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-01 01:58:55.000000 flax-0.7.1/flax/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-08-01 01:58:55.000000 flax-0.7.1/flax/testing/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-01 01:58:55.000000 flax-0.7.1/flax/traceback_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.612033 flax-0.7.1/flax/training/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/dynamic_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/lr_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/orbax_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/prefetch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-01 01:58:55.000000 flax-0.7.1/flax/training/train_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-01 01:58:55.000000 flax-0.7.1/flax/traverse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 01:58:55.000000 flax-0.7.1/flax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.604033 flax-0.7.1/flax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-01 01:59:13.000000 flax-0.7.1/flax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-08-01 01:59:13.000000 flax-0.7.1/flax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:59:13.000000 flax-0.7.1/flax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 01:59:13.000000 flax-0.7.1/flax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 01:59:13.000000 flax-0.7.1/flax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.612033 flax-0.7.1/images/
--rw-r--r--   0 runner    (1001) docker     (123)    80407 2023-08-01 01:58:55.000000 flax-0.7.1/images/flax_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-08-01 01:58:55.000000 flax-0.7.1/images/flax_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-08-01 01:58:55.000000 flax-0.7.1/images/flax_logo_250px.png
--rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-08-01 01:58:55.000000 flax-0.7.1/images/flax_logo_500px.png
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-08-01 01:58:55.000000 flax-0.7.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-08-01 01:58:55.000000 flax-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:59:13.620033 flax-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.616033 flax-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-08-01 01:58:55.000000 flax-0.7.1/tests/checkpoints_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-01 01:58:55.000000 flax-0.7.1/tests/colab_tpu_jax_version.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.616033 flax-0.7.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/core_frozen_dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/core_lift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/core_meta_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/core_scope_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.616033 flax-0.7.1/tests/core/design/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_auto_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_big_resnets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_custom_vjp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_flow_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_scan_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_tied_autoencoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_vmap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-01 01:58:55.000000 flax-0.7.1/tests/core/design/core_weight_std_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 01:58:55.000000 flax-0.7.1/tests/download_dataset_metadata.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-01 01:58:55.000000 flax-0.7.1/tests/early_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 01:58:55.000000 flax-0.7.1/tests/import_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-08-01 01:58:55.000000 flax-0.7.1/tests/io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-01 01:58:55.000000 flax-0.7.1/tests/jax_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:59:13.620033 flax-0.7.1/tests/linen/
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/initializers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/kw_only_dataclasses_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_activation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_combinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_dtypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_meta_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    65084 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_module_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    55533 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/linen_transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/partitioning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/summary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-01 01:58:55.000000 flax-0.7.1/tests/linen/toplevel_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3960 2023-08-01 01:58:55.000000 flax-0.7.1/tests/run_all_tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-08-01 01:58:55.000000 flax-0.7.1/tests/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-01 01:58:55.000000 flax-0.7.1/tests/struct_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-08-01 01:58:55.000000 flax-0.7.1/tests/tensorboard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-01 01:58:55.000000 flax-0.7.1/tests/traceback_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-08-01 01:58:55.000000 flax-0.7.1/tests/traverse_util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.499148 flax-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-09 01:43:27.000000 flax-0.7.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.447147 flax-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.447147 flax-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-09 01:43:27.000000 flax-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.447147 flax-0.7.2/.github/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-09 01:43:27.000000 flax-0.7.2/.github/analytics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-08-09 01:43:27.000000 flax-0.7.2/.github/analytics/get_repo_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-09 01:43:27.000000 flax-0.7.2/.github/analytics/issue_activity_since_date.gql
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-09 01:43:27.000000 flax-0.7.2/.github/analytics/pr_data_query.gql
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-09 01:43:27.000000 flax-0.7.2/.github/analytics/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-09 01:43:27.000000 flax-0.7.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.447147 flax-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-09 01:43:27.000000 flax-0.7.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-09 01:43:27.000000 flax-0.7.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-09 01:43:27.000000 flax-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-09 01:43:27.000000 flax-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-09 01:43:27.000000 flax-0.7.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-09 01:43:27.000000 flax-0.7.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-08-09 01:43:27.000000 flax-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-08-09 01:43:27.000000 flax-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-09 01:43:46.495148 flax-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-08-09 01:43:27.000000 flax-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-09 01:43:27.000000 flax-0.7.2/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.447147 flax-0.7.2/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.447147 flax-0.7.2/dev/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-09 01:43:27.000000 flax-0.7.2/dev/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-09 01:43:27.000000 flax-0.7.2/dev/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-09 01:43:27.000000 flax-0.7.2/dev/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-09 01:43:27.000000 flax-0.7.2/dev/update_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.451147 flax-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-09 01:43:27.000000 flax-0.7.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-09 01:43:27.000000 flax-0.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-09 01:43:27.000000 flax-0.7.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.451147 flax-0.7.2/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-09 01:43:27.000000 flax-0.7.2/docs/_ext/codediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-09 01:43:27.000000 flax-0.7.2/docs/_ext/codediff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-09 01:43:27.000000 flax-0.7.2/docs/_ext/flax_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.443147 flax-0.7.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.451147 flax-0.7.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-09 01:43:27.000000 flax-0.7.2/docs/_static/css/flax_theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.443147 flax-0.7.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.451147 flax-0.7.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-09 01:43:27.000000 flax-0.7.2/docs/_templates/autosummary/flax_module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.455147 flax-0.7.2/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.core.frozen_dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.jax_utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.455147 flax-0.7.2/docs/api_reference/flax.linen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/activation_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/init_apply.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/initializers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/layers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/profiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/spmd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.linen/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.struct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.traceback_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/flax.traverse_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-09 01:43:27.000000 flax-0.7.2/docs/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-08-09 01:43:27.000000 flax-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-08-09 01:43:27.000000 flax-0.7.2/docs/conf_sphinx_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-08-09 01:43:27.000000 flax-0.7.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.455147 flax-0.7.2/docs/developer_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-09 01:43:27.000000 flax-0.7.2/docs/developer_notes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-08-09 01:43:27.000000 flax-0.7.2/docs/developer_notes/lift.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22018 2023-08-09 01:43:27.000000 flax-0.7.2/docs/developer_notes/module_lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-09 01:43:27.000000 flax-0.7.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-08-09 01:43:27.000000 flax-0.7.2/docs/examples_community_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-09 01:43:27.000000 flax-0.7.2/docs/examples_core_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22579 2023-08-09 01:43:27.000000 flax-0.7.2/docs/examples_google_research_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-09 01:43:27.000000 flax-0.7.2/docs/examples_repositories_that_use_flax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flax.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.455147 flax-0.7.2/docs/flip/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flip/0000-template.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flip/1009-optimizer-api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flip/1777-default-dtype.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flip/2434-general-metadata.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flip/2974-kw-only-dataclasses.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-09 01:43:27.000000 flax-0.7.2/docs/flip/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   102681 2023-08-09 01:43:27.000000 flax-0.7.2/docs/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-08-09 01:43:27.000000 flax-0.7.2/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-08-09 01:43:27.000000 flax-0.7.2/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.459147 flax-0.7.2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/arguments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/batch_norm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/convert_pytorch_to_flax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/dropout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/ensembling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/extracting_intermediates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39480 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/flax_basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/flax_basics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    63884 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/flax_on_pjit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/flax_on_pjit.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/full_eval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/haiku_migration_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index_converting_and_upgrading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index_data_preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index_flax_fundamentals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index_model_inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index_parallel_training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/index_training_techniques.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38261 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/jax_for_the_impatient.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/jax_for_the_impatient.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/linen_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/lr_schedule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/model_surgery.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/model_surgery.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/optax_update_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/orbax_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/regular_dict_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/rnncell_upgrade_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/setup_or_nncompact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/state_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/transfer_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (123)    52447 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/use_checkpointing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26556 2023-08-09 01:43:27.000000 flax-0.7.2/docs/guides/use_checkpointing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-09 01:43:27.000000 flax-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-08-09 01:43:27.000000 flax-0.7.2/docs/mission.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.463147 flax-0.7.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/flax_sharp_bits.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/flax_sharp_bits.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/full_eval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/full_eval.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/linen_intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/linen_intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/optax_update_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/optax_update_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/orbax_upgrade_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/orbax_upgrade_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/state_params.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-08-09 01:43:27.000000 flax-0.7.2/docs/notebooks/state_params.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-09 01:43:27.000000 flax-0.7.2/docs/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-08-09 01:43:27.000000 flax-0.7.2/docs/philosophy.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-09 01:43:27.000000 flax-0.7.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.463147 flax-0.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-09 01:43:27.000000 flax-0.7.2/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.463147 flax-0.7.2/examples/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-08-09 01:43:27.000000 flax-0.7.2/examples/cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-09 01:43:27.000000 flax-0.7.2/examples/cloud/launch_gce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-09 01:43:27.000000 flax-0.7.2/examples/cloud/startup_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.463147 flax-0.7.2/examples/imagenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.467147 flax-0.7.2/examples/imagenet/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/configs/fake_data_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/configs/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/configs/v100_x8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/configs/v100_x8_mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)   294627 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/imagenet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/imagenet_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/imagenet_fake_data_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-09 01:43:27.000000 flax-0.7.2/examples/imagenet/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.467147 flax-0.7.2/examples/linen_design_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/attention_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/mlp_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/mlp_inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/mlp_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/tied_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-09 01:43:27.000000 flax-0.7.2/examples/linen_design_test/weight_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.467147 flax-0.7.2/examples/lm1b/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.467147 flax-0.7.2/examples/lm1b/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/temperature_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/temperature_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-09 01:43:27.000000 flax-0.7.2/examples/lm1b/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.467147 flax-0.7.2/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.467147 flax-0.7.2/examples/mnist/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99011 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/mnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/mnist_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-09 01:43:27.000000 flax-0.7.2/examples/mnist/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.471147 flax-0.7.2/examples/nlp_seq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-09 01:43:27.000000 flax-0.7.2/examples/nlp_seq/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-09 01:43:27.000000 flax-0.7.2/examples/nlp_seq/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-09 01:43:27.000000 flax-0.7.2/examples/nlp_seq/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-09 01:43:27.000000 flax-0.7.2/examples/nlp_seq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-09 01:43:27.000000 flax-0.7.2/examples/nlp_seq/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-08-09 01:43:27.000000 flax-0.7.2/examples/nlp_seq/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.471147 flax-0.7.2/examples/ogbg_molpcba/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.471147 flax-0.7.2/examples/ogbg_molpcba/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/configs/default_graph_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/configs/hparam_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/configs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1111228 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/ogbg_molpcba.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/ogbg_molpcba_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ogbg_molpcba/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.475147 flax-0.7.2/examples/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.475147 flax-0.7.2/examples/ppo/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/ppo_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/ppo_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/ppo_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/seed_rl_atari_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-09 01:43:27.000000 flax-0.7.2/examples/ppo/test_episodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.475147 flax-0.7.2/examples/seq2seq/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/seq2seq.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-09 01:43:27.000000 flax-0.7.2/examples/seq2seq/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.475147 flax-0.7.2/examples/sst2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/build_vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.479147 flax-0.7.2/examples/sst2/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/configs/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9834 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/sst2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/train_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117898 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/vocab.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4407 2023-08-09 01:43:27.000000 flax-0.7.2/examples/sst2/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.479147 flax-0.7.2/examples/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/reconstruction.png
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.479147 flax-0.7.2/examples/vae/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/results/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    43139 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/sample.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-09 01:43:27.000000 flax-0.7.2/examples/vae/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.479147 flax-0.7.2/examples/wmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/bleu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.479147 flax-0.7.2/examples/wmt/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/input_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23417 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-09 01:43:27.000000 flax-0.7.2/examples/wmt/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.483147 flax-0.7.2/flax/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-09 01:43:27.000000 flax-0.7.2/flax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-09 01:43:27.000000 flax-0.7.2/flax/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.483147 flax-0.7.2/flax/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/axes_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/flax_functional_engine.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/frozen_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55971 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/lift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.483147 flax-0.7.2/flax/core/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/nn/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/nn/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/partial_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35668 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/tracers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-09 01:43:27.000000 flax-0.7.2/flax/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-08-09 01:43:27.000000 flax-0.7.2/flax/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-09 01:43:27.000000 flax-0.7.2/flax/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-08-09 01:43:27.000000 flax-0.7.2/flax/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-08-09 01:43:27.000000 flax-0.7.2/flax/jax_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.487147 flax-0.7.2/flax/linen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.487147 flax-0.7.2/flax/linen/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/experimental/layers_with_named_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/kw_only_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33001 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88774 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19344 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20309 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59542 2023-08-09 01:43:27.000000 flax-0.7.2/flax/linen/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.487147 flax-0.7.2/flax/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-09 01:43:27.000000 flax-0.7.2/flax/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-08-09 01:43:27.000000 flax-0.7.2/flax/metrics/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.487147 flax-0.7.2/flax/oss/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-09 01:43:27.000000 flax-0.7.2/flax/oss/ .git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-09 01:43:27.000000 flax-0.7.2/flax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-08-09 01:43:27.000000 flax-0.7.2/flax/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-08-09 01:43:27.000000 flax-0.7.2/flax/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.487147 flax-0.7.2/flax/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-09 01:43:27.000000 flax-0.7.2/flax/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-08-09 01:43:27.000000 flax-0.7.2/flax/testing/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-09 01:43:27.000000 flax-0.7.2/flax/traceback_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.491147 flax-0.7.2/flax/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/dynamic_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/lr_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/orbax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/prefetch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-09 01:43:27.000000 flax-0.7.2/flax/training/train_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-09 01:43:27.000000 flax-0.7.2/flax/traverse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-09 01:43:27.000000 flax-0.7.2/flax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.483147 flax-0.7.2/flax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-09 01:43:46.000000 flax-0.7.2/flax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-08-09 01:43:46.000000 flax-0.7.2/flax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:43:46.000000 flax-0.7.2/flax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-09 01:43:46.000000 flax-0.7.2/flax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-09 01:43:46.000000 flax-0.7.2/flax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.491147 flax-0.7.2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    80407 2023-08-09 01:43:27.000000 flax-0.7.2/images/flax_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-08-09 01:43:27.000000 flax-0.7.2/images/flax_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-08-09 01:43:27.000000 flax-0.7.2/images/flax_logo_250px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-08-09 01:43:27.000000 flax-0.7.2/images/flax_logo_500px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-08-09 01:43:27.000000 flax-0.7.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-08-09 01:43:27.000000 flax-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:43:46.499148 flax-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.491147 flax-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-08-09 01:43:27.000000 flax-0.7.2/tests/checkpoints_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-09 01:43:27.000000 flax-0.7.2/tests/colab_tpu_jax_version.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.491147 flax-0.7.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/core_frozen_dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/core_lift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/core_meta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/core_scope_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.495148 flax-0.7.2/tests/core/design/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_auto_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_big_resnets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_custom_vjp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_flow_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_scan_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_tied_autoencoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_vmap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-09 01:43:27.000000 flax-0.7.2/tests/core/design/core_weight_std_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-09 01:43:27.000000 flax-0.7.2/tests/download_dataset_metadata.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-09 01:43:27.000000 flax-0.7.2/tests/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-09 01:43:27.000000 flax-0.7.2/tests/import_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-08-09 01:43:27.000000 flax-0.7.2/tests/io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-09 01:43:27.000000 flax-0.7.2/tests/jax_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:43:46.495148 flax-0.7.2/tests/linen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/kw_only_dataclasses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_combinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_meta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65084 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_module_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55533 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/linen_transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/partitioning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/summary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-09 01:43:27.000000 flax-0.7.2/tests/linen/toplevel_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3960 2023-08-09 01:43:27.000000 flax-0.7.2/tests/run_all_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-08-09 01:43:27.000000 flax-0.7.2/tests/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-09 01:43:27.000000 flax-0.7.2/tests/struct_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-08-09 01:43:27.000000 flax-0.7.2/tests/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-08-09 01:43:27.000000 flax-0.7.2/tests/traceback_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-08-09 01:43:27.000000 flax-0.7.2/tests/traverse_util_test.py
```

### Comparing `flax-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `flax-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/analytics/README.md` & `flax-0.7.2/.github/analytics/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/analytics/get_repo_metrics.py` & `flax-0.7.2/.github/analytics/get_repo_metrics.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/analytics/issue_activity_since_date.gql` & `flax-0.7.2/.github/analytics/issue_activity_since_date.gql`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/analytics/pr_data_query.gql` & `flax-0.7.2/.github/analytics/pr_data_query.gql`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/pull_request_template.md` & `flax-0.7.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/workflows/build.yml` & `flax-0.7.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.github/workflows/pythonpublish.yml` & `flax-0.7.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.pre-commit-config.yaml` & `flax-0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/.readthedocs.yml` & `flax-0.7.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/CHANGELOG.md` & `flax-0.7.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,25 @@
 -
 -
 -
 -
 -
 -
 
+0.7.2
+-----
+New features:
+- make `flax.core.copy` `add_or_replace` optional
+- Add `use_fast_variance` option to `GroupNorm` and `BatchNorm` to allow disabling it.
+
+Bug fixes:
+- Use `field_specifiers` instead of `field_descriptors` in `@dataclass_transform`.
+- Fix `nn.Module` typing.
+- [JAX] Replace uses of `jax.experimental.pjit.with_sharding_constraint` with `jax.lax.with_sharding_constraint`.
+
 0.7.1
 -----
 Breaking changes:
 - Migrating Flax from returning FrozenDicts to returning regular dicts. More details can be found in this [announcement](https://github.com/google/flax/discussions/3191)
 
 New features:
 - Use pyink
```

### Comparing `flax-0.7.1/LICENSE` & `flax-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/PKG-INFO` & `flax-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flax
-Version: 0.7.1
+Version: 0.7.2
 Summary: Flax: A neural network library for JAX designed for flexibility
 Author-email: Flax team <flax-dev@google.com>
 Project-URL: homepage, https://github.com/google/flax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -211,15 +211,15 @@
 To cite this repository:
 
 ```
 @software{flax2020github,
   author = {Jonathan Heek and Anselm Levskaya and Avital Oliver and Marvin Ritter and Bertrand Rondepierre and Andreas Steiner and Marc van {Z}ee},
   title = {{F}lax: A neural network library and ecosystem for {JAX}},
   url = {http://github.com/google/flax},
-  version = {0.7.1},
+  version = {0.7.2},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, names are in alphabetical order, the version number
 is intended to be that from [flax/version.py](https://github.com/google/flax/blob/main/flax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `flax-0.7.1/README.md` & `flax-0.7.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 To cite this repository:
 
 ```
 @software{flax2020github,
   author = {Jonathan Heek and Anselm Levskaya and Avital Oliver and Marvin Ritter and Bertrand Rondepierre and Andreas Steiner and Marc van {Z}ee},
   title = {{F}lax: A neural network library and ecosystem for {JAX}},
   url = {http://github.com/google/flax},
-  version = {0.7.1},
+  version = {0.7.2},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, names are in alphabetical order, the version number
 is intended to be that from [flax/version.py](https://github.com/google/flax/blob/main/flax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `flax-0.7.1/dev/.devcontainer/Dockerfile` & `flax-0.7.2/dev/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/dev/.devcontainer/devcontainer.json` & `flax-0.7.2/dev/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/dev/README.md` & `flax-0.7.2/dev/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/dev/update_requirements.py` & `flax-0.7.2/dev/update_requirements.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/Makefile` & `flax-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/README.md` & `flax-0.7.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/_ext/codediff.py` & `flax-0.7.2/docs/_ext/codediff.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/_ext/codediff_test.py` & `flax-0.7.2/docs/_ext/codediff_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/_ext/flax_module.py` & `flax-0.7.2/docs/_ext/flax_module.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.linen/activation_functions.rst` & `flax-0.7.2/docs/api_reference/flax.linen/activation_functions.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.linen/initializers.rst` & `flax-0.7.2/docs/api_reference/flax.linen/initializers.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.linen/layers.rst` & `flax-0.7.2/docs/api_reference/flax.linen/layers.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.linen/spmd.rst` & `flax-0.7.2/docs/api_reference/flax.linen/spmd.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.linen/transformations.rst` & `flax-0.7.2/docs/api_reference/flax.linen/transformations.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.training.rst` & `flax-0.7.2/docs/api_reference/flax.training.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/api_reference/flax.traverse_util.rst` & `flax-0.7.2/docs/api_reference/flax.traverse_util.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/conf.py` & `flax-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/conf_sphinx_patch.py` & `flax-0.7.2/docs/conf_sphinx_patch.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/contributing.md` & `flax-0.7.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/developer_notes/lift.md` & `flax-0.7.2/docs/developer_notes/lift.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/developer_notes/module_lifecycle.rst` & `flax-0.7.2/docs/developer_notes/module_lifecycle.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/examples_community_examples.rst` & `flax-0.7.2/docs/examples_community_examples.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/examples_core_examples.rst` & `flax-0.7.2/docs/examples_core_examples.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/examples_google_research_examples.rst` & `flax-0.7.2/docs/examples_google_research_examples.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/examples_repositories_that_use_flax.rst` & `flax-0.7.2/docs/examples_repositories_that_use_flax.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flax.png` & `flax-0.7.2/docs/flax.png`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flip/0000-template.md` & `flax-0.7.2/docs/flip/0000-template.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flip/1009-optimizer-api.md` & `flax-0.7.2/docs/flip/1009-optimizer-api.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flip/1777-default-dtype.md` & `flax-0.7.2/docs/flip/1777-default-dtype.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flip/2434-general-metadata.md` & `flax-0.7.2/docs/flip/2434-general-metadata.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flip/2974-kw-only-dataclasses.md` & `flax-0.7.2/docs/flip/2974-kw-only-dataclasses.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/flip/README.md` & `flax-0.7.2/docs/flip/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/getting_started.ipynb` & `flax-0.7.2/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/getting_started.md` & `flax-0.7.2/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/glossary.rst` & `flax-0.7.2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/arguments.md` & `flax-0.7.2/docs/guides/arguments.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/batch_norm.rst` & `flax-0.7.2/docs/guides/batch_norm.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/convert_pytorch_to_flax.rst` & `flax-0.7.2/docs/guides/convert_pytorch_to_flax.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/dropout.rst` & `flax-0.7.2/docs/guides/dropout.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/ensembling.rst` & `flax-0.7.2/docs/guides/ensembling.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/extracting_intermediates.rst` & `flax-0.7.2/docs/guides/extracting_intermediates.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/flax_basics.ipynb` & `flax-0.7.2/docs/guides/flax_basics.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/flax_basics.md` & `flax-0.7.2/docs/guides/flax_basics.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/flax_on_pjit.ipynb` & `flax-0.7.2/docs/guides/flax_on_pjit.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/flax_on_pjit.md` & `flax-0.7.2/docs/guides/flax_on_pjit.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/full_eval.rst` & `flax-0.7.2/docs/guides/full_eval.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/haiku_migration_guide.rst` & `flax-0.7.2/docs/guides/haiku_migration_guide.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/jax_for_the_impatient.ipynb` & `flax-0.7.2/docs/guides/jax_for_the_impatient.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/jax_for_the_impatient.md` & `flax-0.7.2/docs/guides/jax_for_the_impatient.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/linen_upgrade_guide.rst` & `flax-0.7.2/docs/guides/linen_upgrade_guide.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/lr_schedule.rst` & `flax-0.7.2/docs/guides/lr_schedule.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/model_surgery.ipynb` & `flax-0.7.2/docs/guides/model_surgery.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/model_surgery.md` & `flax-0.7.2/docs/guides/model_surgery.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/optax_update_guide.rst` & `flax-0.7.2/docs/guides/optax_update_guide.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/orbax_upgrade_guide.rst` & `flax-0.7.2/docs/guides/orbax_upgrade_guide.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/regular_dict_upgrade_guide.rst` & `flax-0.7.2/docs/guides/regular_dict_upgrade_guide.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/rnncell_upgrade_guide.rst` & `flax-0.7.2/docs/guides/rnncell_upgrade_guide.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/setup_or_nncompact.rst` & `flax-0.7.2/docs/guides/setup_or_nncompact.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/state_params.rst` & `flax-0.7.2/docs/guides/state_params.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/transfer_learning.ipynb` & `flax-0.7.2/docs/guides/transfer_learning.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/transfer_learning.md` & `flax-0.7.2/docs/guides/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/use_checkpointing.ipynb` & `flax-0.7.2/docs/guides/use_checkpointing.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/guides/use_checkpointing.md` & `flax-0.7.2/docs/guides/use_checkpointing.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/index.rst` & `flax-0.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/mission.md` & `flax-0.7.2/docs/mission.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/flax_sharp_bits.ipynb` & `flax-0.7.2/docs/notebooks/flax_sharp_bits.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/flax_sharp_bits.md` & `flax-0.7.2/docs/notebooks/flax_sharp_bits.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/full_eval.ipynb` & `flax-0.7.2/docs/notebooks/full_eval.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/full_eval.md` & `flax-0.7.2/docs/notebooks/full_eval.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/linen_intro.ipynb` & `flax-0.7.2/docs/notebooks/linen_intro.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/linen_intro.md` & `flax-0.7.2/docs/notebooks/linen_intro.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/optax_update_guide.ipynb` & `flax-0.7.2/docs/notebooks/optax_update_guide.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/optax_update_guide.md` & `flax-0.7.2/docs/notebooks/optax_update_guide.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/orbax_upgrade_guide.ipynb` & `flax-0.7.2/docs/notebooks/orbax_upgrade_guide.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/orbax_upgrade_guide.md` & `flax-0.7.2/docs/notebooks/orbax_upgrade_guide.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/state_params.ipynb` & `flax-0.7.2/docs/notebooks/state_params.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/notebooks/state_params.md` & `flax-0.7.2/docs/notebooks/state_params.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/overview.md` & `flax-0.7.2/docs/overview.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/philosophy.md` & `flax-0.7.2/docs/philosophy.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/docs/requirements.txt` & `flax-0.7.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/README.md` & `flax-0.7.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/cloud/README.md` & `flax-0.7.2/examples/cloud/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/cloud/launch_gce.py` & `flax-0.7.2/examples/cloud/launch_gce.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/cloud/startup_script.sh` & `flax-0.7.2/examples/cloud/startup_script.sh`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/README.md` & `flax-0.7.2/examples/imagenet/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/configs/default.py` & `flax-0.7.2/examples/imagenet/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/configs/fake_data_benchmark.py` & `flax-0.7.2/examples/imagenet/configs/fake_data_benchmark.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/configs/tpu.py` & `flax-0.7.2/examples/imagenet/configs/tpu.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/configs/v100_x8.py` & `flax-0.7.2/examples/imagenet/configs/v100_x8.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/configs/v100_x8_mixed_precision.py` & `flax-0.7.2/examples/imagenet/configs/v100_x8_mixed_precision.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/imagenet.ipynb` & `flax-0.7.2/examples/imagenet/imagenet.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/imagenet_benchmark.py` & `flax-0.7.2/examples/imagenet/imagenet_benchmark.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/imagenet_fake_data_benchmark.py` & `flax-0.7.2/examples/imagenet/imagenet_fake_data_benchmark.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/input_pipeline.py` & `flax-0.7.2/examples/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/main.py` & `flax-0.7.2/examples/imagenet/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/models.py` & `flax-0.7.2/examples/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/models_test.py` & `flax-0.7.2/examples/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/train.py` & `flax-0.7.2/examples/imagenet/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/imagenet/train_test.py` & `flax-0.7.2/examples/imagenet/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/attention_simple.py` & `flax-0.7.2/examples/linen_design_test/attention_simple.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/autoencoder.py` & `flax-0.7.2/examples/linen_design_test/autoencoder.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/dense.py` & `flax-0.7.2/examples/linen_design_test/dense.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/linear_regression.py` & `flax-0.7.2/examples/linen_design_test/linear_regression.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/mlp_explicit.py` & `flax-0.7.2/examples/linen_design_test/mlp_explicit.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/mlp_inline.py` & `flax-0.7.2/examples/linen_design_test/mlp_inline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/mlp_lazy.py` & `flax-0.7.2/examples/linen_design_test/mlp_lazy.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/tied_autoencoder.py` & `flax-0.7.2/examples/linen_design_test/tied_autoencoder.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/linen_design_test/weight_std.py` & `flax-0.7.2/examples/linen_design_test/weight_std.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/README.md` & `flax-0.7.2/examples/lm1b/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/configs/default.py` & `flax-0.7.2/examples/lm1b/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/input_pipeline.py` & `flax-0.7.2/examples/lm1b/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/input_pipeline_test.py` & `flax-0.7.2/examples/lm1b/input_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/main.py` & `flax-0.7.2/examples/lm1b/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/models.py` & `flax-0.7.2/examples/lm1b/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/temperature_sampler.py` & `flax-0.7.2/examples/lm1b/temperature_sampler.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/temperature_sampler_test.py` & `flax-0.7.2/examples/lm1b/temperature_sampler_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/tokenizer.py` & `flax-0.7.2/examples/lm1b/tokenizer.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/train.py` & `flax-0.7.2/examples/lm1b/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/lm1b/train_test.py` & `flax-0.7.2/examples/lm1b/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/README.md` & `flax-0.7.2/examples/mnist/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/configs/default.py` & `flax-0.7.2/examples/mnist/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/main.py` & `flax-0.7.2/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/mnist.ipynb` & `flax-0.7.2/examples/mnist/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/mnist_benchmark.py` & `flax-0.7.2/examples/mnist/mnist_benchmark.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/train.py` & `flax-0.7.2/examples/mnist/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/mnist/train_test.py` & `flax-0.7.2/examples/mnist/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/nlp_seq/README.md` & `flax-0.7.2/examples/nlp_seq/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/nlp_seq/input_pipeline.py` & `flax-0.7.2/examples/nlp_seq/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/nlp_seq/input_pipeline_test.py` & `flax-0.7.2/examples/nlp_seq/input_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/nlp_seq/models.py` & `flax-0.7.2/examples/nlp_seq/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/nlp_seq/train.py` & `flax-0.7.2/examples/nlp_seq/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/README.md` & `flax-0.7.2/examples/ogbg_molpcba/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/configs/default.py` & `flax-0.7.2/examples/ogbg_molpcba/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/configs/default_graph_net.py` & `flax-0.7.2/examples/ogbg_molpcba/configs/default_graph_net.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/configs/hparam_sweep.py` & `flax-0.7.2/examples/ogbg_molpcba/configs/hparam_sweep.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/configs/test.py` & `flax-0.7.2/examples/ogbg_molpcba/configs/test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/input_pipeline.py` & `flax-0.7.2/examples/ogbg_molpcba/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/input_pipeline_test.py` & `flax-0.7.2/examples/ogbg_molpcba/input_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/main.py` & `flax-0.7.2/examples/ogbg_molpcba/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/models.py` & `flax-0.7.2/examples/ogbg_molpcba/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/models_test.py` & `flax-0.7.2/examples/ogbg_molpcba/models_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/ogbg_molpcba.ipynb` & `flax-0.7.2/examples/ogbg_molpcba/ogbg_molpcba.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/ogbg_molpcba_benchmark.py` & `flax-0.7.2/examples/ogbg_molpcba/ogbg_molpcba_benchmark.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/train.py` & `flax-0.7.2/examples/ogbg_molpcba/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ogbg_molpcba/train_test.py` & `flax-0.7.2/examples/ogbg_molpcba/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/README.md` & `flax-0.7.2/examples/ppo/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/agent.py` & `flax-0.7.2/examples/ppo/agent.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/configs/default.py` & `flax-0.7.2/examples/ppo/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/env_utils.py` & `flax-0.7.2/examples/ppo/env_utils.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/models.py` & `flax-0.7.2/examples/ppo/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/ppo_lib.py` & `flax-0.7.2/examples/ppo/ppo_lib.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/ppo_lib_test.py` & `flax-0.7.2/examples/ppo/ppo_lib_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/ppo_main.py` & `flax-0.7.2/examples/ppo/ppo_main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/seed_rl_atari_preprocessing.py` & `flax-0.7.2/examples/ppo/seed_rl_atari_preprocessing.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/ppo/test_episodes.py` & `flax-0.7.2/examples/ppo/test_episodes.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/seq2seq/README.md` & `flax-0.7.2/examples/seq2seq/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/seq2seq/input_pipeline.py` & `flax-0.7.2/examples/seq2seq/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/seq2seq/models.py` & `flax-0.7.2/examples/seq2seq/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/seq2seq/seq2seq.ipynb` & `flax-0.7.2/examples/seq2seq/seq2seq.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/seq2seq/train.py` & `flax-0.7.2/examples/seq2seq/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/seq2seq/train_test.py` & `flax-0.7.2/examples/seq2seq/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/README.md` & `flax-0.7.2/examples/sst2/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/build_vocabulary.py` & `flax-0.7.2/examples/sst2/build_vocabulary.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/configs/default.py` & `flax-0.7.2/examples/sst2/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/input_pipeline.py` & `flax-0.7.2/examples/sst2/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/input_pipeline_test.py` & `flax-0.7.2/examples/sst2/input_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/main.py` & `flax-0.7.2/examples/sst2/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/models.py` & `flax-0.7.2/examples/sst2/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/models_test.py` & `flax-0.7.2/examples/sst2/models_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/sst2.ipynb` & `flax-0.7.2/examples/sst2/sst2.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/train.py` & `flax-0.7.2/examples/sst2/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/train_test.py` & `flax-0.7.2/examples/sst2/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/vocab.txt` & `flax-0.7.2/examples/sst2/vocab.txt`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/sst2/vocabulary.py` & `flax-0.7.2/examples/sst2/vocabulary.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/README.md` & `flax-0.7.2/examples/vae/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/input_pipeline.py` & `flax-0.7.2/examples/vae/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/main.py` & `flax-0.7.2/examples/vae/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/models.py` & `flax-0.7.2/examples/vae/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/reconstruction.png` & `flax-0.7.2/examples/vae/reconstruction.png`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/sample.png` & `flax-0.7.2/examples/vae/sample.png`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/train.py` & `flax-0.7.2/examples/vae/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/vae/utils.py` & `flax-0.7.2/examples/vae/utils.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/README.md` & `flax-0.7.2/examples/wmt/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/bleu.py` & `flax-0.7.2/examples/wmt/bleu.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/configs/default.py` & `flax-0.7.2/examples/wmt/configs/default.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/decode.py` & `flax-0.7.2/examples/wmt/decode.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/input_pipeline.py` & `flax-0.7.2/examples/wmt/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/input_pipeline_test.py` & `flax-0.7.2/examples/wmt/input_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/main.py` & `flax-0.7.2/examples/wmt/main.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/models.py` & `flax-0.7.2/examples/wmt/models.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/tokenizer.py` & `flax-0.7.2/examples/wmt/tokenizer.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/train.py` & `flax-0.7.2/examples/wmt/train.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/examples/wmt/train_test.py` & `flax-0.7.2/examples/wmt/train_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/__init__.py` & `flax-0.7.2/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/configurations.py` & `flax-0.7.2/flax/configurations.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/__init__.py` & `flax-0.7.2/flax/core/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/axes_scan.py` & `flax-0.7.2/flax/core/axes_scan.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/flax_functional_engine.ipynb` & `flax-0.7.2/flax/core/flax_functional_engine.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/frozen_dict.py` & `flax-0.7.2/flax/core/frozen_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Frozen Dictionary."""
 
 import collections
-from typing import Any, TypeVar, Mapping, Dict, Tuple, Union, Hashable
+from typing import Any, Dict, Hashable, Optional, Mapping, Tuple, TypeVar, Union
+from types import MappingProxyType
 
 from flax import serialization
 import jax
 
 
 class FrozenKeysView(collections.abc.KeysView):
   """A wrapper for a more useful repr of the keys in a frozen dict."""
@@ -107,15 +108,17 @@
     if self._hash is None:
       h = 0
       for key, value in self.items():
         h ^= hash((key, value))
       self._hash = h
     return self._hash
 
-  def copy(self, add_or_replace: Mapping[K, V]) -> 'FrozenDict[K, V]':
+  def copy(
+      self, add_or_replace: Mapping[K, V] = MappingProxyType({})
+  ) -> 'FrozenDict[K, V]':
     """Create a new FrozenDict with additional or replaced entries."""
     return type(self)({**self, **unfreeze(add_or_replace)})  # type: ignore[arg-type]
 
   def keys(self):
     return FrozenKeysView(self)
 
   def values(self):
@@ -219,15 +222,17 @@
     return ys
   else:
     return x
 
 
 def copy(
     x: Union[FrozenDict, Dict[str, Any]],
-    add_or_replace: Union[FrozenDict, Dict[str, Any]],
+    add_or_replace: Union[FrozenDict[str, Any], Dict[str, Any]] = FrozenDict(
+        {}
+    ),
 ) -> Union[FrozenDict, Dict[str, Any]]:
   """Create a new dict with additional and/or replaced entries. This is a utility
   function that can act on either a FrozenDict or regular dict and mimics the
   behavior of `FrozenDict.copy`.
 
   Example::
```

### Comparing `flax-0.7.1/flax/core/lift.py` & `flax-0.7.2/flax/core/lift.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/meta.py` & `flax-0.7.2/flax/core/meta.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/nn/__init__.py` & `flax-0.7.2/flax/core/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/nn/attention.py` & `flax-0.7.2/flax/core/nn/attention.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/nn/linear.py` & `flax-0.7.2/flax/core/nn/linear.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/nn/normalization.py` & `flax-0.7.2/flax/core/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/nn/stochastic.py` & `flax-0.7.2/flax/core/nn/stochastic.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/partial_eval.py` & `flax-0.7.2/flax/core/partial_eval.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/scope.py` & `flax-0.7.2/flax/core/scope.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/tracers.py` & `flax-0.7.2/flax/core/tracers.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/core/variables.py` & `flax-0.7.2/flax/core/variables.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/errors.py` & `flax-0.7.2/flax/errors.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/ids.py` & `flax-0.7.2/flax/ids.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/io.py` & `flax-0.7.2/flax/io.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/jax_utils.py` & `flax-0.7.2/flax/jax_utils.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/README.md` & `flax-0.7.2/flax/linen/README.md`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/__init__.py` & `flax-0.7.2/flax/linen/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/activation.py` & `flax-0.7.2/flax/linen/activation.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/attention.py` & `flax-0.7.2/flax/linen/attention.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/combinators.py` & `flax-0.7.2/flax/linen/combinators.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/dtypes.py` & `flax-0.7.2/flax/linen/dtypes.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/experimental/layers_with_named_axes.py` & `flax-0.7.2/flax/linen/experimental/layers_with_named_axes.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/initializers.py` & `flax-0.7.2/flax/linen/initializers.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/kw_only_dataclasses.py` & `flax-0.7.2/flax/linen/kw_only_dataclasses.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/linear.py` & `flax-0.7.2/flax/linen/linear.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/module.py` & `flax-0.7.2/flax/linen/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1346,4202 +1346,4204 @@
 00005410: 736f 2074 6865 7920 646f 6e27 7420 6166  so they don't af
 00005420: 6665 6374 2074 6865 2064 6174 6163 6c61  fect the datacla
 00005430: 7373 2062 6568 6176 696f 722e 0a40 6461  ss behavior..@da
 00005440: 7461 636c 6173 735f 7472 616e 7366 6f72  taclass_transfor
 00005450: 6d28 290a 636c 6173 7320 4d6f 6475 6c65  m().class Module
 00005460: 4261 7365 3a0a 2020 6966 2074 7970 696e  Base:.  if typin
 00005470: 672e 5459 5045 5f43 4845 434b 494e 473a  g.TYPE_CHECKING:
-00005480: 0a20 2020 2073 636f 7065 3a20 4f70 7469  .    scope: Opti
-00005490: 6f6e 616c 5b53 636f 7065 5d0a 2020 2020  onal[Scope].    
-000054a0: 5f73 7461 7465 3a20 5f4d 6f64 756c 6549  _state: _ModuleI
-000054b0: 6e74 6572 6e61 6c53 7461 7465 0a20 2020  nternalState.   
-000054c0: 205f 7061 7265 6e74 5f72 6566 3a20 556e   _parent_ref: Un
-000054d0: 696f 6e5b 274d 6f64 756c 6527 2c20 7765  ion['Module', we
-000054e0: 616b 7265 662e 5265 6665 7265 6e63 6554  akref.ReferenceT
-000054f0: 7970 655b 274d 6f64 756c 6527 5d2c 204e  ype['Module'], N
-00005500: 6f6e 655d 0a20 2020 2070 6172 656e 743a  one].    parent:
-00005510: 2055 6e69 6f6e 5b27 4d6f 6475 6c65 272c   Union['Module',
-00005520: 205f 5365 6e74 696e 656c 2c20 4e6f 6e65   _Sentinel, None
-00005530: 5d0a 2020 2020 5f5f 6461 7461 636c 6173  ].    __dataclas
-00005540: 735f 6669 656c 6473 5f5f 3a20 4469 6374  s_fields__: Dict
-00005550: 5b73 7472 2c20 6461 7461 636c 6173 7365  [str, dataclasse
-00005560: 732e 4669 656c 645d 0a0a 0a63 6c61 7373  s.Field]...class
-00005570: 204d 6f64 756c 6528 4d6f 6475 6c65 4261   Module(ModuleBa
-00005580: 7365 293a 0a20 2022 2222 4261 7365 2063  se):.  """Base c
-00005590: 6c61 7373 2066 6f72 2061 6c6c 206e 6575  lass for all neu
-000055a0: 7261 6c20 6e65 7477 6f72 6b20 6d6f 6475  ral network modu
-000055b0: 6c65 732e 204c 6179 6572 7320 616e 6420  les. Layers and 
-000055c0: 6d6f 6465 6c73 2073 686f 756c 6420 7375  models should su
-000055d0: 6263 6c61 7373 2074 6869 7320 636c 6173  bclass this clas
-000055e0: 732e 0a0a 2020 416c 6c20 466c 6178 204d  s...  All Flax M
-000055f0: 6f64 756c 6573 2061 7265 2050 7974 686f  odules are Pytho
-00005600: 6e20 332e 370a 2020 6064 6174 6163 6c61  n 3.7.  `datacla
-00005610: 7373 6573 203c 6874 7470 733a 2f2f 646f  sses <https://do
-00005620: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-00005630: 6c69 6272 6172 792f 6461 7461 636c 6173  library/dataclas
-00005640: 7365 732e 6874 6d6c 3e60 5f2e 2053 696e  ses.html>`_. Sin
-00005650: 6365 0a20 2064 6174 6163 6c61 7373 6573  ce.  dataclasses
-00005660: 2074 616b 6520 6f76 6572 2060 605f 5f69   take over ``__i
-00005670: 6e69 745f 5f60 602c 2079 6f75 2073 686f  nit__``, you sho
-00005680: 756c 6420 696e 7374 6561 6420 6f76 6572  uld instead over
-00005690: 7269 6465 203a 6d65 7468 3a60 7365 7475  ride :meth:`setu
-000056a0: 7060 2c0a 2020 7768 6963 6820 6973 2061  p`,.  which is a
-000056b0: 7574 6f6d 6174 6963 616c 6c79 2063 616c  utomatically cal
-000056c0: 6c65 6420 746f 2069 6e69 7469 616c 697a  led to initializ
-000056d0: 6520 7468 6520 6d6f 6475 6c65 2e0a 0a20  e the module... 
-000056e0: 204d 6f64 756c 6573 2063 616e 2063 6f6e   Modules can con
-000056f0: 7461 696e 2073 7562 6d6f 6475 6c65 732c  tain submodules,
-00005700: 2061 6e64 2069 6e20 7468 6973 2077 6179   and in this way
-00005710: 2063 616e 2062 6520 6e65 7374 6564 2069   can be nested i
-00005720: 6e20 6120 7472 6565 0a20 2073 7472 7563  n a tree.  struc
-00005730: 7475 7265 2e20 5375 626d 6f64 656c 7320  ture. Submodels 
-00005740: 6361 6e20 6265 2061 7373 6967 6e65 6420  can be assigned 
-00005750: 6173 2072 6567 756c 6172 2061 7474 7269  as regular attri
-00005760: 6275 7465 7320 696e 7369 6465 2074 6865  butes inside the
-00005770: 0a20 203a 6d65 7468 3a60 7365 7475 7060  .  :meth:`setup`
-00005780: 206d 6574 686f 642e 0a0a 2020 596f 7520   method...  You 
-00005790: 6361 6e20 6465 6669 6e65 2061 7262 6974  can define arbit
-000057a0: 7261 7279 2022 666f 7277 6172 6420 7061  rary "forward pa
-000057b0: 7373 2220 6d65 7468 6f64 7320 6f6e 2079  ss" methods on y
-000057c0: 6f75 7220 4d6f 6475 6c65 2073 7562 636c  our Module subcl
-000057d0: 6173 732e 0a20 2057 6869 6c65 206e 6f20  ass..  While no 
-000057e0: 6d65 7468 6f64 7320 6172 6520 7370 6563  methods are spec
-000057f0: 6961 6c2d 6361 7365 642c 2060 605f 5f63  ial-cased, ``__c
-00005800: 616c 6c5f 5f60 6020 6973 2061 2070 6f70  all__`` is a pop
-00005810: 756c 6172 2063 686f 6963 6520 6265 6361  ular choice beca
-00005820: 7573 650a 2020 6974 2061 6c6c 6f77 7320  use.  it allows 
-00005830: 796f 7520 746f 2075 7365 206d 6f64 756c  you to use modul
-00005840: 6520 696e 7374 616e 6365 7320 6173 2069  e instances as i
-00005850: 6620 7468 6579 2061 7265 2066 756e 6374  f they are funct
-00005860: 696f 6e73 3a3a 0a0a 2020 2020 6672 6f6d  ions::..    from
-00005870: 2066 6c61 7820 696d 706f 7274 206c 696e   flax import lin
-00005880: 656e 2061 7320 6e6e 0a0a 2020 2020 636c  en as nn..    cl
-00005890: 6173 7320 4d6f 6475 6c65 286e 6e2e 4d6f  ass Module(nn.Mo
-000058a0: 6475 6c65 293a 0a20 2020 2020 2066 6561  dule):.      fea
-000058b0: 7475 7265 733a 2054 7570 6c65 5b69 6e74  tures: Tuple[int
-000058c0: 2c20 2e2e 2e5d 203d 2028 3136 2c20 3429  , ...] = (16, 4)
-000058d0: 0a0a 2020 2020 2020 6465 6620 7365 7475  ..      def setu
-000058e0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000058f0: 2073 656c 662e 6465 6e73 6531 203d 2044   self.dense1 = D
-00005900: 656e 7365 2873 656c 662e 6665 6174 7572  ense(self.featur
-00005910: 6573 5b30 5d29 0a20 2020 2020 2020 2073  es[0]).        s
-00005920: 656c 662e 6465 6e73 6532 203d 2044 656e  elf.dense2 = Den
-00005930: 7365 2873 656c 662e 6665 6174 7572 6573  se(self.features
-00005940: 5b31 5d29 0a0a 2020 2020 2020 6465 6620  [1])..      def 
-00005950: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2078  __call__(self, x
-00005960: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00005970: 6e20 7365 6c66 2e64 656e 7365 3228 6e6e  n self.dense2(nn
-00005980: 2e72 656c 7528 7365 6c66 2e64 656e 7365  .relu(self.dense
-00005990: 3128 7829 2929 0a0a 2020 4f70 7469 6f6e  1(x)))..  Option
-000059a0: 616c 6c79 2c20 666f 7220 6d6f 7265 2063  ally, for more c
-000059b0: 6f6e 6369 7365 206d 6f64 756c 6520 696d  oncise module im
-000059c0: 706c 656d 656e 7461 7469 6f6e 7320 7768  plementations wh
-000059d0: 6572 6520 7375 626d 6f64 756c 6573 0a20  ere submodules. 
-000059e0: 2064 6566 696e 6974 696f 6e73 2061 7265   definitions are
-000059f0: 2063 6f2d 6c6f 6361 7465 6420 7769 7468   co-located with
-00005a00: 2074 6865 6972 2075 7361 6765 2c20 796f   their usage, yo
-00005a10: 7520 6361 6e20 7573 6520 7468 650a 2020  u can use the.  
-00005a20: 3a6d 6574 683a 6063 6f6d 7061 6374 6020  :meth:`compact` 
-00005a30: 7772 6170 7065 722e 0a20 2022 2222 0a0a  wrapper..  """..
-00005a40: 2020 6966 2074 7970 696e 672e 5459 5045    if typing.TYPE
-00005a50: 5f43 4845 434b 494e 473a 0a0a 2020 2020  _CHECKING:..    
-00005a60: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00005a70: 662c 202a 6172 6773 2c20 2a2a 6b77 6172  f, *args, **kwar
-00005a80: 6773 293a 0a20 2020 2020 2023 2074 6869  gs):.      # thi
-00005a90: 7320 7374 7562 206d 616b 6573 2073 7572  s stub makes sur
-00005aa0: 6520 7079 7479 7065 2061 6363 6570 7473  e pytype accepts
-00005ab0: 2063 6f6e 7374 7275 6374 6f72 2061 7267   constructor arg
-00005ac0: 756d 656e 7473 2e0a 2020 2020 2020 7061  uments..      pa
-00005ad0: 7373 0a0a 2020 2020 6465 6620 5f5f 6361  ss..    def __ca
-00005ae0: 6c6c 5f5f 2873 656c 662c 202a 6172 6773  ll__(self, *args
-00005af0: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2041  , **kwargs) -> A
-00005b00: 6e79 3a0a 2020 2020 2020 2320 7468 6973  ny:.      # this
-00005b10: 2073 7475 6220 616c 6c6f 7773 2070 7974   stub allows pyt
-00005b20: 7970 6520 746f 2061 6363 6570 7420 4d6f  ype to accept Mo
-00005b30: 6475 6c65 7320 6173 2043 616c 6c61 626c  dules as Callabl
-00005b40: 6573 2e0a 2020 2020 2020 7061 7373 0a0a  es..      pass..
-00005b50: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-00005b60: 2064 6566 205f 5f69 6e69 745f 7375 6263   def __init_subc
-00005b70: 6c61 7373 5f5f 2863 6c73 2c20 6b77 5f6f  lass__(cls, kw_o
-00005b80: 6e6c 793a 2062 6f6f 6c20 3d20 4661 6c73  nly: bool = Fals
-00005b90: 652c 202a 2a6b 7761 7267 733a 2041 6e79  e, **kwargs: Any
-00005ba0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00005bb0: 2222 4175 746f 6d61 7469 6361 6c6c 7920  ""Automatically 
-00005bc0: 696e 6974 6961 6c69 7a65 7320 616c 6c20  initializes all 
-00005bd0: 7375 6263 6c61 7373 6573 2061 7320 6375  subclasses as cu
-00005be0: 7374 6f6d 2064 6174 6163 6c61 7373 6573  stom dataclasses
-00005bf0: 2e22 2222 0a20 2020 2073 7570 6572 2829  .""".    super()
-00005c00: 2e5f 5f69 6e69 745f 7375 6263 6c61 7373  .__init_subclass
-00005c10: 5f5f 282a 2a6b 7761 7267 7329 0a20 2020  __(**kwargs).   
-00005c20: 2023 2041 6c6c 2046 6c61 7820 4d6f 6475   # All Flax Modu
-00005c30: 6c65 7320 6172 6520 6461 7461 636c 6173  les are dataclas
-00005c40: 7365 732e 2020 5765 2066 6f72 6365 2074  ses.  We force t
-00005c50: 6869 7320 636f 6e76 656e 7469 6f6e 2073  his convention s
-00005c60: 696e 6365 0a20 2020 2023 2069 7420 656e  ince.    # it en
-00005c70: 636f 7572 6167 6573 2074 6865 2073 7461  courages the sta
-00005c80: 7465 6c65 7373 2062 6568 6176 696f 7220  teless behavior 
-00005c90: 6e65 6564 6564 2074 6f20 636c 6f6e 6520  needed to clone 
-00005ca0: 6d6f 6475 6c65 2069 6e73 7461 6e63 6573  module instances
-00005cb0: 2066 6f72 0a20 2020 2023 2066 756e 6374   for.    # funct
-00005cc0: 696f 6e61 6c20 7472 616e 7366 6f72 6d61  ional transforma
-00005cd0: 7469 6f6e 2e20 2049 6e73 7465 6164 206f  tion.  Instead o
-00005ce0: 6620 7573 696e 6720 6120 7079 7468 6f6e  f using a python
-00005cf0: 206d 6574 6163 6c61 7373 2c20 7765 0a20   metaclass, we. 
-00005d00: 2020 2023 2061 7574 6f6d 6174 6963 616c     # automatical
-00005d10: 6c79 2074 7261 6e73 666f 726d 204d 6f64  ly transform Mod
-00005d20: 756c 6573 2069 6e74 6f20 6461 7461 636c  ules into datacl
-00005d30: 6173 7365 7320 6174 2073 7562 636c 6173  asses at subclas
-00005d40: 7320 6372 6561 7469 6f6e 0a20 2020 2023  s creation.    #
-00005d50: 2074 696d 652c 2061 6e64 2077 6520 7365   time, and we se
-00005d60: 7420 7468 6520 6c61 7374 2064 6174 6163  t the last datac
-00005d70: 6c61 7373 2061 7267 756d 656e 7473 2074  lass arguments t
-00005d80: 6f20 6070 6172 656e 7460 2061 6e64 2060  o `parent` and `
-00005d90: 6e61 6d65 602e 0a20 2020 2063 6c73 2e5f  name`..    cls._
-00005da0: 6375 7374 6f6d 697a 6564 5f64 6174 6163  customized_datac
-00005db0: 6c61 7373 5f74 7261 6e73 666f 726d 286b  lass_transform(k
-00005dc0: 775f 6f6e 6c79 290a 2020 2020 2320 5765  w_only).    # We
-00005dd0: 2077 7261 7020 7573 6572 2d64 6566 696e   wrap user-defin
-00005de0: 6564 206d 6574 686f 6473 2069 6e63 6c75  ed methods inclu
-00005df0: 6469 6e67 2073 6574 7570 2061 6e64 205f  ding setup and _
-00005e00: 5f63 616c 6c5f 5f20 746f 2065 6e66 6f72  _call__ to enfor
-00005e10: 6365 0a20 2020 2023 2061 206e 756d 6265  ce.    # a numbe
-00005e20: 7220 6f66 2064 6966 6665 7265 6e74 2063  r of different c
-00005e30: 6865 636b 7320 616e 6420 746f 2070 726f  hecks and to pro
-00005e40: 7669 6465 2063 6c65 6172 2065 7272 6f72  vide clear error
-00005e50: 206d 6573 7361 6765 732e 0a20 2020 2063   messages..    c
-00005e60: 6c73 2e5f 7665 7269 6679 5f73 696e 676c  ls._verify_singl
-00005e70: 655f 6f72 5f6e 6f5f 636f 6d70 6163 7428  e_or_no_compact(
-00005e80: 290a 2020 2020 636c 732e 5f77 7261 705f  ).    cls._wrap_
-00005e90: 6d6f 6475 6c65 5f61 7474 7269 6275 7465  module_attribute
-00005ea0: 7328 290a 2020 2020 2320 5365 7420 656d  s().    # Set em
-00005eb0: 7074 7920 636c 6173 7320 6465 6661 756c  pty class defaul
-00005ec0: 7473 2e0a 2020 2020 636c 732e 5f73 7461  ts..    cls._sta
-00005ed0: 7465 203d 205f 756e 696e 6974 6961 6c69  te = _uninitiali
-00005ee0: 7a65 645f 6d6f 6475 6c65 5f69 6e74 6572  zed_module_inter
-00005ef0: 6e61 6c5f 7374 6174 6520 2023 2074 7970  nal_state  # typ
-00005f00: 653a 2069 676e 6f72 655b 6174 7472 2d64  e: ignore[attr-d
-00005f10: 6566 696e 6564 5d0a 2020 2020 636c 732e  efined].    cls.
-00005f20: 7363 6f70 653a 204f 7074 696f 6e61 6c5b  scope: Optional[
-00005f30: 5363 6f70 655d 203d 204e 6f6e 6520 2023  Scope] = None  #
-00005f40: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-00005f50: 2020 2320 4861 6e64 6c65 7320 7765 616b    # Handles weak
-00005f60: 2072 6566 6572 656e 6369 6e67 206f 6620   referencing of 
-00005f70: 7061 7265 6e74 204d 6f64 756c 6573 2074  parent Modules t
-00005f80: 6f20 7072 6576 656e 7420 7265 6665 7265  o prevent refere
-00005f90: 6e63 6520 6379 636c 6573 2e0a 2020 2020  nce cycles..    
-00005fa0: 636c 732e 5f70 6172 656e 745f 7265 6620  cls._parent_ref 
-00005fb0: 3d20 4e6f 6e65 2020 2320 7479 7065 3a20  = None  # type: 
-00005fc0: 6967 6e6f 7265 5b61 7474 722d 6465 6669  ignore[attr-defi
-00005fd0: 6e65 645d 0a20 2020 2063 6c73 2e70 6172  ned].    cls.par
-00005fe0: 656e 7420 3d20 5061 7265 6e74 4465 7363  ent = ParentDesc
-00005ff0: 7269 7074 6f72 2829 2020 2320 7479 7065  riptor()  # type
-00006000: 3a20 6967 6e6f 7265 5b61 7373 6967 6e6d  : ignore[assignm
-00006010: 656e 745d 0a0a 2020 4063 6c61 7373 6d65  ent]..  @classme
-00006020: 7468 6f64 0a20 2064 6566 205f 6375 7374  thod.  def _cust
-00006030: 6f6d 697a 6564 5f64 6174 6163 6c61 7373  omized_dataclass
-00006040: 5f74 7261 6e73 666f 726d 2863 6c73 2c20  _transform(cls, 
-00006050: 6b77 5f6f 6e6c 793a 2062 6f6f 6c29 3a0a  kw_only: bool):.
-00006060: 2020 2020 2222 2254 7261 6e73 666f 726d      """Transform
-00006070: 7320 6063 6c73 6020 696e 746f 2061 2064  s `cls` into a d
-00006080: 6174 6163 6c61 7373 2c20 7769 7468 2063  ataclass, with c
-00006090: 7573 746f 6d20 6164 6469 7469 6f6e 616c  ustom additional
-000060a0: 2062 6568 6176 696f 722e 0a0a 2020 2020   behavior...    
-000060b0: 312e 2049 6e6a 6563 7420 6070 6172 656e  1. Inject `paren
-000060c0: 7460 2061 6e64 2060 6e61 6d65 6020 6669  t` and `name` fi
-000060d0: 656c 6473 2e20 2028 4966 2074 6865 7920  elds.  (If they 
-000060e0: 6172 6520 616c 7265 6164 7920 7072 6573  are already pres
-000060f0: 656e 742c 0a20 2020 2020 2020 7468 656e  ent,.       then
-00006100: 2063 6865 636b 2074 6861 7420 7468 6579   check that they
-00006110: 2068 6176 6520 7468 6520 6578 7065 6374   have the expect
-00006120: 6564 2074 7970 6573 2e29 0a20 2020 2032  ed types.).    2
-00006130: 2e20 5365 7420 636f 6d70 6172 652c 2068  . Set compare, h
-00006140: 6173 682c 2061 6e64 2072 6570 7220 746f  ash, and repr to
-00006150: 2046 616c 7365 2066 6f72 206e 6f6e 2d69   False for non-i
-00006160: 6e69 7420 6669 656c 6473 2e0a 2020 2020  nit fields..    
-00006170: 332e 2047 656e 6572 6174 6520 6120 6861  3. Generate a ha
-00006180: 7368 2066 756e 6374 696f 6e20 2869 6620  sh function (if 
-00006190: 6e6f 7420 7072 6f76 6964 6564 2062 7920  not provided by 
-000061a0: 636c 7329 2e0a 2020 2020 2222 220a 2020  cls)..    """.  
-000061b0: 2020 2320 4368 6563 6b20 7265 7365 7276    # Check reserv
-000061c0: 6564 2061 7474 7269 6275 7465 7320 6861  ed attributes ha
-000061d0: 7665 2065 7870 6563 7465 6420 7479 7065  ve expected type
-000061e0: 2061 6e6e 6f74 6174 696f 6e73 2e0a 2020   annotations..  
-000061f0: 2020 616e 6e6f 7461 7469 6f6e 7320 3d20    annotations = 
-00006200: 6469 6374 2863 6c73 2e5f 5f64 6963 745f  dict(cls.__dict_
-00006210: 5f2e 6765 7428 275f 5f61 6e6e 6f74 6174  _.get('__annotat
-00006220: 696f 6e73 5f5f 272c 207b 7d29 290a 2020  ions__', {})).  
-00006230: 2020 6966 2061 6e6e 6f74 6174 696f 6e73    if annotations
-00006240: 2e67 6574 2827 7061 7265 6e74 272c 205f  .get('parent', _
-00006250: 5061 7265 6e74 5479 7065 2920 213d 205f  ParentType) != _
-00006260: 5061 7265 6e74 5479 7065 3a0a 2020 2020  ParentType:.    
-00006270: 2020 7261 6973 6520 6572 726f 7273 2e52    raise errors.R
-00006280: 6573 6572 7665 644d 6f64 756c 6541 7474  eservedModuleAtt
-00006290: 7269 6275 7465 4572 726f 7228 616e 6e6f  ributeError(anno
-000062a0: 7461 7469 6f6e 7329 0a20 2020 2069 6620  tations).    if 
-000062b0: 616e 6e6f 7461 7469 6f6e 732e 6765 7428  annotations.get(
-000062c0: 276e 616d 6527 2c20 7374 7229 206e 6f74  'name', str) not
-000062d0: 2069 6e20 2827 7374 7227 2c20 7374 722c   in ('str', str,
-000062e0: 204f 7074 696f 6e61 6c5b 7374 725d 293a   Optional[str]):
-000062f0: 0a20 2020 2020 2072 6169 7365 2065 7272  .      raise err
-00006300: 6f72 732e 5265 7365 7276 6564 4d6f 6475  ors.ReservedModu
-00006310: 6c65 4174 7472 6962 7574 6545 7272 6f72  leAttributeError
-00006320: 2861 6e6e 6f74 6174 696f 6e73 290a 0a20  (annotations).. 
-00006330: 2020 2023 2061 6e79 206e 6f6e 2d69 6e69     # any non-ini
-00006340: 7420 6669 656c 6420 7769 6c6c 206f 6e6c  t field will onl
-00006350: 7920 6265 2073 6574 2069 6e20 7365 7475  y be set in setu
-00006360: 700a 2020 2020 2320 4475 7269 6e67 205f  p.    # During _
-00006370: 5f68 6173 685f 5f20 616e 6420 5f5f 6571  _hash__ and __eq
-00006380: 5f5f 2074 6865 2066 6965 6c64 2069 7320  __ the field is 
-00006390: 6e6f 7420 7365 7420 7965 740a 2020 2020  not set yet.    
-000063a0: 2320 736f 2069 7420 7368 6f75 6c64 206e  # so it should n
-000063b0: 6f74 2062 6520 7573 6564 2069 6e20 636f  ot be used in co
-000063c0: 6d70 6172 652c 2068 6173 6820 6f72 2072  mpare, hash or r
-000063d0: 6570 722e 0a20 2020 2066 6f72 2066 6965  epr..    for fie
-000063e0: 6c64 2069 6e20 616e 6e6f 7461 7469 6f6e  ld in annotation
-000063f0: 733a 0a20 2020 2020 2066 6965 6c64 5f6d  s:.      field_m
-00006400: 6574 6120 3d20 6765 7461 7474 7228 636c  eta = getattr(cl
-00006410: 732c 2066 6965 6c64 2c20 4e6f 6e65 290a  s, field, None).
-00006420: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00006430: 6e63 6528 6669 656c 645f 6d65 7461 2c20  nce(field_meta, 
-00006440: 6461 7461 636c 6173 7365 732e 4669 656c  dataclasses.Fiel
-00006450: 6429 2061 6e64 206e 6f74 2066 6965 6c64  d) and not field
-00006460: 5f6d 6574 612e 696e 6974 3a0a 2020 2020  _meta.init:.    
-00006470: 2020 2020 6669 656c 645f 6d65 7461 2e63      field_meta.c
-00006480: 6f6d 7061 7265 203d 2046 616c 7365 0a20  ompare = False. 
-00006490: 2020 2020 2020 2066 6965 6c64 5f6d 6574         field_met
-000064a0: 612e 6861 7368 203d 2046 616c 7365 0a20  a.hash = False. 
-000064b0: 2020 2020 2020 2066 6965 6c64 5f6d 6574         field_met
-000064c0: 612e 7265 7072 203d 2046 616c 7365 0a0a  a.repr = False..
-000064d0: 2020 2020 6578 7472 615f 6669 656c 6473      extra_fields
-000064e0: 203d 205b 0a20 2020 2020 2020 2028 0a20   = [.        (. 
-000064f0: 2020 2020 2020 2020 2020 2027 7061 7265             'pare
-00006500: 6e74 272c 0a20 2020 2020 2020 2020 2020  nt',.           
-00006510: 205f 5061 7265 6e74 5479 7065 2c0a 2020   _ParentType,.  
-00006520: 2020 2020 2020 2020 2020 6b77 5f6f 6e6c            kw_onl
-00006530: 795f 6461 7461 636c 6173 7365 732e 6669  y_dataclasses.fi
-00006540: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
-00006550: 2020 2020 2072 6570 723d 4661 6c73 652c       repr=False,
-00006560: 2064 6566 6175 6c74 3d5f 756e 7370 6563   default=_unspec
-00006570: 6966 6965 645f 7061 7265 6e74 2c20 6b77  ified_parent, kw
-00006580: 5f6f 6e6c 793d 5472 7565 0a20 2020 2020  _only=True.     
-00006590: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-000065a0: 2020 292c 0a20 2020 2020 2020 2028 0a20    ),.        (. 
-000065b0: 2020 2020 2020 2020 2020 2027 6e61 6d65             'name
-000065c0: 272c 0a20 2020 2020 2020 2020 2020 204f  ',.            O
-000065d0: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
-000065e0: 2020 2020 2020 2020 2020 6b77 5f6f 6e6c            kw_onl
-000065f0: 795f 6461 7461 636c 6173 7365 732e 6669  y_dataclasses.fi
-00006600: 656c 6428 6465 6661 756c 743d 4e6f 6e65  eld(default=None
-00006610: 2c20 6b77 5f6f 6e6c 793d 5472 7565 292c  , kw_only=True),
-00006620: 0a20 2020 2020 2020 2029 2c0a 2020 2020  .        ),.    
-00006630: 5d0a 0a20 2020 2069 6620 6b77 5f6f 6e6c  ]..    if kw_onl
-00006640: 793a 0a20 2020 2020 2069 6620 7475 706c  y:.      if tupl
-00006650: 6528 7379 732e 7665 7273 696f 6e5f 696e  e(sys.version_in
-00006660: 666f 295b 3a33 5d20 3e3d 2028 332c 2031  fo)[:3] >= (3, 1
-00006670: 302c 2030 293a 0a20 2020 2020 2020 2066  0, 0):.        f
-00006680: 6f72 206e 616d 652c 2061 6e6e 6f74 6174  or name, annotat
-00006690: 696f 6e2c 2064 6566 6175 6c74 2069 6e20  ion, default in 
-000066a0: 6578 7472 615f 6669 656c 6473 3a20 2023  extra_fields:  #
-000066b0: 2070 7974 7970 653a 2064 6973 6162 6c65   pytype: disable
-000066c0: 3d69 6e76 616c 6964 2d61 6e6e 6f74 6174  =invalid-annotat
-000066d0: 696f 6e0a 2020 2020 2020 2020 2020 7365  ion.          se
-000066e0: 7461 7474 7228 636c 732c 206e 616d 652c  tattr(cls, name,
-000066f0: 2064 6566 6175 6c74 290a 2020 2020 2020   default).      
-00006700: 2020 2020 636c 732e 5f5f 616e 6e6f 7461      cls.__annota
-00006710: 7469 6f6e 735f 5f5b 6e61 6d65 5d20 3d20  tions__[name] = 
-00006720: 616e 6e6f 7461 7469 6f6e 0a20 2020 2020  annotation.     
-00006730: 2020 2064 6174 6163 6c61 7373 6573 2e64     dataclasses.d
-00006740: 6174 6163 6c61 7373 2820 2023 2074 7970  ataclass(  # typ
-00006750: 653a 2069 676e 6f72 655b 6361 6c6c 2d6f  e: ignore[call-o
-00006760: 7665 726c 6f61 645d 0a20 2020 2020 2020  verload].       
-00006770: 2020 2020 2075 6e73 6166 655f 6861 7368       unsafe_hash
-00006780: 3d27 5f5f 6861 7368 5f5f 2720 6e6f 7420  ='__hash__' not 
-00006790: 696e 2063 6c73 2e5f 5f64 6963 745f 5f2c  in cls.__dict__,
-000067a0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-000067b0: 723d 4661 6c73 652c 0a20 2020 2020 2020  r=False,.       
-000067c0: 2020 2020 206b 775f 6f6e 6c79 3d54 7275       kw_only=Tru
-000067d0: 652c 0a20 2020 2020 2020 2029 2863 6c73  e,.        )(cls
-000067e0: 290a 2020 2020 2020 656c 7365 3a0a 2020  ).      else:.  
-000067f0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00006800: 4572 726f 7228 2760 6b77 5f6f 6e6c 7960  Error('`kw_only`
-00006810: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-00006820: 6520 6265 666f 7265 2050 7920 332e 3130  e before Py 3.10
-00006830: 2e27 290a 2020 2020 656c 7365 3a0a 2020  .').    else:.  
-00006840: 2020 2020 2320 4e6f 7720 6170 706c 7920      # Now apply 
-00006850: 6461 7461 636c 6173 7320 7472 616e 7366  dataclass transf
-00006860: 6f72 6d20 2877 6869 6368 206f 7065 7261  orm (which opera
-00006870: 7465 7320 696e 2d70 6c61 6365 292e 0a20  tes in-place).. 
-00006880: 2020 2020 2023 2044 6f20 6765 6e65 7261       # Do genera
-00006890: 7465 2061 2068 6173 6820 6675 6e63 7469  te a hash functi
-000068a0: 6f6e 206f 6e6c 7920 6966 206e 6f74 2070  on only if not p
-000068b0: 726f 7669 6465 6420 6279 2074 6865 2063  rovided by the c
-000068c0: 6c61 7373 2e0a 2020 2020 2020 6b77 5f6f  lass..      kw_o
-000068d0: 6e6c 795f 6461 7461 636c 6173 7365 732e  nly_dataclasses.
-000068e0: 6461 7461 636c 6173 7328 0a20 2020 2020  dataclass(.     
-000068f0: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
-00006900: 2020 2020 756e 7361 6665 5f68 6173 683d      unsafe_hash=
-00006910: 275f 5f68 6173 685f 5f27 206e 6f74 2069  '__hash__' not i
-00006920: 6e20 636c 732e 5f5f 6469 6374 5f5f 2c0a  n cls.__dict__,.
-00006930: 2020 2020 2020 2020 2020 7265 7072 3d46            repr=F
-00006940: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00006950: 6578 7472 615f 6669 656c 6473 3d65 7874  extra_fields=ext
-00006960: 7261 5f66 6965 6c64 732c 0a20 2020 2020  ra_fields,.     
-00006970: 2029 2020 2320 7079 7479 7065 3a20 6469   )  # pytype: di
-00006980: 7361 626c 653d 7772 6f6e 672d 6b65 7977  sable=wrong-keyw
-00006990: 6f72 642d 6172 6773 0a0a 2020 2020 636c  ord-args..    cl
-000069a0: 732e 5f5f 6861 7368 5f5f 203d 205f 7772  s.__hash__ = _wr
-000069b0: 6170 5f68 6173 6828 636c 732e 5f5f 6861  ap_hash(cls.__ha
-000069c0: 7368 5f5f 2920 2023 2074 7970 653a 2069  sh__)  # type: i
-000069d0: 676e 6f72 655b 6d65 7468 6f64 2d61 7373  gnore[method-ass
-000069e0: 6967 6e5d 0a0a 2020 4063 6c61 7373 6d65  ign]..  @classme
-000069f0: 7468 6f64 0a20 2064 6566 205f 7665 7269  thod.  def _veri
-00006a00: 6679 5f73 696e 676c 655f 6f72 5f6e 6f5f  fy_single_or_no_
-00006a10: 636f 6d70 6163 7428 636c 7329 3a0a 2020  compact(cls):.  
-00006a20: 2020 2222 2253 7461 7469 6361 6c6c 7920    """Statically 
-00006a30: 7665 7269 6669 6573 2074 6861 7420 6174  verifies that at
-00006a40: 206d 6f73 7420 6120 7369 6e67 6c65 206d   most a single m
-00006a50: 6574 686f 6420 6973 206c 6162 656c 6c65  ethod is labelle
-00006a60: 6420 636f 6d70 6163 742e 2222 220a 2020  d compact.""".  
-00006a70: 2020 6d65 7468 6f64 7320 3d20 5b6d 5b30    methods = [m[0
-00006a80: 5d20 666f 7220 6d20 696e 2069 6e73 7065  ] for m in inspe
-00006a90: 6374 2e67 6574 6d65 6d62 6572 7328 636c  ct.getmembers(cl
-00006aa0: 732c 2070 7265 6469 6361 7465 3d63 616c  s, predicate=cal
-00006ab0: 6c61 626c 6529 5d0a 2020 2020 6e5f 636f  lable)].    n_co
-00006ac0: 6d70 6163 745f 666e 7320 3d20 6c65 6e28  mpact_fns = len(
-00006ad0: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-00006ae0: 2020 2020 2020 206d 6574 686f 645f 6e61         method_na
-00006af0: 6d65 0a20 2020 2020 2020 2020 2020 2066  me.            f
-00006b00: 6f72 206d 6574 686f 645f 6e61 6d65 2069  or method_name i
-00006b10: 6e20 6d65 7468 6f64 730a 2020 2020 2020  n methods.      
-00006b20: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-00006b30: 2867 6574 6174 7472 2863 6c73 2c20 6d65  (getattr(cls, me
-00006b40: 7468 6f64 5f6e 616d 6529 2c20 2763 6f6d  thod_name), 'com
-00006b50: 7061 6374 2729 0a20 2020 2020 2020 205d  pact').        ]
-00006b60: 0a20 2020 2029 0a20 2020 2069 6620 6e5f  .    ).    if n_
-00006b70: 636f 6d70 6163 745f 666e 7320 3e20 313a  compact_fns > 1:
-00006b80: 0a20 2020 2020 2072 6169 7365 2065 7272  .      raise err
-00006b90: 6f72 732e 4d75 6c74 6970 6c65 4d65 7468  ors.MultipleMeth
-00006ba0: 6f64 7343 6f6d 7061 6374 4572 726f 7228  odsCompactError(
-00006bb0: 290a 0a20 2040 636c 6173 736d 6574 686f  )..  @classmetho
-00006bc0: 640a 2020 6465 6620 5f77 7261 705f 6d6f  d.  def _wrap_mo
-00006bd0: 6475 6c65 5f61 7474 7269 6275 7465 7328  dule_attributes(
-00006be0: 636c 7329 3a0a 2020 2020 2222 2257 7261  cls):.    """Wra
-00006bf0: 7073 2075 7365 722d 6465 6669 6e65 6420  ps user-defined 
-00006c00: 6e6f 6e2d 696e 6865 7269 7465 6420 6d65  non-inherited me
-00006c10: 7468 6f64 7320 616e 6420 6465 7363 7269  thods and descri
-00006c20: 7074 6f72 7320 7769 7468 2073 7461 7465  ptors with state
-00006c30: 0a20 2020 206d 616e 6167 656d 656e 7420  .    management 
-00006c40: 6675 6e63 7469 6f6e 732e 0a20 2020 2022  functions..    "
-00006c50: 2222 0a20 2020 2023 2077 7261 7020 6d65  "".    # wrap me
-00006c60: 7468 6f64 730a 2020 2020 6d65 7468 6f64  thods.    method
-00006c70: 5f65 7863 6c75 7369 6f6e 7320 3d20 5b66  _exclusions = [f
-00006c80: 2e6e 616d 6520 666f 7220 6620 696e 2064  .name for f in d
-00006c90: 6174 6163 6c61 7373 6573 2e66 6965 6c64  ataclasses.field
-00006ca0: 7328 636c 7329 5d20 2b20 5b0a 2020 2020  s(cls)] + [.    
-00006cb0: 2020 2020 275f 5f65 715f 5f27 2c0a 2020      '__eq__',.  
-00006cc0: 2020 2020 2020 275f 5f72 6570 725f 5f27        '__repr__'
-00006cd0: 2c0a 2020 2020 2020 2020 275f 5f69 6e69  ,.        '__ini
-00006ce0: 745f 5f27 2c0a 2020 2020 2020 2020 275f  t__',.        '_
-00006cf0: 5f68 6173 685f 5f27 2c0a 2020 2020 2020  _hash__',.      
-00006d00: 2020 275f 5f70 6f73 745f 696e 6974 5f5f    '__post_init__
-00006d10: 272c 0a20 2020 205d 0a20 2020 2066 6f72  ',.    ].    for
-00006d20: 206b 6579 2069 6e20 5f67 6574 5f6c 6f63   key in _get_loc
-00006d30: 616c 5f6d 6574 686f 645f 6e61 6d65 7328  al_method_names(
-00006d40: 636c 732c 2065 7863 6c75 6465 3d6d 6574  cls, exclude=met
-00006d50: 686f 645f 6578 636c 7573 696f 6e73 293a  hod_exclusions):
-00006d60: 0a20 2020 2020 206d 6574 686f 6420 3d20  .      method = 
-00006d70: 6765 7461 7474 7228 636c 732c 206b 6579  getattr(cls, key
-00006d80: 290a 2020 2020 2020 6966 2068 6173 6174  ).      if hasat
-00006d90: 7472 286d 6574 686f 642c 2027 6e6f 7772  tr(method, 'nowr
-00006da0: 6170 2729 3a0a 2020 2020 2020 2020 636f  ap'):.        co
-00006db0: 6e74 696e 7565 0a20 2020 2020 2073 6574  ntinue.      set
-00006dc0: 6174 7472 2863 6c73 2c20 6b65 792c 2077  attr(cls, key, w
-00006dd0: 7261 705f 6d65 7468 6f64 5f6f 6e63 6528  rap_method_once(
-00006de0: 6d65 7468 6f64 2929 0a0a 2020 2020 2320  method))..    # 
-00006df0: 7772 6170 2064 6573 6372 6970 746f 7273  wrap descriptors
-00006e00: 0a20 2020 2064 6573 6372 6970 746f 725f  .    descriptor_
-00006e10: 6578 636c 7573 696f 6e73 203d 205b 662e  exclusions = [f.
-00006e20: 6e61 6d65 2066 6f72 2066 2069 6e20 6461  name for f in da
-00006e30: 7461 636c 6173 7365 732e 6669 656c 6473  taclasses.fields
-00006e40: 2863 6c73 295d 202b 205b 0a20 2020 2020  (cls)] + [.     
-00006e50: 2020 2027 7061 7265 6e74 272c 0a20 2020     'parent',.   
-00006e60: 2020 2020 2027 5f5f 6469 6374 5f5f 272c       '__dict__',
-00006e70: 0a20 2020 205d 0a20 2020 2066 6f72 206b  .    ].    for k
-00006e80: 6579 2069 6e20 5f67 6574 5f6c 6f63 616c  ey in _get_local
-00006e90: 5f64 6573 6372 6970 746f 725f 6e61 6d65  _descriptor_name
-00006ea0: 7328 636c 732c 2064 6573 6372 6970 746f  s(cls, descripto
-00006eb0: 725f 6578 636c 7573 696f 6e73 293a 0a20  r_exclusions):. 
-00006ec0: 2020 2020 2023 2064 6f6e 2774 2075 7365       # don't use
-00006ed0: 2067 6574 6174 7472 2068 6572 652c 2073   getattr here, s
-00006ee0: 696e 6365 2069 7420 7769 6c6c 2063 616c  ince it will cal
-00006ef0: 6c20 7468 6520 6465 7363 7269 7074 6f72  l the descriptor
-00006f00: 0a20 2020 2020 2064 6573 6372 6970 746f  .      descripto
-00006f10: 7220 3d20 636c 732e 5f5f 6469 6374 5f5f  r = cls.__dict__
-00006f20: 5b6b 6579 5d0a 2020 2020 2020 6966 2068  [key].      if h
-00006f30: 6173 6174 7472 2864 6573 6372 6970 746f  asattr(descripto
-00006f40: 722c 2027 6e6f 7772 6170 2729 3a0a 2020  r, 'nowrap'):.  
-00006f50: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00006f60: 2020 2020 2073 6574 6174 7472 2863 6c73       setattr(cls
-00006f70: 2c20 6b65 792c 2077 7261 705f 6465 7363  , key, wrap_desc
-00006f80: 7269 7074 6f72 5f6f 6e63 6528 6465 7363  riptor_once(desc
-00006f90: 7269 7074 6f72 2929 0a20 2020 2072 6574  riptor)).    ret
-00006fa0: 7572 6e20 636c 730a 0a20 2064 6566 205f  urn cls..  def _
-00006fb0: 6361 6c6c 5f77 7261 7070 6564 5f6d 6574  call_wrapped_met
-00006fc0: 686f 6428 7365 6c66 2c20 6675 6e2c 2061  hod(self, fun, a
-00006fd0: 7267 732c 206b 7761 7267 7329 3a0a 2020  rgs, kwargs):.  
-00006fe0: 2020 2222 2220 2243 616c 6c73 2061 2077    """ "Calls a w
-00006ff0: 7261 7070 6564 206d 6574 686f 642e 0a0a  rapped method...
-00007000: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-00007010: 6e20 6973 2072 6573 706f 6e73 6962 6c65  n is responsible
-00007020: 2066 6f72 2073 6574 7469 6e67 2075 7020   for setting up 
-00007030: 7468 6520 7468 7265 6164 206c 6f63 616c  the thread local
-00007040: 2073 7461 7465 0a20 2020 2063 6f72 7265   state.    corre
-00007050: 6374 6c79 2062 6566 6f72 6520 6361 6c6c  ctly before call
-00007060: 696e 6720 7468 6520 6d65 7468 6f64 2061  ing the method a
-00007070: 6e64 2063 6c65 616e 696e 6720 7570 2061  nd cleaning up a
-00007080: 6674 6572 7761 7264 732e 0a20 2020 2054  fterwards..    T
-00007090: 6869 7320 696e 636c 7564 6573 2073 746f  his includes sto
-000070a0: 7269 6e67 2069 6e74 6572 6d65 6469 6174  ring intermediat
-000070b0: 6573 2c20 7365 7475 7020 6f66 2074 6865  es, setup of the
-000070c0: 2063 6f6d 7061 6374 2073 636f 7065 2c0a   compact scope,.
-000070d0: 2020 2020 616e 6420 6d61 6b69 6e67 2073      and making s
-000070e0: 7572 6520 7365 7475 7020 6973 2063 616c  ure setup is cal
-000070f0: 6c65 6420 6265 666f 7265 2061 6e79 206f  led before any o
-00007100: 7468 6572 206d 6574 686f 642e 0a0a 2020  ther method...  
-00007110: 2020 4172 6773 3a0a 2020 2020 2020 6675    Args:.      fu
-00007120: 6e3a 2054 6865 2077 7261 7070 6564 206d  n: The wrapped m
-00007130: 6574 686f 642e 0a20 2020 2020 2061 7267  ethod..      arg
-00007140: 733a 204e 616d 6564 2061 7267 756d 656e  s: Named argumen
-00007150: 7473 2070 6173 7365 6420 746f 2060 6066  ts passed to ``f
-00007160: 756e 6060 2e0a 2020 2020 2020 6b77 6172  un``..      kwar
-00007170: 6773 3a20 4b65 7977 6f72 6420 6172 6775  gs: Keyword argu
-00007180: 6d65 6e74 7320 7061 7373 6564 2074 6f20  ments passed to 
-00007190: 6060 6675 6e60 602e 0a0a 2020 2020 5265  ``fun``...    Re
-000071a0: 7475 726e 733a 0a20 2020 2020 2054 6865  turns:.      The
-000071b0: 2072 6573 756c 7473 206f 6620 6361 6c6c   results of call
-000071c0: 696e 6720 6060 6675 6e60 602e 0a20 2020  ing ``fun``..   
-000071d0: 2022 2222 0a20 2020 2069 735f 636f 6d70   """.    is_comp
-000071e0: 6163 745f 6d65 7468 6f64 203d 2068 6173  act_method = has
-000071f0: 6174 7472 2866 756e 2c20 2763 6f6d 7061  attr(fun, 'compa
-00007200: 6374 2729 0a20 2020 2066 756e 5f6e 616d  ct').    fun_nam
-00007210: 6520 3d20 6765 7461 7474 7228 6675 6e2c  e = getattr(fun,
-00007220: 2027 5f5f 6e61 6d65 5f5f 272c 2027 756e   '__name__', 'un
-00007230: 6e61 6d65 645f 6675 6e63 7469 6f6e 2729  named_function')
-00007240: 0a20 2020 2069 735f 7365 7475 705f 6d65  .    is_setup_me
-00007250: 7468 6f64 203d 2066 756e 5f6e 616d 6520  thod = fun_name 
-00007260: 3d3d 2027 7365 7475 7027 0a20 2020 2061  == 'setup'.    a
-00007270: 6464 5f63 616c 6c5f 696e 666f 203d 206e  dd_call_info = n
-00007280: 6f74 2069 735f 7365 7475 705f 6d65 7468  ot is_setup_meth
-00007290: 6f64 2061 6e64 206c 656e 285f 636f 6e74  od and len(_cont
-000072a0: 6578 742e 6361 6c6c 5f69 6e66 6f5f 7374  ext.call_info_st
-000072b0: 6163 6b29 203e 2030 0a20 2020 2023 2057  ack) > 0.    # W
-000072c0: 6520 6c61 7a69 6c79 2063 616c 6c20 7365  e lazily call se
-000072d0: 7475 7028 2920 6f6e 6c79 2077 6865 6e20  tup() only when 
-000072e0: 6e65 6564 6564 2e0a 2020 2020 6966 2069  needed..    if i
-000072f0: 735f 7365 7475 705f 6d65 7468 6f64 3a0a  s_setup_method:.
-00007300: 2020 2020 2020 6966 2073 656c 662e 7363        if self.sc
-00007310: 6f70 6520 6973 204e 6f6e 653a 0a20 2020  ope is None:.   
-00007320: 2020 2020 2072 6169 7365 2065 7272 6f72       raise error
-00007330: 732e 4361 6c6c 5365 7475 7055 6e62 6f75  s.CallSetupUnbou
-00007340: 6e64 4d6f 6475 6c65 4572 726f 7228 290a  ndModuleError().
-00007350: 2020 2020 2020 6973 5f72 6563 7572 7265        is_recurre
-00007360: 6e74 203d 2073 656c 662e 5f73 7461 7465  nt = self._state
-00007370: 2e69 6e5f 7365 7475 700a 2020 2020 2020  .in_setup.      
-00007380: 7365 6c66 2e5f 7374 6174 652e 696e 5f73  self._state.in_s
-00007390: 6574 7570 203d 2054 7275 650a 2020 2020  etup = True.    
-000073a0: 656c 7365 3a0a 2020 2020 2020 7365 6c66  else:.      self
-000073b0: 2e5f 7472 795f 7365 7475 7028 290a 0a20  ._try_setup().. 
-000073c0: 2020 2069 6620 6973 5f63 6f6d 7061 6374     if is_compact
-000073d0: 5f6d 6574 686f 643a 0a20 2020 2020 2069  _method:.      i
-000073e0: 6620 7365 6c66 2e73 636f 7065 2069 7320  f self.scope is 
-000073f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7261  None:.        ra
-00007400: 6973 6520 6572 726f 7273 2e43 616c 6c43  ise errors.CallC
-00007410: 6f6d 7061 6374 556e 626f 756e 644d 6f64  ompactUnboundMod
-00007420: 756c 6545 7272 6f72 2829 0a20 2020 2020  uleError().     
-00007430: 2069 735f 7265 6375 7272 656e 7420 3d20   is_recurrent = 
-00007440: 7365 6c66 2e5f 7374 6174 652e 696e 5f63  self._state.in_c
-00007450: 6f6d 7061 6374 5f6d 6574 686f 640a 2020  ompact_method.  
-00007460: 2020 2020 7365 6c66 2e5f 7374 6174 652e      self._state.
-00007470: 696e 5f63 6f6d 7061 6374 5f6d 6574 686f  in_compact_metho
-00007480: 6420 3d20 5472 7565 0a20 2020 205f 636f  d = True.    _co
-00007490: 6e74 6578 742e 6d6f 6475 6c65 5f73 7461  ntext.module_sta
-000074a0: 636b 2e61 7070 656e 6428 7365 6c66 290a  ck.append(self).
-000074b0: 2020 2020 7472 793a 0a20 2020 2020 2023      try:.      #
-000074c0: 2067 6574 2063 616c 6c20 696e 666f 0a20   get call info. 
-000074d0: 2020 2020 2069 6620 6164 645f 6361 6c6c       if add_call
-000074e0: 5f69 6e66 6f3a 0a20 2020 2020 2020 2061  _info:.        a
-000074f0: 7373 6572 7420 7365 6c66 2e73 636f 7065  ssert self.scope
-00007500: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00007510: 2020 2020 2063 616c 6c5f 696e 6465 7820       call_index 
-00007520: 3d20 5f63 6f6e 7465 7874 2e63 616c 6c5f  = _context.call_
-00007530: 696e 666f 5f73 7461 636b 5b2d 315d 2e67  info_stack[-1].g
-00007540: 6574 5f63 616c 6c5f 696e 6465 7828 7365  et_call_index(se
-00007550: 6c66 290a 2020 2020 2020 2020 7363 6f70  lf).        scop
-00007560: 655f 7061 7468 203d 206a 6178 2e74 7265  e_path = jax.tre
-00007570: 655f 7574 696c 2e74 7265 655f 6d61 7028  e_util.tree_map(
-00007580: 5f66 6978 5f70 6174 685f 7061 7274 2c20  _fix_path_part, 
-00007590: 7365 6c66 2e73 636f 7065 2e70 6174 6829  self.scope.path)
-000075a0: 0a0a 2020 2020 2020 2320 6361 6c6c 206d  ..      # call m
-000075b0: 6574 686f 640a 2020 2020 2020 6966 205f  ethod.      if _
-000075c0: 7573 655f 6e61 6d65 645f 6361 6c6c 3a0a  use_named_call:.
-000075d0: 2020 2020 2020 2020 7769 7468 206a 6178          with jax
-000075e0: 2e6e 616d 6564 5f73 636f 7065 285f 6465  .named_scope(_de
-000075f0: 7269 7665 5f70 726f 6669 6c69 6e67 5f6e  rive_profiling_n
-00007600: 616d 6528 7365 6c66 2c20 6675 6e29 293a  ame(self, fun)):
-00007610: 0a20 2020 2020 2020 2020 2079 203d 2066  .          y = f
-00007620: 756e 2873 656c 662c 202a 6172 6773 2c20  un(self, *args, 
-00007630: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-00007640: 656c 7365 3a0a 2020 2020 2020 2020 7920  else:.        y 
-00007650: 3d20 6675 6e28 7365 6c66 2c20 2a61 7267  = fun(self, *arg
-00007660: 732c 202a 2a6b 7761 7267 7329 0a0a 2020  s, **kwargs)..  
-00007670: 2020 2020 6966 205f 636f 6e74 6578 742e      if _context.
-00007680: 6361 7074 7572 655f 7374 6163 6b3a 0a20  capture_stack:. 
-00007690: 2020 2020 2020 2066 696c 7465 725f 666e         filter_fn
-000076a0: 203d 205f 636f 6e74 6578 742e 6361 7074   = _context.capt
-000076b0: 7572 655f 7374 6163 6b5b 2d31 5d0a 2020  ure_stack[-1].  
-000076c0: 2020 2020 2020 6966 2066 696c 7465 725f        if filter_
-000076d0: 666e 2061 6e64 2066 696c 7465 725f 666e  fn and filter_fn
-000076e0: 2873 656c 662c 2066 756e 5f6e 616d 6529  (self, fun_name)
-000076f0: 3a0a 2020 2020 2020 2020 2020 7365 6c66  :.          self
-00007700: 2e73 6f77 2827 696e 7465 726d 6564 6961  .sow('intermedia
-00007710: 7465 7327 2c20 6675 6e5f 6e61 6d65 2c20  tes', fun_name, 
-00007720: 7929 0a20 2020 2020 2069 6620 6164 645f  y).      if add_
-00007730: 6361 6c6c 5f69 6e66 6f3a 0a20 2020 2020  call_info:.     
-00007740: 2020 205f 6172 6773 2c20 5f6b 7761 7267     _args, _kwarg
-00007750: 732c 205f 7920 3d20 666c 6178 2e6c 696e  s, _y = flax.lin
-00007760: 656e 2e73 756d 6d61 7279 2e5f 7265 7072  en.summary._repr
-00007770: 6573 656e 745f 7472 6565 280a 2020 2020  esent_tree(.    
-00007780: 2020 2020 2020 2020 2861 7267 732c 206b          (args, k
-00007790: 7761 7267 732c 2079 290a 2020 2020 2020  wargs, y).      
-000077a0: 2020 290a 2020 2020 2020 2020 5f63 6f6e    ).        _con
-000077b0: 7465 7874 2e63 616c 6c5f 696e 666f 5f73  text.call_info_s
-000077c0: 7461 636b 5b2d 315d 2e63 616c 6c73 2e61  tack[-1].calls.a
-000077d0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-000077e0: 2020 205f 4361 6c6c 496e 666f 280a 2020     _CallInfo(.  
-000077f0: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00007800: 6c6c 5f69 6e64 6578 2c0a 2020 2020 2020  ll_index,.      
-00007810: 2020 2020 2020 2020 2020 7363 6f70 655f            scope_
-00007820: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
-00007830: 2020 2020 2020 7479 7065 2873 656c 6629        type(self)
-00007840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007850: 2020 6675 6e2e 5f5f 6e61 6d65 5f5f 2c0a    fun.__name__,.
-00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007870: 5f61 7267 732c 0a20 2020 2020 2020 2020  _args,.         
-00007880: 2020 2020 2020 205f 6b77 6172 6773 2c0a         _kwargs,.
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 5f79 2c0a 2020 2020 2020 2020 2020 2020  _y,.            
-000078b0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-000078c0: 2020 7265 7475 726e 2079 0a20 2020 2066    return y.    f
-000078d0: 696e 616c 6c79 3a0a 2020 2020 2020 5f63  inally:.      _c
-000078e0: 6f6e 7465 7874 2e6d 6f64 756c 655f 7374  ontext.module_st
-000078f0: 6163 6b2e 706f 7028 290a 2020 2020 2020  ack.pop().      
-00007900: 6966 2069 735f 636f 6d70 6163 745f 6d65  if is_compact_me
-00007910: 7468 6f64 3a0a 2020 2020 2020 2020 6f62  thod:.        ob
-00007920: 6a65 6374 2e5f 5f73 6574 6174 7472 5f5f  ject.__setattr__
-00007930: 2873 656c 662c 2027 7363 6f70 6527 2c20  (self, 'scope', 
-00007940: 7365 6c66 2e73 636f 7065 2e72 6577 6f75  self.scope.rewou
-00007950: 6e64 2829 290a 2020 2020 2020 2320 7365  nd()).      # se
-00007960: 7475 7020 6f72 2063 6f6d 7061 6374 2063  tup or compact c
-00007970: 616c 6c73 2063 616e 2062 6520 7265 6375  alls can be recu
-00007980: 7272 656e 7420 666f 7220 6578 616d 706c  rrent for exampl
-00007990: 6520 6475 6520 746f 2073 7570 6572 2063  e due to super c
-000079a0: 616c 6c73 0a20 2020 2020 2023 2072 6573  alls.      # res
-000079b0: 6574 7469 6e67 2074 6865 2073 7461 7465  etting the state
-000079c0: 2077 6f75 6c64 2063 6175 7365 2069 7320   would cause is 
-000079d0: 636f 6d70 6163 742f 7365 7475 7020 6d65  compact/setup me
-000079e0: 7468 6f64 0a20 2020 2020 2023 2074 6f20  thod.      # to 
-000079f0: 6265 2073 6574 2074 6f20 4661 6c73 6520  be set to False 
-00007a00: 7072 656d 6174 7572 656c 792e 0a20 2020  prematurely..   
-00007a10: 2020 2069 6620 2869 735f 636f 6d70 6163     if (is_compac
-00007a20: 745f 6d65 7468 6f64 206f 7220 6973 5f73  t_method or is_s
-00007a30: 6574 7570 5f6d 6574 686f 6429 2061 6e64  etup_method) and
-00007a40: 206e 6f74 2069 735f 7265 6375 7272 656e   not is_recurren
-00007a50: 743a 0a20 2020 2020 2020 2073 656c 662e  t:.        self.
-00007a60: 5f73 7461 7465 2e72 6573 6574 2829 0a0a  _state.reset()..
-00007a70: 2020 6465 6620 5f5f 7365 7461 7474 725f    def __setattr_
-00007a80: 5f28 7365 6c66 2c20 6e61 6d65 3a20 7374  _(self, name: st
-00007a90: 722c 2076 616c 3a20 416e 7929 3a0a 2020  r, val: Any):.  
-00007aa0: 2020 2222 2253 6574 7320 616e 2061 7474    """Sets an att
-00007ab0: 7269 6275 7465 206f 6e20 7468 6973 204d  ribute on this M
-00007ac0: 6f64 756c 652e 0a0a 2020 2020 5765 206f  odule...    We o
-00007ad0: 7665 726c 6f61 6420 7365 7461 7474 7220  verload setattr 
-00007ae0: 736f 6c65 6c79 2074 6f20 7375 7070 6f72  solely to suppor
-00007af0: 7420 7079 7468 6f6e 6963 206e 616d 696e  t pythonic namin
-00007b00: 6720 7669 6120 6173 7369 676e 6d65 6e74  g via assignment
-00007b10: 206f 660a 2020 2020 7375 626d 6f64 756c   of.    submodul
-00007b20: 6573 2069 6e20 7468 6520 7370 6563 6961  es in the specia
-00007b30: 6c20 3a6d 6574 683a 6073 6574 7570 6020  l :meth:`setup` 
-00007b40: 6675 6e63 7469 6f6e 3a3a 0a0a 2020 2020  function::..    
-00007b50: 2020 7365 6c66 2e73 7562 6d6f 6475 6c65    self.submodule
-00007b60: 5f6e 616d 6520 3d20 4d79 4d6f 6475 6c65  _name = MyModule
-00007b70: 282e 2e2e 290a 0a20 2020 2057 6520 616c  (...)..    We al
-00007b80: 736f 2073 7570 706f 7274 206c 6973 7473  so support lists
-00007b90: 2061 6e64 206f 7468 6572 2067 656e 6572   and other gener
-00007ba0: 616c 2070 7974 7265 6573 2c20 652e 672e  al pytrees, e.g.
-00007bb0: 3a3a 0a0a 2020 2020 2020 7365 6c66 2e73  ::..      self.s
-00007bc0: 7562 6d6f 6475 6c65 7320 3d20 5b4d 794d  ubmodules = [MyM
-00007bd0: 6f64 756c 6530 282e 2e29 2c20 4d79 4d6f  odule0(..), MyMo
-00007be0: 6475 6c65 3128 2e2e 292c 202e 2e2e 5d0a  dule1(..), ...].
-00007bf0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00007c00: 206e 616d 653a 2041 7474 7269 6275 7465   name: Attribute
-00007c10: 2074 6f20 7365 742e 0a20 2020 2020 2076   to set..      v
-00007c20: 616c 3a20 5661 6c75 6520 6f66 2074 6865  al: Value of the
-00007c30: 2061 7474 7269 6275 7465 2e0a 2020 2020   attribute..    
-00007c40: 2222 220a 2020 2020 6669 656c 6473 203d  """.    fields =
-00007c50: 2073 656c 662e 5f5f 6461 7461 636c 6173   self.__dataclas
-00007c60: 735f 6669 656c 6473 5f5f 2020 2320 7079  s_fields__  # py
-00007c70: 7479 7065 3a20 6469 7361 626c 653d 6174  type: disable=at
-00007c80: 7472 6962 7574 652d 6572 726f 720a 2020  tribute-error.  
-00007c90: 2020 6973 5f64 6174 6163 6c61 7373 5f61    is_dataclass_a
-00007ca0: 7474 7220 3d20 6e61 6d65 2069 6e20 6669  ttr = name in fi
-00007cb0: 656c 6473 2061 6e64 2066 6965 6c64 735b  elds and fields[
-00007cc0: 6e61 6d65 5d2e 696e 6974 0a0a 2020 2020  name].init..    
-00007cd0: 6966 206e 6f74 2073 656c 662e 5f73 7461  if not self._sta
-00007ce0: 7465 2e69 6e5f 7365 7475 703a 0a20 2020  te.in_setup:.   
-00007cf0: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-00007d00: 7374 6174 652e 6973 5f69 6e69 7469 616c  state.is_initial
-00007d10: 697a 6564 3a0a 2020 2020 2020 2020 2320  ized:.        # 
-00007d20: 5365 7474 696e 6720 6174 7472 6962 7574  Setting attribut
-00007d30: 6573 2062 6566 6f72 6520 656e 6420 6f66  es before end of
-00007d40: 204d 6f64 756c 652e 5f5f 706f 7374 5f69   Module.__post_i
-00007d50: 6e69 745f 5f28 290a 2020 2020 2020 2020  nit__().        
-00007d60: 6f62 6a65 6374 2e5f 5f73 6574 6174 7472  object.__setattr
-00007d70: 5f5f 2873 656c 662c 206e 616d 652c 2076  __(self, name, v
-00007d80: 616c 290a 2020 2020 2020 2020 7265 7475  al).        retu
-00007d90: 726e 0a20 2020 2020 2065 6c73 653a 0a20  rn.      else:. 
-00007da0: 2020 2020 2020 2023 2057 6527 7265 2070         # We're p
-00007db0: 6173 7420 616c 6c20 696e 6974 6961 6c69  ast all initiali
-00007dc0: 7a61 7469 6f6e 2061 6e64 2073 6574 7570  zation and setup
-00007dd0: 206c 6f67 6963 3a0a 2020 2020 2020 2020   logic:.        
-00007de0: 2320 5261 6973 6573 2061 2054 7970 6545  # Raises a TypeE
-00007df0: 7272 6f72 206a 7573 7420 6c69 6b65 2066  rror just like f
-00007e00: 726f 7a65 6e20 7079 7468 6f6e 2064 6174  rozen python dat
-00007e10: 6163 6c61 7373 6573 2e0a 2020 2020 2020  aclasses..      
-00007e20: 2020 7261 6973 6520 6572 726f 7273 2e53    raise errors.S
-00007e30: 6574 4174 7472 6962 7574 6546 726f 7a65  etAttributeFroze
-00007e40: 6e4d 6f64 756c 6545 7272 6f72 280a 2020  nModuleError(.  
-00007e50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00007e60: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
-00007e70: 5f2c 206e 616d 652c 2076 616c 0a20 2020  _, name, val.   
-00007e80: 2020 2020 2029 0a0a 2020 2020 2320 5765       )..    # We
-00007e90: 2772 6520 696e 7369 6465 2074 6865 2073  're inside the s
-00007ea0: 6574 7570 2829 206d 6574 686f 643a 0a20  etup() method:. 
-00007eb0: 2020 2069 6620 6973 5f64 6174 6163 6c61     if is_datacla
-00007ec0: 7373 5f61 7474 723a 0a20 2020 2020 2023  ss_attr:.      #
-00007ed0: 2054 6865 7365 206e 616d 6573 2061 7265   These names are
-00007ee0: 2073 7065 6369 6669 6564 2061 7320 6461   specified as da
-00007ef0: 7461 636c 6173 7320 6669 656c 6473 2e20  taclass fields. 
-00007f00: 5468 6579 2073 686f 756c 6420 6e6f 7420  They should not 
-00007f10: 6265 0a20 2020 2020 2023 2069 6e69 7469  be.      # initi
-00007f20: 616c 697a 6564 2077 6974 6869 6e20 7468  alized within th
-00007f30: 6520 7365 7475 7028 2920 6d65 7468 6f64  e setup() method
-00007f40: 2c20 6275 7420 6361 6e20 6265 206d 6f64  , but can be mod
-00007f50: 6966 6965 6420 6672 6565 6c79 0a20 2020  ified freely.   
-00007f60: 2020 2023 2062 6566 6f72 6520 6974 2e0a     # before it..
-00007f70: 2020 2020 2020 7261 6973 6520 6572 726f        raise erro
-00007f80: 7273 2e53 6574 4174 7472 6962 7574 6549  rs.SetAttributeI
-00007f90: 6e4d 6f64 756c 6553 6574 7570 4572 726f  nModuleSetupErro
-00007fa0: 7228 290a 0a20 2020 2023 2056 616c 7565  r()..    # Value
-00007fb0: 7320 2874 6861 7420 6d61 7920 6265 2076  s (that may be v
-00007fc0: 6172 6961 626c 6573 206f 7220 7375 626d  ariables or subm
-00007fd0: 6f64 756c 6573 2920 6172 6520 6265 696e  odules) are bein
-00007fe0: 6720 6465 6669 6e65 6420 616e 640a 2020  g defined and.  
-00007ff0: 2020 2320 6174 7461 6368 6564 2069 6e20    # attached in 
-00008000: 7365 7475 7028 292c 2077 6520 7275 6e20  setup(), we run 
-00008010: 736f 6d65 2065 7874 7261 206c 6f67 6963  some extra logic
-00008020: 2069 6e20 7468 6174 2063 6173 652e 0a20   in that case.. 
-00008030: 2020 2073 656c 662e 5f72 6567 6973 7465     self._registe
-00008040: 725f 7375 626d 6f64 756c 6573 286e 616d  r_submodules(nam
-00008050: 652c 2076 616c 290a 0a20 2064 6566 205f  e, val)..  def _
-00008060: 5f67 6574 6174 7472 5f5f 2873 656c 662c  _getattr__(self,
-00008070: 206e 616d 653a 2073 7472 2920 2d3e 2041   name: str) -> A
-00008080: 6e79 3a0a 2020 2020 2222 2243 616c 6c20  ny:.    """Call 
-00008090: 7365 7475 7028 2920 6265 666f 7265 2067  setup() before g
-000080a0: 6574 7469 6e67 2061 6e79 2073 6574 7570  etting any setup
-000080b0: 2d64 6566 696e 6564 2061 7474 7269 6275  -defined attribu
-000080c0: 7465 732e 2222 220a 2020 2020 2320 5765  tes.""".    # We
-000080d0: 2064 6f6e 2774 2077 616e 7420 746f 2072   don't want to r
-000080e0: 6574 7572 6e20 616e 7974 6869 6e67 2066  eturn anything f
-000080f0: 6f72 2070 7974 686f 6e20 636f 7079 202f  or python copy /
-00008100: 2070 6963 6b6c 6520 6d65 7468 6f64 732e   pickle methods.
-00008110: 0a20 2020 2069 6620 6e61 6d65 2069 6e20  .    if name in 
-00008120: 5f55 4e44 4546 494e 4544 5f43 4f50 595f  _UNDEFINED_COPY_
-00008130: 5049 434b 4c45 5f4d 4554 484f 4453 3a0a  PICKLE_METHODS:.
-00008140: 2020 2020 2020 7261 6973 6520 4174 7472        raise Attr
-00008150: 6962 7574 6545 7272 6f72 2829 0a20 2020  ibuteError().   
-00008160: 2073 656c 662e 5f74 7279 5f73 6574 7570   self._try_setup
-00008170: 2829 0a20 2020 2069 6620 6e61 6d65 2069  ().    if name i
-00008180: 6e20 7365 6c66 2e5f 5f64 6963 745f 5f3a  n self.__dict__:
-00008190: 0a20 2020 2020 2072 6574 7572 6e20 7365  .      return se
-000081a0: 6c66 2e5f 5f64 6963 745f 5f5b 6e61 6d65  lf.__dict__[name
-000081b0: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
-000081c0: 2020 6d73 6720 3d20 6627 227b 7365 6c66    msg = f'"{self
-000081d0: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-000081e0: 655f 5f7d 2220 6f62 6a65 6374 2068 6173  e__}" object has
-000081f0: 206e 6f20 6174 7472 6962 7574 6520 227b   no attribute "{
-00008200: 6e61 6d65 7d22 2e27 0a20 2020 2020 2069  name}".'.      i
-00008210: 6620 7365 6c66 2e73 636f 7065 2069 7320  f self.scope is 
-00008220: 4e6f 6e65 3a0a 2020 2020 2020 2020 6d73  None:.        ms
-00008230: 6720 2b3d 2028 0a20 2020 2020 2020 2020  g += (.         
-00008240: 2020 2066 2720 4966 2022 7b6e 616d 657d     f' If "{name}
-00008250: 2220 6973 2064 6566 696e 6564 2069 6e20  " is defined in 
-00008260: 5c27 2e73 6574 7570 2829 5c27 2c20 7265  \'.setup()\', re
-00008270: 6d65 6d62 6572 2074 6865 7365 2066 6965  member these fie
-00008280: 6c64 7320 270a 2020 2020 2020 2020 2020  lds '.          
-00008290: 2020 2261 7265 206f 6e6c 7920 6163 6365    "are only acce
-000082a0: 7373 6962 6c65 2066 726f 6d20 696e 7369  ssible from insi
-000082b0: 6465 2027 696e 6974 2720 6f72 2027 6170  de 'init' or 'ap
-000082c0: 706c 7927 2e22 0a20 2020 2020 2020 2029  ply'.".        )
-000082d0: 0a20 2020 2020 2072 6169 7365 2041 7474  .      raise Att
-000082e0: 7269 6275 7465 4572 726f 7228 6d73 6729  ributeError(msg)
-000082f0: 0a0a 2020 6465 6620 5f5f 6469 725f 5f28  ..  def __dir__(
-00008300: 7365 6c66 2920 2d3e 204c 6973 745b 7374  self) -> List[st
-00008310: 725d 3a0a 2020 2020 2222 2243 616c 6c20  r]:.    """Call 
-00008320: 7365 7475 7028 2920 6265 666f 7265 206c  setup() before l
-00008330: 6973 7469 6e67 2061 7474 7269 6275 7465  isting attribute
-00008340: 732e 2222 220a 2020 2020 7365 6c66 2e5f  s.""".    self._
-00008350: 7472 795f 7365 7475 7028 290a 2020 2020  try_setup().    
-00008360: 7265 7475 726e 206f 626a 6563 742e 5f5f  return object.__
-00008370: 6469 725f 5f28 7365 6c66 2920 2023 2074  dir__(self)  # t
-00008380: 7970 653a 2069 676e 6f72 650a 0a20 2064  ype: ignore..  d
-00008390: 6566 205f 5f70 6f73 745f 696e 6974 5f5f  ef __post_init__
-000083a0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000083b0: 2020 2020 2320 444f 204e 4f54 2052 454d      # DO NOT REM
-000083c0: 4f56 4520 2d20 4d61 726b 6572 2066 6f72  OVE - Marker for
-000083d0: 2069 6e74 6572 6e61 6c20 6c6f 6767 696e   internal loggin
-000083e0: 672e 0a20 2020 2023 2049 6e20 6461 7461  g..    # In data
-000083f0: 636c 6173 7365 732c 205f 5f69 6e69 745f  classes, __init_
-00008400: 5f20 6973 206f 7665 7272 6964 6465 6e20  _ is overridden 
-00008410: 746f 2070 726f 6365 7373 2064 6174 6163  to process datac
-00008420: 6c61 7373 2061 7267 756d 656e 7473 2c0a  lass arguments,.
-00008430: 2020 2020 2320 616e 6420 5f5f 706f 7374      # and __post
-00008440: 5f69 6e69 745f 5f20 6973 2063 616c 6c65  _init__ is calle
-00008450: 6420 696d 6d65 6469 6174 656c 7920 6166  d immediately af
-00008460: 7465 7277 6172 6473 2e20 4865 7265 2c20  terwards. Here, 
-00008470: 6465 7065 6e64 696e 6720 6f6e 2074 6865  depending on the
-00008480: 0a20 2020 2023 2074 7970 6520 6f66 2060  .    # type of `
-00008490: 7061 7265 6e74 6020 7061 7373 6564 2074  parent` passed t
-000084a0: 6f20 696e 6974 6961 6c69 7a65 2074 6865  o initialize the
-000084b0: 204d 6f64 756c 652c 2077 6520 6569 7468   Module, we eith
-000084c0: 6572 2064 6566 6572 0a20 2020 2023 2069  er defer.    # i
-000084d0: 6e69 7469 616c 697a 6174 696f 6e2c 2061  nitialization, a
-000084e0: 7474 6163 6820 7468 6973 204d 6f64 756c  ttach this Modul
-000084f0: 6520 6173 2061 2073 7562 6d6f 6475 6c65  e as a submodule
-00008500: 206f 6620 6120 7061 7265 6e74 2c20 6f72   of a parent, or
-00008510: 2062 696e 640a 2020 2020 2320 7468 6973   bind.    # this
-00008520: 204d 6f64 756c 6520 6174 2074 6865 2074   Module at the t
-00008530: 6f70 2d6c 6576 656c 2074 6f20 7661 7269  op-level to vari
-00008540: 6162 6c65 7320 616e 6420 726e 6773 2e0a  ables and rngs..
-00008550: 0a20 2020 206f 626a 6563 742e 5f5f 7365  .    object.__se
-00008560: 7461 7474 725f 5f28 7365 6c66 2c20 275f  tattr__(self, '_
-00008570: 6964 272c 2075 7569 6428 2929 0a20 2020  id', uuid()).   
-00008580: 206f 626a 6563 742e 5f5f 7365 7461 7474   object.__setatt
-00008590: 725f 5f28 7365 6c66 2c20 275f 7374 6174  r__(self, '_stat
-000085a0: 6527 2c20 5f4d 6f64 756c 6549 6e74 6572  e', _ModuleInter
-000085b0: 6e61 6c53 7461 7465 2829 290a 0a20 2020  nalState())..   
-000085c0: 2023 2054 7970 6963 616c 6c79 2077 6520   # Typically we 
-000085d0: 7365 7420 7468 6520 7061 7265 6e74 2062  set the parent b
-000085e0: 6173 6564 206f 6e20 7468 6520 6479 6e61  ased on the dyna
-000085f0: 6d69 6320 6d6f 6475 6c65 2063 6f6e 7465  mic module conte
-00008600: 7874 2e0a 2020 2020 6966 2073 656c 662e  xt..    if self.
-00008610: 7061 7265 6e74 2069 7320 5f75 6e73 7065  parent is _unspe
-00008620: 6369 6669 6564 5f70 6172 656e 743a 2020  cified_parent:  
-00008630: 2320 7079 7479 7065 3a20 6469 7361 626c  # pytype: disabl
-00008640: 653d 6174 7472 6962 7574 652d 6572 726f  e=attribute-erro
-00008650: 720a 2020 2020 2020 6f62 6a65 6374 2e5f  r.      object._
-00008660: 5f73 6574 6174 7472 5f5f 2873 656c 662c  _setattr__(self,
-00008670: 2027 7061 7265 6e74 272c 205f 636f 6e74   'parent', _cont
-00008680: 6578 742e 6d6f 6475 6c65 5f73 7461 636b  ext.module_stack
-00008690: 5b2d 315d 290a 0a20 2020 2023 2049 6e69  [-1])..    # Ini
-000086a0: 7469 616c 697a 6174 696f 6e20 6973 2064  tialization is d
-000086b0: 6566 6572 7265 6420 666f 7220 746f 7020  eferred for top 
-000086c0: 6c65 7665 6c20 4d6f 6475 6c65 7320 6f72  level Modules or
-000086d0: 2061 6e79 206f 7468 6572 2022 6f72 7068   any other "orph
-000086e0: 616e 220a 2020 2020 2320 4d6f 6475 6c65  an".    # Module
-000086f0: 7320 756e 7469 6c20 6174 7461 6368 6d65  s until attachme
-00008700: 6e74 2062 7920 5f5f 7365 7461 7474 725f  nt by __setattr_
-00008710: 5f20 692e 652e 204d 794d 6f64 756c 6528  _ i.e. MyModule(
-00008720: 2e2e 2e2c 2070 6172 656e 743d 4e6f 6e65  ..., parent=None
-00008730: 290a 2020 2020 6966 2073 656c 662e 7061  ).    if self.pa
-00008740: 7265 6e74 2069 7320 4e6f 6e65 3a0a 2020  rent is None:.  
-00008750: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-00008760: 2320 5265 6769 7374 6572 2073 7562 6d6f  # Register submo
-00008770: 6475 6c65 206f 6e20 7061 7265 6e74 204d  dule on parent M
-00008780: 6f64 756c 652e 0a20 2020 2069 6620 6973  odule..    if is
-00008790: 696e 7374 616e 6365 2873 656c 662e 7061  instance(self.pa
-000087a0: 7265 6e74 2c20 4d6f 6475 6c65 293a 0a20  rent, Module):. 
-000087b0: 2020 2020 2023 2057 6865 6e20 696e 6974       # When init
-000087c0: 6961 6c69 7a69 6e67 2061 6e20 756e 6e61  ializing an unna
-000087d0: 6d65 6420 4d6f 6475 6c65 2069 6e73 6964  med Module insid
-000087e0: 6520 7365 7475 7028 290a 2020 2020 2020  e setup().      
-000087f0: 2320 696e 6974 6961 6c69 7a61 7469 6f6e  # initialization
-00008800: 2069 7320 6465 6665 7272 6564 2075 6e74   is deferred unt
-00008810: 696c 2061 7474 6163 686d 656e 7420 6279  il attachment by
-00008820: 205f 5f73 6574 6174 7472 5f5f 0a20 2020   __setattr__.   
-00008830: 2020 2023 2069 2e65 2e20 7365 6c66 2e6d     # i.e. self.m
-00008840: 796d 6f64 756c 6520 3d20 4d79 4d6f 6475  ymodule = MyModu
-00008850: 6c65 282e 2e2e 290a 2020 2020 2020 7365  le(...).      se
-00008860: 6c66 2e6e 616d 653a 204f 7074 696f 6e61  lf.name: Optiona
-00008870: 6c5b 7374 725d 0a20 2020 2020 2069 6620  l[str].      if 
-00008880: 7365 6c66 2e70 6172 656e 742e 5f73 7461  self.parent._sta
-00008890: 7465 2e69 6e5f 7365 7475 7020 616e 6420  te.in_setup and 
-000088a0: 7365 6c66 2e6e 616d 6520 6973 204e 6f6e  self.name is Non
-000088b0: 653a 2020 2320 7079 7479 7065 3a20 6469  e:  # pytype: di
-000088c0: 7361 626c 653d 6174 7472 6962 7574 652d  sable=attribute-
-000088d0: 6572 726f 720a 2020 2020 2020 2020 7265  error.        re
-000088e0: 7475 726e 0a20 2020 2020 2069 6620 6e6f  turn.      if no
-000088f0: 7420 7365 6c66 2e70 6172 656e 742e 5f69  t self.parent._i
-00008900: 6e69 7469 616c 697a 6174 696f 6e5f 616c  nitialization_al
-00008910: 6c6f 7765 643a 0a20 2020 2020 2020 2072  lowed:.        r
-00008920: 6169 7365 2065 7272 6f72 732e 4173 7369  aise errors.Assi
-00008930: 676e 5375 624d 6f64 756c 6545 7272 6f72  gnSubModuleError
-00008940: 2873 656c 662e 5f5f 636c 6173 735f 5f2e  (self.__class__.
-00008950: 5f5f 6e61 6d65 5f5f 290a 2020 2020 2020  __name__).      
-00008960: 2320 4175 746f 6e61 6d69 6e67 206f 6620  # Autonaming of 
-00008970: 7375 626d 6f64 756c 6573 2e0a 2020 2020  submodules..    
-00008980: 2020 6966 2073 656c 662e 6e61 6d65 2069    if self.name i
-00008990: 7320 4e6f 6e65 3a20 2023 2070 7974 7970  s None:  # pytyp
-000089a0: 653a 2064 6973 6162 6c65 3d61 7474 7269  e: disable=attri
-000089b0: 6275 7465 2d65 7272 6f72 0a20 2020 2020  bute-error.     
-000089c0: 2020 2070 7265 6669 7820 3d20 6627 7b73     prefix = f'{s
-000089d0: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
-000089e0: 6e61 6d65 5f5f 7d27 0a20 2020 2020 2020  name__}'.       
-000089f0: 2063 7572 736f 7220 3d20 7365 6c66 2e70   cursor = self.p
-00008a00: 6172 656e 742e 5f73 7461 7465 2e61 7574  arent._state.aut
-00008a10: 6f6e 616d 655f 6375 7273 6f72 2e67 6574  oname_cursor.get
-00008a20: 2870 7265 6669 782c 2030 290a 2020 2020  (prefix, 0).    
-00008a30: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
-00008a40: 6627 7b70 7265 6669 787d 5f7b 6375 7273  f'{prefix}_{curs
-00008a50: 6f72 7d27 0a20 2020 2020 2020 2073 656c  or}'.        sel
-00008a60: 662e 7061 7265 6e74 2e5f 7374 6174 652e  f.parent._state.
-00008a70: 6175 746f 6e61 6d65 5f63 7572 736f 725b  autoname_cursor[
-00008a80: 7072 6566 6978 5d20 3d20 6375 7273 6f72  prefix] = cursor
-00008a90: 202b 2031 0a20 2020 2020 2023 2041 6c6c   + 1.      # All
-00008aa0: 6f77 2073 636f 7065 2061 6c69 6173 696e  ow scope aliasin
-00008ab0: 6720 756e 6465 7220 7472 616e 7366 6f72  g under transfor
-00008ac0: 6d73 2066 6f72 2073 7562 6d6f 6475 6c65  ms for submodule
-00008ad0: 7320 6465 6669 6e65 6420 696e 2073 6574  s defined in set
-00008ae0: 7570 2e0a 2020 2020 2020 7265 7573 655f  up..      reuse_
-00008af0: 7363 6f70 6573 203d 2028 0a20 2020 2020  scopes = (.     
-00008b00: 2020 2020 2073 656c 662e 7061 7265 6e74       self.parent
-00008b10: 2e5f 7374 6174 652e 696e 5f73 6574 7570  ._state.in_setup
-00008b20: 0a20 2020 2020 2020 2020 2061 6e64 2073  .          and s
-00008b30: 656c 662e 7061 7265 6e74 2e5f 7374 6174  elf.parent._stat
-00008b40: 652e 7365 7475 705f 6361 6c6c 6564 203d  e.setup_called =
-00008b50: 3d20 5365 7475 7053 7461 7465 2e54 5241  = SetupState.TRA
-00008b60: 4e53 464f 524d 4544 0a20 2020 2020 2029  NSFORMED.      )
-00008b70: 0a20 2020 2020 2023 2050 6572 666f 726d  .      # Perform
-00008b80: 206e 616d 652d 636f 6c6c 6973 696f 6e20   name-collision 
-00008b90: 6368 6563 6b2e 0a20 2020 2020 2069 6620  check..      if 
-00008ba0: 7365 6c66 2e70 6172 656e 742e 5f6e 616d  self.parent._nam
-00008bb0: 655f 7461 6b65 6e28 7365 6c66 2e6e 616d  e_taken(self.nam
-00008bc0: 652c 2073 656c 662c 2072 6575 7365 5f73  e, self, reuse_s
-00008bd0: 636f 7065 733d 7265 7573 655f 7363 6f70  copes=reuse_scop
-00008be0: 6573 293a 0a20 2020 2020 2020 2070 6172  es):.        par
-00008bf0: 656e 745f 636c 6173 7320 3d20 7365 6c66  ent_class = self
-00008c00: 2e70 6172 656e 742e 5f5f 636c 6173 735f  .parent.__class_
-00008c10: 5f2e 5f5f 6e61 6d65 5f5f 0a20 2020 2020  _.__name__.     
-00008c20: 2020 2072 6169 7365 2065 7272 6f72 732e     raise errors.
-00008c30: 4e61 6d65 496e 5573 6545 7272 6f72 2827  NameInUseError('
-00008c40: 7375 626d 6f64 756c 6527 2c20 7365 6c66  submodule', self
-00008c50: 2e6e 616d 652c 2070 6172 656e 745f 636c  .name, parent_cl
-00008c60: 6173 7329 0a20 2020 2020 2023 2046 696e  ass).      # Fin
-00008c70: 616c 697a 6520 6174 7461 6368 6d65 6e74  alize attachment
-00008c80: 2074 6f20 7061 7265 6e74 2061 6e64 2073   to parent and s
-00008c90: 636f 7065 2069 6e69 7469 616c 697a 6174  cope initializat
-00008ca0: 696f 6e2e 0a20 2020 2020 2073 656c 662e  ion..      self.
-00008cb0: 7061 7265 6e74 2e5f 7374 6174 652e 6368  parent._state.ch
-00008cc0: 696c 6472 656e 5b73 656c 662e 6e61 6d65  ildren[self.name
-00008cd0: 5d20 3d20 7365 6c66 0a20 2020 2020 2061  ] = self.      a
-00008ce0: 7373 6572 7420 7365 6c66 2e70 6172 656e  ssert self.paren
-00008cf0: 742e 7363 6f70 6520 6973 206e 6f74 204e  t.scope is not N
-00008d00: 6f6e 650a 2020 2020 2020 6f62 6a65 6374  one.      object
-00008d10: 2e5f 5f73 6574 6174 7472 5f5f 280a 2020  .__setattr__(.  
-00008d20: 2020 2020 2020 2020 7365 6c66 2c20 2773          self, 's
-00008d30: 636f 7065 272c 2073 656c 662e 7061 7265  cope', self.pare
-00008d40: 6e74 2e73 636f 7065 2e70 7573 6828 7365  nt.scope.push(se
-00008d50: 6c66 2e6e 616d 652c 2072 6575 7365 3d72  lf.name, reuse=r
-00008d60: 6575 7365 5f73 636f 7065 7329 0a20 2020  euse_scopes).   
-00008d70: 2020 2029 0a0a 2020 2020 2320 546f 702d     )..    # Top-
-00008d80: 6c65 7665 6c20 696e 766f 6361 7469 6f6e  level invocation
-00008d90: 2077 6974 6820 6120 6675 6e63 7469 6f6e   with a function
-00008da0: 616c 2053 636f 7065 2e0a 2020 2020 656c  al Scope..    el
-00008db0: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
-00008dc0: 6c66 2e70 6172 656e 742c 2053 636f 7065  lf.parent, Scope
-00008dd0: 293a 0a20 2020 2020 206f 626a 6563 742e  ):.      object.
-00008de0: 5f5f 7365 7461 7474 725f 5f28 7365 6c66  __setattr__(self
-00008df0: 2c20 2773 636f 7065 272c 2073 656c 662e  , 'scope', self.
-00008e00: 7061 7265 6e74 290a 2020 2020 656c 7365  parent).    else
-00008e10: 3a0a 2020 2020 2020 7261 6973 6520 5661  :.      raise Va
-00008e20: 6c75 6545 7272 6f72 2827 7061 7265 6e74  lueError('parent
-00008e30: 206d 7573 7420 6265 204e 6f6e 652c 204d   must be None, M
-00008e40: 6f64 756c 6520 6f72 2053 636f 7065 2729  odule or Scope')
-00008e50: 0a0a 2020 2020 2320 6561 6765 726c 7920  ..    # eagerly 
-00008e60: 6269 6e64 2073 7562 6d6f 6475 6c65 7320  bind submodules 
-00008e70: 6966 2073 636f 7065 2069 7320 6176 6169  if scope is avai
-00008e80: 6c61 626c 650a 2020 2020 6966 2073 656c  lable.    if sel
-00008e90: 662e 7363 6f70 6520 6973 206e 6f74 204e  f.scope is not N
-00008ea0: 6f6e 653a 0a20 2020 2020 2066 6f72 2066  one:.      for f
-00008eb0: 6965 6c64 2069 6e20 6461 7461 636c 6173  ield in dataclas
-00008ec0: 7365 732e 6669 656c 6473 2873 656c 6629  ses.fields(self)
-00008ed0: 3a0a 2020 2020 2020 2020 6966 2066 6965  :.        if fie
-00008ee0: 6c64 2e6e 616d 6520 6e6f 7420 696e 2028  ld.name not in (
-00008ef0: 2770 6172 656e 7427 2c20 276e 616d 6527  'parent', 'name'
-00008f00: 2920 616e 6420 6669 656c 642e 696e 6974  ) and field.init
-00008f10: 3a0a 2020 2020 2020 2020 2020 7365 6c66  :.          self
-00008f20: 2e5f 7265 6769 7374 6572 5f73 7562 6d6f  ._register_submo
-00008f30: 6475 6c65 7328 6669 656c 642e 6e61 6d65  dules(field.name
-00008f40: 2c20 6765 7461 7474 7228 7365 6c66 2c20  , getattr(self, 
-00008f50: 6669 656c 642e 6e61 6d65 2929 0a0a 2020  field.name))..  
-00008f60: 2020 7365 6c66 2e5f 7374 6174 652e 6973    self._state.is
-00008f70: 5f69 6e69 7469 616c 697a 6564 203d 2054  _initialized = T
-00008f80: 7275 650a 0a20 2064 6566 205f 5f72 6570  rue..  def __rep
-00008f90: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
-00008fa0: 3a0a 2020 2020 7265 7475 726e 205f 6d6f  :.    return _mo
-00008fb0: 6475 6c65 5f72 6570 7228 7365 6c66 290a  dule_repr(self).
-00008fc0: 0a20 2064 6566 2073 6574 7570 2873 656c  .  def setup(sel
-00008fd0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00008fe0: 2222 2249 6e69 7469 616c 697a 6573 2061  """Initializes a
-00008ff0: 204d 6f64 756c 6520 6c61 7a69 6c79 2028   Module lazily (
-00009000: 7369 6d69 6c61 7220 746f 2061 206c 617a  similar to a laz
-00009010: 7920 6060 5f5f 696e 6974 5f5f 6060 292e  y ``__init__``).
-00009020: 0a0a 2020 2020 6060 7365 7475 7060 6020  ..    ``setup`` 
-00009030: 6973 2063 616c 6c65 6420 6f6e 6365 206c  is called once l
-00009040: 617a 696c 7920 6f6e 2061 206d 6f64 756c  azily on a modul
-00009050: 6520 696e 7374 616e 6365 2077 6865 6e20  e instance when 
-00009060: 6120 6d6f 6475 6c65 0a20 2020 2069 7320  a module.    is 
-00009070: 626f 756e 642c 2069 6d6d 6564 6961 7465  bound, immediate
-00009080: 6c79 2062 6566 6f72 6520 616e 7920 6f74  ly before any ot
-00009090: 6865 7220 6d65 7468 6f64 7320 6c69 6b65  her methods like
-000090a0: 2060 605f 5f63 616c 6c5f 5f60 6020 6172   ``__call__`` ar
-000090b0: 650a 2020 2020 696e 766f 6b65 642c 206f  e.    invoked, o
-000090c0: 7220 6265 666f 7265 2061 2060 6073 6574  r before a ``set
-000090d0: 7570 6060 2d64 6566 696e 6564 2061 7474  up``-defined att
-000090e0: 7269 6275 7465 206f 6e20 6073 656c 6660  ribute on `self`
-000090f0: 2069 7320 6163 6365 7373 6564 2e0a 0a20   is accessed... 
-00009100: 2020 2054 6869 7320 6361 6e20 6861 7070     This can happ
-00009110: 656e 2069 6e20 7468 7265 6520 6361 7365  en in three case
-00009120: 733a 0a0a 2020 2020 2020 312e 2049 6d6d  s:..      1. Imm
-00009130: 6564 6961 7465 6c79 2077 6865 6e20 696e  ediately when in
-00009140: 766f 6b69 6e67 203a 6d65 7468 3a60 6170  voking :meth:`ap
-00009150: 706c 7960 2c20 3a6d 6574 683a 6069 6e69  ply`, :meth:`ini
-00009160: 7460 206f 720a 2020 2020 2020 2020 203a  t` or.         :
-00009170: 6d65 7468 3a60 696e 6974 5f61 6e64 5f6f  meth:`init_and_o
-00009180: 7574 7075 7460 2e0a 0a20 2020 2020 2032  utput`...      2
-00009190: 2e20 4f6e 6365 2074 6865 206d 6f64 756c  . Once the modul
-000091a0: 6520 6973 2067 6976 656e 2061 206e 616d  e is given a nam
-000091b0: 6520 6279 2062 6569 6e67 2061 7373 6967  e by being assig
-000091c0: 6e65 6420 746f 2061 6e20 6174 7472 6962  ned to an attrib
-000091d0: 7574 6520 6f66 0a20 2020 2020 2020 2020  ute of.         
-000091e0: 616e 6f74 6865 7220 6d6f 6475 6c65 2069  another module i
-000091f0: 6e73 6964 6520 7468 6520 6f74 6865 7220  nside the other 
-00009200: 6d6f 6475 6c65 2773 2060 6073 6574 7570  module's ``setup
-00009210: 6060 206d 6574 686f 640a 2020 2020 2020  `` method.      
-00009220: 2020 2028 7365 6520 3a6d 6574 683a 605f     (see :meth:`_
-00009230: 5f73 6574 6174 7472 5f5f 6029 3a3a 0a0a  _setattr__`)::..
-00009240: 2020 2020 2020 2020 2020 2063 6c61 7373             class
-00009250: 204d 794d 6f64 756c 6528 6e6e 2e4d 6f64   MyModule(nn.Mod
-00009260: 756c 6529 3a0a 2020 2020 2020 2020 2020  ule):.          
-00009270: 2020 2064 6566 2073 6574 7570 2873 656c     def setup(sel
-00009280: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-00009290: 2020 2073 7562 6d6f 6475 6c65 203d 2043     submodule = C
-000092a0: 6f6e 7628 2e2e 2e29 0a0a 2020 2020 2020  onv(...)..      
-000092b0: 2020 2020 2020 2020 2023 2041 6363 6573           # Acces
-000092c0: 7369 6e67 2060 7375 626d 6f64 756c 6560  sing `submodule`
-000092d0: 2061 7474 7269 6275 7465 7320 646f 6573   attributes does
-000092e0: 206e 6f74 2079 6574 2077 6f72 6b20 6865   not yet work he
-000092f0: 7265 2e0a 0a20 2020 2020 2020 2020 2020  re...           
-00009300: 2020 2020 2320 5468 6520 666f 6c6c 6f77      # The follow
-00009310: 696e 6720 6c69 6e65 2069 6e76 6f6b 6573  ing line invokes
-00009320: 2060 7365 6c66 2e5f 5f73 6574 6174 7472   `self.__setattr
-00009330: 5f5f 602c 2077 6869 6368 2067 6976 6573  __`, which gives
-00009340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009350: 2320 6073 7562 6d6f 6475 6c65 6020 7468  # `submodule` th
-00009360: 6520 6e61 6d65 2022 636f 6e76 3122 2e0a  e name "conv1"..
-00009370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00009380: 656c 662e 636f 6e76 3120 3d20 7375 626d  elf.conv1 = subm
-00009390: 6f64 756c 650a 0a20 2020 2020 2020 2020  odule..         
-000093a0: 2020 2020 2020 2320 4163 6365 7373 696e        # Accessin
-000093b0: 6720 6073 7562 6d6f 6475 6c65 6020 6174  g `submodule` at
-000093c0: 7472 6962 7574 6573 206f 7220 6d65 7468  tributes or meth
-000093d0: 6f64 7320 6973 206e 6f77 2073 6166 6520  ods is now safe 
-000093e0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-000093f0: 2020 2023 2065 6974 6865 7220 6361 7573     # either caus
-00009400: 6573 2073 6574 7570 2829 2074 6f20 6265  es setup() to be
-00009410: 2063 616c 6c65 6420 6f6e 6365 2e0a 0a20   called once... 
-00009420: 2020 2020 2033 2e20 4f6e 6365 2061 206d       3. Once a m
-00009430: 6f64 756c 6520 6973 2063 6f6e 7374 7275  odule is constru
-00009440: 6374 6564 2069 6e73 6964 6520 6120 6d65  cted inside a me
-00009450: 7468 6f64 2077 7261 7070 6564 2077 6974  thod wrapped wit
-00009460: 680a 2020 2020 2020 2020 203a 6d65 7468  h.         :meth
-00009470: 3a60 636f 6d70 6163 7460 2c20 696d 6d65  :`compact`, imme
-00009480: 6469 6174 656c 7920 6265 666f 7265 2061  diately before a
-00009490: 6e6f 7468 6572 206d 6574 686f 6420 6973  nother method is
-000094a0: 2063 616c 6c65 6420 6f72 0a20 2020 2020   called or.     
-000094b0: 2020 2020 6060 7365 7475 7060 6020 6465      ``setup`` de
-000094c0: 6669 6e65 6420 6174 7472 6962 7574 6520  fined attribute 
-000094d0: 6973 2061 6363 6573 7365 642e 0a20 2020  is accessed..   
-000094e0: 2022 2222 0a20 2020 2070 6173 730a 0a20   """.    pass.. 
-000094f0: 2064 6566 205f 7265 6769 7374 6572 5f73   def _register_s
-00009500: 7562 6d6f 6475 6c65 7328 7365 6c66 2c20  ubmodules(self, 
-00009510: 6e61 6d65 2c20 7661 6c29 3a0a 2020 2020  name, val):.    
-00009520: 2222 2252 6567 6973 7465 7273 2061 2073  """Registers a s
-00009530: 7562 6d6f 6475 6c65 2e22 2222 0a20 2020  ubmodule.""".   
-00009540: 2061 7373 6572 7420 7365 6c66 2e73 636f   assert self.sco
-00009550: 7065 2c20 2754 7279 696e 6720 746f 2072  pe, 'Trying to r
-00009560: 6567 6973 7465 7220 7375 626d 6f64 756c  egister submodul
-00009570: 6573 206f 6e20 756e 626f 756e 6420 7363  es on unbound sc
-00009580: 6f70 652e 270a 2020 2020 726f 6f74 203d  ope.'.    root =
-00009590: 2073 656c 662e 7363 6f70 652e 726f 6f74   self.scope.root
-000095a0: 0a20 2020 2063 6163 6865 203d 205f 6361  .    cache = _ca
-000095b0: 6368 6573 2e67 6574 2872 6f6f 742c 2077  ches.get(root, w
-000095c0: 6561 6b72 6566 2e57 6561 6b56 616c 7565  eakref.WeakValue
-000095d0: 4469 6374 696f 6e61 7279 2829 290a 2020  Dictionary()).  
-000095e0: 2020 5f63 6163 6865 735b 726f 6f74 5d20    _caches[root] 
-000095f0: 3d20 6361 6368 650a 2020 2020 7175 6575  = cache.    queu
-00009600: 6520 3d20 5b5d 0a20 2020 2070 7265 7365  e = [].    prese
-00009610: 7276 655f 6164 6f70 7465 645f 6e61 6d65  rve_adopted_name
-00009620: 7320 3d20 636f 6e66 6967 2e66 6c61 785f  s = config.flax_
-00009630: 7072 6573 6572 7665 5f61 646f 7074 6564  preserve_adopted
-00009640: 5f6e 616d 6573 0a20 2020 2069 6620 6861  _names.    if ha
-00009650: 7361 7474 7228 7479 7065 2873 656c 6629  sattr(type(self)
-00009660: 2c20 2770 7265 7365 7276 655f 6164 6f70  , 'preserve_adop
-00009670: 7465 645f 6e61 6d65 7327 293a 0a20 2020  ted_names'):.   
-00009680: 2020 2070 7265 7365 7276 655f 6164 6f70     preserve_adop
-00009690: 7465 645f 6e61 6d65 7320 3d20 7479 7065  ted_names = type
-000096a0: 2873 656c 6629 2e70 7265 7365 7276 655f  (self).preserve_
-000096b0: 6164 6f70 7465 645f 6e61 6d65 730a 0a20  adopted_names.. 
-000096c0: 2020 2064 6566 2061 646f 7074 5f61 7474     def adopt_att
-000096d0: 725f 6d6f 6475 6c65 7328 6361 6368 652c  r_modules(cache,
-000096e0: 2071 7565 7565 2c20 7375 6666 6978 2c20   queue, suffix, 
-000096f0: 7375 6276 616c 7565 293a 0a20 2020 2020  subvalue):.     
-00009700: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-00009710: 7562 7661 6c75 652c 204d 6f64 756c 6529  ubvalue, Module)
-00009720: 3a0a 2020 2020 2020 2020 6164 6f70 7465  :.        adopte
-00009730: 645f 6e61 6d65 203d 204e 6f6e 650a 2020  d_name = None.  
-00009740: 2020 2020 2020 6966 2073 7562 7661 6c75        if subvalu
-00009750: 652e 7061 7265 6e74 2069 7320 4e6f 6e65  e.parent is None
-00009760: 3a0a 2020 2020 2020 2020 2020 2320 5072  :.          # Pr
-00009770: 6573 6572 7665 2073 6861 7269 6e67 2d62  eserve sharing-b
-00009780: 792d 7265 6665 7265 6e63 6520 7265 6c61  y-reference rela
-00009790: 7469 6f6e 7368 6970 7320 6475 7269 6e67  tionships during
-000097a0: 2061 646f 7074 696f 6e0a 2020 2020 2020   adoption.      
-000097b0: 2020 2020 2320 7669 6120 6361 6368 6520      # via cache 
-000097c0: 6b65 7965 6420 6f6e 2075 6e69 7175 6520  keyed on unique 
-000097d0: 696e 7374 616e 6365 2069 6473 2e0a 2020  instance ids..  
-000097e0: 2020 2020 2020 2020 6b65 7920 3d20 7375          key = su
-000097f0: 6276 616c 7565 2e5f 6964 0a20 2020 2020  bvalue._id.     
-00009800: 2020 2020 2023 204d 6f64 756c 6520 7761       # Module wa
-00009810: 7320 7061 7373 6564 2066 726f 6d20 6f75  s passed from ou
-00009820: 7473 6964 652e 2049 7420 6e65 6564 7320  tside. It needs 
-00009830: 746f 2062 6520 636c 6f6e 6564 2e0a 2020  to be cloned..  
-00009840: 2020 2020 2020 2020 2320 4f75 7473 6964          # Outsid
-00009850: 6520 6d6f 6475 6c65 7320 6172 6520 6e61  e modules are na
-00009860: 6d65 6420 6279 2061 7474 6163 686d 656e  med by attachmen
-00009870: 742c 206e 6f74 2061 6e20 6f75 7465 7220  t, not an outer 
-00009880: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00009890: 2320 554e 4c45 5353 2077 6527 7265 2075  # UNLESS we're u
-000098a0: 7369 6e67 206e 6577 2061 646f 7074 6564  sing new adopted
-000098b0: 206e 616d 6520 706f 6c69 6379 2c20 696e   name policy, in
-000098c0: 2077 6869 6368 2063 6173 6520 616e 2065   which case an e
-000098d0: 7869 7374 696e 670a 2020 2020 2020 2020  xisting.        
-000098e0: 2020 2320 6e61 6d65 2077 696c 6c20 6265    # name will be
-000098f0: 2075 7365 642c 2061 7320 6973 206f 6674   used, as is oft
-00009900: 656e 2073 7570 706c 6965 6420 6279 2063  en supplied by c
-00009910: 6f6e 6669 6720 7379 7374 656d 732e 0a20  onfig systems.. 
-00009920: 2020 2020 2020 2020 2069 6620 7072 6573           if pres
-00009930: 6572 7665 5f61 646f 7074 6564 5f6e 616d  erve_adopted_nam
-00009940: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00009950: 6164 6f70 7465 645f 6e61 6d65 203d 206f  adopted_name = o
-00009960: 626a 6563 742e 5f5f 6765 7461 7474 7269  bject.__getattri
-00009970: 6275 7465 5f5f 2873 7562 7661 6c75 652c  bute__(subvalue,
-00009980: 2027 6e61 6d65 2729 0a20 2020 2020 2020   'name').       
-00009990: 2020 2069 6620 6b65 7920 696e 2063 6163     if key in cac
-000099a0: 6865 3a0a 2020 2020 2020 2020 2020 2020  he:.            
-000099b0: 7375 6276 616c 7565 203d 2063 6163 6865  subvalue = cache
-000099c0: 5b6b 6579 5d0a 2020 2020 2020 2020 2020  [key].          
-000099d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000099e0: 2020 7375 6276 616c 7565 203d 2073 7562    subvalue = sub
-000099f0: 7661 6c75 652e 636c 6f6e 6528 6e61 6d65  value.clone(name
-00009a00: 3d4e 6f6e 6529 0a20 2020 2020 2020 2020  =None).         
-00009a10: 2020 2063 6163 6865 5b6b 6579 5d20 3d20     cache[key] = 
-00009a20: 7375 6276 616c 7565 0a20 2020 2020 2020  subvalue.       
-00009a30: 2069 6620 7375 6276 616c 7565 2e6e 616d   if subvalue.nam
-00009a40: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00009a50: 2020 2020 206f 626a 6563 742e 5f5f 7365       object.__se
-00009a60: 7461 7474 725f 5f28 7375 6276 616c 7565  tattr__(subvalue
-00009a70: 2c20 2770 6172 656e 7427 2c20 7365 6c66  , 'parent', self
-00009a80: 290a 2020 2020 2020 2020 2020 6966 2061  ).          if a
-00009a90: 646f 7074 6564 5f6e 616d 6520 6973 204e  dopted_name is N
-00009aa0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00009ab0: 2061 646f 7074 6564 5f6e 616d 6520 3d20   adopted_name = 
-00009ac0: 6627 7b6e 616d 657d 7b73 7566 6669 787d  f'{name}{suffix}
-00009ad0: 270a 2020 2020 2020 2020 2020 6f62 6a65  '.          obje
-00009ae0: 6374 2e5f 5f73 6574 6174 7472 5f5f 2873  ct.__setattr__(s
-00009af0: 7562 7661 6c75 652c 2027 6e61 6d65 272c  ubvalue, 'name',
-00009b00: 2061 646f 7074 6564 5f6e 616d 6529 0a20   adopted_name). 
-00009b10: 2020 2020 2020 2020 2071 7565 7565 2e61           queue.a
-00009b20: 7070 656e 6428 7375 6276 616c 7565 290a  ppend(subvalue).
-00009b30: 2020 2020 2020 7265 7475 726e 2073 7562        return sub
-00009b40: 7661 6c75 650a 0a20 2020 2076 616c 203d  value..    val =
-00009b50: 205f 6672 6565 7a65 5f61 7474 7228 0a20   _freeze_attr(. 
-00009b60: 2020 2020 2020 205f 6d61 705f 6f76 6572         _map_over
-00009b70: 5f6d 6f64 756c 6573 5f69 6e5f 7472 6565  _modules_in_tree
-00009b80: 280a 2020 2020 2020 2020 2020 2020 6675  (.            fu
-00009b90: 6e63 746f 6f6c 732e 7061 7274 6961 6c28  nctools.partial(
-00009ba0: 6164 6f70 745f 6174 7472 5f6d 6f64 756c  adopt_attr_modul
-00009bb0: 6573 2c20 6361 6368 652c 2071 7565 7565  es, cache, queue
-00009bc0: 292c 2076 616c 0a20 2020 2020 2020 2029  ), val.        )
-00009bd0: 0a20 2020 2029 0a20 2020 206f 626a 6563  .    ).    objec
-00009be0: 742e 5f5f 7365 7461 7474 725f 5f28 7365  t.__setattr__(se
-00009bf0: 6c66 2c20 6e61 6d65 2c20 7661 6c29 0a20  lf, name, val). 
-00009c00: 2020 2066 6f72 2078 2069 6e20 7175 6575     for x in queu
-00009c10: 653a 0a20 2020 2020 2078 2e5f 5f70 6f73  e:.      x.__pos
-00009c20: 745f 696e 6974 5f5f 2829 0a0a 2020 6465  t_init__()..  de
-00009c30: 6620 5f74 7279 5f73 6574 7570 2873 656c  f _try_setup(sel
-00009c40: 662c 2073 6861 6c6c 6f77 3a20 626f 6f6c  f, shallow: bool
-00009c50: 203d 2046 616c 7365 2920 2d3e 204e 6f6e   = False) -> Non
-00009c60: 653a 0a20 2020 2022 2222 5472 6965 7320  e:.    """Tries 
-00009c70: 746f 2073 6574 7570 206d 6f64 756c 6520  to setup module 
-00009c80: 6966 2073 636f 7065 2069 7320 6176 6169  if scope is avai
-00009c90: 6c61 626c 6520 616e 6420 7365 7475 7020  lable and setup 
-00009ca0: 6861 7320 6e6f 7420 6265 656e 2063 616c  has not been cal
-00009cb0: 6c65 6420 7965 742e 2222 220a 2020 2020  led yet.""".    
-00009cc0: 6966 2028 0a20 2020 2020 2020 2073 656c  if (.        sel
-00009cd0: 662e 7363 6f70 650a 2020 2020 2020 2020  f.scope.        
-00009ce0: 616e 6420 6e6f 7420 7365 6c66 2e5f 7374  and not self._st
-00009cf0: 6174 652e 696e 5f73 6574 7570 0a20 2020  ate.in_setup.   
-00009d00: 2020 2020 2061 6e64 2073 656c 662e 5f73       and self._s
-00009d10: 7461 7465 2e73 6574 7570 5f63 616c 6c65  tate.setup_calle
-00009d20: 6420 213d 2053 6574 7570 5374 6174 652e  d != SetupState.
-00009d30: 444f 4e45 0a20 2020 2029 3a0a 2020 2020  DONE.    ):.    
-00009d40: 2020 7472 793a 0a20 2020 2020 2020 2073    try:.        s
-00009d50: 656c 662e 5f73 7461 7465 2e69 6e5f 7365  elf._state.in_se
-00009d60: 7475 7020 3d20 5472 7565 0a20 2020 2020  tup = True.     
-00009d70: 2020 2023 2041 2073 6861 6c6c 6f77 2073     # A shallow s
-00009d80: 6574 7570 2077 696c 6c20 6f6e 6c79 2072  etup will only r
-00009d90: 6567 6973 7465 7220 6174 7472 6962 7574  egister attribut
-00009da0: 6520 7375 626d 6f64 756c 6573 2062 7574  e submodules but
-00009db0: 2069 7420 646f 6573 0a20 2020 2020 2020   it does.       
-00009dc0: 2023 206e 6f74 2063 616c 6c20 7468 6520   # not call the 
-00009dd0: 7573 6572 2773 2073 6574 7570 2e20 5468  user's setup. Th
-00009de0: 6973 2061 766f 6964 7320 7275 6e6e 696e  is avoids runnin
-00009df0: 6720 6265 666f 7265 2061 0a20 2020 2020  g before a.     
-00009e00: 2020 2023 2074 7261 6e73 666f 726d 6174     # transformat
-00009e10: 696f 6e2e 0a20 2020 2020 2020 2066 6f72  ion..        for
-00009e20: 2066 6965 6c64 2069 6e20 6461 7461 636c   field in datacl
-00009e30: 6173 7365 732e 6669 656c 6473 2873 656c  asses.fields(sel
-00009e40: 6629 3a0a 2020 2020 2020 2020 2020 6966  f):.          if
-00009e50: 2066 6965 6c64 2e6e 616d 6520 6e6f 7420   field.name not 
-00009e60: 696e 2028 2770 6172 656e 7427 2c20 276e  in ('parent', 'n
-00009e70: 616d 6527 2920 616e 6420 6669 656c 642e  ame') and field.
-00009e80: 696e 6974 3a0a 2020 2020 2020 2020 2020  init:.          
-00009e90: 2020 7365 6c66 2e5f 7265 6769 7374 6572    self._register
-00009ea0: 5f73 7562 6d6f 6475 6c65 7328 6669 656c  _submodules(fiel
-00009eb0: 642e 6e61 6d65 2c20 6765 7461 7474 7228  d.name, getattr(
-00009ec0: 7365 6c66 2c20 6669 656c 642e 6e61 6d65  self, field.name
-00009ed0: 2929 0a20 2020 2020 2020 2069 6620 6e6f  )).        if no
-00009ee0: 7420 7368 616c 6c6f 773a 0a20 2020 2020  t shallow:.     
-00009ef0: 2020 2020 2073 656c 662e 7365 7475 7028       self.setup(
-00009f00: 290a 2020 2020 2020 2020 2320 5765 2072  ).        # We r
-00009f10: 756e 2073 7461 7469 6320 6368 6563 6b73  un static checks
-00009f20: 2061 6273 7472 6163 746c 7920 6f6e 6365   abstractly once
-00009f30: 2066 6f72 2073 6574 7570 2062 6566 6f72   for setup befor
-00009f40: 6520 616e 7920 7472 616e 7366 6f72 6d73  e any transforms
-00009f50: 0a20 2020 2020 2020 2023 2074 6f20 6465  .        # to de
-00009f60: 7465 6374 206e 616d 6520 636f 6c6c 6973  tect name collis
-00009f70: 696f 6e73 2061 6e64 206f 7468 6572 2070  ions and other p
-00009f80: 7974 686f 6e20 6572 726f 7273 2e0a 2020  ython errors..  
-00009f90: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00009fa0: 5f73 7461 7465 2e73 6574 7570 5f63 616c  _state.setup_cal
-00009fb0: 6c65 6420 3d3d 2053 6574 7570 5374 6174  led == SetupStat
-00009fc0: 652e 4e45 573a 0a20 2020 2020 2020 2020  e.NEW:.         
-00009fd0: 2073 656c 662e 5f76 616c 6964 6174 655f   self._validate_
-00009fe0: 7365 7475 7028 290a 2020 2020 2020 6669  setup().      fi
-00009ff0: 6e61 6c6c 793a 0a20 2020 2020 2020 2073  nally:.        s
-0000a000: 656c 662e 5f73 7461 7465 2e69 6e5f 7365  elf._state.in_se
-0000a010: 7475 7020 3d20 4661 6c73 650a 2020 2020  tup = False.    
-0000a020: 2020 2020 6966 206e 6f74 2073 6861 6c6c      if not shall
-0000a030: 6f77 3a0a 2020 2020 2020 2020 2020 7365  ow:.          se
-0000a040: 6c66 2e5f 7374 6174 652e 7365 7475 705f  lf._state.setup_
-0000a050: 6361 6c6c 6564 203d 2053 6574 7570 5374  called = SetupSt
-0000a060: 6174 652e 444f 4e45 0a0a 2020 6465 6620  ate.DONE..  def 
-0000a070: 5f76 616c 6964 6174 655f 7365 7475 7028  _validate_setup(
-0000a080: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000a090: 2020 2022 2222 4162 7374 7261 6374 6c79     """Abstractly
-0000a0a0: 2065 7661 6c75 6174 6573 2073 6574 7570   evaluates setup
-0000a0b0: 206f 6e6c 7920 746f 2072 756e 2073 7461   only to run sta
-0000a0c0: 7469 6320 6368 6563 6b73 2e22 2222 0a0a  tic checks."""..
-0000a0d0: 2020 2020 6465 6620 7275 6e5f 7365 7475      def run_setu
-0000a0e0: 705f 6f6e 6c79 2878 293a 0a20 2020 2020  p_only(x):.     
-0000a0f0: 2077 7261 7070 6564 5f69 6420 3d20 7772   wrapped_id = wr
-0000a100: 6170 5f6d 6574 686f 645f 6f6e 6365 286c  ap_method_once(l
-0000a110: 616d 6264 6120 6d2c 2078 3a20 7829 0a20  ambda m, x: x). 
-0000a120: 2020 2020 2077 6974 6820 5465 7374 5363       with TestSc
-0000a130: 6f70 6528 7b7d 2c20 726e 6773 3d7b 7d2c  ope({}, rngs={},
-0000a140: 206d 7574 6162 6c65 3d54 7275 6529 2e74   mutable=True).t
-0000a150: 656d 706f 7261 7279 2829 2061 7320 726f  emporary() as ro
-0000a160: 6f74 3a0a 2020 2020 2020 2020 7265 7475  ot:.        retu
-0000a170: 726e 2077 7261 7070 6564 5f69 6428 7365  rn wrapped_id(se
-0000a180: 6c66 2e63 6c6f 6e65 2870 6172 656e 743d  lf.clone(parent=
-0000a190: 726f 6f74 292c 2078 290a 0a20 2020 205f  root), x)..    _
-0000a1a0: 203d 206a 6178 2e65 7661 6c5f 7368 6170   = jax.eval_shap
-0000a1b0: 6528 7275 6e5f 7365 7475 705f 6f6e 6c79  e(run_setup_only
-0000a1c0: 2c20 3029 0a0a 2020 6465 6620 5f6e 616d  , 0)..  def _nam
-0000a1d0: 655f 7461 6b65 6e28 0a20 2020 2020 2073  e_taken(.      s
-0000a1e0: 656c 662c 0a20 2020 2020 206e 616d 653a  elf,.      name:
-0000a1f0: 2073 7472 2c0a 2020 2020 2020 6d6f 6475   str,.      modu
-0000a200: 6c65 3a20 4f70 7469 6f6e 616c 5b27 4d6f  le: Optional['Mo
-0000a210: 6475 6c65 275d 203d 204e 6f6e 652c 0a20  dule'] = None,. 
-0000a220: 2020 2020 2072 6575 7365 5f73 636f 7065       reuse_scope
-0000a230: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-0000a240: 0a20 2020 2020 2063 6f6c 6c65 6374 696f  .      collectio
-0000a250: 6e3a 204f 7074 696f 6e61 6c5b 7374 725d  n: Optional[str]
-0000a260: 203d 204e 6f6e 652c 0a20 2029 202d 3e20   = None,.  ) -> 
-0000a270: 626f 6f6c 3a0a 2020 2020 6173 7365 7274  bool:.    assert
-0000a280: 2073 656c 662e 7363 6f70 6520 6973 206e   self.scope is n
-0000a290: 6f74 204e 6f6e 650a 2020 2020 6966 2072  ot None.    if r
-0000a2a0: 6575 7365 5f73 636f 7065 733a 0a20 2020  euse_scopes:.   
-0000a2b0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0000a2c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000a2d0: 7363 6f70 652e 6e61 6d65 5f72 6573 6572  scope.name_reser
-0000a2e0: 7665 6428 6e61 6d65 2c20 636f 6c6c 6563  ved(name, collec
-0000a2f0: 7469 6f6e 290a 0a20 2040 7072 6f70 6572  tion)..  @proper
-0000a300: 7479 0a20 2064 6566 205f 696e 6974 6961  ty.  def _initia
-0000a310: 6c69 7a61 7469 6f6e 5f61 6c6c 6f77 6564  lization_allowed
-0000a320: 2873 656c 6629 3a0a 2020 2020 7265 7475  (self):.    retu
-0000a330: 726e 2028 0a20 2020 2020 2020 206e 6f74  rn (.        not
-0000a340: 2073 656c 662e 5f73 7461 7465 2e69 735f   self._state.is_
-0000a350: 696e 6974 6961 6c69 7a65 6420 2023 2061  initialized  # a
-0000a360: 6c6c 6f77 2065 6167 6572 2061 7474 6163  llow eager attac
-0000a370: 686d 656e 7420 696e 2070 6f73 742d 696e  hment in post-in
-0000a380: 6974 0a20 2020 2020 2020 206f 7220 7365  it.        or se
-0000a390: 6c66 2e5f 7374 6174 652e 696e 5f73 6574  lf._state.in_set
-0000a3a0: 7570 0a20 2020 2020 2020 206f 7220 7365  up.        or se
-0000a3b0: 6c66 2e5f 7374 6174 652e 696e 5f63 6f6d  lf._state.in_com
-0000a3c0: 7061 6374 5f6d 6574 686f 640a 2020 2020  pact_method.    
-0000a3d0: 290a 0a20 2064 6566 2063 6c6f 6e65 280a  )..  def clone(.
-0000a3e0: 2020 2020 2020 7365 6c66 3a20 4d2c 0a20        self: M,. 
-0000a3f0: 2020 2020 202a 2c0a 2020 2020 2020 7061       *,.      pa
-0000a400: 7265 6e74 3a20 4f70 7469 6f6e 616c 5b55  rent: Optional[U
-0000a410: 6e69 6f6e 5b53 636f 7065 2c20 274d 6f64  nion[Scope, 'Mod
-0000a420: 756c 6527 5d5d 203d 204e 6f6e 652c 0a20  ule']] = None,. 
-0000a430: 2020 2020 205f 6465 6570 5f63 6c6f 6e65       _deep_clone
-0000a440: 3a20 556e 696f 6e5b 626f 6f6c 2c20 7765  : Union[bool, we
-0000a450: 616b 7265 662e 5765 616b 5661 6c75 6544  akref.WeakValueD
-0000a460: 6963 7469 6f6e 6172 795d 203d 2046 616c  ictionary] = Fal
-0000a470: 7365 2c0a 2020 2020 2020 2a2a 7570 6461  se,.      **upda
-0000a480: 7465 732c 0a20 2029 202d 3e20 4d3a 0a20  tes,.  ) -> M:. 
-0000a490: 2020 2022 2222 4372 6561 7465 7320 6120     """Creates a 
-0000a4a0: 636c 6f6e 6520 6f66 2074 6869 7320 4d6f  clone of this Mo
-0000a4b0: 6475 6c65 2c20 7769 7468 206f 7074 696f  dule, with optio
-0000a4c0: 6e61 6c6c 7920 7570 6461 7465 6420 6172  nally updated ar
-0000a4d0: 6775 6d65 6e74 732e 0a0a 2020 2020 4172  guments...    Ar
-0000a4e0: 6773 3a0a 2020 2020 2020 7061 7265 6e74  gs:.      parent
-0000a4f0: 3a20 5468 6520 7061 7265 6e74 206f 6620  : The parent of 
-0000a500: 7468 6520 636c 6f6e 652e 2054 6865 2063  the clone. The c
-0000a510: 6c6f 6e65 2077 696c 6c20 6861 7665 206e  lone will have n
-0000a520: 6f20 7061 7265 6e74 2069 6620 6e6f 0a20  o parent if no. 
-0000a530: 2020 2020 2020 2065 7870 6c69 6369 7420         explicit 
-0000a540: 7061 7265 6e74 2069 7320 7370 6563 6966  parent is specif
-0000a550: 6965 642e 0a20 2020 2020 205f 6465 6570  ied..      _deep
-0000a560: 5f63 6c6f 6e65 3a20 4120 626f 6f6c 6561  _clone: A boolea
-0000a570: 6e20 6f72 2061 2077 6561 6b20 7661 6c75  n or a weak valu
-0000a580: 6520 6469 6374 696f 6e61 7279 2074 6f20  e dictionary to 
-0000a590: 636f 6e74 726f 6c20 6465 6570 2063 6c6f  control deep clo
-0000a5a0: 6e69 6e67 0a20 2020 2020 2020 206f 6620  ning.        of 
-0000a5b0: 7375 626d 6f64 756c 6573 2e20 4966 2054  submodules. If T
-0000a5c0: 7275 652c 2073 7562 6d6f 6475 6c65 7320  rue, submodules 
-0000a5d0: 7769 6c6c 2062 6520 636c 6f6e 6564 2072  will be cloned r
-0000a5e0: 6563 7572 7369 7665 6c79 2e20 4966 2061  ecursively. If a
-0000a5f0: 0a20 2020 2020 2020 2077 6561 6b20 7661  .        weak va
-0000a600: 6c75 6520 6469 6374 696f 6e61 7279 2069  lue dictionary i
-0000a610: 7320 7061 7373 6564 2c20 6974 2077 696c  s passed, it wil
-0000a620: 6c20 6265 2075 7365 6420 746f 2063 6163  l be used to cac
-0000a630: 6865 2063 6c6f 6e65 640a 2020 2020 2020  he cloned.      
-0000a640: 2020 7375 626d 6f64 756c 6573 2e20 5468    submodules. Th
-0000a650: 6973 2066 6c61 6720 6973 2075 7365 6420  is flag is used 
-0000a660: 6279 2069 6e69 742f 6170 706c 792f 6269  by init/apply/bi
-0000a670: 6e64 2074 6f20 6176 6f69 6420 7363 6f70  nd to avoid scop
-0000a680: 650a 2020 2020 2020 2020 6c65 616b 6167  e.        leakag
-0000a690: 652e 0a20 2020 2020 202a 2a75 7064 6174  e..      **updat
-0000a6a0: 6573 3a20 4174 7472 6962 7574 6520 7570  es: Attribute up
-0000a6b0: 6461 7465 732e 0a20 2020 2052 6574 7572  dates..    Retur
-0000a6c0: 6e73 3a0a 2020 2020 2020 4120 636c 6f6e  ns:.      A clon
-0000a6d0: 6520 6f66 2074 6865 2074 6869 7320 4d6f  e of the this Mo
-0000a6e0: 6475 6c65 2077 6974 6820 7468 6520 7570  dule with the up
-0000a6f0: 6461 7465 6420 6174 7472 6962 7574 6573  dated attributes
-0000a700: 2061 6e64 2070 6172 656e 742e 0a20 2020   and parent..   
-0000a710: 2022 2222 0a20 2020 2061 7474 7273 203d   """.    attrs =
-0000a720: 207b 0a20 2020 2020 2020 2066 2e6e 616d   {.        f.nam
-0000a730: 653a 2067 6574 6174 7472 2873 656c 662c  e: getattr(self,
-0000a740: 2066 2e6e 616d 6529 0a20 2020 2020 2020   f.name).       
-0000a750: 2066 6f72 2066 2069 6e20 6461 7461 636c   for f in datacl
-0000a760: 6173 7365 732e 6669 656c 6473 2873 656c  asses.fields(sel
-0000a770: 6629 0a20 2020 2020 2020 2069 6620 662e  f).        if f.
-0000a780: 696e 6974 0a20 2020 207d 0a0a 2020 2020  init.    }..    
-0000a790: 6174 7472 732e 7570 6461 7465 2870 6172  attrs.update(par
-0000a7a0: 656e 743d 7061 7265 6e74 2c20 2a2a 7570  ent=parent, **up
-0000a7b0: 6461 7465 7329 0a0a 2020 2020 2320 4865  dates)..    # He
-0000a7c0: 7265 2077 6520 696d 706c 656d 656e 7420  re we implement 
-0000a7d0: 6465 6570 2063 6c6f 6e69 6e67 206f 6620  deep cloning of 
-0000a7e0: 7375 626d 6f64 756c 6573 2c20 7468 6973  submodules, this
-0000a7f0: 2069 7320 6e65 6365 7373 6172 7920 746f   is necessary to
-0000a800: 2061 766f 6964 2073 636f 7065 206c 6561   avoid scope lea
-0000a810: 6b61 6765 0a20 2020 2023 2066 726f 6d20  kage.    # from 
-0000a820: 6578 7465 726e 616c 2073 7562 6d6f 6475  external submodu
-0000a830: 6c65 7320 696e 746f 2069 6e69 742f 6170  les into init/ap
-0000a840: 706c 792f 6269 6e64 2077 6869 6c65 2070  ply/bind while p
-0000a850: 7265 7365 7276 696e 6720 7368 6172 696e  reserving sharin
-0000a860: 672d 6279 2d72 6566 6572 656e 6365 0a20  g-by-reference. 
-0000a870: 2020 2023 2072 656c 6174 696f 6e73 6869     # relationshi
-0000a880: 7073 2062 6574 7765 656e 2073 7562 6d6f  ps between submo
-0000a890: 6475 6c65 732e 0a20 2020 2069 6620 5f64  dules..    if _d
-0000a8a0: 6565 705f 636c 6f6e 6520 213d 2046 616c  eep_clone != Fal
-0000a8b0: 7365 3a0a 2020 2020 2020 2320 5765 2075  se:.      # We u
-0000a8c0: 7365 2061 2077 6561 6b20 7661 6c75 6520  se a weak value 
-0000a8d0: 6469 6374 696f 6e61 7279 2074 6f20 6361  dictionary to ca
-0000a8e0: 6368 6520 636c 6f6e 6564 2073 7562 6d6f  che cloned submo
-0000a8f0: 6475 6c65 732e 2057 6865 6e20 6120 7368  dules. When a sh
-0000a900: 6172 6564 0a20 2020 2020 2023 2073 7562  ared.      # sub
-0000a910: 6d6f 6475 6c65 2069 7320 636c 6f6e 6564  module is cloned
-0000a920: 2c20 6974 7320 6f6e 6c79 2063 6c6f 6e65  , its only clone
-0000a930: 6420 6f6e 6365 2065 6c73 6520 6974 7320  d once else its 
-0000a940: 6665 7463 6865 6420 6672 6f6d 2074 6865  fetched from the
-0000a950: 2063 6163 6865 2e0a 2020 2020 2020 6361   cache..      ca
-0000a960: 6368 6520 3d20 280a 2020 2020 2020 2020  che = (.        
-0000a970: 2020 7765 616b 7265 662e 5765 616b 5661    weakref.WeakVa
-0000a980: 6c75 6544 6963 7469 6f6e 6172 7928 290a  lueDictionary().
-0000a990: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0000a9a0: 6e73 7461 6e63 6528 5f64 6565 705f 636c  nstance(_deep_cl
-0000a9b0: 6f6e 652c 2062 6f6f 6c29 0a20 2020 2020  one, bool).     
-0000a9c0: 2020 2020 2065 6c73 6520 5f64 6565 705f       else _deep_
-0000a9d0: 636c 6f6e 650a 2020 2020 2020 290a 0a20  clone.      ).. 
-0000a9e0: 2020 2020 2064 6566 2063 6c6f 6e65 5f66       def clone_f
-0000a9f0: 6e28 6d3a 204d 6f64 756c 6529 202d 3e20  n(m: Module) -> 
-0000aa00: 4d6f 6475 6c65 3a0a 2020 2020 2020 2020  Module:.        
-0000aa10: 6966 2068 6173 6174 7472 286d 2c20 275f  if hasattr(m, '_
-0000aa20: 6964 2729 3a0a 2020 2020 2020 2020 2020  id'):.          
-0000aa30: 6b65 7920 3d20 6d2e 5f69 640a 2020 2020  key = m._id.    
-0000aa40: 2020 2020 2020 6966 206b 6579 2069 6e20        if key in 
-0000aa50: 6361 6368 653a 0a20 2020 2020 2020 2020  cache:.         
-0000aa60: 2020 2072 6574 7572 6e20 6361 6368 655b     return cache[
-0000aa70: 6b65 795d 0a20 2020 2020 2020 2020 2065  key].          e
-0000aa80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000aa90: 2063 6c6f 6e65 203d 206d 2e63 6c6f 6e65   clone = m.clone
-0000aaa0: 285f 6465 6570 5f63 6c6f 6e65 3d63 6163  (_deep_clone=cac
-0000aab0: 6865 290a 2020 2020 2020 2020 2020 2020  he).            
-0000aac0: 6361 6368 655b 6b65 795d 203d 2063 6c6f  cache[key] = clo
-0000aad0: 6e65 0a20 2020 2020 2020 2020 2020 2072  ne.            r
-0000aae0: 6574 7572 6e20 636c 6f6e 650a 2020 2020  eturn clone.    
-0000aaf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ab00: 2020 2020 2320 4966 2074 6865 206d 6f64      # If the mod
-0000ab10: 756c 6520 646f 6573 6e27 7420 6861 7665  ule doesn't have
-0000ab20: 2061 6e20 5f69 6420 6174 7472 6962 7574   an _id attribut
-0000ab30: 6520 6974 2063 6f75 6c64 2062 6520 6120  e it could be a 
-0000ab40: 6d6f 636b 206f 626a 6563 740a 2020 2020  mock object.    
-0000ab50: 2020 2020 2020 2320 736f 2077 6520 7265        # so we re
-0000ab60: 7475 726e 2069 7420 6173 2069 732e 0a20  turn it as is.. 
-0000ab70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000ab80: 6d0a 0a20 2020 2020 2023 205f 6d61 705f  m..      # _map_
-0000ab90: 7375 626d 6f64 756c 6573 2077 696c 6c20  submodules will 
-0000aba0: 6d61 7020 6f76 6572 2061 6c6c 2073 7562  map over all sub
-0000abb0: 6d6f 6475 6c65 7320 696e 7369 6465 2061  modules inside a
-0000abc0: 7474 7273 0a20 2020 2020 2023 2076 616c  ttrs.      # val
-0000abd0: 7565 2068 6572 6520 6361 6e20 6265 2061  ue here can be a
-0000abe0: 6e79 2070 7974 7265 652c 206e 6f6e 2d6d  ny pytree, non-m
-0000abf0: 6f64 756c 6520 7661 6c75 6573 2061 7265  odule values are
-0000ac00: 2069 676e 6f72 6564 0a20 2020 2020 2066   ignored.      f
-0000ac10: 6f72 2066 6965 6c64 5f6e 616d 652c 2076  or field_name, v
-0000ac20: 616c 7565 2069 6e20 6174 7472 732e 6974  alue in attrs.it
-0000ac30: 656d 7328 293a 0a20 2020 2020 2020 2061  ems():.        a
-0000ac40: 7474 7273 5b66 6965 6c64 5f6e 616d 655d  ttrs[field_name]
-0000ac50: 203d 205f 6d61 705f 7375 626d 6f64 756c   = _map_submodul
-0000ac60: 6573 2863 6c6f 6e65 5f66 6e2c 2076 616c  es(clone_fn, val
-0000ac70: 7565 290a 0a20 2020 206d 6f64 756c 6520  ue)..    module 
-0000ac80: 3d20 7365 6c66 2e5f 5f63 6c61 7373 5f5f  = self.__class__
-0000ac90: 282a 2a61 7474 7273 290a 0a20 2020 2072  (**attrs)..    r
-0000aca0: 6574 7572 6e20 6d6f 6475 6c65 0a0a 2020  eturn module..  
-0000acb0: 6465 6620 7661 7269 6162 6c65 280a 2020  def variable(.  
-0000acc0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000acd0: 636f 6c3a 2073 7472 2c0a 2020 2020 2020  col: str,.      
-0000ace0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-0000acf0: 2069 6e69 745f 666e 3a20 4f70 7469 6f6e   init_fn: Option
-0000ad00: 616c 5b43 616c 6c61 626c 655b 2e2e 2e2c  al[Callable[...,
-0000ad10: 2041 6e79 5d5d 203d 204e 6f6e 652c 0a20   Any]] = None,. 
-0000ad20: 2020 2020 202a 696e 6974 5f61 7267 732c       *init_args,
-0000ad30: 0a20 2020 2020 2075 6e62 6f78 3a20 626f  .      unbox: bo
-0000ad40: 6f6c 203d 2054 7275 652c 0a20 2029 202d  ol = True,.  ) -
-0000ad50: 3e20 5661 7269 6162 6c65 3a0a 2020 2020  > Variable:.    
-0000ad60: 2222 2244 6563 6c61 7265 7320 616e 6420  """Declares and 
-0000ad70: 7265 7475 726e 7320 6120 7661 7269 6162  returns a variab
-0000ad80: 6c65 2069 6e20 7468 6973 204d 6f64 756c  le in this Modul
-0000ad90: 652e 0a0a 2020 2020 5365 6520 3a6d 6f64  e...    See :mod
-0000ada0: 3a60 666c 6178 2e63 6f72 652e 7661 7269  :`flax.core.vari
-0000adb0: 6162 6c65 7360 2066 6f72 206d 6f72 6520  ables` for more 
-0000adc0: 696e 666f 726d 6174 696f 6e2e 2053 6565  information. See
-0000add0: 2061 6c73 6f20 3a6d 6574 683a 6070 6172   also :meth:`par
-0000ade0: 616d 600a 2020 2020 666f 7220 6120 7368  am`.    for a sh
-0000adf0: 6f72 7468 616e 6420 7761 7920 746f 2064  orthand way to d
-0000ae00: 6566 696e 6520 7265 6164 2d6f 6e6c 7920  efine read-only 
-0000ae10: 7661 7269 6162 6c65 7320 696e 2074 6865  variables in the
-0000ae20: 2022 7061 7261 6d73 220a 2020 2020 636f   "params".    co
-0000ae30: 6c6c 6563 7469 6f6e 2e0a 0a20 2020 2043  llection...    C
-0000ae40: 6f6e 7472 6172 7920 746f 203a 6d65 7468  ontrary to :meth
-0000ae50: 3a60 7061 7261 6d60 2c20 616c 6c20 6172  :`param`, all ar
-0000ae60: 6775 6d65 6e74 7320 7061 7373 696e 6720  guments passing 
-0000ae70: 7573 696e 6720 6069 6e69 745f 666e 6020  using `init_fn` 
-0000ae80: 7368 6f75 6c64 2062 650a 2020 2020 7061  should be.    pa
-0000ae90: 7373 6564 206f 6e20 6578 706c 6963 6974  ssed on explicit
-0000aea0: 6c79 3a3a 0a0a 2020 2020 2020 6b65 7920  ly::..      key 
-0000aeb0: 3d20 7365 6c66 2e6d 616b 655f 726e 6728  = self.make_rng(
-0000aec0: 2773 7461 7473 2729 0a20 2020 2020 206d  'stats').      m
-0000aed0: 6561 6e20 3d20 7365 6c66 2e76 6172 6961  ean = self.varia
-0000aee0: 626c 6528 2773 7461 7473 272c 2027 6d65  ble('stats', 'me
-0000aef0: 616e 272c 206c 6563 756e 5f6e 6f72 6d61  an', lecun_norma
-0000af00: 6c28 292c 206b 6579 2c20 2832 2c20 3229  l(), key, (2, 2)
-0000af10: 290a 0a20 2020 2049 6e20 7468 6520 6578  )..    In the ex
-0000af20: 616d 706c 6520 6162 6f76 652c 2074 6865  ample above, the
-0000af30: 2066 756e 6374 696f 6e20 606c 6563 756e   function `lecun
-0000af40: 5f6e 6f72 6d61 6c60 2065 7870 6563 7473  _normal` expects
-0000af50: 2074 776f 2061 7267 756d 656e 7473 3a0a   two arguments:.
-0000af60: 2020 2020 606b 6579 6020 616e 6420 6073      `key` and `s
-0000af70: 6861 7065 602c 2061 6e64 2062 6f74 6820  hape`, and both 
-0000af80: 6861 7665 2074 6f20 6265 2070 6173 7365  have to be passe
-0000af90: 6420 6f6e 2e20 5468 6520 5052 4e47 2066  d on. The PRNG f
-0000afa0: 6f72 2060 7374 6174 7360 2068 6173 0a20  or `stats` has. 
-0000afb0: 2020 2074 6f20 6265 2070 726f 7669 6465     to be provide
-0000afc0: 6420 6578 706c 6963 6974 6c79 2077 6865  d explicitly whe
-0000afd0: 6e20 6361 6c6c 696e 6720 3a6d 6574 683a  n calling :meth:
-0000afe0: 6069 6e69 7460 2061 6e64 203a 6d65 7468  `init` and :meth
-0000aff0: 3a60 6170 706c 7960 2e0a 0a20 2020 2041  :`apply`...    A
-0000b000: 7267 733a 0a20 2020 2020 2063 6f6c 3a20  rgs:.      col: 
-0000b010: 5468 6520 7661 7269 6162 6c65 2063 6f6c  The variable col
-0000b020: 6c65 6374 696f 6e20 6e61 6d65 2e0a 2020  lection name..  
-0000b030: 2020 2020 6e61 6d65 3a20 5468 6520 7661      name: The va
-0000b040: 7269 6162 6c65 206e 616d 652e 0a20 2020  riable name..   
-0000b050: 2020 2069 6e69 745f 666e 3a20 5468 6520     init_fn: The 
-0000b060: 6675 6e63 7469 6f6e 2074 6861 7420 7769  function that wi
-0000b070: 6c6c 2062 6520 6361 6c6c 6564 2074 6f20  ll be called to 
-0000b080: 636f 6d70 7574 6520 7468 6520 696e 6974  compute the init
-0000b090: 6961 6c20 7661 6c75 650a 2020 2020 2020  ial value.      
-0000b0a0: 2020 6f66 2074 6869 7320 7661 7269 6162    of this variab
-0000b0b0: 6c65 2e20 5468 6973 2066 756e 6374 696f  le. This functio
-0000b0c0: 6e20 7769 6c6c 206f 6e6c 7920 6265 2063  n will only be c
-0000b0d0: 616c 6c65 6420 7468 6520 6669 7273 7420  alled the first 
-0000b0e0: 7469 6d65 0a20 2020 2020 2020 2074 6869  time.        thi
-0000b0f0: 7320 7661 7269 6162 6c65 2069 7320 7573  s variable is us
-0000b100: 6564 2069 6e20 7468 6973 206d 6f64 756c  ed in this modul
-0000b110: 652e 2049 6620 4e6f 6e65 2c20 7468 6520  e. If None, the 
-0000b120: 7661 7269 6162 6c65 206d 7573 740a 2020  variable must.  
-0000b130: 2020 2020 2020 616c 7265 6164 7920 6265        already be
-0000b140: 2069 6e69 7469 616c 697a 6564 206f 7468   initialized oth
-0000b150: 6572 7769 7365 2061 6e20 6572 726f 7220  erwise an error 
-0000b160: 6973 2072 6169 7365 642e 0a20 2020 2020  is raised..     
-0000b170: 202a 696e 6974 5f61 7267 733a 2054 6865   *init_args: The
-0000b180: 2061 7267 756d 656e 7473 2074 6f20 7061   arguments to pa
-0000b190: 7373 2074 6f20 696e 6974 5f66 6e2e 0a20  ss to init_fn.. 
-0000b1a0: 2020 2020 2075 6e62 6f78 3a20 4966 2054       unbox: If T
-0000b1b0: 7275 652c 2060 6041 7869 734d 6574 6164  rue, ``AxisMetad
-0000b1c0: 6174 6160 6020 696e 7374 616e 6365 7320  ata`` instances 
-0000b1d0: 6172 6520 7265 706c 6163 6564 2062 7920  are replaced by 
-0000b1e0: 7468 6569 7220 756e 626f 7865 640a 2020  their unboxed.  
-0000b1f0: 2020 2020 2020 7661 6c75 652c 2073 6565        value, see
-0000b200: 2060 6066 6c61 782e 6e6e 2e6d 6574 612e   ``flax.nn.meta.
-0000b210: 756e 626f 7860 6020 2864 6566 6175 6c74  unbox`` (default
-0000b220: 3a20 5472 7565 292e 0a0a 2020 2020 5265  : True)...    Re
-0000b230: 7475 726e 733a 0a20 2020 2020 2041 203a  turns:.      A :
-0000b240: 636c 6173 733a 6066 6c61 782e 636f 7265  class:`flax.core
-0000b250: 2e76 6172 6961 626c 6573 2e56 6172 6961  .variables.Varia
-0000b260: 626c 6560 2074 6861 7420 6361 6e20 6265  ble` that can be
-0000b270: 2072 6561 6420 6f72 2073 6574 2076 6961   read or set via
-0000b280: 0a20 2020 2020 2022 2e76 616c 7565 2220  .      ".value" 
-0000b290: 6174 7472 6962 7574 652e 2054 6872 6f77  attribute. Throw
-0000b2a0: 7320 616e 2065 7272 6f72 2069 6620 7468  s an error if th
-0000b2b0: 6520 7661 7269 6162 6c65 2065 7869 7374  e variable exist
-0000b2c0: 7320 616c 7265 6164 792e 0a20 2020 2022  s already..    "
-0000b2d0: 2222 0a20 2020 2069 6620 6e6f 7420 7365  "".    if not se
-0000b2e0: 6c66 2e5f 696e 6974 6961 6c69 7a61 7469  lf._initializati
-0000b2f0: 6f6e 5f61 6c6c 6f77 6564 3a0a 2020 2020  on_allowed:.    
-0000b300: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000b310: 6f72 280a 2020 2020 2020 2020 2020 2756  or(.          'V
-0000b320: 6172 6961 626c 6573 206d 7573 7420 6265  ariables must be
-0000b330: 2069 6e69 7469 616c 697a 6564 2069 6e20   initialized in 
-0000b340: 6073 6574 7570 2829 6020 6f72 2069 6e20  `setup()` or in 
-0000b350: 6120 6d65 7468 6f64 2027 0a20 2020 2020  a method '.     
-0000b360: 2020 2020 2027 7772 6170 7065 6420 696e       'wrapped in
-0000b370: 2060 4063 6f6d 7061 6374 6027 0a20 2020   `@compact`'.   
-0000b380: 2020 2029 0a20 2020 2069 6620 7365 6c66     ).    if self
-0000b390: 2e5f 6e61 6d65 5f74 616b 656e 286e 616d  ._name_taken(nam
-0000b3a0: 652c 2063 6f6c 6c65 6374 696f 6e3d 636f  e, collection=co
-0000b3b0: 6c29 3a0a 2020 2020 2020 7261 6973 6520  l):.      raise 
-0000b3c0: 6572 726f 7273 2e4e 616d 6549 6e55 7365  errors.NameInUse
-0000b3d0: 4572 726f 7228 2776 6172 6961 626c 6527  Error('variable'
-0000b3e0: 2c20 6e61 6d65 2c20 7365 6c66 2e5f 5f63  , name, self.__c
-0000b3f0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f29  lass__.__name__)
-0000b400: 0a20 2020 2061 7373 6572 7420 7365 6c66  .    assert self
-0000b410: 2e73 636f 7065 2069 7320 6e6f 7420 4e6f  .scope is not No
-0000b420: 6e65 0a20 2020 2076 203d 2073 656c 662e  ne.    v = self.
-0000b430: 7363 6f70 652e 7661 7269 6162 6c65 2863  scope.variable(c
-0000b440: 6f6c 2c20 6e61 6d65 2c20 696e 6974 5f66  ol, name, init_f
-0000b450: 6e2c 202a 696e 6974 5f61 7267 732c 2075  n, *init_args, u
-0000b460: 6e62 6f78 3d75 6e62 6f78 290a 2020 2020  nbox=unbox).    
-0000b470: 7365 6c66 2e5f 7374 6174 652e 6368 696c  self._state.chil
-0000b480: 6472 656e 5b6e 616d 655d 203d 2063 6f6c  dren[name] = col
-0000b490: 0a20 2020 2072 6574 7572 6e20 760a 0a20  .    return v.. 
-0000b4a0: 2064 6566 2070 6172 616d 280a 2020 2020   def param(.    
-0000b4b0: 2020 7365 6c66 2c20 6e61 6d65 3a20 7374    self, name: st
-0000b4c0: 722c 2069 6e69 745f 666e 3a20 4361 6c6c  r, init_fn: Call
-0000b4d0: 6162 6c65 5b2e 2e2e 2c20 545d 2c20 2a69  able[..., T], *i
-0000b4e0: 6e69 745f 6172 6773 2c20 756e 626f 783a  nit_args, unbox:
-0000b4f0: 2062 6f6f 6c20 3d20 5472 7565 0a20 2029   bool = True.  )
-0000b500: 202d 3e20 543a 0a20 2020 2022 2222 4465   -> T:.    """De
-0000b510: 636c 6172 6573 2061 6e64 2072 6574 7572  clares and retur
-0000b520: 6e73 2061 2070 6172 616d 6574 6572 2069  ns a parameter i
-0000b530: 6e20 7468 6973 204d 6f64 756c 652e 0a0a  n this Module...
-0000b540: 2020 2020 5061 7261 6d65 7465 7273 2061      Parameters a
-0000b550: 7265 2072 6561 642d 6f6e 6c79 2076 6172  re read-only var
-0000b560: 6961 626c 6573 2069 6e20 7468 6520 636f  iables in the co
-0000b570: 6c6c 6563 7469 6f6e 206e 616d 6564 2022  llection named "
-0000b580: 7061 7261 6d73 222e 2053 6565 0a20 2020  params". See.   
-0000b590: 203a 6d6f 643a 6066 6c61 782e 636f 7265   :mod:`flax.core
-0000b5a0: 2e76 6172 6961 626c 6573 6020 666f 7220  .variables` for 
-0000b5b0: 6d6f 7265 2064 6574 6169 6c73 206f 6e20  more details on 
-0000b5c0: 7661 7269 6162 6c65 732e 0a0a 2020 2020  variables...    
-0000b5d0: 5468 6520 6669 7273 7420 6172 6775 6d65  The first argume
-0000b5e0: 6e74 206f 6620 6069 6e69 745f 666e 6020  nt of `init_fn` 
-0000b5f0: 6973 2061 7373 756d 6564 2074 6f20 6265  is assumed to be
-0000b600: 2061 2050 524e 4720 6b65 792c 2077 6869   a PRNG key, whi
-0000b610: 6368 2069 730a 2020 2020 7072 6f76 6964  ch is.    provid
-0000b620: 6564 2061 7574 6f6d 6174 6963 616c 6c79  ed automatically
-0000b630: 2061 6e64 2064 6f65 7320 6e6f 7420 6861   and does not ha
-0000b640: 7665 2074 6f20 6265 2070 6173 7365 6420  ve to be passed 
-0000b650: 7573 696e 6720 6069 6e69 745f 6172 6773  using `init_args
-0000b660: 603a 3a0a 0a20 2020 2020 206d 6561 6e20  `::..      mean 
-0000b670: 3d20 7365 6c66 2e70 6172 616d 2827 6d65  = self.param('me
-0000b680: 616e 272c 206c 6563 756e 5f6e 6f72 6d61  an', lecun_norma
-0000b690: 6c28 292c 2028 322c 2032 2929 0a0a 2020  l(), (2, 2))..  
-0000b6a0: 2020 496e 2074 6865 2065 7861 6d70 6c65    In the example
-0000b6b0: 2061 626f 7665 2c20 7468 6520 6675 6e63   above, the func
-0000b6c0: 7469 6f6e 2060 6c65 6375 6e5f 6e6f 726d  tion `lecun_norm
-0000b6d0: 616c 6020 6578 7065 6374 7320 7477 6f20  al` expects two 
-0000b6e0: 6172 6775 6d65 6e74 733a 0a20 2020 2060  arguments:.    `
-0000b6f0: 6b65 7960 2061 6e64 2060 7368 6170 6560  key` and `shape`
-0000b700: 2c20 6275 7420 6f6e 6c79 2060 7368 6170  , but only `shap
-0000b710: 6560 2068 6173 2074 6f20 6265 2070 726f  e` has to be pro
-0000b720: 7669 6465 6420 6578 706c 6963 6974 6c79  vided explicitly
-0000b730: 3b20 606b 6579 600a 2020 2020 6973 2073  ; `key`.    is s
-0000b740: 6574 2061 7574 6f6d 6174 6963 616c 6c79  et automatically
-0000b750: 2075 7369 6e67 2074 6865 2050 524e 4720   using the PRNG 
-0000b760: 666f 7220 6070 6172 616d 7360 2074 6861  for `params` tha
-0000b770: 7420 6973 2070 6173 7365 6420 7768 656e  t is passed when
-0000b780: 0a20 2020 2069 6e69 7469 616c 697a 696e  .    initializin
-0000b790: 6720 7468 6520 6d6f 6475 6c65 2075 7369  g the module usi
-0000b7a0: 6e67 203a 6d65 7468 3a60 696e 6974 602e  ng :meth:`init`.
-0000b7b0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-0000b7c0: 2020 6e61 6d65 3a20 5468 6520 7061 7261    name: The para
-0000b7d0: 6d65 7465 7220 6e61 6d65 2e0a 2020 2020  meter name..    
-0000b7e0: 2020 696e 6974 5f66 6e3a 2054 6865 2066    init_fn: The f
-0000b7f0: 756e 6374 696f 6e20 7468 6174 2077 696c  unction that wil
-0000b800: 6c20 6265 2063 616c 6c65 6420 746f 2063  l be called to c
-0000b810: 6f6d 7075 7465 2074 6865 2069 6e69 7469  ompute the initi
-0000b820: 616c 2076 616c 7565 0a20 2020 2020 2020  al value.       
-0000b830: 206f 6620 7468 6973 2076 6172 6961 626c   of this variabl
-0000b840: 652e 2054 6869 7320 6675 6e63 7469 6f6e  e. This function
-0000b850: 2077 696c 6c20 6f6e 6c79 2062 6520 6361   will only be ca
-0000b860: 6c6c 6564 2074 6865 2066 6972 7374 2074  lled the first t
-0000b870: 696d 650a 2020 2020 2020 2020 7468 6973  ime.        this
-0000b880: 2070 6172 616d 6574 6572 2069 7320 7573   parameter is us
-0000b890: 6564 2069 6e20 7468 6973 206d 6f64 756c  ed in this modul
-0000b8a0: 652e 0a20 2020 2020 202a 696e 6974 5f61  e..      *init_a
-0000b8b0: 7267 733a 2054 6865 2061 7267 756d 656e  rgs: The argumen
-0000b8c0: 7473 2074 6f20 7061 7373 2074 6f20 696e  ts to pass to in
-0000b8d0: 6974 5f66 6e2e 0a20 2020 2020 2075 6e62  it_fn..      unb
-0000b8e0: 6f78 3a20 4966 2054 7275 652c 2060 6041  ox: If True, ``A
-0000b8f0: 7869 734d 6574 6164 6174 6160 6020 696e  xisMetadata`` in
-0000b900: 7374 616e 6365 7320 6172 6520 7265 706c  stances are repl
-0000b910: 6163 6564 2062 7920 7468 6569 7220 756e  aced by their un
-0000b920: 626f 7865 640a 2020 2020 2020 2020 7661  boxed.        va
-0000b930: 6c75 652c 2073 6565 2060 6066 6c61 782e  lue, see ``flax.
-0000b940: 6e6e 2e6d 6574 612e 756e 626f 7860 6020  nn.meta.unbox`` 
-0000b950: 2864 6566 6175 6c74 3a20 5472 7565 292e  (default: True).
-0000b960: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000b970: 2020 2020 2054 6865 2076 616c 7565 206f       The value o
-0000b980: 6620 7468 6520 696e 6974 6961 6c69 7a65  f the initialize
-0000b990: 6420 7061 7261 6d65 7465 722e 2054 6872  d parameter. Thr
-0000b9a0: 6f77 7320 616e 2065 7272 6f72 2069 6620  ows an error if 
-0000b9b0: 7468 6520 7061 7261 6d65 7465 720a 2020  the parameter.  
-0000b9c0: 2020 2020 6578 6973 7473 2061 6c72 6561      exists alrea
-0000b9d0: 6479 2e0a 2020 2020 2222 220a 2020 2020  dy..    """.    
-0000b9e0: 6966 206e 6f74 2073 656c 662e 5f69 6e69  if not self._ini
-0000b9f0: 7469 616c 697a 6174 696f 6e5f 616c 6c6f  tialization_allo
-0000ba00: 7765 643a 0a20 2020 2020 2072 6169 7365  wed:.      raise
-0000ba10: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-0000ba20: 2020 2020 2020 2027 5061 7261 6d65 7465         'Paramete
-0000ba30: 7273 206d 7573 7420 6265 2069 6e69 7469  rs must be initi
-0000ba40: 616c 697a 6564 2069 6e20 6073 6574 7570  alized in `setup
-0000ba50: 2829 6020 6f72 2069 6e20 6120 6d65 7468  ()` or in a meth
-0000ba60: 6f64 2027 0a20 2020 2020 2020 2020 2027  od '.          '
-0000ba70: 7772 6170 7065 6420 696e 2060 4063 6f6d  wrapped in `@com
-0000ba80: 7061 6374 6027 0a20 2020 2020 2029 0a20  pact`'.      ). 
-0000ba90: 2020 2069 6620 7365 6c66 2e5f 6e61 6d65     if self._name
-0000baa0: 5f74 616b 656e 286e 616d 652c 2063 6f6c  _taken(name, col
-0000bab0: 6c65 6374 696f 6e3d 2770 6172 616d 7327  lection='params'
-0000bac0: 293a 0a20 2020 2020 2072 6169 7365 2065  ):.      raise e
-0000bad0: 7272 6f72 732e 4e61 6d65 496e 5573 6545  rrors.NameInUseE
-0000bae0: 7272 6f72 2827 7061 7261 6d27 2c20 6e61  rror('param', na
-0000baf0: 6d65 2c20 7365 6c66 2e5f 5f63 6c61 7373  me, self.__class
-0000bb00: 5f5f 2e5f 5f6e 616d 655f 5f29 0a20 2020  __.__name__).   
-0000bb10: 2061 7373 6572 7420 7365 6c66 2e73 636f   assert self.sco
-0000bb20: 7065 2069 7320 6e6f 7420 4e6f 6e65 0a20  pe is not None. 
-0000bb30: 2020 2076 203d 2073 656c 662e 7363 6f70     v = self.scop
-0000bb40: 652e 7061 7261 6d28 6e61 6d65 2c20 696e  e.param(name, in
-0000bb50: 6974 5f66 6e2c 202a 696e 6974 5f61 7267  it_fn, *init_arg
-0000bb60: 732c 2075 6e62 6f78 3d75 6e62 6f78 290a  s, unbox=unbox).
-0000bb70: 2020 2020 7365 6c66 2e5f 7374 6174 652e      self._state.
-0000bb80: 6368 696c 6472 656e 5b6e 616d 655d 203d  children[name] =
-0000bb90: 2027 7061 7261 6d73 270a 2020 2020 7265   'params'.    re
-0000bba0: 7475 726e 2076 0a0a 2020 6465 6620 6861  turn v..  def ha
-0000bbb0: 735f 7661 7269 6162 6c65 2873 656c 662c  s_variable(self,
-0000bbc0: 2063 6f6c 3a20 7374 722c 206e 616d 653a   col: str, name:
-0000bbd0: 2073 7472 2920 2d3e 2062 6f6f 6c3a 0a20   str) -> bool:. 
-0000bbe0: 2020 2022 2222 4368 6563 6b73 2069 6620     """Checks if 
-0000bbf0: 6120 7661 7269 6162 6c65 206f 6620 6769  a variable of gi
-0000bc00: 7665 6e20 636f 6c6c 6563 7469 6f6e 2061  ven collection a
-0000bc10: 6e64 206e 616d 6520 6578 6973 7473 2069  nd name exists i
-0000bc20: 6e20 7468 6973 204d 6f64 756c 652e 0a0a  n this Module...
-0000bc30: 2020 2020 5365 6520 3a6d 6f64 3a60 666c      See :mod:`fl
-0000bc40: 6178 2e63 6f72 652e 7661 7269 6162 6c65  ax.core.variable
-0000bc50: 7360 2066 6f72 206d 6f72 6520 6578 706c  s` for more expl
-0000bc60: 616e 6174 696f 6e20 6f6e 2076 6172 6961  anation on varia
-0000bc70: 626c 6573 2061 6e64 0a20 2020 2063 6f6c  bles and.    col
-0000bc80: 6c65 6374 696f 6e73 2e0a 0a20 2020 2041  lections...    A
-0000bc90: 7267 733a 0a20 2020 2020 2063 6f6c 3a20  rgs:.      col: 
-0000bca0: 5468 6520 7661 7269 6162 6c65 2063 6f6c  The variable col
-0000bcb0: 6c65 6374 696f 6e20 6e61 6d65 2e0a 2020  lection name..  
-0000bcc0: 2020 2020 6e61 6d65 3a20 5468 6520 6e61      name: The na
-0000bcd0: 6d65 206f 6620 7468 6520 7661 7269 6162  me of the variab
-0000bce0: 6c65 2e0a 2020 2020 5265 7475 726e 733a  le..    Returns:
-0000bcf0: 0a20 2020 2020 2054 7275 6520 6966 2074  .      True if t
-0000bd00: 6865 2076 6172 6961 626c 6520 6578 6973  he variable exis
-0000bd10: 7473 2e0a 2020 2020 2222 220a 2020 2020  ts..    """.    
-0000bd20: 6966 2073 656c 662e 7363 6f70 6520 6973  if self.scope is
-0000bd30: 204e 6f6e 653a 0a20 2020 2020 2072 6169   None:.      rai
-0000bd40: 7365 2056 616c 7565 4572 726f 7228 2243  se ValueError("C
-0000bd50: 616e 2774 2061 6363 6573 7320 7661 7269  an't access vari
-0000bd60: 6162 6c65 7320 6f6e 2075 6e62 6f75 6e64  ables on unbound
-0000bd70: 206d 6f64 756c 6573 2229 0a20 2020 2072   modules").    r
-0000bd80: 6574 7572 6e20 7365 6c66 2e73 636f 7065  eturn self.scope
-0000bd90: 2e68 6173 5f76 6172 6961 626c 6528 636f  .has_variable(co
-0000bda0: 6c2c 206e 616d 6529 0a0a 2020 6465 6620  l, name)..  def 
-0000bdb0: 6973 5f6d 7574 6162 6c65 5f63 6f6c 6c65  is_mutable_colle
-0000bdc0: 6374 696f 6e28 7365 6c66 2c20 636f 6c3a  ction(self, col:
-0000bdd0: 2073 7472 2920 2d3e 2062 6f6f 6c3a 0a20   str) -> bool:. 
-0000bde0: 2020 2022 2222 5265 7475 726e 7320 7472     """Returns tr
-0000bdf0: 7565 2069 6620 7468 6520 636f 6c6c 6563  ue if the collec
-0000be00: 7469 6f6e 2060 636f 6c60 2069 7320 6d75  tion `col` is mu
-0000be10: 7461 626c 652e 2222 220a 2020 2020 6966  table.""".    if
-0000be20: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
-0000be30: 6f6e 653a 0a20 2020 2020 2072 6169 7365  one:.      raise
-0000be40: 2056 616c 7565 4572 726f 7228 2243 616e   ValueError("Can
-0000be50: 2774 2063 6865 636b 206d 7574 6162 696c  't check mutabil
-0000be60: 6974 7920 6f6e 2075 6e62 6f75 6e64 206d  ity on unbound m
-0000be70: 6f64 756c 6573 2229 0a20 2020 2072 6574  odules").    ret
-0000be80: 7572 6e20 7365 6c66 2e73 636f 7065 2e69  urn self.scope.i
-0000be90: 735f 6d75 7461 626c 655f 636f 6c6c 6563  s_mutable_collec
-0000bea0: 7469 6f6e 2863 6f6c 290a 0a20 2064 6566  tion(col)..  def
-0000beb0: 2068 6173 5f72 6e67 2873 656c 662c 206e   has_rng(self, n
-0000bec0: 616d 653a 2073 7472 2920 2d3e 2062 6f6f  ame: str) -> boo
-0000bed0: 6c3a 0a20 2020 2022 2222 5265 7475 726e  l:.    """Return
-0000bee0: 7320 7472 7565 2069 6620 6120 5052 4e47  s true if a PRNG
-0000bef0: 5365 7175 656e 6365 2077 6974 6820 6e61  Sequence with na
-0000bf00: 6d65 2060 6e61 6d65 6020 6578 6973 7473  me `name` exists
-0000bf10: 2e22 2222 0a20 2020 2069 6620 7365 6c66  .""".    if self
-0000bf20: 2e73 636f 7065 2069 7320 4e6f 6e65 3a0a  .scope is None:.
-0000bf30: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000bf40: 6545 7272 6f72 2822 4361 6e27 7420 7175  eError("Can't qu
-0000bf50: 6572 7920 666f 7220 524e 4773 206f 6e20  ery for RNGs on 
-0000bf60: 756e 626f 756e 6420 6d6f 6475 6c65 7322  unbound modules"
-0000bf70: 290a 2020 2020 7265 7475 726e 2073 656c  ).    return sel
-0000bf80: 662e 7363 6f70 652e 6861 735f 726e 6728  f.scope.has_rng(
-0000bf90: 6e61 6d65 290a 0a20 2064 6566 206d 616b  name)..  def mak
-0000bfa0: 655f 726e 6728 7365 6c66 2c20 6e61 6d65  e_rng(self, name
-0000bfb0: 3a20 7374 7229 202d 3e20 4b65 7941 7272  : str) -> KeyArr
-0000bfc0: 6179 3a0a 2020 2020 2222 2252 6574 7572  ay:.    """Retur
-0000bfd0: 6e73 2061 206e 6577 2052 4e47 206b 6579  ns a new RNG key
-0000bfe0: 2066 726f 6d20 6120 6769 7665 6e20 524e   from a given RN
-0000bff0: 4720 7365 7175 656e 6365 2066 6f72 2074  G sequence for t
-0000c000: 6869 7320 4d6f 6475 6c65 2e0a 0a20 2020  his Module...   
-0000c010: 2054 6865 206e 6577 2052 4e47 206b 6579   The new RNG key
-0000c020: 2069 7320 7370 6c69 7420 6672 6f6d 2074   is split from t
-0000c030: 6865 2070 7265 7669 6f75 7320 6f6e 652e  he previous one.
-0000c040: 2054 6875 732c 2065 7665 7279 2063 616c   Thus, every cal
-0000c050: 6c20 746f 0a20 2020 2060 6d61 6b65 5f72  l to.    `make_r
-0000c060: 6e67 6020 7265 7475 726e 7320 6120 6e65  ng` returns a ne
-0000c070: 7720 524e 4720 6b65 792c 2077 6869 6c65  w RNG key, while
-0000c080: 2073 7469 6c6c 2067 7561 7261 6e74 6565   still guarantee
-0000c090: 696e 6720 6675 6c6c 0a20 2020 2072 6570  ing full.    rep
-0000c0a0: 726f 6475 6369 6269 6c69 7479 2e0a 0a20  roducibility... 
-0000c0b0: 2020 2054 4f44 4f3a 204c 696e 6b20 746f     TODO: Link to
-0000c0c0: 2046 6c61 7820 524e 4720 6465 7369 676e   Flax RNG design
-0000c0d0: 206e 6f74 652e 0a0a 2020 2020 4172 6773   note...    Args
-0000c0e0: 3a0a 2020 2020 2020 6e61 6d65 3a20 5468  :.      name: Th
-0000c0f0: 6520 524e 4720 7365 7175 656e 6365 206e  e RNG sequence n
-0000c100: 616d 652e 0a20 2020 2052 6574 7572 6e73  ame..    Returns
-0000c110: 3a0a 2020 2020 2020 5468 6520 6e65 776c  :.      The newl
-0000c120: 7920 6765 6e65 7261 7465 6420 524e 4720  y generated RNG 
-0000c130: 6b65 792e 0a20 2020 2022 2222 0a20 2020  key..    """.   
-0000c140: 2069 6620 7365 6c66 2e73 636f 7065 2069   if self.scope i
-0000c150: 7320 4e6f 6e65 3a0a 2020 2020 2020 7261  s None:.      ra
-0000c160: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-0000c170: 4361 6e27 7420 7573 6520 524e 4773 206f  Can't use RNGs o
-0000c180: 6e20 756e 626f 756e 6420 6d6f 6475 6c65  n unbound module
-0000c190: 7322 290a 2020 2020 7265 7475 726e 2073  s").    return s
-0000c1a0: 656c 662e 7363 6f70 652e 6d61 6b65 5f72  elf.scope.make_r
-0000c1b0: 6e67 286e 616d 6529 0a0a 2020 6465 6620  ng(name)..  def 
-0000c1c0: 6973 5f69 6e69 7469 616c 697a 696e 6728  is_initializing(
-0000c1d0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-0000c1e0: 2020 2022 2222 5265 7475 726e 7320 5472     """Returns Tr
-0000c1f0: 7565 2069 6620 7275 6e6e 696e 6720 756e  ue if running un
-0000c200: 6465 7220 7365 6c66 2e69 6e69 7428 2e2e  der self.init(..
-0000c210: 2e29 206f 7220 6e6e 2e69 6e69 7428 2e2e  .) or nn.init(..
-0000c220: 2e29 2829 2e0a 0a20 2020 2054 6869 7320  .)()...    This 
-0000c230: 6973 2061 2068 656c 7065 7220 6d65 7468  is a helper meth
-0000c240: 6f64 2074 6f20 6861 6e64 6c65 2074 6865  od to handle the
-0000c250: 2063 6f6d 6d6f 6e20 6361 7365 206f 6620   common case of 
-0000c260: 7369 6d70 6c65 2069 6e69 7469 616c 697a  simple initializ
-0000c270: 6174 696f 6e0a 2020 2020 7768 6572 6520  ation.    where 
-0000c280: 7765 2077 6973 6820 746f 2068 6176 6520  we wish to have 
-0000c290: 7365 7475 7020 6c6f 6769 6320 6f63 6375  setup logic occu
-0000c2a0: 7220 7768 656e 206f 6e6c 7920 6361 6c6c  r when only call
-0000c2b0: 6564 2075 6e64 6572 0a20 2020 2060 606d  ed under.    ``m
-0000c2c0: 6f64 756c 652e 696e 6974 6060 206f 7220  odule.init`` or 
-0000c2d0: 6060 6e6e 2e69 6e69 7460 602e 2020 466f  ``nn.init``.  Fo
-0000c2e0: 7220 6d6f 7265 2063 6f6d 706c 6963 6174  r more complicat
-0000c2f0: 6564 206d 756c 7469 2d70 6861 7365 0a20  ed multi-phase. 
-0000c300: 2020 2069 6e69 7469 616c 697a 6174 696f     initializatio
-0000c310: 6e20 7363 656e 6172 696f 7320 6974 2069  n scenarios it i
-0000c320: 7320 6265 7474 6572 2074 6f20 7465 7374  s better to test
-0000c330: 2066 6f72 2074 6865 206d 7574 6162 696c   for the mutabil
-0000c340: 6974 7920 6f66 0a20 2020 2070 6172 7469  ity of.    parti
-0000c350: 6375 6c61 7220 7661 7269 6162 6c65 2063  cular variable c
-0000c360: 6f6c 6c65 6374 696f 6e73 206f 7220 666f  ollections or fo
-0000c370: 7220 7468 6520 7072 6573 656e 6365 206f  r the presence o
-0000c380: 6620 7061 7274 6963 756c 6172 0a20 2020  f particular.   
-0000c390: 2076 6172 6961 626c 6573 2074 6861 7420   variables that 
-0000c3a0: 706f 7465 6e74 6961 6c6c 7920 6e65 6564  potentially need
-0000c3b0: 2074 6f20 6265 2069 6e69 7469 616c 697a   to be initializ
-0000c3c0: 6564 2e0a 2020 2020 2222 220a 2020 2020  ed..    """.    
-0000c3d0: 6966 2073 656c 662e 7363 6f70 6520 6973  if self.scope is
-0000c3e0: 204e 6f6e 653a 0a20 2020 2020 2072 6169   None:.      rai
-0000c3f0: 7365 2056 616c 7565 4572 726f 7228 2243  se ValueError("C
-0000c400: 616e 2774 2063 6865 636b 2069 6620 7275  an't check if ru
-0000c410: 6e6e 696e 6720 756e 6465 7220 696e 6974  nning under init
-0000c420: 2829 206f 6e20 756e 626f 756e 6420 6d6f  () on unbound mo
-0000c430: 6475 6c65 7322 290a 2020 2020 7265 7475  dules").    retu
-0000c440: 726e 2073 656c 662e 7363 6f70 652e 6765  rn self.scope.ge
-0000c450: 745f 666c 6167 2827 696e 6974 6961 6c69  t_flag('initiali
-0000c460: 7a69 6e67 272c 2046 616c 7365 290a 0a20  zing', False).. 
-0000c470: 2064 6566 205f 6d6f 6475 6c65 5f63 6865   def _module_che
-0000c480: 636b 7328 7365 6c66 293a 0a20 2020 2022  cks(self):.    "
-0000c490: 2222 5275 6e20 7374 616e 6461 7264 2072  ""Run standard r
-0000c4a0: 756e 7469 6d65 2063 6865 636b 732e 2222  untime checks.""
-0000c4b0: 220a 0a20 2020 2069 6620 6e6f 7420 6973  "..    if not is
-0000c4c0: 696e 7374 616e 6365 2873 656c 662c 204d  instance(self, M
-0000c4d0: 6f64 756c 6529 3a0a 2020 2020 2020 7261  odule):.      ra
-0000c4e0: 6973 6520 6572 726f 7273 2e49 6e76 616c  ise errors.Inval
-0000c4f0: 6964 496e 7374 616e 6365 4d6f 6475 6c65  idInstanceModule
-0000c500: 4572 726f 7228 290a 0a20 2020 206f 7665  Error()..    ove
-0000c510: 7272 6964 6465 6e5f 706f 7374 5f69 6e69  rridden_post_ini
-0000c520: 7420 3d20 7365 6c66 2e5f 5f70 6f73 745f  t = self.__post_
-0000c530: 696e 6974 5f5f 2021 3d20 4d6f 6475 6c65  init__ != Module
-0000c540: 2e5f 5f70 6f73 745f 696e 6974 5f5f 0a20  .__post_init__. 
-0000c550: 2020 2069 6620 6f76 6572 7269 6464 656e     if overridden
-0000c560: 5f70 6f73 745f 696e 6974 2061 6e64 206e  _post_init and n
-0000c570: 6f74 2068 6173 6174 7472 2873 656c 662c  ot hasattr(self,
-0000c580: 2027 5f69 6427 293a 0a20 2020 2020 2072   '_id'):.      r
-0000c590: 6169 7365 2065 7272 6f72 732e 496e 636f  aise errors.Inco
-0000c5a0: 7272 6563 7450 6f73 7449 6e69 744f 7665  rrectPostInitOve
-0000c5b0: 7272 6964 6545 7272 6f72 2829 0a0a 2020  rrideError()..  
-0000c5c0: 4074 7261 6365 6261 636b 5f75 7469 6c2e  @traceback_util.
-0000c5d0: 6170 695f 626f 756e 6461 7279 0a20 2064  api_boundary.  d
-0000c5e0: 6566 2062 696e 6428 0a20 2020 2020 2073  ef bind(.      s
-0000c5f0: 656c 663a 204d 2c0a 2020 2020 2020 7661  elf: M,.      va
-0000c600: 7269 6162 6c65 733a 2056 6172 6961 626c  riables: Variabl
-0000c610: 6544 6963 742c 0a20 2020 2020 202a 6172  eDict,.      *ar
-0000c620: 6773 2c0a 2020 2020 2020 726e 6773 3a20  gs,.      rngs: 
-0000c630: 4f70 7469 6f6e 616c 5b52 4e47 5365 7175  Optional[RNGSequ
-0000c640: 656e 6365 735d 203d 204e 6f6e 652c 0a20  ences] = None,. 
-0000c650: 2020 2020 206d 7574 6162 6c65 3a20 436f       mutable: Co
-0000c660: 6c6c 6563 7469 6f6e 4669 6c74 6572 203d  llectionFilter =
-0000c670: 2046 616c 7365 2c0a 2020 2920 2d3e 204d   False,.  ) -> M
-0000c680: 3a0a 2020 2020 2222 2243 7265 6174 6573  :.    """Creates
-0000c690: 2061 6e20 696e 7465 7261 6374 6976 6520   an interactive 
-0000c6a0: 4d6f 6475 6c65 2069 6e73 7461 6e63 6520  Module instance 
-0000c6b0: 6279 2062 696e 6469 6e67 2076 6172 6961  by binding varia
-0000c6c0: 626c 6573 2061 6e64 2052 4e47 732e 0a0a  bles and RNGs...
-0000c6d0: 2020 2020 6060 6269 6e64 6060 2070 726f      ``bind`` pro
-0000c6e0: 7669 6465 7320 616e 2022 696e 7465 7261  vides an "intera
-0000c6f0: 6374 6976 6522 2069 6e73 7461 6e63 6520  ctive" instance 
-0000c700: 6f66 2061 204d 6f64 756c 6520 6469 7265  of a Module dire
-0000c710: 6374 6c79 2077 6974 686f 7574 0a20 2020  ctly without.   
-0000c720: 2074 7261 6e73 666f 726d 696e 6720 6120   transforming a 
-0000c730: 6675 6e63 7469 6f6e 2077 6974 6820 6060  function with ``
-0000c740: 6170 706c 7960 602e 2054 6869 7320 6973  apply``. This is
-0000c750: 2070 6172 7469 6375 6c61 726c 7920 7573   particularly us
-0000c760: 6566 756c 2066 6f72 0a20 2020 2064 6562  eful for.    deb
-0000c770: 7567 6769 6e67 2061 6e64 2069 6e74 6572  ugging and inter
-0000c780: 6163 7469 7665 2075 7365 2063 6173 6573  active use cases
-0000c790: 206c 696b 6520 6e6f 7465 626f 6f6b 7320   like notebooks 
-0000c7a0: 7768 6572 6520 6120 6675 6e63 7469 6f6e  where a function
-0000c7b0: 2077 6f75 6c64 0a20 2020 206c 696d 6974   would.    limit
-0000c7c0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
-0000c7d0: 7370 6c69 7420 7570 2063 6f64 6520 696e  split up code in
-0000c7e0: 746f 2064 6966 6665 7265 6e74 2063 656c  to different cel
-0000c7f0: 6c73 2e0a 0a20 2020 204f 6e63 6520 7468  ls...    Once th
-0000c800: 6520 7661 7269 6162 6c65 7320 2861 6e64  e variables (and
-0000c810: 206f 7074 696f 6e61 6c6c 7920 524e 4773   optionally RNGs
-0000c820: 2920 6172 6520 626f 756e 6420 746f 2061  ) are bound to a
-0000c830: 2060 604d 6f64 756c 6560 6020 6974 0a20   ``Module`` it. 
-0000c840: 2020 2062 6563 6f6d 6573 2061 2073 7461     becomes a sta
-0000c850: 7465 6675 6c20 6f62 6a65 6374 2e20 4e6f  teful object. No
-0000c860: 7465 2074 6861 7420 6964 696f 6d61 7469  te that idiomati
-0000c870: 6320 4a41 5820 6973 2066 756e 6374 696f  c JAX is functio
-0000c880: 6e61 6c20 616e 640a 2020 2020 7468 6572  nal and.    ther
-0000c890: 6566 6f72 6520 616e 2069 6e74 6572 6163  efore an interac
-0000c8a0: 7469 7665 2069 6e73 7461 6e63 6520 646f  tive instance do
-0000c8b0: 6573 206e 6f74 206d 6978 2077 656c 6c20  es not mix well 
-0000c8c0: 7769 7468 2076 616e 696c 6c61 204a 4158  with vanilla JAX
-0000c8d0: 2041 5049 732e 0a20 2020 2060 6062 696e   APIs..    ``bin
-0000c8e0: 6428 2960 6020 7368 6f75 6c64 206f 6e6c  d()`` should onl
-0000c8f0: 7920 6265 2075 7365 6420 666f 7220 696e  y be used for in
-0000c900: 7465 7261 6374 6976 6520 6578 7065 7269  teractive experi
-0000c910: 6d65 6e74 6174 696f 6e2c 2061 6e64 2069  mentation, and i
-0000c920: 6e20 616c 6c0a 2020 2020 6f74 6865 7220  n all.    other 
-0000c930: 6361 7365 7320 7765 2073 7472 6f6e 676c  cases we strongl
-0000c940: 7920 656e 636f 7572 6167 6520 7573 6572  y encourage user
-0000c950: 7320 746f 2075 7365 2060 6061 7070 6c79  s to use ``apply
-0000c960: 2829 6060 2069 6e73 7465 6164 2e0a 0a20  ()`` instead... 
-0000c970: 2020 2045 7861 6d70 6c65 3a3a 0a0a 2020     Example::..  
-0000c980: 2020 2020 696d 706f 7274 206a 6178 0a20      import jax. 
-0000c990: 2020 2020 2069 6d70 6f72 7420 6a61 782e       import jax.
-0000c9a0: 6e75 6d70 7920 6173 206a 6e70 0a20 2020  numpy as jnp.   
-0000c9b0: 2020 2069 6d70 6f72 7420 666c 6178 2e6c     import flax.l
-0000c9c0: 696e 656e 2061 7320 6e6e 0a0a 2020 2020  inen as nn..    
-0000c9d0: 2020 636c 6173 7320 4175 746f 456e 636f    class AutoEnco
-0000c9e0: 6465 7228 6e6e 2e4d 6f64 756c 6529 3a0a  der(nn.Module):.
-0000c9f0: 2020 2020 2020 2020 6465 6620 7365 7475          def setu
-0000ca00: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0000ca10: 2020 2073 656c 662e 656e 636f 6465 7220     self.encoder 
-0000ca20: 3d20 6e6e 2e44 656e 7365 2833 290a 2020  = nn.Dense(3).  
-0000ca30: 2020 2020 2020 2020 7365 6c66 2e64 6563          self.dec
-0000ca40: 6f64 6572 203d 206e 6e2e 4465 6e73 6528  oder = nn.Dense(
-0000ca50: 3529 0a0a 2020 2020 2020 2020 6465 6620  5)..        def 
-0000ca60: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2078  __call__(self, x
-0000ca70: 293a 0a20 2020 2020 2020 2020 2072 6574  ):.          ret
-0000ca80: 7572 6e20 7365 6c66 2e64 6563 6f64 6572  urn self.decoder
-0000ca90: 2873 656c 662e 656e 636f 6465 7228 7829  (self.encoder(x)
-0000caa0: 290a 0a20 2020 2020 2078 203d 206a 6e70  )..      x = jnp
-0000cab0: 2e6f 6e65 7328 2831 362c 2039 2929 0a20  .ones((16, 9)). 
-0000cac0: 2020 2020 2061 6520 3d20 4175 746f 456e       ae = AutoEn
-0000cad0: 636f 6465 7228 290a 2020 2020 2020 7661  coder().      va
-0000cae0: 7269 6162 6c65 7320 3d20 6165 2e69 6e69  riables = ae.ini
-0000caf0: 7428 6a61 782e 7261 6e64 6f6d 2e50 524e  t(jax.random.PRN
-0000cb00: 474b 6579 2830 292c 2078 290a 2020 2020  GKey(0), x).    
-0000cb10: 2020 6d6f 6465 6c20 3d20 6165 2e62 696e    model = ae.bin
-0000cb20: 6428 7661 7269 6162 6c65 7329 0a20 2020  d(variables).   
-0000cb30: 2020 207a 203d 206d 6f64 656c 2e65 6e63     z = model.enc
-0000cb40: 6f64 6572 2878 290a 2020 2020 2020 785f  oder(x).      x_
-0000cb50: 7265 636f 6e73 7472 7563 7465 6420 3d20  reconstructed = 
-0000cb60: 6d6f 6465 6c2e 6465 636f 6465 7228 7a29  model.decoder(z)
-0000cb70: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-0000cb80: 2020 7661 7269 6162 6c65 733a 2041 2064    variables: A d
-0000cb90: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-0000cba0: 6e69 6e67 2076 6172 6961 626c 6573 206b  ning variables k
-0000cbb0: 6579 6564 2062 7920 7661 7269 6162 6c65  eyed by variable
-0000cbc0: 0a20 2020 2020 2020 2063 6f6c 6c65 6374  .        collect
-0000cbd0: 696f 6e73 2e20 5365 6520 3a6d 6f64 3a60  ions. See :mod:`
-0000cbe0: 666c 6178 2e63 6f72 652e 7661 7269 6162  flax.core.variab
-0000cbf0: 6c65 7360 2066 6f72 206d 6f72 6520 6465  les` for more de
-0000cc00: 7461 696c 730a 2020 2020 2020 2020 6162  tails.        ab
-0000cc10: 6f75 7420 7661 7269 6162 6c65 732e 0a20  out variables.. 
-0000cc20: 2020 2020 202a 6172 6773 3a20 4e61 6d65       *args: Name
-0000cc30: 6420 6172 6775 6d65 6e74 7320 286e 6f74  d arguments (not
-0000cc40: 2075 7365 6429 2e0a 2020 2020 2020 726e   used)..      rn
-0000cc50: 6773 3a20 6120 6469 6374 206f 6620 5052  gs: a dict of PR
-0000cc60: 4e47 4b65 7973 2074 6f20 696e 6974 6961  NGKeys to initia
-0000cc70: 6c69 7a65 2074 6865 2050 524e 4720 7365  lize the PRNG se
-0000cc80: 7175 656e 6365 732e 0a20 2020 2020 206d  quences..      m
-0000cc90: 7574 6162 6c65 3a20 4361 6e20 6265 2062  utable: Can be b
-0000cca0: 6f6f 6c2c 2073 7472 2c20 6f72 206c 6973  ool, str, or lis
-0000ccb0: 742e 2053 7065 6369 6669 6573 2077 6869  t. Specifies whi
-0000ccc0: 6368 2063 6f6c 6c65 6374 696f 6e73 2073  ch collections s
-0000ccd0: 686f 756c 6420 6265 0a20 2020 2020 2020  hould be.       
-0000cce0: 2074 7265 6174 6564 2061 7320 6d75 7461   treated as muta
-0000ccf0: 626c 653a 0a20 2020 2020 2020 2020 2060  ble:.          `
-0000cd00: 6062 6f6f 6c60 603a 2061 6c6c 2f6e 6f20  `bool``: all/no 
-0000cd10: 636f 6c6c 6563 7469 6f6e 7320 6172 6520  collections are 
-0000cd20: 6d75 7461 626c 652e 0a20 2020 2020 2020  mutable..       
-0000cd30: 2020 2060 6073 7472 6060 3a20 5468 6520     ``str``: The 
-0000cd40: 6e61 6d65 206f 6620 6120 7369 6e67 6c65  name of a single
-0000cd50: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
-0000cd60: 696f 6e2e 0a20 2020 2020 2020 2020 2060  ion..          `
-0000cd70: 606c 6973 7460 603a 2041 206c 6973 7420  `list``: A list 
-0000cd80: 6f66 206e 616d 6573 206f 6620 6d75 7461  of names of muta
-0000cd90: 626c 6520 636f 6c6c 6563 7469 6f6e 732e  ble collections.
-0000cda0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000cdb0: 2020 2020 2041 2063 6f70 7920 6f66 2074       A copy of t
-0000cdc0: 6869 7320 696e 7374 616e 6365 2077 6974  his instance wit
-0000cdd0: 6820 626f 756e 6420 7661 7269 6162 6c65  h bound variable
-0000cde0: 7320 616e 6420 524e 4773 2e0a 2020 2020  s and RNGs..    
-0000cdf0: 2222 220a 2020 2020 4d6f 6475 6c65 2e5f  """.    Module._
-0000ce00: 6d6f 6475 6c65 5f63 6865 636b 7328 7365  module_checks(se
-0000ce10: 6c66 290a 0a20 2020 2064 656c 2061 7267  lf)..    del arg
-0000ce20: 730a 2020 2020 7363 6f70 6520 3d20 636f  s.    scope = co
-0000ce30: 7265 2e62 696e 6428 7661 7269 6162 6c65  re.bind(variable
-0000ce40: 732c 2072 6e67 733d 726e 6773 2c20 6d75  s, rngs=rngs, mu
-0000ce50: 7461 626c 653d 6d75 7461 626c 6529 0a20  table=mutable). 
-0000ce60: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
-0000ce70: 6c6f 6e65 2870 6172 656e 743d 7363 6f70  lone(parent=scop
-0000ce80: 652c 205f 6465 6570 5f63 6c6f 6e65 3d54  e, _deep_clone=T
-0000ce90: 7275 6529 0a0a 2020 6465 6620 756e 6269  rue)..  def unbi
-0000cea0: 6e64 2873 656c 663a 204d 2920 2d3e 2054  nd(self: M) -> T
-0000ceb0: 7570 6c65 5b4d 2c20 5661 7269 6162 6c65  uple[M, Variable
-0000cec0: 4469 6374 5d3a 0a20 2020 2022 2222 5265  Dict]:.    """Re
-0000ced0: 7475 726e 7320 616e 2075 6e62 6f75 6e64  turns an unbound
-0000cee0: 2063 6f70 7920 6f66 2061 204d 6f64 756c   copy of a Modul
-0000cef0: 6520 616e 6420 6974 7320 7661 7269 6162  e and its variab
-0000cf00: 6c65 732e 0a0a 2020 2020 6060 756e 6269  les...    ``unbi
-0000cf10: 6e64 6060 2068 656c 7073 2063 7265 6174  nd`` helps creat
-0000cf20: 6520 6120 7374 6174 656c 6573 7320 7665  e a stateless ve
-0000cf30: 7273 696f 6e20 6f66 2061 2062 6f75 6e64  rsion of a bound
-0000cf40: 204d 6f64 756c 652e 0a0a 2020 2020 416e   Module...    An
-0000cf50: 2065 7861 6d70 6c65 206f 6620 6120 636f   example of a co
-0000cf60: 6d6d 6f6e 2075 7365 2063 6173 653a 2074  mmon use case: t
-0000cf70: 6f20 6578 7472 6163 7420 6120 7375 622d  o extract a sub-
-0000cf80: 4d6f 6475 6c65 2064 6566 696e 6564 2069  Module defined i
-0000cf90: 6e73 6964 650a 2020 2020 6060 7365 7475  nside.    ``setu
-0000cfa0: 7028 2960 6020 616e 6420 6974 7320 636f  p()`` and its co
-0000cfb0: 7272 6573 706f 6e64 696e 6720 7661 7269  rresponding vari
-0000cfc0: 6162 6c65 733a 2031 2920 7465 6d70 6f72  ables: 1) tempor
-0000cfd0: 6172 696c 7920 6060 6269 6e64 6060 2074  arily ``bind`` t
-0000cfe0: 6865 2070 6172 656e 740a 2020 2020 4d6f  he parent.    Mo
-0000cff0: 6475 6c65 3b20 616e 6420 7468 656e 2032  dule; and then 2
-0000d000: 2920 6060 756e 6269 6e64 6060 2074 6865  ) ``unbind`` the
-0000d010: 2064 6573 6972 6564 2073 7562 2d4d 6f64   desired sub-Mod
-0000d020: 756c 652e 2028 5265 6361 6c6c 2074 6861  ule. (Recall tha
-0000d030: 7420 6060 7365 7475 7028 2960 600a 2020  t ``setup()``.  
-0000d040: 2020 6973 206f 6e6c 7920 6361 6c6c 6564    is only called
-0000d050: 2077 6865 6e20 7468 6520 4d6f 6475 6c65   when the Module
-0000d060: 2069 7320 626f 756e 642e 293a 3a0a 0a20   is bound.)::.. 
-0000d070: 2020 2020 2063 6c61 7373 2041 7574 6f45       class AutoE
-0000d080: 6e63 6f64 6572 286e 6e2e 4d6f 6475 6c65  ncoder(nn.Module
-0000d090: 293a 0a20 2020 2020 2020 2064 6566 2073  ):.        def s
-0000d0a0: 6574 7570 2873 656c 6629 3a0a 2020 2020  etup(self):.    
-0000d0b0: 2020 2020 2020 7365 6c66 2e65 6e63 6f64        self.encod
-0000d0c0: 6572 203d 2045 6e63 6f64 6572 2829 0a20  er = Encoder(). 
-0000d0d0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0000d0e0: 636f 6465 7220 3d20 4465 636f 6465 7228  coder = Decoder(
-0000d0f0: 290a 0a20 2020 2020 2020 2064 6566 205f  )..        def _
-0000d100: 5f63 616c 6c5f 5f28 7365 6c66 2c20 7829  _call__(self, x)
-0000d110: 3a0a 2020 2020 2020 2020 2020 7265 7475  :.          retu
-0000d120: 726e 2073 656c 662e 6465 636f 6465 7228  rn self.decoder(
-0000d130: 7365 6c66 2e65 6e63 6f64 6572 2878 2929  self.encoder(x))
-0000d140: 0a0a 2020 2020 2020 6d6f 6475 6c65 203d  ..      module =
-0000d150: 2041 7574 6f45 6e63 6f64 6572 2829 0a20   AutoEncoder(). 
-0000d160: 2020 2020 2076 6172 6961 626c 6573 203d       variables =
-0000d170: 206d 6f64 756c 652e 696e 6974 286a 6178   module.init(jax
-0000d180: 2e72 616e 646f 6d2e 5052 4e47 4b65 7928  .random.PRNGKey(
-0000d190: 3029 2c20 6a6e 702e 6f6e 6573 2828 312c  0), jnp.ones((1,
-0000d1a0: 2037 3834 2929 290a 2020 2020 2020 2e2e   784))).      ..
-0000d1b0: 2e0a 2020 2020 2020 2320 4578 7472 6163  ..      # Extrac
-0000d1c0: 7420 7468 6520 456e 636f 6465 7220 7375  t the Encoder su
-0000d1d0: 622d 4d6f 6475 6c65 2061 6e64 2069 7473  b-Module and its
-0000d1e0: 2076 6172 6961 626c 6573 0a20 2020 2020   variables.     
-0000d1f0: 2065 6e63 6f64 6572 2c20 656e 636f 6465   encoder, encode
-0000d200: 725f 7661 7273 203d 206d 6f64 756c 652e  r_vars = module.
-0000d210: 6269 6e64 2876 6172 6961 626c 6573 292e  bind(variables).
-0000d220: 656e 636f 6465 722e 756e 6269 6e64 2829  encoder.unbind()
-0000d230: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000d240: 2020 2020 2041 2074 7570 6c65 2077 6974       A tuple wit
-0000d250: 6820 616e 2075 6e62 6f75 6e64 2063 6f70  h an unbound cop
-0000d260: 7920 6f66 2074 6869 7320 4d6f 6475 6c65  y of this Module
-0000d270: 2061 6e64 2069 7473 2076 6172 6961 626c   and its variabl
-0000d280: 6573 2e0a 2020 2020 2222 220a 2020 2020  es..    """.    
-0000d290: 4d6f 6475 6c65 2e5f 6d6f 6475 6c65 5f63  Module._module_c
-0000d2a0: 6865 636b 7328 7365 6c66 290a 0a20 2020  hecks(self)..   
-0000d2b0: 2069 6620 7365 6c66 2e73 636f 7065 2069   if self.scope i
-0000d2c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 7261  s None:.      ra
-0000d2d0: 6973 6520 6572 726f 7273 2e43 616c 6c55  ise errors.CallU
-0000d2e0: 6e62 696e 644f 6e55 6e62 6f75 6e64 4d6f  nbindOnUnboundMo
-0000d2f0: 6475 6c65 4572 726f 7228 290a 0a20 2020  duleError()..   
-0000d300: 2076 6172 6961 626c 6573 203d 2073 656c   variables = sel
-0000d310: 662e 7661 7269 6162 6c65 730a 2020 2020  f.variables.    
-0000d320: 6d6f 6475 6c65 203d 2073 656c 662e 636c  module = self.cl
-0000d330: 6f6e 6528 290a 2020 2020 7265 7475 726e  one().    return
-0000d340: 206d 6f64 756c 652c 2076 6172 6961 626c   module, variabl
-0000d350: 6573 0a0a 2020 4074 7261 6365 6261 636b  es..  @traceback
-0000d360: 5f75 7469 6c2e 6170 695f 626f 756e 6461  _util.api_bounda
-0000d370: 7279 0a20 2064 6566 2061 7070 6c79 280a  ry.  def apply(.
-0000d380: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000d390: 2020 7661 7269 6162 6c65 733a 2056 6172    variables: Var
-0000d3a0: 6961 626c 6544 6963 742c 0a20 2020 2020  iableDict,.     
-0000d3b0: 202a 6172 6773 2c0a 2020 2020 2020 726e   *args,.      rn
-0000d3c0: 6773 3a20 4f70 7469 6f6e 616c 5b52 4e47  gs: Optional[RNG
-0000d3d0: 5365 7175 656e 6365 735d 203d 204e 6f6e  Sequences] = Non
-0000d3e0: 652c 0a20 2020 2020 206d 6574 686f 643a  e,.      method:
-0000d3f0: 2055 6e69 6f6e 5b43 616c 6c61 626c 655b   Union[Callable[
-0000d400: 2e2e 2e2c 2041 6e79 5d2c 2073 7472 2c20  ..., Any], str, 
-0000d410: 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0a 2020  None] = None,.  
-0000d420: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
-0000d430: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
-0000d440: 4661 6c73 652c 0a20 2020 2020 2063 6170  False,.      cap
-0000d450: 7475 7265 5f69 6e74 6572 6d65 6469 6174  ture_intermediat
-0000d460: 6573 3a20 556e 696f 6e5b 0a20 2020 2020  es: Union[.     
-0000d470: 2020 2020 2062 6f6f 6c2c 2043 616c 6c61       bool, Calla
-0000d480: 626c 655b 5b27 4d6f 6475 6c65 272c 2073  ble[['Module', s
-0000d490: 7472 5d2c 2062 6f6f 6c5d 0a20 2020 2020  tr], bool].     
-0000d4a0: 205d 203d 2046 616c 7365 2c0a 2020 2020   ] = False,.    
-0000d4b0: 2020 2a2a 6b77 6172 6773 2c0a 2020 2920    **kwargs,.  ) 
-0000d4c0: 2d3e 2055 6e69 6f6e 5b41 6e79 2c20 5475  -> Union[Any, Tu
-0000d4d0: 706c 655b 416e 792c 2055 6e69 6f6e 5b46  ple[Any, Union[F
-0000d4e0: 726f 7a65 6e56 6172 6961 626c 6544 6963  rozenVariableDic
-0000d4f0: 742c 2044 6963 745b 7374 722c 2041 6e79  t, Dict[str, Any
-0000d500: 5d5d 5d5d 3a0a 2020 2020 2222 2241 7070  ]]]]:.    """App
-0000d510: 6c69 6573 2061 206d 6f64 756c 6520 6d65  lies a module me
-0000d520: 7468 6f64 2074 6f20 7661 7269 6162 6c65  thod to variable
-0000d530: 7320 616e 6420 7265 7475 726e 7320 6f75  s and returns ou
-0000d540: 7470 7574 2061 6e64 206d 6f64 6966 6965  tput and modifie
-0000d550: 6420 7661 7269 6162 6c65 732e 0a0a 2020  d variables...  
-0000d560: 2020 4e6f 7465 2074 6861 7420 606d 6574    Note that `met
-0000d570: 686f 6460 2073 686f 756c 6420 6265 2073  hod` should be s
-0000d580: 6574 2069 6620 6f6e 6520 776f 756c 6420  et if one would 
-0000d590: 6c69 6b65 2074 6f20 6361 6c6c 2060 6170  like to call `ap
-0000d5a0: 706c 7960 206f 6e20 610a 2020 2020 6469  ply` on a.    di
-0000d5b0: 6666 6572 656e 7420 636c 6173 7320 6d65  fferent class me
-0000d5c0: 7468 6f64 2074 6861 6e20 6060 5f5f 6361  thod than ``__ca
-0000d5d0: 6c6c 5f5f 6060 2e20 466f 7220 696e 7374  ll__``. For inst
-0000d5e0: 616e 6365 2c20 7375 7070 6f73 6520 610a  ance, suppose a.
-0000d5f0: 2020 2020 5472 616e 7366 6f72 6d65 7220      Transformer 
-0000d600: 6d6f 6475 6c65 7320 6861 7320 6120 6d65  modules has a me
-0000d610: 7468 6f64 2063 616c 6c65 6420 6065 6e63  thod called `enc
-0000d620: 6f64 6560 2c20 7468 656e 2074 6865 2066  ode`, then the f
-0000d630: 6f6c 6c6f 7769 6e67 2063 616c 6c73 0a20  ollowing calls. 
-0000d640: 2020 2060 6170 706c 7960 206f 6e20 7468     `apply` on th
-0000d650: 6174 206d 6574 686f 643a 3a0a 0a20 2020  at method::..   
-0000d660: 2020 206d 6f64 656c 203d 2054 7261 6e73     model = Trans
-0000d670: 666f 726d 6572 2829 0a20 2020 2020 2065  former().      e
-0000d680: 6e63 6f64 6564 203d 206d 6f64 656c 2e61  ncoded = model.a
-0000d690: 7070 6c79 287b 2770 6172 616d 7327 3a20  pply({'params': 
-0000d6a0: 7061 7261 6d73 7d2c 2078 2c20 6d65 7468  params}, x, meth
-0000d6b0: 6f64 3d54 7261 6e73 666f 726d 6572 2e65  od=Transformer.e
-0000d6c0: 6e63 6f64 6529 0a0a 2020 2020 4966 2061  ncode)..    If a
-0000d6d0: 2066 756e 6374 696f 6e20 696e 7374 616e   function instan
-0000d6e0: 6365 2069 7320 7072 6f76 6964 6564 2c20  ce is provided, 
-0000d6f0: 7468 6520 756e 626f 756e 6420 6675 6e63  the unbound func
-0000d700: 7469 6f6e 2069 7320 7573 6564 2e20 466f  tion is used. Fo
-0000d710: 720a 2020 2020 696e 7374 616e 6365 2c20  r.    instance, 
-0000d720: 7468 6520 6578 616d 706c 6520 6265 6c6f  the example belo
-0000d730: 7720 6973 2065 7175 6976 616c 656e 7420  w is equivalent 
-0000d740: 746f 2074 6865 206f 6e65 2061 626f 7665  to the one above
-0000d750: 3a3a 0a0a 2020 2020 2020 656e 636f 6465  ::..      encode
-0000d760: 6420 3d20 6d6f 6465 6c2e 6170 706c 7928  d = model.apply(
-0000d770: 7b27 7061 7261 6d73 273a 2070 6172 616d  {'params': param
-0000d780: 737d 2c20 782c 206d 6574 686f 643d 6d6f  s}, x, method=mo
-0000d790: 6465 6c2e 656e 636f 6465 290a 0a20 2020  del.encode)..   
-0000d7a0: 2059 6f75 2063 616e 2061 6c73 6f20 7061   You can also pa
-0000d7b0: 7373 2061 2073 7472 696e 6720 746f 2061  ss a string to a
-0000d7c0: 2063 616c 6c61 626c 6520 6174 7472 6962   callable attrib
-0000d7d0: 7574 6520 6f66 2074 6865 206d 6f64 756c  ute of the modul
-0000d7e0: 652e 2046 6f72 0a20 2020 2065 7861 6d70  e. For.    examp
-0000d7f0: 6c65 2c20 7468 6520 7072 6576 696f 7573  le, the previous
-0000d800: 2063 616e 2062 6520 7772 6974 7465 6e20   can be written 
-0000d810: 6173 3a3a 0a0a 2020 2020 2020 656e 636f  as::..      enco
-0000d820: 6465 6420 3d20 6d6f 6465 6c2e 6170 706c  ded = model.appl
-0000d830: 7928 7b27 7061 7261 6d73 273a 2070 6172  y({'params': par
-0000d840: 616d 737d 2c20 782c 206d 6574 686f 643d  ams}, x, method=
-0000d850: 2765 6e63 6f64 6527 290a 0a20 2020 204e  'encode')..    N
-0000d860: 6f74 6520 6060 6d65 7468 6f64 6060 2063  ote ``method`` c
-0000d870: 616e 2061 6c73 6f20 6265 2061 2066 756e  an also be a fun
-0000d880: 6374 696f 6e20 7468 6174 2069 7320 6e6f  ction that is no
-0000d890: 7420 6465 6669 6e65 6420 696e 0a20 2020  t defined in.   
-0000d8a0: 2060 6054 7261 6e73 666f 726d 6572 6060   ``Transformer``
-0000d8b0: 2e20 496e 2074 6861 7420 6361 7365 2c20  . In that case, 
-0000d8c0: 7468 6520 6675 6e63 7469 6f6e 2073 686f  the function sho
-0000d8d0: 756c 6420 6861 7665 2061 7420 6c65 6173  uld have at leas
-0000d8e0: 7420 6f6e 650a 2020 2020 6172 6775 6d65  t one.    argume
-0000d8f0: 6e74 2072 6570 7265 7365 6e74 696e 6720  nt representing 
-0000d900: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
-0000d910: 6865 204d 6f64 756c 6520 636c 6173 733a  he Module class:
-0000d920: 3a0a 0a20 2020 2020 2064 6566 206f 7468  :..      def oth
-0000d930: 6572 5f66 6e28 696e 7374 616e 6365 2c20  er_fn(instance, 
-0000d940: 2e2e 2e29 3a0a 2020 2020 2020 2020 696e  ...):.        in
-0000d950: 7374 616e 6365 2e73 6f6d 655f 6d6f 6475  stance.some_modu
-0000d960: 6c65 5f61 7474 7228 2e2e 2e29 0a20 2020  le_attr(...).   
-0000d970: 2020 2020 202e 2e2e 0a0a 2020 2020 2020       .....      
-0000d980: 6d6f 6465 6c2e 6170 706c 7928 7b27 7061  model.apply({'pa
-0000d990: 7261 6d73 273a 2070 6172 616d 737d 2c20  rams': params}, 
-0000d9a0: 782c 206d 6574 686f 643d 6f74 6865 725f  x, method=other_
-0000d9b0: 666e 290a 0a20 2020 2041 7267 733a 0a20  fn)..    Args:. 
-0000d9c0: 2020 2020 2076 6172 6961 626c 6573 3a20       variables: 
-0000d9d0: 4120 6469 6374 696f 6e61 7279 2063 6f6e  A dictionary con
-0000d9e0: 7461 696e 696e 6720 7661 7269 6162 6c65  taining variable
-0000d9f0: 7320 6b65 7965 6420 6279 2076 6172 6961  s keyed by varia
-0000da00: 626c 650a 2020 2020 2020 2020 636f 6c6c  ble.        coll
-0000da10: 6563 7469 6f6e 732e 2053 6565 203a 6d6f  ections. See :mo
-0000da20: 643a 6066 6c61 782e 636f 7265 2e76 6172  d:`flax.core.var
-0000da30: 6961 626c 6573 6020 666f 7220 6d6f 7265  iables` for more
-0000da40: 2064 6574 6169 6c73 0a20 2020 2020 2020   details.       
-0000da50: 2061 626f 7574 2076 6172 6961 626c 6573   about variables
-0000da60: 2e0a 2020 2020 2020 2a61 7267 733a 204e  ..      *args: N
-0000da70: 616d 6564 2061 7267 756d 656e 7473 2070  amed arguments p
-0000da80: 6173 7365 6420 746f 2074 6865 2073 7065  assed to the spe
-0000da90: 6369 6669 6564 2061 7070 6c79 206d 6574  cified apply met
-0000daa0: 686f 642e 0a20 2020 2020 2072 6e67 733a  hod..      rngs:
-0000dab0: 2061 2064 6963 7420 6f66 2050 524e 474b   a dict of PRNGK
-0000dac0: 6579 7320 746f 2069 6e69 7469 616c 697a  eys to initializ
-0000dad0: 6520 7468 6520 5052 4e47 2073 6571 7565  e the PRNG seque
-0000dae0: 6e63 6573 2e0a 2020 2020 2020 2020 5468  nces..        Th
-0000daf0: 6520 2270 6172 616d 7322 2050 524e 4720  e "params" PRNG 
-0000db00: 7365 7175 656e 6365 2069 7320 7573 6564  sequence is used
-0000db10: 2074 6f20 696e 6974 6961 6c69 7a65 2070   to initialize p
-0000db20: 6172 616d 6574 6572 732e 0a20 2020 2020  arameters..     
-0000db30: 206d 6574 686f 643a 2041 2066 756e 6374   method: A funct
-0000db40: 696f 6e20 746f 2063 616c 6c20 6170 706c  ion to call appl
-0000db50: 7920 6f6e 2e20 5468 6973 2069 7320 6765  y on. This is ge
-0000db60: 6e65 7261 6c6c 7920 6120 6675 6e63 7469  nerally a functi
-0000db70: 6f6e 2069 6e20 7468 650a 2020 2020 2020  on in the.      
-0000db80: 2020 6d6f 6475 6c65 2e20 4966 2070 726f    module. If pro
-0000db90: 7669 6465 642c 2061 7070 6c69 6573 2074  vided, applies t
-0000dba0: 6869 7320 6d65 7468 6f64 2e20 4966 206e  his method. If n
-0000dbb0: 6f74 2070 726f 7669 6465 642c 2061 7070  ot provided, app
-0000dbc0: 6c69 6573 2074 6865 0a20 2020 2020 2020  lies the.       
-0000dbd0: 2060 605f 5f63 616c 6c5f 5f60 6020 6d65   ``__call__`` me
-0000dbe0: 7468 6f64 206f 6620 7468 6520 6d6f 6475  thod of the modu
-0000dbf0: 6c65 2e20 4120 7374 7269 6e67 2063 616e  le. A string can
-0000dc00: 2061 6c73 6f20 6265 2070 726f 7669 6465   also be provide
-0000dc10: 6420 746f 0a20 2020 2020 2020 2073 7065  d to.        spe
-0000dc20: 6369 6679 2061 206d 6574 686f 6420 6279  cify a method by
-0000dc30: 206e 616d 652e 0a20 2020 2020 206d 7574   name..      mut
-0000dc40: 6162 6c65 3a20 4361 6e20 6265 2062 6f6f  able: Can be boo
-0000dc50: 6c2c 2073 7472 2c20 6f72 206c 6973 742e  l, str, or list.
-0000dc60: 2053 7065 6369 6669 6573 2077 6869 6368   Specifies which
-0000dc70: 2063 6f6c 6c65 6374 696f 6e73 2073 686f   collections sho
-0000dc80: 756c 6420 6265 0a20 2020 2020 2020 2020  uld be.         
-0000dc90: 2020 2020 2020 7472 6561 7465 6420 6173        treated as
-0000dca0: 206d 7574 6162 6c65 3a20 6060 626f 6f6c   mutable: ``bool
-0000dcb0: 6060 3a20 616c 6c2f 6e6f 2063 6f6c 6c65  ``: all/no colle
-0000dcc0: 6374 696f 6e73 2061 7265 206d 7574 6162  ctions are mutab
-0000dcd0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
-0000dce0: 2020 2060 6073 7472 6060 3a20 5468 6520     ``str``: The 
-0000dcf0: 6e61 6d65 206f 6620 6120 7369 6e67 6c65  name of a single
-0000dd00: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
-0000dd10: 696f 6e2e 2060 606c 6973 7460 603a 2041  ion. ``list``: A
-0000dd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd30: 6c69 7374 206f 6620 6e61 6d65 7320 6f66  list of names of
-0000dd40: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
-0000dd50: 696f 6e73 2e0a 2020 2020 2020 6361 7074  ions..      capt
-0000dd60: 7572 655f 696e 7465 726d 6564 6961 7465  ure_intermediate
-0000dd70: 733a 2049 6620 6054 7275 6560 2c20 6361  s: If `True`, ca
-0000dd80: 7074 7572 6573 2069 6e74 6572 6d65 6469  ptures intermedi
-0000dd90: 6174 6520 7265 7475 726e 2076 616c 7565  ate return value
-0000dda0: 730a 2020 2020 2020 2020 6f66 2061 6c6c  s.        of all
-0000ddb0: 204d 6f64 756c 6573 2069 6e73 6964 6520   Modules inside 
-0000ddc0: 7468 6520 2269 6e74 6572 6d65 6469 6174  the "intermediat
-0000ddd0: 6573 2220 636f 6c6c 6563 7469 6f6e 2e20  es" collection. 
-0000dde0: 4279 2064 6566 6175 6c74 206f 6e6c 790a  By default only.
-0000ddf0: 2020 2020 2020 2020 7468 6520 7265 7475          the retu
-0000de00: 726e 2076 616c 7565 7320 6f66 2061 6c6c  rn values of all
-0000de10: 2060 605f 5f63 616c 6c5f 5f60 6020 6d65   ``__call__`` me
-0000de20: 7468 6f64 7320 6172 6520 7374 6f72 6564  thods are stored
-0000de30: 2e20 4120 6675 6e63 7469 6f6e 2063 616e  . A function can
-0000de40: 0a20 2020 2020 2020 2062 6520 7061 7373  .        be pass
-0000de50: 6564 2074 6f20 6368 616e 6765 2074 6865  ed to change the
-0000de60: 2066 696c 7465 7220 6265 6861 7669 6f72   filter behavior
-0000de70: 2e20 5468 6520 6669 6c74 6572 2066 756e  . The filter fun
-0000de80: 6374 696f 6e20 7461 6b65 730a 2020 2020  ction takes.    
-0000de90: 2020 2020 7468 6520 4d6f 6475 6c65 2069      the Module i
-0000dea0: 6e73 7461 6e63 6520 616e 6420 6d65 7468  nstance and meth
-0000deb0: 6f64 206e 616d 6520 616e 6420 7265 7475  od name and retu
-0000dec0: 726e 7320 6120 626f 6f6c 2069 6e64 6963  rns a bool indic
-0000ded0: 6174 696e 670a 2020 2020 2020 2020 7768  ating.        wh
-0000dee0: 6574 6865 7220 7468 6520 6f75 7470 7574  ether the output
-0000def0: 206f 6620 7468 6174 206d 6574 686f 6420   of that method 
-0000df00: 696e 766f 6361 7469 6f6e 2073 686f 756c  invocation shoul
-0000df10: 6420 6265 2073 746f 7265 642e 0a20 2020  d be stored..   
-0000df20: 2020 202a 2a6b 7761 7267 733a 204b 6579     **kwargs: Key
-0000df30: 776f 7264 2061 7267 756d 656e 7473 2070  word arguments p
-0000df40: 6173 7365 6420 746f 2074 6865 2073 7065  assed to the spe
-0000df50: 6369 6669 6564 2061 7070 6c79 206d 6574  cified apply met
-0000df60: 686f 642e 0a20 2020 2052 6574 7572 6e73  hod..    Returns
-0000df70: 3a0a 2020 2020 2020 4966 2060 606d 7574  :.      If ``mut
-0000df80: 6162 6c65 6060 2069 7320 4661 6c73 652c  able`` is False,
-0000df90: 2072 6574 7572 6e73 206f 7574 7075 742e   returns output.
-0000dfa0: 2049 6620 616e 7920 636f 6c6c 6563 7469   If any collecti
-0000dfb0: 6f6e 7320 6172 650a 2020 2020 2020 6d75  ons are.      mu
-0000dfc0: 7461 626c 652c 2072 6574 7572 6e73 2060  table, returns `
-0000dfd0: 6028 6f75 7470 7574 2c20 7661 7273 2960  `(output, vars)`
-0000dfe0: 602c 2077 6865 7265 2060 6076 6172 7360  `, where ``vars`
-0000dff0: 6020 6172 6520 6973 2061 2064 6963 740a  ` are is a dict.
-0000e000: 2020 2020 2020 6f66 2074 6865 206d 6f64        of the mod
-0000e010: 6966 6965 6420 636f 6c6c 6563 7469 6f6e  ified collection
-0000e020: 732e 0a20 2020 2022 2222 0a20 2020 204d  s..    """.    M
-0000e030: 6f64 756c 652e 5f6d 6f64 756c 655f 6368  odule._module_ch
-0000e040: 6563 6b73 2873 656c 6629 0a0a 2020 2020  ecks(self)..    
-0000e050: 6966 2069 7369 6e73 7461 6e63 6528 6d65  if isinstance(me
-0000e060: 7468 6f64 2c20 7374 7229 3a0a 2020 2020  thod, str):.    
-0000e070: 2020 6174 7472 6962 7574 655f 6e61 6d65    attribute_name
-0000e080: 203d 206d 6574 686f 640a 2020 2020 2020   = method.      
-0000e090: 6d65 7468 6f64 203d 2067 6574 6174 7472  method = getattr
-0000e0a0: 2873 656c 662c 2061 7474 7269 6275 7465  (self, attribute
-0000e0b0: 5f6e 616d 6529 0a20 2020 2020 2069 6620  _name).      if 
-0000e0c0: 6e6f 7420 6361 6c6c 6162 6c65 286d 6574  not callable(met
-0000e0d0: 686f 6429 3a0a 2020 2020 2020 2020 636c  hod):.        cl
-0000e0e0: 6173 735f 6e61 6d65 203d 2074 7970 6528  ass_name = type(
-0000e0f0: 7365 6c66 292e 5f5f 6e61 6d65 5f5f 0a20  self).__name__. 
-0000e100: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-0000e110: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-0000e120: 2020 2020 6622 277b 636c 6173 735f 6e61      f"'{class_na
-0000e130: 6d65 7d2e 7b61 7474 7269 6275 7465 5f6e  me}.{attribute_n
-0000e140: 616d 657d 2720 6d75 7374 2062 6520 6120  ame}' must be a 
-0000e150: 6361 6c6c 6162 6c65 2c20 676f 7422 0a20  callable, got". 
-0000e160: 2020 2020 2020 2020 2020 2066 2720 7b74             f' {t
-0000e170: 7970 6528 6d65 7468 6f64 297d 2e27 0a20  ype(method)}.'. 
-0000e180: 2020 2020 2020 2029 0a20 2020 2065 6c69         ).    eli
-0000e190: 6620 6d65 7468 6f64 2069 7320 4e6f 6e65  f method is None
-0000e1a0: 3a0a 2020 2020 2020 6d65 7468 6f64 203d  :.      method =
-0000e1b0: 2073 656c 662e 5f5f 6361 6c6c 5f5f 0a20   self.__call__. 
-0000e1c0: 2020 206d 6574 686f 6420 3d20 5f67 6574     method = _get
-0000e1d0: 5f75 6e62 6f75 6e64 5f66 6e28 6d65 7468  _unbound_fn(meth
-0000e1e0: 6f64 290a 2020 2020 7265 7475 726e 2061  od).    return a
-0000e1f0: 7070 6c79 280a 2020 2020 2020 2020 6d65  pply(.        me
-0000e200: 7468 6f64 2c0a 2020 2020 2020 2020 7365  thod,.        se
-0000e210: 6c66 2c0a 2020 2020 2020 2020 6d75 7461  lf,.        muta
-0000e220: 626c 653d 6d75 7461 626c 652c 0a20 2020  ble=mutable,.   
-0000e230: 2020 2020 2063 6170 7475 7265 5f69 6e74       capture_int
-0000e240: 6572 6d65 6469 6174 6573 3d63 6170 7475  ermediates=captu
-0000e250: 7265 5f69 6e74 6572 6d65 6469 6174 6573  re_intermediates
-0000e260: 2c0a 2020 2020 2928 7661 7269 6162 6c65  ,.    )(variable
-0000e270: 732c 202a 6172 6773 2c20 2a2a 6b77 6172  s, *args, **kwar
-0000e280: 6773 2c20 726e 6773 3d72 6e67 7329 0a0a  gs, rngs=rngs)..
-0000e290: 2020 4074 7261 6365 6261 636b 5f75 7469    @traceback_uti
-0000e2a0: 6c2e 6170 695f 626f 756e 6461 7279 0a20  l.api_boundary. 
-0000e2b0: 2064 6566 2069 6e69 745f 7769 7468 5f6f   def init_with_o
-0000e2c0: 7574 7075 7428 0a20 2020 2020 2073 656c  utput(.      sel
-0000e2d0: 662c 0a20 2020 2020 2072 6e67 733a 2055  f,.      rngs: U
-0000e2e0: 6e69 6f6e 5b4b 6579 4172 7261 792c 2052  nion[KeyArray, R
-0000e2f0: 4e47 5365 7175 656e 6365 735d 2c0a 2020  NGSequences],.  
-0000e300: 2020 2020 2a61 7267 732c 0a20 2020 2020      *args,.     
-0000e310: 206d 6574 686f 643a 2055 6e69 6f6e 5b43   method: Union[C
-0000e320: 616c 6c61 626c 655b 2e2e 2e2c 2041 6e79  allable[..., Any
-0000e330: 5d2c 2073 7472 2c20 4e6f 6e65 5d20 3d20  ], str, None] = 
-0000e340: 4e6f 6e65 2c0a 2020 2020 2020 6d75 7461  None,.      muta
-0000e350: 626c 653a 2043 6f6c 6c65 6374 696f 6e46  ble: CollectionF
-0000e360: 696c 7465 7220 3d20 4465 6e79 4c69 7374  ilter = DenyList
-0000e370: 2827 696e 7465 726d 6564 6961 7465 7327  ('intermediates'
-0000e380: 292c 0a20 2020 2020 2063 6170 7475 7265  ),.      capture
-0000e390: 5f69 6e74 6572 6d65 6469 6174 6573 3a20  _intermediates: 
-0000e3a0: 556e 696f 6e5b 0a20 2020 2020 2020 2020  Union[.         
-0000e3b0: 2062 6f6f 6c2c 2043 616c 6c61 626c 655b   bool, Callable[
-0000e3c0: 5b27 4d6f 6475 6c65 272c 2073 7472 5d2c  ['Module', str],
-0000e3d0: 2062 6f6f 6c5d 0a20 2020 2020 205d 203d   bool].      ] =
-0000e3e0: 2046 616c 7365 2c0a 2020 2020 2020 2a2a   False,.      **
-0000e3f0: 6b77 6172 6773 2c0a 2020 2920 2d3e 2054  kwargs,.  ) -> T
-0000e400: 7570 6c65 5b41 6e79 2c20 556e 696f 6e5b  uple[Any, Union[
-0000e410: 4672 6f7a 656e 5661 7269 6162 6c65 4469  FrozenVariableDi
-0000e420: 6374 2c20 4469 6374 5b73 7472 2c20 416e  ct, Dict[str, An
-0000e430: 795d 5d5d 3a0a 2020 2020 2222 2249 6e69  y]]]:.    """Ini
-0000e440: 7469 616c 697a 6573 2061 206d 6f64 756c  tializes a modul
-0000e450: 6520 6d65 7468 6f64 2077 6974 6820 7661  e method with va
-0000e460: 7269 6162 6c65 7320 616e 6420 7265 7475  riables and retu
-0000e470: 726e 7320 6f75 7470 7574 2061 6e64 206d  rns output and m
-0000e480: 6f64 6966 6965 6420 7661 7269 6162 6c65  odified variable
-0000e490: 732e 0a0a 2020 2020 4172 6773 3a0a 2020  s...    Args:.  
-0000e4a0: 2020 2020 726e 6773 3a20 5468 6520 726e      rngs: The rn
-0000e4b0: 6773 2066 6f72 2074 6865 2076 6172 6961  gs for the varia
-0000e4c0: 626c 6520 636f 6c6c 6563 7469 6f6e 732e  ble collections.
-0000e4d0: 0a20 2020 2020 202a 6172 6773 3a20 4e61  .      *args: Na
-0000e4e0: 6d65 6420 6172 6775 6d65 6e74 7320 7061  med arguments pa
-0000e4f0: 7373 6564 2074 6f20 7468 6520 696e 6974  ssed to the init
-0000e500: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
-0000e510: 206d 6574 686f 643a 2041 6e20 6f70 7469   method: An opti
-0000e520: 6f6e 616c 206d 6574 686f 642e 2049 6620  onal method. If 
-0000e530: 7072 6f76 6964 6564 2c20 6170 706c 6965  provided, applie
-0000e540: 7320 7468 6973 206d 6574 686f 642e 2049  s this method. I
-0000e550: 6620 6e6f 740a 2020 2020 2020 2020 7072  f not.        pr
-0000e560: 6f76 6964 6564 2c20 6170 706c 6965 7320  ovided, applies 
-0000e570: 7468 6520 6060 5f5f 6361 6c6c 5f5f 6060  the ``__call__``
-0000e580: 206d 6574 686f 642e 2041 2073 7472 696e   method. A strin
-0000e590: 6720 6361 6e20 616c 736f 2062 6527 0a20  g can also be'. 
-0000e5a0: 2020 2020 2020 2070 726f 7669 6465 6420         provided 
-0000e5b0: 746f 2073 7065 6369 6679 2061 206d 6574  to specify a met
-0000e5c0: 686f 6420 6279 206e 616d 652e 0a20 2020  hod by name..   
-0000e5d0: 2020 206d 7574 6162 6c65 3a20 4361 6e20     mutable: Can 
-0000e5e0: 6265 2062 6f6f 6c2c 2073 7472 2c20 6f72  be bool, str, or
-0000e5f0: 206c 6973 742e 2053 7065 6369 6669 6573   list. Specifies
-0000e600: 2077 6869 6368 2063 6f6c 6c65 6374 696f   which collectio
-0000e610: 6e73 2073 686f 756c 6420 6265 0a20 2020  ns should be.   
-0000e620: 2020 2020 2074 7265 6174 6564 2061 7320       treated as 
-0000e630: 6d75 7461 626c 653a 2060 6062 6f6f 6c60  mutable: ``bool`
-0000e640: 603a 2061 6c6c 2f6e 6f20 636f 6c6c 6563  `: all/no collec
-0000e650: 7469 6f6e 7320 6172 6520 6d75 7461 626c  tions are mutabl
-0000e660: 652e 0a20 2020 2020 2020 2060 6073 7472  e..        ``str
-0000e670: 6060 3a20 5468 6520 6e61 6d65 206f 6620  ``: The name of 
-0000e680: 6120 7369 6e67 6c65 206d 7574 6162 6c65  a single mutable
-0000e690: 2063 6f6c 6c65 6374 696f 6e2e 2060 606c   collection. ``l
-0000e6a0: 6973 7460 603a 2041 0a20 2020 2020 2020  ist``: A.       
-0000e6b0: 206c 6973 7420 6f66 206e 616d 6573 206f   list of names o
-0000e6c0: 6620 6d75 7461 626c 6520 636f 6c6c 6563  f mutable collec
-0000e6d0: 7469 6f6e 732e 2042 7920 6465 6661 756c  tions. By defaul
-0000e6e0: 7420 616c 6c20 636f 6c6c 6563 7469 6f6e  t all collection
-0000e6f0: 730a 2020 2020 2020 2020 6578 6365 7074  s.        except
-0000e700: 2022 696e 7465 726d 6564 6961 7465 7322   "intermediates"
-0000e710: 2061 7265 206d 7574 6162 6c65 2e0a 2020   are mutable..  
-0000e720: 2020 2020 6361 7074 7572 655f 696e 7465      capture_inte
-0000e730: 726d 6564 6961 7465 733a 2049 6620 6054  rmediates: If `T
-0000e740: 7275 6560 2c20 6361 7074 7572 6573 2069  rue`, captures i
-0000e750: 6e74 6572 6d65 6469 6174 6520 7265 7475  ntermediate retu
-0000e760: 726e 2076 616c 7565 730a 2020 2020 2020  rn values.      
-0000e770: 2020 6f66 2061 6c6c 204d 6f64 756c 6573    of all Modules
-0000e780: 2069 6e73 6964 6520 7468 6520 2269 6e74   inside the "int
-0000e790: 6572 6d65 6469 6174 6573 2220 636f 6c6c  ermediates" coll
-0000e7a0: 6563 7469 6f6e 2e20 4279 2064 6566 6175  ection. By defau
-0000e7b0: 6c74 206f 6e6c 790a 2020 2020 2020 2020  lt only.        
-0000e7c0: 7468 6520 7265 7475 726e 2076 616c 7565  the return value
-0000e7d0: 7320 6f66 2061 6c6c 2060 605f 5f63 616c  s of all ``__cal
-0000e7e0: 6c5f 5f60 6020 6d65 7468 6f64 7320 6172  l__`` methods ar
-0000e7f0: 6520 7374 6f72 6564 2e20 4120 6675 6e63  e stored. A func
-0000e800: 7469 6f6e 2063 616e 0a20 2020 2020 2020  tion can.       
-0000e810: 2062 6520 7061 7373 6564 2074 6f20 6368   be passed to ch
-0000e820: 616e 6765 2074 6865 2066 696c 7465 7220  ange the filter 
-0000e830: 6265 6861 7669 6f72 2e20 5468 6520 6669  behavior. The fi
-0000e840: 6c74 6572 2066 756e 6374 696f 6e20 7461  lter function ta
-0000e850: 6b65 730a 2020 2020 2020 2020 7468 6520  kes.        the 
-0000e860: 4d6f 6475 6c65 2069 6e73 7461 6e63 6520  Module instance 
-0000e870: 616e 6420 6d65 7468 6f64 206e 616d 6520  and method name 
-0000e880: 616e 6420 7265 7475 726e 7320 6120 626f  and returns a bo
-0000e890: 6f6c 2069 6e64 6963 6174 696e 670a 2020  ol indicating.  
-0000e8a0: 2020 2020 2020 7768 6574 6865 7220 7468        whether th
-0000e8b0: 6520 6f75 7470 7574 206f 6620 7468 6174  e output of that
-0000e8c0: 206d 6574 686f 6420 696e 766f 6361 7469   method invocati
-0000e8d0: 6f6e 2073 686f 756c 6420 6265 2073 746f  on should be sto
-0000e8e0: 7265 642e 0a20 2020 2020 202a 2a6b 7761  red..      **kwa
-0000e8f0: 7267 733a 204b 6579 776f 7264 2061 7267  rgs: Keyword arg
-0000e900: 756d 656e 7473 2070 6173 7365 6420 746f  uments passed to
-0000e910: 2074 6865 2069 6e69 7420 6675 6e63 7469   the init functi
-0000e920: 6f6e 2e0a 2020 2020 5265 7475 726e 733a  on..    Returns:
-0000e930: 0a20 2020 2020 2060 286f 7574 7075 742c  .      `(output,
-0000e940: 2076 6172 7329 6060 2c20 7768 6572 6520   vars)``, where 
-0000e950: 6060 7661 7273 6060 2061 7265 2069 7320  ``vars`` are is 
-0000e960: 6120 6469 6374 206f 6620 7468 6520 6d6f  a dict of the mo
-0000e970: 6469 6669 6564 0a20 2020 2020 2063 6f6c  dified.      col
-0000e980: 6c65 6374 696f 6e73 2e0a 2020 2020 2222  lections..    ""
-0000e990: 220a 2020 2020 4d6f 6475 6c65 2e5f 6d6f  ".    Module._mo
-0000e9a0: 6475 6c65 5f63 6865 636b 7328 7365 6c66  dule_checks(self
-0000e9b0: 290a 0a20 2020 2069 6620 6e6f 7420 6973  )..    if not is
-0000e9c0: 696e 7374 616e 6365 2872 6e67 732c 2064  instance(rngs, d
-0000e9d0: 6963 7429 3a0a 2020 2020 2020 6966 206e  ict):.      if n
-0000e9e0: 6f74 2063 6f72 652e 7363 6f70 652e 5f69  ot core.scope._i
-0000e9f0: 735f 7661 6c69 645f 726e 6728 726e 6773  s_valid_rng(rngs
-0000ea00: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-0000ea10: 2065 7272 6f72 732e 496e 7661 6c69 6452   errors.InvalidR
-0000ea20: 6e67 4572 726f 7228 0a20 2020 2020 2020  ngError(.       
-0000ea30: 2020 2020 2027 524e 4773 2073 686f 756c       'RNGs shoul
-0000ea40: 6420 6265 206f 6620 7368 6170 6520 2832  d be of shape (2
-0000ea50: 2c29 206f 7220 4b65 7941 7272 6179 2069  ,) or KeyArray i
-0000ea60: 6e20 4d6f 6475 6c65 2027 0a20 2020 2020  n Module '.     
-0000ea70: 2020 2020 2020 2066 277b 7365 6c66 2e5f         f'{self._
-0000ea80: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
-0000ea90: 5f7d 2c20 6275 7420 726e 6773 2061 7265  _}, but rngs are
-0000eaa0: 3a20 7b72 6e67 737d 270a 2020 2020 2020  : {rngs}'.      
-0000eab0: 2020 290a 2020 2020 2020 726e 6773 203d    ).      rngs =
-0000eac0: 207b 2770 6172 616d 7327 3a20 726e 6773   {'params': rngs
-0000ead0: 7d0a 0a20 2020 2069 6620 6973 696e 7374  }..    if isinst
-0000eae0: 616e 6365 286d 6574 686f 642c 2073 7472  ance(method, str
-0000eaf0: 293a 0a20 2020 2020 2061 7474 7269 6275  ):.      attribu
-0000eb00: 7465 5f6e 616d 6520 3d20 6d65 7468 6f64  te_name = method
-0000eb10: 0a20 2020 2020 206d 6574 686f 6420 3d20  .      method = 
-0000eb20: 6765 7461 7474 7228 7365 6c66 2c20 6174  getattr(self, at
-0000eb30: 7472 6962 7574 655f 6e61 6d65 290a 2020  tribute_name).  
-0000eb40: 2020 2020 6966 206e 6f74 2063 616c 6c61      if not calla
-0000eb50: 626c 6528 6d65 7468 6f64 293a 0a20 2020  ble(method):.   
-0000eb60: 2020 2020 2063 6c61 7373 5f6e 616d 6520       class_name 
-0000eb70: 3d20 7479 7065 2873 656c 6629 2e5f 5f6e  = type(self).__n
-0000eb80: 616d 655f 5f0a 2020 2020 2020 2020 7261  ame__.        ra
-0000eb90: 6973 6520 5479 7065 4572 726f 7228 0a20  ise TypeError(. 
-0000eba0: 2020 2020 2020 2020 2020 2066 2227 7b63             f"'{c
-0000ebb0: 6c61 7373 5f6e 616d 657d 2e7b 6174 7472  lass_name}.{attr
-0000ebc0: 6962 7574 655f 6e61 6d65 7d27 206d 7573  ibute_name}' mus
-0000ebd0: 7420 6265 2061 2063 616c 6c61 626c 652c  t be a callable,
-0000ebe0: 2067 6f74 220a 2020 2020 2020 2020 2020   got".          
-0000ebf0: 2020 6627 207b 7479 7065 286d 6574 686f    f' {type(metho
-0000ec00: 6429 7d2e 270a 2020 2020 2020 2020 290a  d)}.'.        ).
-0000ec10: 2020 2020 656c 6966 206d 6574 686f 6420      elif method 
-0000ec20: 6973 204e 6f6e 653a 0a20 2020 2020 206d  is None:.      m
-0000ec30: 6574 686f 6420 3d20 7365 6c66 2e5f 5f63  ethod = self.__c
-0000ec40: 616c 6c5f 5f0a 2020 2020 6d65 7468 6f64  all__.    method
-0000ec50: 203d 205f 6765 745f 756e 626f 756e 645f   = _get_unbound_
-0000ec60: 666e 286d 6574 686f 6429 0a20 2020 2072  fn(method).    r
-0000ec70: 6574 7572 6e20 696e 6974 5f77 6974 685f  eturn init_with_
-0000ec80: 6f75 7470 7574 280a 2020 2020 2020 2020  output(.        
-0000ec90: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
-0000eca0: 7365 6c66 2c0a 2020 2020 2020 2020 6d75  self,.        mu
-0000ecb0: 7461 626c 653d 6d75 7461 626c 652c 0a20  table=mutable,. 
-0000ecc0: 2020 2020 2020 2063 6170 7475 7265 5f69         capture_i
-0000ecd0: 6e74 6572 6d65 6469 6174 6573 3d63 6170  ntermediates=cap
-0000ece0: 7475 7265 5f69 6e74 6572 6d65 6469 6174  ture_intermediat
-0000ecf0: 6573 2c0a 2020 2020 2928 726e 6773 2c20  es,.    )(rngs, 
-0000ed00: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-0000ed10: 0a0a 2020 4074 7261 6365 6261 636b 5f75  ..  @traceback_u
-0000ed20: 7469 6c2e 6170 695f 626f 756e 6461 7279  til.api_boundary
-0000ed30: 0a20 2064 6566 2069 6e69 7428 0a20 2020  .  def init(.   
-0000ed40: 2020 2073 656c 662c 0a20 2020 2020 2072     self,.      r
-0000ed50: 6e67 733a 2055 6e69 6f6e 5b4b 6579 4172  ngs: Union[KeyAr
-0000ed60: 7261 792c 2052 4e47 5365 7175 656e 6365  ray, RNGSequence
-0000ed70: 735d 2c0a 2020 2020 2020 2a61 7267 732c  s],.      *args,
-0000ed80: 0a20 2020 2020 206d 6574 686f 643a 2055  .      method: U
-0000ed90: 6e69 6f6e 5b43 616c 6c61 626c 655b 2e2e  nion[Callable[..
-0000eda0: 2e2c 2041 6e79 5d2c 2073 7472 2c20 4e6f  ., Any], str, No
-0000edb0: 6e65 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ne] = None,.    
-0000edc0: 2020 6d75 7461 626c 653a 2043 6f6c 6c65    mutable: Colle
-0000edd0: 6374 696f 6e46 696c 7465 7220 3d20 4465  ctionFilter = De
-0000ede0: 6e79 4c69 7374 2827 696e 7465 726d 6564  nyList('intermed
-0000edf0: 6961 7465 7327 292c 0a20 2020 2020 2063  iates'),.      c
-0000ee00: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
-0000ee10: 6174 6573 3a20 556e 696f 6e5b 0a20 2020  ates: Union[.   
-0000ee20: 2020 2020 2020 2062 6f6f 6c2c 2043 616c         bool, Cal
-0000ee30: 6c61 626c 655b 5b27 4d6f 6475 6c65 272c  lable[['Module',
-0000ee40: 2073 7472 5d2c 2062 6f6f 6c5d 0a20 2020   str], bool].   
-0000ee50: 2020 205d 203d 2046 616c 7365 2c0a 2020     ] = False,.  
-0000ee60: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
-0000ee70: 2920 2d3e 2055 6e69 6f6e 5b46 726f 7a65  ) -> Union[Froze
-0000ee80: 6e56 6172 6961 626c 6544 6963 742c 2044  nVariableDict, D
-0000ee90: 6963 745b 7374 722c 2041 6e79 5d5d 3a0a  ict[str, Any]]:.
-0000eea0: 2020 2020 2222 2249 6e69 7469 616c 697a      """Initializ
-0000eeb0: 6573 2061 206d 6f64 756c 6520 6d65 7468  es a module meth
-0000eec0: 6f64 2077 6974 6820 7661 7269 6162 6c65  od with variable
-0000eed0: 7320 616e 6420 7265 7475 726e 7320 6d6f  s and returns mo
-0000eee0: 6469 6669 6564 2076 6172 6961 626c 6573  dified variables
-0000eef0: 2e0a 0a20 2020 2060 6069 6e69 7460 6020  ...    ``init`` 
-0000ef00: 7461 6b65 7320 6173 2066 6972 7374 2061  takes as first a
-0000ef10: 7267 756d 656e 7420 6569 7468 6572 2061  rgument either a
-0000ef20: 2073 696e 676c 6520 6060 5052 4e47 4b65   single ``PRNGKe
-0000ef30: 7960 602c 206f 7220 6120 6469 6374 696f  y``, or a dictio
-0000ef40: 6e61 7279 206d 6170 7069 6e67 2076 6172  nary mapping var
-0000ef50: 6961 626c 6520 636f 6c6c 6563 7469 6f6e  iable collection
-0000ef60: 7320 6e61 6d65 7320 746f 2074 6865 6972  s names to their
-0000ef70: 2060 6050 524e 474b 6579 7360 602c 2061   ``PRNGKeys``, a
-0000ef80: 6e64 2077 696c 6c20 6361 6c6c 2060 606d  nd will call ``m
-0000ef90: 6574 686f 6460 6020 2877 6869 6368 2069  ethod`` (which i
-0000efa0: 7320 7468 6520 6d6f 6475 6c65 2773 2060  s the module's `
-0000efb0: 605f 5f63 616c 6c5f 5f60 6020 6675 6e63  `__call__`` func
-0000efc0: 7469 6f6e 2062 7920 6465 6661 756c 7429  tion by default)
-0000efd0: 2070 6173 7369 6e67 2060 602a 6172 6773   passing ``*args
-0000efe0: 6060 2061 6e64 2060 602a 2a6b 7761 7267  `` and ``**kwarg
-0000eff0: 7360 602c 2061 6e64 2072 6574 7572 6e73  s``, and returns
-0000f000: 0a20 2020 2061 2064 6963 7469 6f6e 6172  .    a dictionar
-0000f010: 7920 6f66 2069 6e69 7469 616c 697a 6564  y of initialized
-0000f020: 2076 6172 6961 626c 6573 2e0a 0a20 2020   variables...   
-0000f030: 2045 7861 6d70 6c65 3a3a 0a0a 2020 2020   Example::..    
-0000f040: 2020 3e3e 3e20 696d 706f 7274 2066 6c61    >>> import fla
-0000f050: 782e 6c69 6e65 6e20 6173 206e 6e0a 2020  x.linen as nn.  
-0000f060: 2020 2020 3e3e 3e20 696d 706f 7274 206a      >>> import j
-0000f070: 6178 2e6e 756d 7079 2061 7320 6a6e 700a  ax.numpy as jnp.
-0000f080: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-0000f090: 206a 6178 0a20 2020 2020 202e 2e2e 0a20   jax.      .... 
-0000f0a0: 2020 2020 203e 3e3e 2063 6c61 7373 2046       >>> class F
-0000f0b0: 6f6f 286e 6e2e 4d6f 6475 6c65 293a 0a20  oo(nn.Module):. 
-0000f0c0: 2020 2020 202e 2e2e 2020 2040 6e6e 2e63       ...   @nn.c
-0000f0d0: 6f6d 7061 6374 0a20 2020 2020 202e 2e2e  ompact.      ...
-0000f0e0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-0000f0f0: 7365 6c66 2c20 782c 2074 7261 696e 293a  self, x, train):
-0000f100: 0a20 2020 2020 202e 2e2e 2020 2020 2078  .      ...     x
-0000f110: 203d 206e 6e2e 4465 6e73 6528 3136 2928   = nn.Dense(16)(
-0000f120: 7829 0a20 2020 2020 202e 2e2e 2020 2020  x).      ...    
-0000f130: 2078 203d 206e 6e2e 4261 7463 684e 6f72   x = nn.BatchNor
-0000f140: 6d28 7573 655f 7275 6e6e 696e 675f 6176  m(use_running_av
-0000f150: 6572 6167 653d 6e6f 7420 7472 6169 6e29  erage=not train)
-0000f160: 2878 290a 2020 2020 2020 2e2e 2e20 2020  (x).      ...   
-0000f170: 2020 7820 3d20 6e6e 2e72 656c 7528 7829    x = nn.relu(x)
-0000f180: 0a20 2020 2020 202e 2e2e 2020 2020 2072  .      ...     r
-0000f190: 6574 7572 6e20 6e6e 2e44 656e 7365 2831  eturn nn.Dense(1
-0000f1a0: 2928 7829 0a20 2020 2020 202e 2e2e 0a20  )(x).      .... 
-0000f1b0: 2020 2020 203e 3e3e 206d 6f64 756c 6520       >>> module 
-0000f1c0: 3d20 466f 6f28 290a 2020 2020 2020 3e3e  = Foo().      >>
-0000f1d0: 3e20 6b65 7920 3d20 6a61 782e 7261 6e64  > key = jax.rand
-0000f1e0: 6f6d 2e50 524e 474b 6579 2830 290a 2020  om.PRNGKey(0).  
-0000f1f0: 2020 2020 3e3e 3e20 7661 7269 6162 6c65      >>> variable
-0000f200: 7320 3d20 6d6f 6475 6c65 2e69 6e69 7428  s = module.init(
-0000f210: 6b65 792c 206a 6e70 2e65 6d70 7479 2828  key, jnp.empty((
-0000f220: 312c 2037 2929 2c20 7472 6169 6e3d 4661  1, 7)), train=Fa
-0000f230: 6c73 6529 0a0a 2020 2020 4966 2079 6f75  lse)..    If you
-0000f240: 2070 6173 7320 6120 7369 6e67 6c65 2060   pass a single `
-0000f250: 6050 524e 474b 6579 6060 2c20 466c 6178  `PRNGKey``, Flax
-0000f260: 2077 696c 6c20 7573 6520 6974 2074 6f20   will use it to 
-0000f270: 6665 6564 2074 6865 2060 6027 7061 7261  feed the ``'para
-0000f280: 6d73 2760 6020 524e 4720 7374 7265 616d  ms'`` RNG stream
-0000f290: 2e0a 2020 2020 4966 2079 6f75 2077 616e  ..    If you wan
-0000f2a0: 7420 746f 2075 7365 2061 2064 6966 6665  t to use a diffe
-0000f2b0: 7265 6e74 2052 4e47 2073 7472 6561 6d20  rent RNG stream 
-0000f2c0: 6f72 206e 6565 6420 746f 2075 7365 206d  or need to use m
-0000f2d0: 756c 7469 706c 6520 7374 7265 616d 732c  ultiple streams,
-0000f2e0: 2079 6f75 206d 7573 7420 7061 7373 2061   you must pass a
-0000f2f0: 0a20 2020 2064 6963 7469 6f6e 6172 7920  .    dictionary 
-0000f300: 6d61 7070 696e 6720 6561 6368 2052 4e47  mapping each RNG
-0000f310: 2073 7472 6561 6d20 6e61 6d65 2074 6f20   stream name to 
-0000f320: 6974 7320 636f 7272 6573 706f 6e64 696e  its correspondin
-0000f330: 6720 6060 5052 4e47 4b65 7960 6020 746f  g ``PRNGKey`` to
-0000f340: 2060 6069 6e69 7460 602e 0a0a 2020 2020   ``init``...    
-0000f350: 4578 616d 706c 653a 3a0a 0a20 2020 2020  Example::..     
-0000f360: 203e 3e3e 2063 6c61 7373 2046 6f6f 286e   >>> class Foo(n
-0000f370: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2020  n.Module):.     
-0000f380: 202e 2e2e 2020 2040 6e6e 2e63 6f6d 7061   ...   @nn.compa
-0000f390: 6374 0a20 2020 2020 202e 2e2e 2020 2064  ct.      ...   d
-0000f3a0: 6566 205f 5f63 616c 6c5f 5f28 7365 6c66  ef __call__(self
-0000f3b0: 2c20 782c 2074 7261 696e 293a 0a20 2020  , x, train):.   
-0000f3c0: 2020 202e 2e2e 2020 2020 2078 203d 206e     ...     x = n
-0000f3d0: 6e2e 4465 6e73 6528 3136 2928 7829 0a20  n.Dense(16)(x). 
-0000f3e0: 2020 2020 202e 2e2e 2020 2020 2078 203d       ...     x =
-0000f3f0: 206e 6e2e 4261 7463 684e 6f72 6d28 7573   nn.BatchNorm(us
-0000f400: 655f 7275 6e6e 696e 675f 6176 6572 6167  e_running_averag
-0000f410: 653d 6e6f 7420 7472 6169 6e29 2878 290a  e=not train)(x).
-0000f420: 2020 2020 2020 2e2e 2e20 2020 2020 7820        ...     x 
-0000f430: 3d20 6e6e 2e72 656c 7528 7829 0a20 2020  = nn.relu(x).   
-0000f440: 2020 202e 2e2e 0a20 2020 2020 202e 2e2e     ....      ...
-0000f450: 2020 2020 2023 2041 6464 2067 6175 7373       # Add gauss
-0000f460: 6961 6e20 6e6f 6973 650a 2020 2020 2020  ian noise.      
-0000f470: 2e2e 2e20 2020 2020 6e6f 6973 655f 6b65  ...     noise_ke
-0000f480: 7920 3d20 7365 6c66 2e6d 616b 655f 726e  y = self.make_rn
-0000f490: 6728 276e 6f69 7365 2729 0a20 2020 2020  g('noise').     
-0000f4a0: 202e 2e2e 2020 2020 2078 203d 2078 202b   ...     x = x +
-0000f4b0: 206a 6178 2e72 616e 646f 6d2e 6e6f 726d   jax.random.norm
-0000f4c0: 616c 286e 6f69 7365 5f6b 6579 2c20 782e  al(noise_key, x.
-0000f4d0: 7368 6170 6529 0a20 2020 2020 202e 2e2e  shape).      ...
-0000f4e0: 0a20 2020 2020 202e 2e2e 2020 2020 2072  .      ...     r
-0000f4f0: 6574 7572 6e20 6e6e 2e44 656e 7365 2831  eturn nn.Dense(1
-0000f500: 2928 7829 0a20 2020 2020 202e 2e2e 0a20  )(x).      .... 
-0000f510: 2020 2020 203e 3e3e 206d 6f64 756c 6520       >>> module 
-0000f520: 3d20 466f 6f28 290a 2020 2020 2020 3e3e  = Foo().      >>
-0000f530: 3e20 726e 6773 203d 207b 2770 6172 616d  > rngs = {'param
-0000f540: 7327 3a20 6a61 782e 7261 6e64 6f6d 2e50  s': jax.random.P
-0000f550: 524e 474b 6579 2830 292c 2027 6e6f 6973  RNGKey(0), 'nois
-0000f560: 6527 3a20 6a61 782e 7261 6e64 6f6d 2e50  e': jax.random.P
-0000f570: 524e 474b 6579 2831 297d 0a20 2020 2020  RNGKey(1)}.     
-0000f580: 203e 3e3e 2076 6172 6961 626c 6573 203d   >>> variables =
-0000f590: 206d 6f64 756c 652e 696e 6974 2872 6e67   module.init(rng
-0000f5a0: 732c 206a 6e70 2e65 6d70 7479 2828 312c  s, jnp.empty((1,
-0000f5b0: 2037 2929 2c20 7472 6169 6e3d 4661 6c73   7)), train=Fals
-0000f5c0: 6529 0a0a 2020 2020 4a69 7474 696e 6720  e)..    Jitting 
-0000f5d0: 6069 6e69 7460 2069 6e69 7469 616c 697a  `init` initializ
-0000f5e0: 6573 2061 206d 6f64 656c 206c 617a 696c  es a model lazil
-0000f5f0: 7920 7573 696e 6720 6f6e 6c79 2074 6865  y using only the
-0000f600: 2073 6861 7065 7320 6f66 2074 6865 0a20   shapes of the. 
-0000f610: 2020 2070 726f 7669 6465 6420 6172 6775     provided argu
-0000f620: 6d65 6e74 732c 2061 6e64 2061 766f 6964  ments, and avoid
-0000f630: 7320 636f 6d70 7574 696e 6720 7468 6520  s computing the 
-0000f640: 666f 7277 6172 6420 7061 7373 2077 6974  forward pass wit
-0000f650: 6820 6163 7475 616c 0a20 2020 2076 616c  h actual.    val
-0000f660: 7565 732e 2045 7861 6d70 6c65 3a3a 0a0a  ues. Example::..
-0000f670: 2020 2020 2020 3e3e 3e20 6d6f 6475 6c65        >>> module
-0000f680: 203d 206e 6e2e 4465 6e73 6528 3129 0a20   = nn.Dense(1). 
-0000f690: 2020 2020 203e 3e3e 2069 6e69 745f 6a69       >>> init_ji
-0000f6a0: 7420 3d20 6a61 782e 6a69 7428 6d6f 6475  t = jax.jit(modu
-0000f6b0: 6c65 2e69 6e69 7429 0a20 2020 2020 203e  le.init).      >
-0000f6c0: 3e3e 2076 6172 6961 626c 6573 203d 2069  >> variables = i
-0000f6d0: 6e69 745f 6a69 7428 6a61 782e 7261 6e64  nit_jit(jax.rand
-0000f6e0: 6f6d 2e50 524e 474b 6579 2830 292c 206a  om.PRNGKey(0), j
-0000f6f0: 6e70 2e65 6d70 7479 2828 312c 2037 2929  np.empty((1, 7))
-0000f700: 290a 0a20 2020 2060 6069 6e69 7460 6020  )..    ``init`` 
-0000f710: 6973 2061 206c 6967 6874 2077 7261 7070  is a light wrapp
-0000f720: 6572 206f 7665 7220 6060 6170 706c 7960  er over ``apply`
-0000f730: 602c 2073 6f20 6f74 6865 7220 6060 6170  `, so other ``ap
-0000f740: 706c 7960 6020 6172 6775 6d65 6e74 7320  ply`` arguments 
-0000f750: 6c69 6b65 0a20 2020 2060 606d 6574 686f  like.    ``metho
-0000f760: 6460 602c 2060 606d 7574 6162 6c65 6060  d``, ``mutable``
-0000f770: 2c20 616e 6420 6060 6361 7074 7572 655f  , and ``capture_
-0000f780: 696e 7465 726d 6564 6961 7465 7360 6020  intermediates`` 
-0000f790: 6172 6520 616c 736f 2061 7661 696c 6162  are also availab
-0000f7a0: 6c65 2e0a 0a20 2020 2041 7267 733a 0a20  le...    Args:. 
-0000f7b0: 2020 2020 2072 6e67 733a 2054 6865 2072       rngs: The r
-0000f7c0: 6e67 7320 666f 7220 7468 6520 7661 7269  ngs for the vari
-0000f7d0: 6162 6c65 2063 6f6c 6c65 6374 696f 6e73  able collections
-0000f7e0: 2e0a 2020 2020 2020 2a61 7267 733a 204e  ..      *args: N
-0000f7f0: 616d 6564 2061 7267 756d 656e 7473 2070  amed arguments p
-0000f800: 6173 7365 6420 746f 2074 6865 2069 6e69  assed to the ini
-0000f810: 7420 6675 6e63 7469 6f6e 2e0a 2020 2020  t function..    
-0000f820: 2020 6d65 7468 6f64 3a20 416e 206f 7074    method: An opt
-0000f830: 696f 6e61 6c20 6d65 7468 6f64 2e20 4966  ional method. If
-0000f840: 2070 726f 7669 6465 642c 2061 7070 6c69   provided, appli
-0000f850: 6573 2074 6869 7320 6d65 7468 6f64 2e20  es this method. 
-0000f860: 4966 206e 6f74 0a20 2020 2020 2020 2070  If not.        p
-0000f870: 726f 7669 6465 642c 2061 7070 6c69 6573  rovided, applies
-0000f880: 2074 6865 2060 605f 5f63 616c 6c5f 5f60   the ``__call__`
-0000f890: 6020 6d65 7468 6f64 2e20 4120 7374 7269  ` method. A stri
-0000f8a0: 6e67 2063 616e 2061 6c73 6f20 6265 0a20  ng can also be. 
-0000f8b0: 2020 2020 2020 2070 726f 7669 6465 6420         provided 
-0000f8c0: 746f 2073 7065 6369 6679 2061 206d 6574  to specify a met
-0000f8d0: 686f 6420 6279 206e 616d 652e 0a20 2020  hod by name..   
-0000f8e0: 2020 206d 7574 6162 6c65 3a20 4361 6e20     mutable: Can 
-0000f8f0: 6265 2062 6f6f 6c2c 2073 7472 2c20 6f72  be bool, str, or
-0000f900: 206c 6973 742e 2053 7065 6369 6669 6573   list. Specifies
-0000f910: 2077 6869 6368 2063 6f6c 6c65 6374 696f   which collectio
-0000f920: 6e73 2073 686f 756c 6420 6265 0a20 2020  ns should be.   
-0000f930: 2020 2020 2074 7265 6174 6564 2061 7320       treated as 
-0000f940: 6d75 7461 626c 653a 2060 6062 6f6f 6c60  mutable: ``bool`
-0000f950: 603a 2061 6c6c 2f6e 6f20 636f 6c6c 6563  `: all/no collec
-0000f960: 7469 6f6e 7320 6172 6520 6d75 7461 626c  tions are mutabl
-0000f970: 652e 0a20 2020 2020 2020 2060 6073 7472  e..        ``str
-0000f980: 6060 3a20 5468 6520 6e61 6d65 206f 6620  ``: The name of 
-0000f990: 6120 7369 6e67 6c65 206d 7574 6162 6c65  a single mutable
-0000f9a0: 2063 6f6c 6c65 6374 696f 6e2e 2060 606c   collection. ``l
-0000f9b0: 6973 7460 603a 2041 0a20 2020 2020 2020  ist``: A.       
-0000f9c0: 206c 6973 7420 6f66 206e 616d 6573 206f   list of names o
-0000f9d0: 6620 6d75 7461 626c 6520 636f 6c6c 6563  f mutable collec
-0000f9e0: 7469 6f6e 732e 2042 7920 6465 6661 756c  tions. By defaul
-0000f9f0: 7420 616c 6c20 636f 6c6c 6563 7469 6f6e  t all collection
-0000fa00: 730a 2020 2020 2020 2020 6578 6365 7074  s.        except
-0000fa10: 2022 696e 7465 726d 6564 6961 7465 7322   "intermediates"
-0000fa20: 2061 7265 206d 7574 6162 6c65 2e0a 2020   are mutable..  
-0000fa30: 2020 2020 6361 7074 7572 655f 696e 7465      capture_inte
-0000fa40: 726d 6564 6961 7465 733a 2049 6620 6054  rmediates: If `T
-0000fa50: 7275 6560 2c20 6361 7074 7572 6573 2069  rue`, captures i
-0000fa60: 6e74 6572 6d65 6469 6174 6520 7265 7475  ntermediate retu
-0000fa70: 726e 2076 616c 7565 730a 2020 2020 2020  rn values.      
-0000fa80: 2020 6f66 2061 6c6c 204d 6f64 756c 6573    of all Modules
-0000fa90: 2069 6e73 6964 6520 7468 6520 2269 6e74   inside the "int
-0000faa0: 6572 6d65 6469 6174 6573 2220 636f 6c6c  ermediates" coll
-0000fab0: 6563 7469 6f6e 2e20 4279 2064 6566 6175  ection. By defau
-0000fac0: 6c74 206f 6e6c 790a 2020 2020 2020 2020  lt only.        
-0000fad0: 7468 6520 7265 7475 726e 2076 616c 7565  the return value
-0000fae0: 7320 6f66 2061 6c6c 2060 605f 5f63 616c  s of all ``__cal
-0000faf0: 6c5f 5f60 6020 6d65 7468 6f64 7320 6172  l__`` methods ar
-0000fb00: 6520 7374 6f72 6564 2e20 4120 6675 6e63  e stored. A func
-0000fb10: 7469 6f6e 2063 616e 0a20 2020 2020 2020  tion can.       
-0000fb20: 2062 6520 7061 7373 6564 2074 6f20 6368   be passed to ch
-0000fb30: 616e 6765 2074 6865 2066 696c 7465 7220  ange the filter 
-0000fb40: 6265 6861 7669 6f72 2e20 5468 6520 6669  behavior. The fi
-0000fb50: 6c74 6572 2066 756e 6374 696f 6e20 7461  lter function ta
-0000fb60: 6b65 730a 2020 2020 2020 2020 7468 6520  kes.        the 
-0000fb70: 4d6f 6475 6c65 2069 6e73 7461 6e63 6520  Module instance 
-0000fb80: 616e 6420 6d65 7468 6f64 206e 616d 6520  and method name 
-0000fb90: 616e 6420 7265 7475 726e 7320 6120 626f  and returns a bo
-0000fba0: 6f6c 2069 6e64 6963 6174 696e 670a 2020  ol indicating.  
-0000fbb0: 2020 2020 2020 7768 6574 6865 7220 7468        whether th
-0000fbc0: 6520 6f75 7470 7574 206f 6620 7468 6174  e output of that
-0000fbd0: 206d 6574 686f 6420 696e 766f 6361 7469   method invocati
-0000fbe0: 6f6e 2073 686f 756c 6420 6265 2073 746f  on should be sto
-0000fbf0: 7265 642e 0a20 2020 2020 202a 2a6b 7761  red..      **kwa
-0000fc00: 7267 733a 204b 6579 776f 7264 2061 7267  rgs: Keyword arg
-0000fc10: 756d 656e 7473 2070 6173 7365 6420 746f  uments passed to
-0000fc20: 2074 6865 2069 6e69 7420 6675 6e63 7469   the init functi
-0000fc30: 6f6e 2e0a 2020 2020 5265 7475 726e 733a  on..    Returns:
-0000fc40: 0a20 2020 2020 2054 6865 2069 6e69 7469  .      The initi
-0000fc50: 616c 697a 6564 2076 6172 6961 626c 6520  alized variable 
-0000fc60: 6469 6374 2e0a 2020 2020 2222 220a 2020  dict..    """.  
-0000fc70: 2020 4d6f 6475 6c65 2e5f 6d6f 6475 6c65    Module._module
-0000fc80: 5f63 6865 636b 7328 7365 6c66 290a 0a20  _checks(self).. 
-0000fc90: 2020 205f 2c20 765f 6f75 7420 3d20 7365     _, v_out = se
-0000fca0: 6c66 2e69 6e69 745f 7769 7468 5f6f 7574  lf.init_with_out
-0000fcb0: 7075 7428 0a20 2020 2020 2020 2072 6e67  put(.        rng
-0000fcc0: 732c 0a20 2020 2020 2020 202a 6172 6773  s,.        *args
-0000fcd0: 2c0a 2020 2020 2020 2020 6d65 7468 6f64  ,.        method
-0000fce0: 3d6d 6574 686f 642c 0a20 2020 2020 2020  =method,.       
-0000fcf0: 206d 7574 6162 6c65 3d6d 7574 6162 6c65   mutable=mutable
-0000fd00: 2c0a 2020 2020 2020 2020 6361 7074 7572  ,.        captur
-0000fd10: 655f 696e 7465 726d 6564 6961 7465 733d  e_intermediates=
-0000fd20: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
-0000fd30: 6961 7465 732c 0a20 2020 2020 2020 202a  iates,.        *
-0000fd40: 2a6b 7761 7267 732c 0a20 2020 2029 0a20  *kwargs,.    ). 
-0000fd50: 2020 2072 6574 7572 6e20 765f 6f75 740a     return v_out.
-0000fd60: 0a20 2040 7472 6163 6562 6163 6b5f 7574  .  @traceback_ut
-0000fd70: 696c 2e61 7069 5f62 6f75 6e64 6172 790a  il.api_boundary.
-0000fd80: 2020 6465 6620 6c61 7a79 5f69 6e69 7428    def lazy_init(
-0000fd90: 0a20 2020 2020 2073 656c 662c 0a20 2020  .      self,.   
-0000fda0: 2020 2072 6e67 733a 2055 6e69 6f6e 5b4b     rngs: Union[K
-0000fdb0: 6579 4172 7261 792c 2052 4e47 5365 7175  eyArray, RNGSequ
-0000fdc0: 656e 6365 735d 2c0a 2020 2020 2020 2a61  ences],.      *a
-0000fdd0: 7267 732c 0a20 2020 2020 206d 6574 686f  rgs,.      metho
-0000fde0: 643a 204f 7074 696f 6e61 6c5b 4361 6c6c  d: Optional[Call
-0000fdf0: 6162 6c65 5b2e 2e2e 2c20 416e 795d 5d20  able[..., Any]] 
-0000fe00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 6d75  = None,.      mu
-0000fe10: 7461 626c 653a 2043 6f6c 6c65 6374 696f  table: Collectio
-0000fe20: 6e46 696c 7465 7220 3d20 4465 6e79 4c69  nFilter = DenyLi
-0000fe30: 7374 2827 696e 7465 726d 6564 6961 7465  st('intermediate
-0000fe40: 7327 292c 0a20 2020 2020 202a 2a6b 7761  s'),.      **kwa
-0000fe50: 7267 732c 0a20 2029 202d 3e20 4672 6f7a  rgs,.  ) -> Froz
-0000fe60: 656e 5661 7269 6162 6c65 4469 6374 3a0a  enVariableDict:.
-0000fe70: 2020 2020 2222 2249 6e69 7469 616c 697a      """Initializ
-0000fe80: 6573 2061 206d 6f64 756c 6520 7769 7468  es a module with
-0000fe90: 6f75 7420 636f 6d70 7574 696e 6720 6f6e  out computing on
-0000fea0: 2061 6e20 6163 7475 616c 2069 6e70 7574   an actual input
-0000feb0: 2e0a 0a20 2020 206c 617a 795f 696e 6974  ...    lazy_init
-0000fec0: 2077 696c 6c20 696e 6974 6961 6c69 7a65   will initialize
-0000fed0: 2074 6865 2076 6172 6961 626c 6573 2077   the variables w
-0000fee0: 6974 686f 7574 2064 6f69 6e67 2075 6e6e  ithout doing unn
-0000fef0: 6563 6573 7361 7279 2063 6f6d 7075 7465  ecessary compute
-0000ff00: 2e0a 2020 2020 5468 6520 696e 7075 7420  ..    The input 
-0000ff10: 6461 7461 2073 686f 756c 6420 6265 2070  data should be p
-0000ff20: 6173 7365 6420 6173 2061 2060 606a 6178  assed as a ``jax
-0000ff30: 2e53 6861 7065 4474 7970 6553 7472 7563  .ShapeDtypeStruc
-0000ff40: 7460 6020 7768 6963 6820 7370 6563 6966  t`` which specif
-0000ff50: 6965 730a 2020 2020 7468 6520 7368 6170  ies.    the shap
-0000ff60: 6520 616e 6420 6474 7970 6520 6f66 2074  e and dtype of t
-0000ff70: 6865 2069 6e70 7574 2062 7574 206e 6f20  he input but no 
-0000ff80: 636f 6e63 7265 7465 2064 6174 612e 0a0a  concrete data...
-0000ff90: 2020 2020 4578 616d 706c 653a 3a0a 0a20      Example::.. 
-0000ffa0: 2020 2020 206d 6f64 656c 203d 206e 6e2e       model = nn.
-0000ffb0: 4465 6e73 6528 6665 6174 7572 6573 3d32  Dense(features=2
-0000ffc0: 3536 290a 2020 2020 2020 7661 7269 6162  56).      variab
-0000ffd0: 6c65 7320 3d20 6d6f 6465 6c2e 6c61 7a79  les = model.lazy
-0000ffe0: 5f69 6e69 7428 726e 672c 206a 6178 2e53  _init(rng, jax.S
-0000fff0: 6861 7065 4474 7970 6553 7472 7563 7428  hapeDtypeStruct(
-00010000: 2831 2c20 3132 3829 2c20 6a6e 702e 666c  (1, 128), jnp.fl
-00010010: 6f61 7433 3229 290a 0a20 2020 2054 6865  oat32))..    The
-00010020: 2061 7267 7320 616e 6420 6b77 6172 6773   args and kwargs
-00010030: 2061 7267 7320 7061 7373 6564 2074 6f20   args passed to 
-00010040: 6060 6c61 7a79 5f69 6e69 7460 6020 6361  ``lazy_init`` ca
-00010050: 6e20 6265 2061 206d 6978 206f 660a 2020  n be a mix of.  
-00010060: 2020 636f 6e63 7265 7465 2028 6a61 7820    concrete (jax 
-00010070: 6172 7261 7973 2c20 7363 616c 6172 732c  arrays, scalars,
-00010080: 2062 6f6f 6c73 2920 616e 6420 6162 7374   bools) and abst
-00010090: 7261 6374 2028 5368 6170 6544 7479 7065  ract (ShapeDtype
-000100a0: 5374 7275 6374 2920 7661 6c75 6573 2e0a  Struct) values..
-000100b0: 2020 2020 436f 6e63 7265 7465 2076 616c      Concrete val
-000100c0: 7565 7320 6172 6520 6f6e 6c79 206e 6563  ues are only nec
-000100d0: 6573 7361 7279 2066 6f72 2061 7267 756d  essary for argum
-000100e0: 656e 7473 2074 6861 7420 6166 6665 6374  ents that affect
-000100f0: 0a20 2020 2074 6865 2069 6e69 7469 616c  .    the initial
-00010100: 697a 6174 696f 6e20 6f66 2076 6172 6961  ization of varia
-00010110: 626c 6573 2e20 466f 7220 6578 616d 706c  bles. For exampl
-00010120: 652c 2074 6865 206d 6f64 656c 206d 6967  e, the model mig
-00010130: 6874 2065 7870 6563 740a 2020 2020 6120  ht expect.    a 
-00010140: 6b65 7977 6f72 6420 6172 6720 7468 6174  keyword arg that
-00010150: 2065 6e61 626c 6573 2f64 6973 6162 6c65   enables/disable
-00010160: 7320 6120 7375 6270 6172 7420 6f66 2074  s a subpart of t
-00010170: 6865 206d 6f64 656c 2e0a 2020 2020 496e  he model..    In
-00010180: 2074 6869 7320 6361 7365 2c20 616e 2065   this case, an e
-00010190: 7870 6c69 6369 7420 7661 6c75 6520 2854  xplicit value (T
-000101a0: 7275 652f 466c 6173 6529 2073 686f 756c  rue/Flase) shoul
-000101b0: 6420 6265 2070 6173 7365 6420 6f74 6865  d be passed othe
-000101c0: 7277 6973 650a 2020 2020 6060 6c61 7a79  rwise.    ``lazy
-000101d0: 5f69 6e69 7460 6020 6361 6e6e 6f74 2069  _init`` cannot i
-000101e0: 6e66 6572 2077 6869 6368 2076 6172 6961  nfer which varia
-000101f0: 626c 6573 2073 686f 756c 6420 6265 2069  bles should be i
-00010200: 6e69 7469 616c 697a 6564 2e0a 0a20 2020  nitialized...   
-00010210: 2041 7267 733a 0a20 2020 2020 2072 6e67   Args:.      rng
-00010220: 733a 2054 6865 2072 6e67 7320 666f 7220  s: The rngs for 
-00010230: 7468 6520 7661 7269 6162 6c65 2063 6f6c  the variable col
-00010240: 6c65 6374 696f 6e73 2e0a 2020 2020 2020  lections..      
-00010250: 2a61 7267 733a 2061 7267 756d 656e 7473  *args: arguments
-00010260: 2070 6173 7365 6420 746f 2074 6865 2069   passed to the i
-00010270: 6e69 7420 6675 6e63 7469 6f6e 2e0a 2020  nit function..  
-00010280: 2020 2020 6d65 7468 6f64 3a20 416e 206f      method: An o
-00010290: 7074 696f 6e61 6c20 6d65 7468 6f64 2e20  ptional method. 
-000102a0: 4966 2070 726f 7669 6465 642c 2061 7070  If provided, app
-000102b0: 6c69 6573 2074 6869 7320 6d65 7468 6f64  lies this method
-000102c0: 2e20 4966 206e 6f74 0a20 2020 2020 2020  . If not.       
-000102d0: 2070 726f 7669 6465 642c 2061 7070 6c69   provided, appli
-000102e0: 6573 2074 6865 2060 605f 5f63 616c 6c5f  es the ``__call_
-000102f0: 5f60 6020 6d65 7468 6f64 2e0a 2020 2020  _`` method..    
-00010300: 2020 6d75 7461 626c 653a 2043 616e 2062    mutable: Can b
-00010310: 6520 626f 6f6c 2c20 7374 722c 206f 7220  e bool, str, or 
-00010320: 6c69 7374 2e20 5370 6563 6966 6965 7320  list. Specifies 
-00010330: 7768 6963 6820 636f 6c6c 6563 7469 6f6e  which collection
-00010340: 7320 7368 6f75 6c64 2062 650a 2020 2020  s should be.    
-00010350: 2020 2020 7472 6561 7465 6420 6173 206d      treated as m
-00010360: 7574 6162 6c65 3a20 6060 626f 6f6c 6060  utable: ``bool``
-00010370: 3a20 616c 6c2f 6e6f 2063 6f6c 6c65 6374  : all/no collect
-00010380: 696f 6e73 2061 7265 206d 7574 6162 6c65  ions are mutable
-00010390: 2e0a 2020 2020 2020 2020 6060 7374 7260  ..        ``str`
-000103a0: 603a 2054 6865 206e 616d 6520 6f66 2061  `: The name of a
-000103b0: 2073 696e 676c 6520 6d75 7461 626c 6520   single mutable 
-000103c0: 636f 6c6c 6563 7469 6f6e 2e20 6060 6c69  collection. ``li
-000103d0: 7374 6060 3a20 410a 2020 2020 2020 2020  st``: A.        
-000103e0: 6c69 7374 206f 6620 6e61 6d65 7320 6f66  list of names of
-000103f0: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
-00010400: 696f 6e73 2e20 4279 2064 6566 6175 6c74  ions. By default
-00010410: 2061 6c6c 2063 6f6c 6c65 6374 696f 6e73   all collections
-00010420: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00010430: 2269 6e74 6572 6d65 6469 6174 6573 2220  "intermediates" 
-00010440: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
-00010450: 2020 202a 2a6b 7761 7267 733a 204b 6579     **kwargs: Key
-00010460: 776f 7264 2061 7267 756d 656e 7473 2070  word arguments p
-00010470: 6173 7365 6420 746f 2074 6865 2069 6e69  assed to the ini
-00010480: 7420 6675 6e63 7469 6f6e 2e0a 2020 2020  t function..    
-00010490: 5265 7475 726e 733a 0a20 2020 2020 2054  Returns:.      T
-000104a0: 6865 2069 6e69 7469 616c 697a 6564 2076  he initialized v
-000104b0: 6172 6961 626c 6520 6469 6374 2e0a 2020  ariable dict..  
-000104c0: 2020 2222 220a 2020 2020 4d6f 6475 6c65    """.    Module
-000104d0: 2e5f 6d6f 6475 6c65 5f63 6865 636b 7328  ._module_checks(
-000104e0: 7365 6c66 290a 0a20 2020 2064 6566 206c  self)..    def l
-000104f0: 617a 795f 7772 6170 7065 7228 726e 6773  azy_wrapper(rngs
-00010500: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00010510: 7329 3a0a 2020 2020 2020 7265 7475 726e  s):.      return
-00010520: 2073 656c 662e 696e 6974 2872 6e67 732c   self.init(rngs,
-00010530: 202a 6172 6773 2c20 6d65 7468 6f64 3d6d   *args, method=m
-00010540: 6574 686f 642c 206d 7574 6162 6c65 3d6d  ethod, mutable=m
-00010550: 7574 6162 6c65 2c20 2a2a 6b77 6172 6773  utable, **kwargs
-00010560: 290a 0a20 2020 2072 6574 7572 6e20 7061  )..    return pa
-00010570: 7274 6961 6c5f 6576 616c 2e6c 617a 795f  rtial_eval.lazy_
-00010580: 696e 6974 286c 617a 795f 7772 6170 7065  init(lazy_wrappe
-00010590: 7229 2872 6e67 732c 202a 6172 6773 2c20  r)(rngs, *args, 
-000105a0: 2a2a 6b77 6172 6773 290a 0a20 2040 7072  **kwargs)..  @pr
-000105b0: 6f70 6572 7479 0a20 2064 6566 2076 6172  operty.  def var
-000105c0: 6961 626c 6573 2873 656c 6629 202d 3e20  iables(self) -> 
-000105d0: 5661 7269 6162 6c65 4469 6374 3a0a 2020  VariableDict:.  
-000105e0: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
-000105f0: 2076 6172 6961 626c 6573 2069 6e20 7468   variables in th
-00010600: 6973 206d 6f64 756c 652e 2222 220a 2020  is module.""".  
-00010610: 2020 6966 2073 656c 662e 7363 6f70 6520    if self.scope 
-00010620: 6973 204e 6f6e 653a 0a20 2020 2020 2072  is None:.      r
-00010630: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00010640: 2243 616e 2774 2061 6363 6573 7320 7661  "Can't access va
-00010650: 7269 6162 6c65 7320 6f6e 2075 6e62 6f75  riables on unbou
-00010660: 6e64 206d 6f64 756c 6573 2229 0a20 2020  nd modules").   
-00010670: 2072 6574 7572 6e20 7365 6c66 2e73 636f   return self.sco
-00010680: 7065 2e76 6172 6961 626c 6573 2829 0a0a  pe.variables()..
-00010690: 2020 6465 6620 6765 745f 7661 7269 6162    def get_variab
-000106a0: 6c65 2873 656c 662c 2063 6f6c 3a20 7374  le(self, col: st
-000106b0: 722c 206e 616d 653a 2073 7472 2c20 6465  r, name: str, de
-000106c0: 6661 756c 743a 204f 7074 696f 6e61 6c5b  fault: Optional[
-000106d0: 545d 203d 204e 6f6e 6529 202d 3e20 543a  T] = None) -> T:
-000106e0: 0a20 2020 2022 2222 5265 7472 6965 7665  .    """Retrieve
-000106f0: 7320 7468 6520 7661 6c75 6520 6f66 2061  s the value of a
-00010700: 2056 6172 6961 626c 652e 0a0a 2020 2020   Variable...    
-00010710: 4172 6773 3a0a 2020 2020 2020 636f 6c3a  Args:.      col:
-00010720: 2074 6865 2076 6172 6961 626c 6520 636f   the variable co
-00010730: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00010740: 6e61 6d65 3a20 7468 6520 6e61 6d65 206f  name: the name o
-00010750: 6620 7468 6520 7661 7269 6162 6c65 2e0a  f the variable..
-00010760: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
-00010770: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-00010780: 2074 6f20 7265 7475 726e 2069 6620 7468   to return if th
-00010790: 6520 7661 7269 6162 6c65 2064 6f65 7320  e variable does 
-000107a0: 6e6f 7420 6578 6973 7420 696e 0a20 2020  not exist in.   
-000107b0: 2020 2020 2074 6869 7320 7363 6f70 652e       this scope.
-000107c0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000107d0: 2020 2020 2054 6865 2076 616c 7565 206f       The value o
-000107e0: 6620 7468 6520 696e 7075 7420 7661 7269  f the input vari
-000107f0: 6162 6c65 2c20 6f66 2074 6865 2064 6566  able, of the def
-00010800: 6175 6c74 2076 616c 7565 2069 6620 7468  ault value if th
-00010810: 6520 7661 7269 6162 6c65 0a20 2020 2020  e variable.     
-00010820: 2064 6f65 736e 2774 2065 7869 7374 2069   doesn't exist i
-00010830: 6e20 7468 6973 2073 636f 7065 2e0a 2020  n this scope..  
-00010840: 2020 2222 220a 2020 2020 6966 2073 656c    """.    if sel
-00010850: 662e 7363 6f70 6520 6973 204e 6f6e 653a  f.scope is None:
-00010860: 0a20 2020 2020 2072 6169 7365 2056 616c  .      raise Val
-00010870: 7565 4572 726f 7228 2243 616e 2774 2061  ueError("Can't a
-00010880: 6363 6573 7320 7661 7269 6162 6c65 7320  ccess variables 
-00010890: 6f6e 2075 6e62 6f75 6e64 206d 6f64 756c  on unbound modul
-000108a0: 6573 2229 0a20 2020 2072 6574 7572 6e20  es").    return 
-000108b0: 7365 6c66 2e73 636f 7065 2e67 6574 5f76  self.scope.get_v
-000108c0: 6172 6961 626c 6528 636f 6c2c 206e 616d  ariable(col, nam
-000108d0: 652c 2064 6566 6175 6c74 290a 0a20 2064  e, default)..  d
-000108e0: 6566 2070 7574 5f76 6172 6961 626c 6528  ef put_variable(
-000108f0: 7365 6c66 2c20 636f 6c3a 2073 7472 2c20  self, col: str, 
-00010900: 6e61 6d65 3a20 7374 722c 2076 616c 7565  name: str, value
-00010910: 3a20 416e 7929 3a0a 2020 2020 2222 2255  : Any):.    """U
-00010920: 7064 6174 6573 2074 6865 2076 616c 7565  pdates the value
-00010930: 206f 6620 7468 6520 6769 7665 6e20 7661   of the given va
-00010940: 7269 6162 6c65 2069 6620 6974 2069 7320  riable if it is 
-00010950: 6d75 7461 626c 652c 206f 7220 616e 2065  mutable, or an e
-00010960: 7272 6f72 206f 7468 6572 7769 7365 2e0a  rror otherwise..
-00010970: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00010980: 2063 6f6c 3a20 7468 6520 7661 7269 6162   col: the variab
-00010990: 6c65 2063 6f6c 6c65 6374 696f 6e2e 0a20  le collection.. 
-000109a0: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-000109b0: 616d 6520 6f66 2074 6865 2076 6172 6961  ame of the varia
-000109c0: 626c 652e 0a20 2020 2020 2076 616c 7565  ble..      value
-000109d0: 3a20 7468 6520 6e65 7720 7661 6c75 6520  : the new value 
-000109e0: 6f66 2074 6865 2076 6172 6961 626c 652e  of the variable.
-000109f0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00010a00: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
-00010a10: 6e65 3a0a 2020 2020 2020 7261 6973 6520  ne:.      raise 
-00010a20: 5661 6c75 6545 7272 6f72 2822 4361 6e27  ValueError("Can'
-00010a30: 7420 6163 6365 7373 2076 6172 6961 626c  t access variabl
-00010a40: 6573 206f 6e20 756e 626f 756e 6420 6d6f  es on unbound mo
-00010a50: 6475 6c65 7322 290a 2020 2020 7365 6c66  dules").    self
-00010a60: 2e73 636f 7065 2e70 7574 5f76 6172 6961  .scope.put_varia
-00010a70: 626c 6528 636f 6c2c 206e 616d 652c 2076  ble(col, name, v
-00010a80: 616c 7565 290a 0a20 2040 6f76 6572 6c6f  alue)..  @overlo
-00010a90: 6164 0a20 2064 6566 2073 6f77 2873 656c  ad.  def sow(sel
-00010aa0: 662c 2063 6f6c 3a20 7374 722c 206e 616d  f, col: str, nam
-00010ab0: 653a 2073 7472 2c20 7661 6c75 653a 2041  e: str, value: A
-00010ac0: 6e79 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ny) -> bool:.   
-00010ad0: 202e 2e2e 0a0a 2020 406f 7665 726c 6f61   .....  @overloa
-00010ae0: 640a 2020 6465 6620 736f 7728 0a20 2020  d.  def sow(.   
-00010af0: 2020 2073 656c 662c 0a20 2020 2020 2063     self,.      c
-00010b00: 6f6c 3a20 7374 722c 0a20 2020 2020 206e  ol: str,.      n
-00010b10: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
-00010b20: 7661 6c75 653a 2054 2c0a 2020 2020 2020  value: T,.      
-00010b30: 7265 6475 6365 5f66 6e3a 2043 616c 6c61  reduce_fn: Calla
-00010b40: 626c 655b 5b4b 2c20 545d 2c20 4b5d 203d  ble[[K, T], K] =
-00010b50: 2074 7570 6c65 5f72 6564 7563 652c 0a20   tuple_reduce,. 
-00010b60: 2020 2020 2069 6e69 745f 666e 3a20 4361       init_fn: Ca
-00010b70: 6c6c 6162 6c65 5b5b 5d2c 204b 5d20 3d20  llable[[], K] = 
-00010b80: 7475 706c 655f 696e 6974 2c20 2023 2074  tuple_init,  # t
-00010b90: 7970 653a 2069 676e 6f72 650a 2020 2920  ype: ignore.  ) 
-00010ba0: 2d3e 2062 6f6f 6c3a 0a20 2020 202e 2e2e  -> bool:.    ...
-00010bb0: 0a0a 2020 6465 6620 736f 7728 0a20 2020  ..  def sow(.   
-00010bc0: 2020 2073 656c 662c 0a20 2020 2020 2063     self,.      c
-00010bd0: 6f6c 3a20 7374 722c 0a20 2020 2020 206e  ol: str,.      n
-00010be0: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
-00010bf0: 7661 6c75 653a 2054 2c0a 2020 2020 2020  value: T,.      
-00010c00: 7265 6475 6365 5f66 6e3a 2043 616c 6c61  reduce_fn: Calla
-00010c10: 626c 655b 5b4b 2c20 545d 2c20 4b5d 203d  ble[[K, T], K] =
-00010c20: 2074 7570 6c65 5f72 6564 7563 652c 0a20   tuple_reduce,. 
-00010c30: 2020 2020 2069 6e69 745f 666e 3a20 4361       init_fn: Ca
-00010c40: 6c6c 6162 6c65 5b5b 5d2c 204b 5d20 3d20  llable[[], K] = 
-00010c50: 7475 706c 655f 696e 6974 2c20 2023 2074  tuple_init,  # t
-00010c60: 7970 653a 2069 676e 6f72 650a 2020 2920  ype: ignore.  ) 
-00010c70: 2d3e 2062 6f6f 6c3a 0a20 2020 2022 2222  -> bool:.    """
-00010c80: 5374 6f72 6573 2061 2076 616c 7565 2069  Stores a value i
-00010c90: 6e20 6120 636f 6c6c 6563 7469 6f6e 2e0a  n a collection..
-00010ca0: 0a20 2020 2043 6f6c 6c65 6374 696f 6e73  .    Collections
-00010cb0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00010cc0: 636f 6c6c 6563 7420 696e 7465 726d 6564  collect intermed
-00010cd0: 6961 7465 2076 616c 7565 7320 7769 7468  iate values with
-00010ce0: 6f75 740a 2020 2020 7468 6520 6f76 6572  out.    the over
-00010cf0: 6865 6164 206f 6620 6578 706c 6963 6974  head of explicit
-00010d00: 6c79 2070 6173 7369 6e67 2061 2063 6f6e  ly passing a con
-00010d10: 7461 696e 6572 2074 6872 6f75 6768 2065  tainer through e
-00010d20: 6163 6820 4d6f 6475 6c65 2063 616c 6c2e  ach Module call.
-00010d30: 0a0a 2020 2020 4966 2074 6865 2074 6172  ..    If the tar
-00010d40: 6765 7420 636f 6c6c 6563 7469 6f6e 2069  get collection i
-00010d50: 7320 6e6f 7420 6d75 7461 626c 6520 6073  s not mutable `s
-00010d60: 6f77 6020 6265 6861 7665 7320 6c69 6b65  ow` behaves like
-00010d70: 2061 206e 6f2d 6f70 0a20 2020 2061 6e64   a no-op.    and
-00010d80: 2072 6574 7572 6e73 2060 4661 6c73 6560   returns `False`
-00010d90: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a3a  ...    Example::
-00010da0: 0a0a 2020 2020 2020 696d 706f 7274 206a  ..      import j
-00010db0: 6178 0a20 2020 2020 2069 6d70 6f72 7420  ax.      import 
-00010dc0: 6a61 782e 6e75 6d70 7920 6173 206a 6e70  jax.numpy as jnp
-00010dd0: 0a20 2020 2020 2069 6d70 6f72 7420 666c  .      import fl
-00010de0: 6178 2e6c 696e 656e 2061 7320 6e6e 0a0a  ax.linen as nn..
-00010df0: 2020 2020 2020 636c 6173 7320 466f 6f28        class Foo(
-00010e00: 6e6e 2e4d 6f64 756c 6529 3a0a 2020 2020  nn.Module):.    
-00010e10: 2020 2020 406e 6e2e 636f 6d70 6163 740a      @nn.compact.
-00010e20: 2020 2020 2020 2020 6465 6620 5f5f 6361          def __ca
-00010e30: 6c6c 5f5f 2873 656c 662c 2078 293a 0a20  ll__(self, x):. 
-00010e40: 2020 2020 2020 2020 2068 203d 206e 6e2e           h = nn.
-00010e50: 4465 6e73 6528 3429 2878 290a 2020 2020  Dense(4)(x).    
-00010e60: 2020 2020 2020 7365 6c66 2e73 6f77 2827        self.sow('
-00010e70: 696e 7465 726d 6564 6961 7465 7327 2c20  intermediates', 
-00010e80: 2768 272c 2068 290a 2020 2020 2020 2020  'h', h).        
-00010e90: 2020 7265 7475 726e 206e 6e2e 4465 6e73    return nn.Dens
-00010ea0: 6528 3229 2868 290a 0a20 2020 2020 2078  e(2)(h)..      x
-00010eb0: 203d 206a 6e70 2e6f 6e65 7328 2831 362c   = jnp.ones((16,
-00010ec0: 2039 2929 0a20 2020 2020 206d 6f64 656c   9)).      model
-00010ed0: 203d 2046 6f6f 2829 0a20 2020 2020 2076   = Foo().      v
-00010ee0: 6172 6961 626c 6573 203d 206d 6f64 656c  ariables = model
-00010ef0: 2e69 6e69 7428 6a61 782e 7261 6e64 6f6d  .init(jax.random
-00010f00: 2e50 524e 474b 6579 2830 292c 2078 290a  .PRNGKey(0), x).
-00010f10: 2020 2020 2020 792c 2073 7461 7465 203d        y, state =
-00010f20: 206d 6f64 656c 2e61 7070 6c79 2876 6172   model.apply(var
-00010f30: 6961 626c 6573 2c20 782c 206d 7574 6162  iables, x, mutab
-00010f40: 6c65 3d5b 2769 6e74 6572 6d65 6469 6174  le=['intermediat
-00010f50: 6573 275d 290a 2020 2020 2020 7072 696e  es']).      prin
-00010f60: 7428 7374 6174 655b 2769 6e74 6572 6d65  t(state['interme
-00010f70: 6469 6174 6573 275d 2920 2023 207b 2768  diates'])  # {'h
-00010f80: 273a 2028 2e2e 2e2c 297d 0a0a 2020 2020  ': (...,)}..    
-00010f90: 4279 2064 6566 6175 6c74 2074 6865 2076  By default the v
-00010fa0: 616c 7565 7320 6172 6520 7374 6f72 6564  alues are stored
-00010fb0: 2069 6e20 6120 7475 706c 6520 616e 6420   in a tuple and 
-00010fc0: 6561 6368 2073 746f 7265 6420 7661 6c75  each stored valu
-00010fd0: 650a 2020 2020 6973 2061 7070 656e 6465  e.    is appende
-00010fe0: 6420 6174 2074 6865 2065 6e64 2e20 5468  d at the end. Th
-00010ff0: 6973 2077 6179 2061 6c6c 2069 6e74 6572  is way all inter
-00011000: 6d65 6469 6174 6573 2063 616e 2062 6520  mediates can be 
-00011010: 7472 6163 6b65 6420 7768 656e 0a20 2020  tracked when.   
-00011020: 2074 6865 2073 616d 6520 6d6f 6475 6c65   the same module
-00011030: 2069 7320 6361 6c6c 6564 206d 756c 7469   is called multi
-00011040: 706c 6520 7469 6d65 732e 2041 6c74 6572  ple times. Alter
-00011050: 6e61 7469 7665 6c79 2c20 6120 6375 7374  natively, a cust
-00011060: 6f6d 0a20 2020 2069 6e69 742f 7265 6475  om.    init/redu
-00011070: 6365 2066 756e 6374 696f 6e20 6361 6e20  ce function can 
-00011080: 6265 2070 6173 7365 643a 3a0a 0a20 2020  be passed::..   
-00011090: 2020 2063 6c61 7373 2046 6f6f 3228 6e6e     class Foo2(nn
-000110a0: 2e4d 6f64 756c 6529 3a0a 2020 2020 2020  .Module):.      
-000110b0: 2020 406e 6e2e 636f 6d70 6163 740a 2020    @nn.compact.  
-000110c0: 2020 2020 2020 6465 6620 5f5f 6361 6c6c        def __call
-000110d0: 5f5f 2873 656c 662c 2078 293a 0a20 2020  __(self, x):.   
-000110e0: 2020 2020 2020 2069 6e69 745f 666e 203d         init_fn =
-000110f0: 206c 616d 6264 613a 2030 0a20 2020 2020   lambda: 0.     
-00011100: 2020 2020 2072 6564 7563 655f 666e 203d       reduce_fn =
-00011110: 206c 616d 6264 6120 612c 2062 3a20 6120   lambda a, b: a 
-00011120: 2b20 620a 2020 2020 2020 2020 2020 7365  + b.          se
-00011130: 6c66 2e73 6f77 2827 696e 7465 726d 6564  lf.sow('intermed
-00011140: 6961 7465 7327 2c20 2768 272c 2078 2c0a  iates', 'h', x,.
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2069 6e69 745f 666e 3d69 6e69 745f     init_fn=init_
-00011170: 666e 2c20 7265 6475 6365 5f66 6e3d 7265  fn, reduce_fn=re
-00011180: 6475 6365 5f66 6e29 0a20 2020 2020 2020  duce_fn).       
-00011190: 2020 2073 656c 662e 736f 7728 2769 6e74     self.sow('int
-000111a0: 6572 6d65 6469 6174 6573 272c 2027 6827  ermediates', 'h'
-000111b0: 2c20 7820 2a20 322c 0a20 2020 2020 2020  , x * 2,.       
-000111c0: 2020 2020 2020 2020 2020 2020 696e 6974              init
-000111d0: 5f66 6e3d 696e 6974 5f66 6e2c 2072 6564  _fn=init_fn, red
-000111e0: 7563 655f 666e 3d72 6564 7563 655f 666e  uce_fn=reduce_fn
-000111f0: 290a 2020 2020 2020 2020 2020 7265 7475  ).          retu
-00011200: 726e 2078 0a0a 2020 2020 2020 6d6f 6465  rn x..      mode
-00011210: 6c20 3d20 466f 6f32 2829 0a20 2020 2020  l = Foo2().     
-00011220: 2076 6172 6961 626c 6573 203d 206d 6f64   variables = mod
-00011230: 656c 2e69 6e69 7428 6a61 782e 7261 6e64  el.init(jax.rand
-00011240: 6f6d 2e50 524e 474b 6579 2830 292c 2078  om.PRNGKey(0), x
-00011250: 290a 2020 2020 2020 792c 2073 7461 7465  ).      y, state
-00011260: 203d 206d 6f64 656c 2e61 7070 6c79 2876   = model.apply(v
-00011270: 6172 6961 626c 6573 2c20 6a6e 702e 6f6e  ariables, jnp.on
-00011280: 6573 2828 312c 2031 2929 2c20 6d75 7461  es((1, 1)), muta
-00011290: 626c 653d 5b27 696e 7465 726d 6564 6961  ble=['intermedia
-000112a0: 7465 7327 5d29 0a20 2020 2020 2070 7269  tes']).      pri
-000112b0: 6e74 2873 7461 7465 5b27 696e 7465 726d  nt(state['interm
-000112c0: 6564 6961 7465 7327 5d29 2020 2320 3d3d  ediates'])  # ==
-000112d0: 3e20 7b27 6827 3a20 5b5b 332e 5d5d 7d0a  > {'h': [[3.]]}.
-000112e0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000112f0: 2063 6f6c 3a20 5468 6520 6e61 6d65 206f   col: The name o
-00011300: 6620 7468 6520 7661 7269 6162 6c65 2063  f the variable c
-00011310: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00011320: 206e 616d 653a 2054 6865 206e 616d 6520   name: The name 
-00011330: 6f66 2074 6865 2076 6172 6961 626c 652e  of the variable.
-00011340: 0a20 2020 2020 2076 616c 7565 3a20 5468  .      value: Th
-00011350: 6520 7661 6c75 6520 6f66 2074 6865 2076  e value of the v
-00011360: 6172 6961 626c 652e 0a20 2020 2020 2072  ariable..      r
-00011370: 6564 7563 655f 666e 3a20 5468 6520 6675  educe_fn: The fu
-00011380: 6e63 7469 6f6e 2075 7365 6420 746f 2063  nction used to c
-00011390: 6f6d 6269 6e65 2074 6865 2065 7869 7374  ombine the exist
-000113a0: 696e 6720 7661 6c75 6520 7769 7468 0a20  ing value with. 
-000113b0: 2020 2020 2020 2074 6865 206e 6577 2076         the new v
-000113c0: 616c 7565 2e20 5468 6520 6465 6661 756c  alue. The defaul
-000113d0: 7420 6973 2074 6f20 6170 7065 6e64 2074  t is to append t
-000113e0: 6865 2076 616c 7565 2074 6f20 6120 7475  he value to a tu
-000113f0: 706c 652e 0a20 2020 2020 2069 6e69 745f  ple..      init_
-00011400: 666e 3a20 466f 7220 7468 6520 6669 7273  fn: For the firs
-00011410: 7420 7661 6c75 6520 7374 6f72 6564 2c20  t value stored, 
-00011420: 6072 6564 7563 655f 666e 6020 7769 6c6c  `reduce_fn` will
-00011430: 2062 6520 7061 7373 6564 0a20 2020 2020   be passed.     
-00011440: 2020 2074 6865 2072 6573 756c 7420 6f66     the result of
-00011450: 2060 696e 6974 5f66 6e60 2074 6f67 6574   `init_fn` toget
-00011460: 6865 7220 7769 7468 2074 6865 2076 616c  her with the val
-00011470: 7565 2074 6f20 6265 2073 746f 7265 642e  ue to be stored.
-00011480: 0a20 2020 2020 2020 2054 6865 2064 6566  .        The def
-00011490: 6175 6c74 2069 7320 616e 2065 6d70 7479  ault is an empty
-000114a0: 2074 7570 6c65 2e0a 0a20 2020 2052 6574   tuple...    Ret
-000114b0: 7572 6e73 3a0a 2020 2020 2020 6054 7275  urns:.      `Tru
-000114c0: 6560 2069 6620 7468 6520 7661 6c75 6520  e` if the value 
-000114d0: 6861 7320 6265 656e 2073 746f 7265 6420  has been stored 
-000114e0: 7375 6363 6573 7366 756c 6c79 2c20 6046  successfully, `F
-000114f0: 616c 7365 6020 6f74 6865 7277 6973 652e  alse` otherwise.
-00011500: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00011510: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
-00011520: 6e65 3a0a 2020 2020 2020 7261 6973 6520  ne:.      raise 
-00011530: 5661 6c75 6545 7272 6f72 2822 4361 6e27  ValueError("Can'
-00011540: 7420 7374 6f72 6520 7661 7269 6162 6c65  t store variable
-00011550: 7320 6f6e 2075 6e62 6f75 6e64 206d 6f64  s on unbound mod
-00011560: 756c 6573 2229 0a20 2020 2069 6620 6e6f  ules").    if no
-00011570: 7420 7365 6c66 2e73 636f 7065 2e69 735f  t self.scope.is_
-00011580: 6d75 7461 626c 655f 636f 6c6c 6563 7469  mutable_collecti
-00011590: 6f6e 2863 6f6c 293a 0a20 2020 2020 2072  on(col):.      r
-000115a0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000115b0: 6966 2073 656c 662e 7363 6f70 652e 6861  if self.scope.ha
-000115c0: 735f 7661 7269 6162 6c65 2863 6f6c 2c20  s_variable(col, 
-000115d0: 6e61 6d65 293a 0a20 2020 2020 2078 7320  name):.      xs 
-000115e0: 3d20 7365 6c66 2e73 636f 7065 2e67 6574  = self.scope.get
-000115f0: 5f76 6172 6961 626c 6528 636f 6c2c 206e  _variable(col, n
-00011600: 616d 6529 0a20 2020 2065 6c73 653a 0a20  ame).    else:. 
-00011610: 2020 2020 2073 656c 662e 7363 6f70 652e       self.scope.
-00011620: 7265 7365 7276 6528 6e61 6d65 2c20 636f  reserve(name, co
-00011630: 6c29 0a20 2020 2020 2073 656c 662e 5f73  l).      self._s
-00011640: 7461 7465 2e63 6869 6c64 7265 6e5b 6e61  tate.children[na
-00011650: 6d65 5d20 3d20 636f 6c0a 2020 2020 2020  me] = col.      
-00011660: 7873 203d 2069 6e69 745f 666e 2829 0a20  xs = init_fn(). 
-00011670: 2020 2078 7320 3d20 7265 6475 6365 5f66     xs = reduce_f
-00011680: 6e28 7873 2c20 7661 6c75 6529 0a20 2020  n(xs, value).   
-00011690: 2073 656c 662e 7363 6f70 652e 7075 745f   self.scope.put_
-000116a0: 7661 7269 6162 6c65 2863 6f6c 2c20 6e61  variable(col, na
-000116b0: 6d65 2c20 7873 290a 2020 2020 7265 7475  me, xs).    retu
-000116c0: 726e 2054 7275 650a 0a20 2064 6566 2070  rn True..  def p
-000116d0: 6572 7475 7262 280a 2020 2020 2020 7365  erturb(.      se
-000116e0: 6c66 2c20 6e61 6d65 3a20 7374 722c 2076  lf, name: str, v
-000116f0: 616c 7565 3a20 542c 2063 6f6c 6c65 6374  alue: T, collect
-00011700: 696f 6e3a 2073 7472 203d 2027 7065 7274  ion: str = 'pert
-00011710: 7572 6261 7469 6f6e 7327 0a20 2029 202d  urbations'.  ) -
-00011720: 3e20 543a 0a20 2020 2022 2222 4164 6420  > T:.    """Add 
-00011730: 616e 207a 6572 6f2d 7661 6c75 6520 7661  an zero-value va
-00011740: 7269 6162 6c65 2028 2770 6572 7475 7262  riable ('perturb
-00011750: 6174 696f 6e27 2920 746f 2074 6865 2069  ation') to the i
-00011760: 6e74 6572 6d65 6469 6174 6520 7661 6c75  ntermediate valu
-00011770: 652e 0a0a 2020 2020 5468 6520 6772 6164  e...    The grad
-00011780: 6965 6e74 206f 6620 6076 616c 7565 6020  ient of `value` 
-00011790: 776f 756c 6420 6265 2074 6865 2073 616d  would be the sam
-000117a0: 6520 6173 2074 6865 2067 7261 6469 656e  e as the gradien
-000117b0: 7420 6f66 2074 6869 730a 2020 2020 7065  t of this.    pe
-000117c0: 7274 7572 6261 7469 6f6e 2076 6172 6961  rturbation varia
-000117d0: 626c 652e 2054 6865 7265 666f 7265 2c20  ble. Therefore, 
-000117e0: 6966 2079 6f75 2064 6566 696e 6520 796f  if you define yo
-000117f0: 7572 206c 6f73 7320 6675 6e63 7469 6f6e  ur loss function
-00011800: 2077 6974 680a 2020 2020 626f 7468 2070   with.    both p
-00011810: 6172 616d 7320 616e 6420 7065 7274 7572  arams and pertur
-00011820: 6261 7469 6f6e 7320 6173 2073 7461 6e64  bations as stand
-00011830: 616c 6f6e 6520 6172 6775 6d65 6e74 732c  alone arguments,
-00011840: 2079 6f75 2063 616e 2067 6574 2074 6865   you can get the
-00011850: 0a20 2020 2069 6e74 6572 6d65 6469 6174  .    intermediat
-00011860: 6520 6772 6164 6965 6e74 7320 6f66 2060  e gradients of `
-00011870: 7661 6c75 6560 2062 7920 7275 6e6e 696e  value` by runnin
-00011880: 6720 606a 6178 2e67 7261 6460 206f 6e20  g `jax.grad` on 
-00011890: 7468 6520 7065 7274 7572 6261 7469 6f6e  the perturbation
-000118a0: 0a20 2020 2061 7267 756d 656e 742e 0a0a  .    argument...
-000118b0: 2020 2020 4e6f 7465 3a20 7468 6973 2069      Note: this i
-000118c0: 7320 616e 2065 7870 6572 696d 656e 7461  s an experimenta
-000118d0: 6c20 4150 4920 616e 6420 6d61 7920 6265  l API and may be
-000118e0: 2074 7765 616b 6564 206c 6174 6572 2066   tweaked later f
-000118f0: 6f72 2062 6574 7465 720a 2020 2020 7065  or better.    pe
-00011900: 7266 6f72 6d61 6e63 6520 616e 6420 7573  rformance and us
-00011910: 6162 696c 6974 792e 0a20 2020 2041 7420  ability..    At 
-00011920: 6974 7320 6375 7272 656e 7420 7374 6167  its current stag
-00011930: 652c 2069 7420 6372 6561 7465 7320 6578  e, it creates ex
-00011940: 7472 6120 6475 6d6d 7920 7661 7269 6162  tra dummy variab
-00011950: 6c65 7320 7468 6174 206f 6363 7570 6965  les that occupie
-00011960: 7320 6578 7472 610a 2020 2020 6d65 6d6f  s extra.    memo
-00011970: 7279 2073 7061 6365 2e20 5573 6520 6974  ry space. Use it
-00011980: 206f 6e6c 7920 746f 2064 6562 7567 2067   only to debug g
-00011990: 7261 6469 656e 7473 2069 6e20 7472 6169  radients in trai
-000119a0: 6e69 6e67 2e0a 0a20 2020 2045 7861 6d70  ning...    Examp
-000119b0: 6c65 3a3a 0a0a 2020 2020 2020 696d 706f  le::..      impo
-000119c0: 7274 206a 6178 0a20 2020 2020 2069 6d70  rt jax.      imp
-000119d0: 6f72 7420 6a61 782e 6e75 6d70 7920 6173  ort jax.numpy as
-000119e0: 206a 6e70 0a20 2020 2020 2069 6d70 6f72   jnp.      impor
-000119f0: 7420 666c 6178 2e6c 696e 656e 2061 7320  t flax.linen as 
-00011a00: 6e6e 0a0a 2020 2020 2020 636c 6173 7320  nn..      class 
-00011a10: 466f 6f28 6e6e 2e4d 6f64 756c 6529 3a0a  Foo(nn.Module):.
-00011a20: 2020 2020 2020 2020 2020 406e 6e2e 636f            @nn.co
-00011a30: 6d70 6163 740a 2020 2020 2020 2020 2020  mpact.          
-00011a40: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00011a50: 662c 2078 293a 0a20 2020 2020 2020 2020  f, x):.         
-00011a60: 2020 2020 2078 203d 206e 6e2e 4465 6e73       x = nn.Dens
-00011a70: 6528 3329 2878 290a 2020 2020 2020 2020  e(3)(x).        
-00011a80: 2020 2020 2020 7820 3d20 7365 6c66 2e70        x = self.p
-00011a90: 6572 7475 7262 2827 6465 6e73 6533 272c  erturb('dense3',
-00011aa0: 2078 290a 2020 2020 2020 2020 2020 2020   x).            
-00011ab0: 2020 7265 7475 726e 206e 6e2e 4465 6e73    return nn.Dens
-00011ac0: 6528 3229 2878 290a 0a20 2020 2020 2064  e(2)(x)..      d
-00011ad0: 6566 206c 6f73 7328 7061 7261 6d73 2c20  ef loss(params, 
-00011ae0: 7065 7274 7572 6261 7469 6f6e 732c 2069  perturbations, i
-00011af0: 6e70 7574 732c 2074 6172 6765 7473 293a  nputs, targets):
-00011b00: 0a20 2020 2020 2020 2076 6172 6961 626c  .        variabl
-00011b10: 6573 203d 207b 2770 6172 616d 7327 3a20  es = {'params': 
-00011b20: 7061 7261 6d73 2c20 2770 6572 7475 7262  params, 'perturb
-00011b30: 6174 696f 6e73 273a 2070 6572 7475 7262  ations': perturb
-00011b40: 6174 696f 6e73 7d0a 2020 2020 2020 2020  ations}.        
-00011b50: 7072 6564 7320 3d20 6d6f 6465 6c2e 6170  preds = model.ap
-00011b60: 706c 7928 7661 7269 6162 6c65 732c 2069  ply(variables, i
-00011b70: 6e70 7574 7329 0a20 2020 2020 2020 2072  nputs).        r
-00011b80: 6574 7572 6e20 6a6e 702e 7371 7561 7265  eturn jnp.square
-00011b90: 2870 7265 6473 202d 2074 6172 6765 7473  (preds - targets
-00011ba0: 292e 6d65 616e 2829 0a0a 2020 2020 2020  ).mean()..      
-00011bb0: 7820 3d20 6a6e 702e 6f6e 6573 2828 322c  x = jnp.ones((2,
-00011bc0: 2039 2929 0a20 2020 2020 2079 203d 206a   9)).      y = j
-00011bd0: 6e70 2e6f 6e65 7328 2832 2c20 3229 290a  np.ones((2, 2)).
-00011be0: 2020 2020 2020 6d6f 6465 6c20 3d20 466f        model = Fo
-00011bf0: 6f28 290a 2020 2020 2020 7661 7269 6162  o().      variab
-00011c00: 6c65 7320 3d20 6d6f 6465 6c2e 696e 6974  les = model.init
-00011c10: 286a 6178 2e72 616e 646f 6d2e 5052 4e47  (jax.random.PRNG
-00011c20: 4b65 7928 3029 2c20 7829 0a20 2020 2020  Key(0), x).     
-00011c30: 2069 6e74 6d5f 6772 6164 7320 3d20 6a61   intm_grads = ja
-00011c40: 782e 6772 6164 286c 6f73 732c 2061 7267  x.grad(loss, arg
-00011c50: 6e75 6d73 3d31 2928 7661 7269 6162 6c65  nums=1)(variable
-00011c60: 735b 2770 6172 616d 7327 5d2c 2076 6172  s['params'], var
-00011c70: 6961 626c 6573 5b27 7065 7274 7572 6261  iables['perturba
-00011c80: 7469 6f6e 7327 5d2c 2078 2c20 7929 0a20  tions'], x, y). 
-00011c90: 2020 2020 2070 7269 6e74 2869 6e74 6d5f       print(intm_
-00011ca0: 6772 6164 735b 2764 656e 7365 3327 5d29  grads['dense3'])
-00011cb0: 2023 203d 3d3e 205b 5b2d 312e 3435 3639   # ==> [[-1.4569
-00011cc0: 3234 2020 202d 302e 3434 3333 3235 3337  24   -0.44332537
-00011cd0: 2020 302e 3032 3432 3238 3437 5d0a 2020    0.02422847].  
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d00: 2320 2020 2020 205b 2d31 2e34 3536 3932  #      [-1.45692
-00011d10: 3420 2020 2d30 2e34 3433 3332 3533 3720  4   -0.44332537 
-00011d20: 2030 2e30 3234 3232 3834 375d 5d0a 0a20   0.02422847]].. 
-00011d30: 2020 2049 6620 7065 7274 7572 6261 7469     If perturbati
-00011d40: 6f6e 7320 6172 6520 6e6f 7420 7061 7373  ons are not pass
-00011d50: 6564 2074 6f20 6061 7070 6c79 602c 2060  ed to `apply`, `
-00011d60: 7065 7274 7572 6260 2062 6568 6176 6573  perturb` behaves
-00011d70: 206c 696b 6520 6120 6e6f 2d6f 700a 2020   like a no-op.  
-00011d80: 2020 736f 2079 6f75 2063 616e 2065 6173    so you can eas
-00011d90: 696c 7920 6469 7361 626c 6520 7468 6520  ily disable the 
-00011da0: 6265 6861 7669 6f72 2077 6865 6e20 6e6f  behavior when no
-00011db0: 7420 6e65 6564 6564 3a3a 0a0a 2020 2020  t needed::..    
-00011dc0: 2020 6d6f 6465 6c2e 6170 706c 7928 7b27    model.apply({'
-00011dd0: 7061 7261 6d73 273a 2070 6172 616d 732c  params': params,
-00011de0: 2027 7065 7274 7572 6261 7469 6f6e 7327   'perturbations'
-00011df0: 3a20 7065 7274 7572 6261 7469 6f6e 737d  : perturbations}
-00011e00: 2c20 7829 2023 2077 6f72 6b73 2061 7320  , x) # works as 
-00011e10: 6578 7065 6374 6564 0a20 2020 2020 206d  expected.      m
-00011e20: 6f64 656c 2e61 7070 6c79 287b 2770 6172  odel.apply({'par
-00011e30: 616d 7327 3a20 7061 7261 6d73 7d2c 2078  ams': params}, x
-00011e40: 2920 2320 6265 6861 7665 7320 6c69 6b65  ) # behaves like
-00011e50: 2061 206e 6f2d 6f70 0a0a 2020 2020 2222   a no-op..    ""
-00011e60: 220a 0a20 2020 2064 6566 205f 726f 6f74  "..    def _root
-00011e70: 5f68 6173 5f63 6f6c 6c65 6374 696f 6e28  _has_collection(
-00011e80: 293a 0a20 2020 2020 2022 2222 5265 7475  ):.      """Retu
-00011e90: 726e 7320 5472 7565 2069 6620 7468 6520  rns True if the 
-00011ea0: 726f 6f74 2073 636f 7065 2068 6173 2074  root scope has t
-00011eb0: 6865 2063 6f6c 6c65 6374 696f 6e2e 2222  he collection.""
-00011ec0: 220a 2020 2020 2020 6173 7365 7274 2073  ".      assert s
-00011ed0: 656c 662e 7363 6f70 6520 6973 206e 6f74  elf.scope is not
-00011ee0: 204e 6f6e 650a 2020 2020 2020 7265 7475   None.      retu
-00011ef0: 726e 2063 6f6c 6c65 6374 696f 6e20 696e  rn collection in
-00011f00: 2073 656c 662e 7363 6f70 652e 726f 6f74   self.scope.root
-00011f10: 2e5f 7661 7269 6162 6c65 730a 0a20 2020  ._variables..   
-00011f20: 2023 2077 6520 7769 6c6c 206f 6e6c 7920   # we will only 
-00011f30: 6164 6420 7468 6520 7065 7274 7572 6261  add the perturba
-00011f40: 7469 6f6e 2076 6172 6961 626c 6520 6966  tion variable if
-00011f50: 2074 6865 2063 6f6c 6c65 6374 696f 6e20   the collection 
-00011f60: 6973 206d 7574 6162 6c65 0a20 2020 2023  is mutable.    #
-00011f70: 2028 652e 672e 2064 7572 696e 6720 6069   (e.g. during `i
-00011f80: 6e69 7460 2920 6f72 2069 6620 7468 6520  nit`) or if the 
-00011f90: 636f 6c6c 6563 7469 6f6e 2077 6173 2070  collection was p
-00011fa0: 6173 7365 6420 746f 2060 6170 706c 7960  assed to `apply`
-00011fb0: 2028 636f 6e74 6169 6e65 6420 696e 0a20   (contained in. 
-00011fc0: 2020 2023 2074 6865 2072 6f6f 7420 7363     # the root sc
-00011fd0: 6f70 6529 2e0a 2020 2020 6966 2073 656c  ope)..    if sel
-00011fe0: 662e 6973 5f6d 7574 6162 6c65 5f63 6f6c  f.is_mutable_col
-00011ff0: 6c65 6374 696f 6e28 636f 6c6c 6563 7469  lection(collecti
-00012000: 6f6e 2920 6f72 205f 726f 6f74 5f68 6173  on) or _root_has
-00012010: 5f63 6f6c 6c65 6374 696f 6e28 293a 0a20  _collection():. 
-00012020: 2020 2020 2076 616c 7565 202b 3d20 7365       value += se
-00012030: 6c66 2e76 6172 6961 626c 6528 636f 6c6c  lf.variable(coll
-00012040: 6563 7469 6f6e 2c20 6e61 6d65 2c20 6c61  ection, name, la
-00012050: 6d62 6461 3a20 6a6e 702e 7a65 726f 735f  mbda: jnp.zeros_
-00012060: 6c69 6b65 2876 616c 7565 2929 2e76 616c  like(value)).val
-00012070: 7565 2020 2320 7479 7065 3a20 6967 6e6f  ue  # type: igno
-00012080: 7265 0a20 2020 2072 6574 7572 6e20 7661  re.    return va
-00012090: 6c75 650a 0a20 2064 6566 2074 6162 756c  lue..  def tabul
-000120a0: 6174 6528 0a20 2020 2020 2073 656c 662c  ate(.      self,
-000120b0: 0a20 2020 2020 2072 6e67 733a 2055 6e69  .      rngs: Uni
-000120c0: 6f6e 5b4b 6579 4172 7261 792c 2052 4e47  on[KeyArray, RNG
-000120d0: 5365 7175 656e 6365 735d 2c0a 2020 2020  Sequences],.    
-000120e0: 2020 2a61 7267 732c 0a20 2020 2020 2064    *args,.      d
-000120f0: 6570 7468 3a20 4f70 7469 6f6e 616c 5b69  epth: Optional[i
-00012100: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-00012110: 2020 7368 6f77 5f72 6570 6561 7465 643a    show_repeated:
-00012120: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00012130: 2020 2020 206d 7574 6162 6c65 3a20 436f       mutable: Co
-00012140: 6c6c 6563 7469 6f6e 4669 6c74 6572 203d  llectionFilter =
-00012150: 2054 7275 652c 0a20 2020 2020 2063 6f6e   True,.      con
-00012160: 736f 6c65 5f6b 7761 7267 733a 204f 7074  sole_kwargs: Opt
-00012170: 696f 6e61 6c5b 4d61 7070 696e 675b 7374  ional[Mapping[st
-00012180: 722c 2041 6e79 5d5d 203d 204e 6f6e 652c  r, Any]] = None,
-00012190: 0a20 2020 2020 2074 6162 6c65 5f6b 7761  .      table_kwa
-000121a0: 7267 733a 204d 6170 7069 6e67 5b73 7472  rgs: Mapping[str
-000121b0: 2c20 416e 795d 203d 204d 6170 7069 6e67  , Any] = Mapping
-000121c0: 5072 6f78 7954 7970 6528 7b7d 292c 0a20  ProxyType({}),. 
-000121d0: 2020 2020 2063 6f6c 756d 6e5f 6b77 6172       column_kwar
-000121e0: 6773 3a20 4d61 7070 696e 675b 7374 722c  gs: Mapping[str,
-000121f0: 2041 6e79 5d20 3d20 4d61 7070 696e 6750   Any] = MappingP
-00012200: 726f 7879 5479 7065 287b 7d29 2c0a 2020  roxyType({}),.  
-00012210: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
-00012220: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-00012230: 2243 7265 6174 6573 2061 2073 756d 6d61  "Creates a summa
-00012240: 7279 206f 6620 7468 6520 4d6f 6475 6c65  ry of the Module
-00012250: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
-00012260: 6120 7461 626c 652e 0a0a 2020 2020 5468  a table...    Th
-00012270: 6973 206d 6574 686f 6420 6861 7320 7468  is method has th
-00012280: 6520 7361 6d65 2073 6967 6e61 7475 7265  e same signature
-00012290: 2061 6e64 2069 6e74 6572 6e61 6c6c 7920   and internally 
-000122a0: 6361 6c6c 7320 604d 6f64 756c 652e 696e  calls `Module.in
-000122b0: 6974 602c 0a20 2020 2062 7574 2069 6e73  it`,.    but ins
-000122c0: 7465 6164 206f 6620 7265 7475 726e 696e  tead of returnin
-000122d0: 6720 7468 6520 7661 7269 6162 6c65 732c  g the variables,
-000122e0: 2069 7420 7265 7475 726e 7320 7468 6520   it returns the 
-000122f0: 7374 7269 6e67 2073 756d 6d61 7269 7a69  string summarizi
-00012300: 6e67 0a20 2020 2074 6865 204d 6f64 756c  ng.    the Modul
-00012310: 6520 696e 2061 2074 6162 6c65 2e20 6074  e in a table. `t
-00012320: 6162 756c 6174 6560 2075 7365 7320 606a  abulate` uses `j
-00012330: 6178 2e65 7661 6c5f 7368 6170 6560 2074  ax.eval_shape` t
-00012340: 6f20 7275 6e20 7468 6520 666f 7277 6172  o run the forwar
-00012350: 640a 2020 2020 636f 6d70 7574 6174 696f  d.    computatio
-00012360: 6e20 7769 7468 6f75 7420 636f 6e73 756d  n without consum
-00012370: 696e 6720 616e 7920 464c 4f50 7320 6f72  ing any FLOPs or
-00012380: 2061 6c6c 6f63 6174 696e 6720 6d65 6d6f   allocating memo
-00012390: 7279 2e0a 0a20 2020 2041 6464 6974 696f  ry...    Additio
-000123a0: 6e61 6c20 6172 6775 6d65 6e74 7320 6361  nal arguments ca
-000123b0: 6e20 6265 2070 6173 7365 6420 696e 746f  n be passed into
-000123c0: 2074 6865 2060 636f 6e73 6f6c 655f 6b77   the `console_kw
-000123d0: 6172 6773 6020 6172 6775 6d65 6e74 2c20  args` argument, 
-000123e0: 666f 7220 6578 616d 706c 652c 0a20 2020  for example,.   
-000123f0: 2060 7b27 7769 6474 6827 3a20 3132 307d   `{'width': 120}
-00012400: 602e 2046 6f72 2061 2066 756c 6c20 6c69  `. For a full li
-00012410: 7374 206f 6620 6063 6f6e 736f 6c65 5f6b  st of `console_k
-00012420: 7761 7267 7360 2061 7267 756d 656e 7473  wargs` arguments
-00012430: 2c20 7365 653a 0a20 2020 2068 7474 7073  , see:.    https
-00012440: 3a2f 2f72 6963 682e 7265 6164 7468 6564  ://rich.readthed
-00012450: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-00012460: 2f72 6566 6572 656e 6365 2f63 6f6e 736f  /reference/conso
-00012470: 6c65 2e68 746d 6c23 7269 6368 2e63 6f6e  le.html#rich.con
-00012480: 736f 6c65 2e43 6f6e 736f 6c65 0a0a 2020  sole.Console..  
-00012490: 2020 4578 616d 706c 653a 3a0a 0a20 2020    Example::..   
-000124a0: 2020 2069 6d70 6f72 7420 6a61 780a 2020     import jax.  
-000124b0: 2020 2020 696d 706f 7274 206a 6178 2e6e      import jax.n
-000124c0: 756d 7079 2061 7320 6a6e 700a 2020 2020  umpy as jnp.    
-000124d0: 2020 696d 706f 7274 2066 6c61 782e 6c69    import flax.li
-000124e0: 6e65 6e20 6173 206e 6e0a 0a20 2020 2020  nen as nn..     
-000124f0: 2063 6c61 7373 2046 6f6f 286e 6e2e 4d6f   class Foo(nn.Mo
-00012500: 6475 6c65 293a 0a20 2020 2020 2020 2020  dule):.         
-00012510: 2040 6e6e 2e63 6f6d 7061 6374 0a20 2020   @nn.compact.   
-00012520: 2020 2020 2020 2064 6566 205f 5f63 616c         def __cal
-00012530: 6c5f 5f28 7365 6c66 2c20 7829 3a0a 2020  l__(self, x):.  
-00012540: 2020 2020 2020 2020 2020 2020 6820 3d20              h = 
-00012550: 6e6e 2e44 656e 7365 2834 2928 7829 0a20  nn.Dense(4)(x). 
-00012560: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012570: 7572 6e20 6e6e 2e44 656e 7365 2832 2928  urn nn.Dense(2)(
-00012580: 6829 0a0a 2020 2020 2020 7820 3d20 6a6e  h)..      x = jn
-00012590: 702e 6f6e 6573 2828 3136 2c20 3929 290a  p.ones((16, 9)).
-000125a0: 0a20 2020 2020 2070 7269 6e74 2846 6f6f  .      print(Foo
-000125b0: 2829 2e74 6162 756c 6174 6528 6a61 782e  ().tabulate(jax.
-000125c0: 7261 6e64 6f6d 2e50 524e 474b 6579 2830  random.PRNGKey(0
-000125d0: 292c 2078 2929 0a0a 0a20 2020 2054 6869  ), x))...    Thi
-000125e0: 7320 6769 7665 7320 7468 6520 666f 6c6c  s gives the foll
-000125f0: 6f77 696e 6720 6f75 7470 7574 3a3a 0a0a  owing output::..
-00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012620: 2020 2020 2020 466f 6f20 5375 6d6d 6172        Foo Summar
-00012630: 790a 2020 2020 2020 e294 8fe2 9481 e294  y.      ........
-00012640: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00012650: e294 81e2 9481 e294 b3e2 9481 e294 81e2  ................
-00012660: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00012670: 81e2 94b3 e294 81e2 9481 e294 81e2 9481  ................
-00012680: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00012690: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000126a0: 81e2 94b3 e294 81e2 9481 e294 81e2 9481  ................
-000126b0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-000126c0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000126d0: 81e2 94b3 e294 81e2 9481 e294 81e2 9481  ................
-000126e0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-000126f0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00012700: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00012710: e294 81e2 9481 e294 930a 2020 2020 2020  ..........      
-00012720: e294 8320 7061 7468 2020 2020 e294 8320  ... path    ... 
-00012730: 6d6f 6475 6c65 20e2 9483 2069 6e70 7574  module ... input
-00012740: 7320 2020 2020 2020 20e2 9483 206f 7574  s        ... out
-00012750: 7075 7473 2020 2020 2020 20e2 9483 2070  puts       ... p
-00012760: 6172 616d 7320 2020 2020 2020 2020 2020  arams           
-00012770: 2020 2020 e294 830a 2020 2020 2020 e294      ....      ..
-00012780: a1e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00012790: e294 81e2 9481 e294 81e2 9481 e295 87e2  ................
-000127a0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000127b0: 81e2 9481 e294 81e2 9587 e294 81e2 9481  ................
-000127c0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-000127d0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-000127e0: 81e2 9481 e294 81e2 9587 e294 81e2 9481  ................
-000127f0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00012800: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00012810: 81e2 9481 e294 81e2 9587 e294 81e2 9481  ................
-00012820: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00012830: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00012840: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00012850: e294 81e2 9481 e294 81e2 9481 e294 a90a  ................
-00012860: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00012870: 2020 e294 8220 466f 6f20 2020 20e2 9482    ... Foo    ...
-00012880: 2066 6c6f 6174 3332 5b31 362c 395d 20e2   float32[16,9] .
-00012890: 9482 2066 6c6f 6174 3332 5b31 362c 325d  .. float32[16,2]
-000128a0: 20e2 9482 2020 2020 2020 2020 2020 2020   ...            
-000128b0: 2020 2020 2020 2020 2020 e294 820a 2020            ....  
-000128c0: 2020 2020 e294 9ce2 9480 e294 80e2 9480      ............
-000128d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000128e0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-000128f0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012920: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012940: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012950: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012990: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000129a0: 9480 e294 a40a 2020 2020 2020 e294 8220  ......      ... 
-000129b0: 4465 6e73 655f 3020 e294 8220 4465 6e73  Dense_0 ... Dens
-000129c0: 6520 20e2 9482 2066 6c6f 6174 3332 5b31  e  ... float32[1
-000129d0: 362c 395d 20e2 9482 2066 6c6f 6174 3332  6,9] ... float32
-000129e0: 5b31 362c 345d 20e2 9482 2062 6961 733a  [16,4] ... bias:
-000129f0: 2066 6c6f 6174 3332 5b34 5d20 2020 2020   float32[4]     
-00012a00: e294 820a 2020 2020 2020 e294 8220 2020  ....      ...   
-00012a10: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00012a20: 20e2 9482 2020 2020 2020 2020 2020 2020   ...            
-00012a30: 2020 20e2 9482 2020 2020 2020 2020 2020     ...          
-00012a40: 2020 2020 20e2 9482 206b 6572 6e65 6c3a       ... kernel:
-00012a50: 2066 6c6f 6174 3332 5b39 2c34 5d20 e294   float32[9,4] ..
-00012a60: 820a 2020 2020 2020 e294 8220 2020 2020  ..      ...     
-00012a70: 2020 2020 e294 8220 2020 2020 2020 20e2      ...        .
-00012a80: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00012a90: 20e2 9482 2020 2020 2020 2020 2020 2020   ...            
-00012aa0: 2020 20e2 9482 2020 2020 2020 2020 2020     ...          
-00012ab0: 2020 2020 2020 2020 2020 2020 e294 820a              ....
-00012ac0: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00012ad0: 2020 e294 8220 2020 2020 2020 20e2 9482    ...        ...
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00012af0: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00012b00: 20e2 9482 2034 3020 2831 3630 2042 2920   ... 40 (160 B) 
-00012b10: 2020 2020 2020 2020 2020 e294 820a 2020            ....  
-00012b20: 2020 2020 e294 9ce2 9480 e294 80e2 9480      ............
-00012b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012b40: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00012b50: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012b80: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012b90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012ba0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012bb0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012bc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012bd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012be0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012bf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012c00: 9480 e294 a40a 2020 2020 2020 e294 8220  ......      ... 
-00012c10: 4465 6e73 655f 3120 e294 8220 4465 6e73  Dense_1 ... Dens
-00012c20: 6520 20e2 9482 2066 6c6f 6174 3332 5b31  e  ... float32[1
-00012c30: 362c 345d 20e2 9482 2066 6c6f 6174 3332  6,4] ... float32
-00012c40: 5b31 362c 325d 20e2 9482 2062 6961 733a  [16,2] ... bias:
-00012c50: 2066 6c6f 6174 3332 5b32 5d20 2020 2020   float32[2]     
-00012c60: e294 820a 2020 2020 2020 e294 8220 2020  ....      ...   
-00012c70: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00012c80: 20e2 9482 2020 2020 2020 2020 2020 2020   ...            
-00012c90: 2020 20e2 9482 2020 2020 2020 2020 2020     ...          
-00012ca0: 2020 2020 20e2 9482 206b 6572 6e65 6c3a       ... kernel:
-00012cb0: 2066 6c6f 6174 3332 5b34 2c32 5d20 e294   float32[4,2] ..
-00012cc0: 820a 2020 2020 2020 e294 8220 2020 2020  ..      ...     
-00012cd0: 2020 2020 e294 8220 2020 2020 2020 20e2      ...        .
-00012ce0: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00012cf0: 20e2 9482 2020 2020 2020 2020 2020 2020   ...            
-00012d00: 2020 20e2 9482 2020 2020 2020 2020 2020     ...          
-00012d10: 2020 2020 2020 2020 2020 2020 e294 820a              ....
-00012d20: 2020 2020 2020 e294 8220 2020 2020 2020        ...       
-00012d30: 2020 e294 8220 2020 2020 2020 20e2 9482    ...        ...
-00012d40: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00012d50: 9482 2020 2020 2020 2020 2020 2020 2020  ..              
-00012d60: 20e2 9482 2031 3020 2834 3020 4229 2020   ... 10 (40 B)  
-00012d70: 2020 2020 2020 2020 2020 e294 820a 2020            ....  
-00012d80: 2020 2020 e294 9ce2 9480 e294 80e2 9480      ............
-00012d90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012da0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00012db0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012de0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012df0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012e00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012e10: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00012e20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012e30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012e40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012e50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012e60: 9480 e294 a40a 2020 2020 2020 e294 8220  ......      ... 
-00012e70: 2020 2020 2020 2020 e294 8220 2020 2020          ...     
-00012e80: 2020 20e2 9482 2020 2020 2020 2020 2020     ...          
-00012e90: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
-00012ea0: 2054 6f74 616c 20e2 9482 2035 3020 2832   Total ... 50 (2
-00012eb0: 3030 2042 2920 2020 2020 2020 2020 2020  00 B)           
-00012ec0: e294 820a 2020 2020 2020 e294 94e2 9480  ....      ......
-00012ed0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012ee0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
-00012ef0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012f00: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-00012f10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012f20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012f30: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-00012f40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012f50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012f60: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-00012f70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00012f80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00012f90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00012fa0: 9480 e294 80e2 9480 e294 980a 0a20 2020  .............   
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 2020 2020 2020 2020 2054 6f74 616c 2050           Total P
-00012fd0: 6172 616d 6574 6572 733a 2035 3020 2832  arameters: 50 (2
-00012fe0: 3030 2042 290a 0a20 2020 202a 2a4e 6f74  00 B)..    **Not
-00012ff0: 652a 2a3a 2072 6f77 7320 6f72 6465 7220  e**: rows order 
-00013000: 696e 2074 6865 2074 6162 6c65 2064 6f65  in the table doe
-00013010: 7320 6e6f 7420 7265 7072 6573 656e 7420  s not represent 
-00013020: 6578 6563 7574 696f 6e20 6f72 6465 722c  execution order,
-00013030: 0a20 2020 2069 6e73 7465 6164 2069 7420  .    instead it 
-00013040: 616c 6967 6e73 2077 6974 6820 7468 6520  aligns with the 
-00013050: 6f72 6465 7220 6f66 206b 6579 7320 696e  order of keys in
-00013060: 2060 7661 7269 6162 6c65 7360 2077 6869   `variables` whi
-00013070: 6368 2061 7265 2073 6f72 7465 640a 2020  ch are sorted.  
-00013080: 2020 616c 7068 6162 6574 6963 616c 6c79    alphabetically
-00013090: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-000130a0: 2020 2072 6e67 733a 2054 6865 2072 6e67     rngs: The rng
-000130b0: 7320 666f 7220 7468 6520 7661 7269 6162  s for the variab
-000130c0: 6c65 2063 6f6c 6c65 6374 696f 6e73 2061  le collections a
-000130d0: 7320 7061 7373 6564 2074 6f20 604d 6f64  s passed to `Mod
-000130e0: 756c 652e 696e 6974 602e 0a20 2020 2020  ule.init`..     
-000130f0: 202a 6172 6773 3a20 5468 6520 6172 6775   *args: The argu
-00013100: 6d65 6e74 7320 746f 2074 6865 2066 6f72  ments to the for
-00013110: 7761 7264 2063 6f6d 7075 7461 7469 6f6e  ward computation
-00013120: 2e0a 2020 2020 2020 6465 7074 683a 2063  ..      depth: c
-00013130: 6f6e 7472 6f6c 7320 686f 7720 6d61 6e79  ontrols how many
-00013140: 2073 7562 6d6f 6475 6c65 2064 6565 7020   submodule deep 
-00013150: 7468 6520 7375 6d6d 6172 7920 6361 6e20  the summary can 
-00013160: 676f 2e20 4279 2064 6566 6175 6c74 2069  go. By default i
-00013170: 7473 0a20 2020 2020 2020 2060 4e6f 6e65  ts.        `None
-00013180: 6020 7768 6963 6820 6d65 616e 7320 6e6f  ` which means no
-00013190: 206c 696d 6974 2e20 4966 2061 2073 7562   limit. If a sub
-000131a0: 6d6f 6475 6c65 2069 7320 6e6f 7420 7368  module is not sh
-000131b0: 6f77 6e20 6265 6361 7573 6520 6f66 2074  own because of t
-000131c0: 6865 0a20 2020 2020 2020 2064 6570 7468  he.        depth
-000131d0: 206c 696d 6974 2c20 6974 7320 7061 7261   limit, its para
-000131e0: 6d65 7465 7220 636f 756e 7420 616e 6420  meter count and 
-000131f0: 6279 7465 7320 7769 6c6c 2062 6520 6164  bytes will be ad
-00013200: 6465 6420 746f 2074 6865 2072 6f77 206f  ded to the row o
-00013210: 6620 6974 730a 2020 2020 2020 2020 6669  f its.        fi
-00013220: 7273 7420 7368 6f77 6e20 616e 6365 7374  rst shown ancest
-00013230: 6f72 2073 7563 6820 7468 6174 2074 6865  or such that the
-00013240: 2073 756d 206f 6620 616c 6c20 726f 7773   sum of all rows
-00013250: 2061 6c77 6179 7320 6164 6473 2075 7020   always adds up 
-00013260: 746f 2074 6865 0a20 2020 2020 2020 2074  to the.        t
-00013270: 6f74 616c 206e 756d 6265 7220 6f66 2070  otal number of p
-00013280: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
-00013290: 204d 6f64 756c 652e 0a20 2020 2020 2073   Module..      s
-000132a0: 686f 775f 7265 7065 6174 6564 3a20 4966  how_repeated: If
-000132b0: 2060 5472 7565 602c 2072 6570 6561 7465   `True`, repeate
-000132c0: 6420 6361 6c6c 7320 746f 2074 6865 2073  d calls to the s
-000132d0: 616d 6520 6d6f 6475 6c65 2077 696c 6c20  ame module will 
-000132e0: 6265 2073 686f 776e 0a20 2020 2020 2020  be shown.       
-000132f0: 2069 6e20 7468 6520 7461 626c 652c 206f   in the table, o
-00013300: 7468 6572 7769 7365 206f 6e6c 7920 7468  therwise only th
-00013310: 6520 6669 7273 7420 6361 6c6c 2077 696c  e first call wil
-00013320: 6c20 6265 2073 686f 776e 2e20 4465 6661  l be shown. Defa
-00013330: 756c 7420 6973 0a20 2020 2020 2020 2060  ult is.        `
-00013340: 4661 6c73 6560 2e0a 2020 2020 2020 6d75  False`..      mu
-00013350: 7461 626c 653a 2043 616e 2062 6520 626f  table: Can be bo
-00013360: 6f6c 2c20 7374 722c 206f 7220 6c69 7374  ol, str, or list
-00013370: 2e20 5370 6563 6966 6965 7320 7768 6963  . Specifies whic
-00013380: 6820 636f 6c6c 6563 7469 6f6e 7320 7368  h collections sh
-00013390: 6f75 6c64 2062 650a 2020 2020 2020 2020  ould be.        
-000133a0: 7472 6561 7465 6420 6173 206d 7574 6162  treated as mutab
-000133b0: 6c65 3a20 6060 626f 6f6c 6060 3a20 616c  le: ``bool``: al
-000133c0: 6c2f 6e6f 2063 6f6c 6c65 6374 696f 6e73  l/no collections
-000133d0: 2061 7265 206d 7574 6162 6c65 2e20 6060   are mutable. ``
-000133e0: 7374 7260 603a 2054 6865 0a20 2020 2020  str``: The.     
-000133f0: 2020 206e 616d 6520 6f66 2061 2073 696e     name of a sin
-00013400: 676c 6520 6d75 7461 626c 6520 636f 6c6c  gle mutable coll
-00013410: 6563 7469 6f6e 2e20 6060 6c69 7374 6060  ection. ``list``
-00013420: 3a20 4120 6c69 7374 206f 6620 6e61 6d65  : A list of name
-00013430: 7320 6f66 206d 7574 6162 6c65 0a20 2020  s of mutable.   
-00013440: 2020 2020 2063 6f6c 6c65 6374 696f 6e73       collections
-00013450: 2e20 4279 2064 6566 6175 6c74 2061 6c6c  . By default all
-00013460: 2063 6f6c 6c65 6374 696f 6e73 2065 7863   collections exc
-00013470: 6570 7420 2769 6e74 6572 6d65 6469 6174  ept 'intermediat
-00013480: 6573 2720 6172 650a 2020 2020 2020 2020  es' are.        
-00013490: 6d75 7461 626c 652e 0a20 2020 2020 2063  mutable..      c
-000134a0: 6f6e 736f 6c65 5f6b 7761 7267 733a 2041  onsole_kwargs: A
-000134b0: 6e20 6f70 7469 6f6e 616c 2064 6963 7469  n optional dicti
-000134c0: 6f6e 6172 7920 7769 7468 2061 6464 6974  onary with addit
-000134d0: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
-000134e0: 6775 6d65 6e74 7320 7468 6174 0a20 2020  guments that.   
-000134f0: 2020 2020 2061 7265 2070 6173 7365 6420       are passed 
-00013500: 746f 2060 7269 6368 2e63 6f6e 736f 6c65  to `rich.console
-00013510: 2e43 6f6e 736f 6c65 6020 7768 656e 2072  .Console` when r
-00013520: 656e 6465 7269 6e67 2074 6865 2074 6162  endering the tab
-00013530: 6c65 2e20 4465 6661 756c 7420 6172 6775  le. Default argu
-00013540: 6d65 6e74 730a 2020 2020 2020 2020 6172  ments.        ar
-00013550: 6520 607b 2766 6f72 6365 5f74 6572 6d69  e `{'force_termi
-00013560: 6e61 6c27 3a20 5472 7565 2c20 2766 6f72  nal': True, 'for
-00013570: 6365 5f6a 7570 7974 6572 273a 2046 616c  ce_jupyter': Fal
-00013580: 7365 7d60 2e0a 2020 2020 2020 7461 626c  se}`..      tabl
-00013590: 655f 6b77 6172 6773 3a20 416e 206f 7074  e_kwargs: An opt
-000135a0: 696f 6e61 6c20 6469 6374 696f 6e61 7279  ional dictionary
-000135b0: 2077 6974 6820 6164 6469 7469 6f6e 616c   with additional
-000135c0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-000135d0: 7473 2074 6861 740a 2020 2020 2020 2020  ts that.        
-000135e0: 6172 6520 7061 7373 6564 2074 6f20 6072  are passed to `r
-000135f0: 6963 682e 7461 626c 652e 5461 626c 6560  ich.table.Table`
-00013600: 2063 6f6e 7374 7275 6374 6f72 2e0a 2020   constructor..  
-00013610: 2020 2020 636f 6c75 6d6e 5f6b 7761 7267      column_kwarg
-00013620: 733a 2041 6e20 6f70 7469 6f6e 616c 2064  s: An optional d
-00013630: 6963 7469 6f6e 6172 7920 7769 7468 2061  ictionary with a
-00013640: 6464 6974 696f 6e61 6c20 6b65 7977 6f72  dditional keywor
-00013650: 6420 6172 6775 6d65 6e74 7320 7468 6174  d arguments that
-00013660: 0a20 2020 2020 2020 2061 7265 2070 6173  .        are pas
-00013670: 7365 6420 746f 2060 7269 6368 2e74 6162  sed to `rich.tab
-00013680: 6c65 2e54 6162 6c65 2e61 6464 5f63 6f6c  le.Table.add_col
-00013690: 756d 6e60 2077 6865 6e20 6164 6469 6e67  umn` when adding
-000136a0: 2063 6f6c 756d 6e73 2074 6f20 7468 6520   columns to the 
-000136b0: 7461 626c 652e 0a20 2020 2020 202a 2a6b  table..      **k
-000136c0: 7761 7267 733a 206b 6579 776f 7264 2061  wargs: keyword a
-000136d0: 7267 756d 656e 7473 2074 6f20 7061 7373  rguments to pass
-000136e0: 2074 6f20 7468 6520 666f 7277 6172 6420   to the forward 
-000136f0: 636f 6d70 7574 6174 696f 6e2e 0a0a 2020  computation...  
-00013700: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00013710: 2041 2073 7472 696e 6720 7375 6d6d 6172   A string summar
-00013720: 697a 696e 6720 7468 6520 4d6f 6475 6c65  izing the Module
-00013730: 2e0a 2020 2020 2222 220a 2020 2020 6672  ..    """.    fr
-00013740: 6f6d 2066 6c61 782e 6c69 6e65 6e20 696d  om flax.linen im
-00013750: 706f 7274 2073 756d 6d61 7279 0a0a 2020  port summary..  
-00013760: 2020 7461 6275 6c61 7465 5f66 6e20 3d20    tabulate_fn = 
-00013770: 7375 6d6d 6172 792e 7461 6275 6c61 7465  summary.tabulate
-00013780: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00013790: 2020 2020 2020 2020 726e 6773 2c0a 2020          rngs,.  
-000137a0: 2020 2020 2020 6465 7074 683d 6465 7074        depth=dept
-000137b0: 682c 0a20 2020 2020 2020 2073 686f 775f  h,.        show_
-000137c0: 7265 7065 6174 6564 3d73 686f 775f 7265  repeated=show_re
-000137d0: 7065 6174 6564 2c0a 2020 2020 2020 2020  peated,.        
-000137e0: 6d75 7461 626c 653d 6d75 7461 626c 652c  mutable=mutable,
-000137f0: 0a20 2020 2020 2020 2063 6f6e 736f 6c65  .        console
-00013800: 5f6b 7761 7267 733d 636f 6e73 6f6c 655f  _kwargs=console_
-00013810: 6b77 6172 6773 2c0a 2020 2020 2020 2020  kwargs,.        
-00013820: 7461 626c 655f 6b77 6172 6773 3d74 6162  table_kwargs=tab
-00013830: 6c65 5f6b 7761 7267 732c 0a20 2020 2020  le_kwargs,.     
-00013840: 2020 2063 6f6c 756d 6e5f 6b77 6172 6773     column_kwargs
-00013850: 3d63 6f6c 756d 6e5f 6b77 6172 6773 2c0a  =column_kwargs,.
-00013860: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
-00013870: 2074 6162 756c 6174 655f 666e 282a 6172   tabulate_fn(*ar
-00013880: 6773 2c20 2a2a 6b77 6172 6773 290a 0a0a  gs, **kwargs)...
-00013890: 5f50 6172 656e 7454 7970 6520 3d20 556e  _ParentType = Un
-000138a0: 696f 6e5b 5479 7065 5b4d 6f64 756c 655d  ion[Type[Module]
-000138b0: 2c20 5479 7065 5b53 636f 7065 5d2c 2054  , Type[Scope], T
-000138c0: 7970 655b 5f53 656e 7469 6e65 6c5d 2c20  ype[_Sentinel], 
-000138d0: 4e6f 6e65 5d0a 0a0a 6465 6620 6d65 7267  None]...def merg
-000138e0: 655f 7061 7261 6d28 6e61 6d65 3a20 7374  e_param(name: st
-000138f0: 722c 2061 3a20 4f70 7469 6f6e 616c 5b54  r, a: Optional[T
-00013900: 5d2c 2062 3a20 4f70 7469 6f6e 616c 5b54  ], b: Optional[T
-00013910: 5d29 202d 3e20 543a 0a20 2022 2222 4d65  ]) -> T:.  """Me
-00013920: 7267 6573 2063 6f6e 7374 7275 6374 696f  rges constructio
-00013930: 6e2d 2061 6e64 2063 616c 6c2d 7469 6d65  n- and call-time
-00013940: 2061 7267 756d 656e 742e 0a0a 2020 5468   argument...  Th
-00013950: 6973 2069 7320 6120 7574 696c 6974 7920  is is a utility 
-00013960: 666f 7220 7375 7070 6f72 7469 6e67 2061  for supporting a
-00013970: 2070 6174 7465 726e 2077 6865 7265 2061   pattern where a
-00013980: 204d 6f64 756c 6520 6879 7065 7270 6172   Module hyperpar
-00013990: 616d 6574 6572 0a20 2063 616e 2062 6520  ameter.  can be 
-000139a0: 7061 7373 6564 2065 6974 6865 7220 746f  passed either to
-000139b0: 2060 605f 5f69 6e69 745f 5f60 6020 6f72   ``__init__`` or
-000139c0: 2060 605f 5f63 616c 6c5f 5f60 602c 2061   ``__call__``, a
-000139d0: 6e64 2074 6865 2076 616c 7565 2074 6861  nd the value tha
-000139e0: 7420 6973 0a20 206e 6f74 2060 4e6f 6e65  t is.  not `None
-000139f0: 6020 7769 6c6c 2062 6520 7573 6564 2e0a  ` will be used..
-00013a00: 0a20 2045 7861 6d70 6c65 3a3a 0a0a 2020  .  Example::..  
-00013a10: 2020 636c 6173 7320 466f 6f28 6e6e 2e4d    class Foo(nn.M
-00013a20: 6f64 756c 6529 3a0a 2020 2020 2020 7472  odule):.      tr
-00013a30: 6169 6e3a 204f 7074 696f 6e61 6c5b 626f  ain: Optional[bo
-00013a40: 6f6c 5d20 3d20 4e6f 6e65 0a0a 2020 2020  ol] = None..    
-00013a50: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
-00013a60: 656c 662c 2074 7261 696e 3a20 4f70 7469  elf, train: Opti
-00013a70: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00013a80: 6529 3a0a 2020 2020 2020 2020 7472 6169  e):.        trai
-00013a90: 6e20 3d20 6e6e 2e6d 6572 6765 5f70 6172  n = nn.merge_par
-00013aa0: 616d 2827 7472 6169 6e27 2c20 7365 6c66  am('train', self
-00013ab0: 2e74 7261 696e 2c20 7472 6169 6e29 0a0a  .train, train)..
-00013ac0: 2020 416e 2065 7272 6f72 2069 7320 7468    An error is th
-00013ad0: 726f 776e 2077 6865 6e20 626f 7468 2061  rown when both a
-00013ae0: 7267 756d 656e 7473 2061 7265 2060 4e6f  rguments are `No
-00013af0: 6e65 6020 6f72 2062 6f74 6820 7661 6c75  ne` or both valu
-00013b00: 6573 2061 7265 206e 6f74 0a20 2060 4e6f  es are not.  `No
-00013b10: 6e65 602e 0a0a 2020 4172 6773 3a0a 2020  ne`...  Args:.  
-00013b20: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
-00013b30: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
-00013b40: 722e 2055 7365 6420 666f 7220 6572 726f  r. Used for erro
-00013b50: 7220 6d65 7373 6167 6573 2e0a 2020 2020  r messages..    
-00013b60: 613a 206f 7074 696f 6e20 610a 2020 2020  a: option a.    
-00013b70: 623a 206f 7074 696f 6e20 620a 2020 5265  b: option b.  Re
-00013b80: 7475 726e 733a 0a20 2020 2061 206f 7220  turns:.    a or 
-00013b90: 6220 7768 6963 6865 7665 7220 6973 206e  b whichever is n
-00013ba0: 6f74 2060 4e6f 6e65 602e 0a0a 2020 2222  ot `None`...  ""
-00013bb0: 220a 2020 6966 2061 2069 7320 4e6f 6e65  ".  if a is None
-00013bc0: 2061 6e64 2062 2069 7320 4e6f 6e65 3a0a   and b is None:.
-00013bd0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00013be0: 7272 6f72 280a 2020 2020 2020 2020 6627  rror(.        f'
-00013bf0: 5061 7261 6d65 7465 7220 227b 6e61 6d65  Parameter "{name
-00013c00: 7d22 206d 7573 7420 6265 2070 6173 7365  }" must be passe
-00013c10: 6420 746f 2074 6865 2063 6f6e 7374 7275  d to the constru
-00013c20: 6374 6f72 206f 7220 6174 2063 616c 6c20  ctor or at call 
-00013c30: 7469 6d65 2e27 0a20 2020 2029 0a20 2069  time.'.    ).  i
-00013c40: 6620 6120 6973 206e 6f74 204e 6f6e 6520  f a is not None 
-00013c50: 616e 6420 6220 6973 206e 6f74 204e 6f6e  and b is not Non
-00013c60: 653a 0a20 2020 2072 6169 7365 2056 616c  e:.    raise Val
-00013c70: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00013c80: 2066 2750 6172 616d 6574 6572 2022 7b6e   f'Parameter "{n
-00013c90: 616d 657d 2220 7761 7320 7061 7373 6564  ame}" was passed
-00013ca0: 2074 6f20 7468 6520 636f 6e73 7472 7563   to the construc
-00013cb0: 746f 7220 616e 6420 6174 2063 616c 6c20  tor and at call 
-00013cc0: 7469 6d65 2e27 0a20 2020 2020 2020 2027  time.'.        '
-00013cd0: 2053 686f 756c 6420 6265 2070 6173 7365   Should be passe
-00013ce0: 6420 6a75 7374 206f 6e63 652e 270a 2020  d just once.'.  
-00013cf0: 2020 290a 2020 6966 2061 2069 7320 4e6f    ).  if a is No
-00013d00: 6e65 3a0a 2020 2020 6173 7365 7274 2062  ne:.    assert b
-00013d10: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00013d20: 2072 6574 7572 6e20 620a 2020 7265 7475   return b.  retu
-00013d30: 726e 2061 0a0a 0a40 7472 6163 6562 6163  rn a...@tracebac
-00013d40: 6b5f 7574 696c 2e61 7069 5f62 6f75 6e64  k_util.api_bound
-00013d50: 6172 790a 6465 6620 6170 706c 7928 0a20  ary.def apply(. 
-00013d60: 2020 2066 6e3a 2043 616c 6c61 626c 655b     fn: Callable[
-00013d70: 2e2e 2e2c 2041 6e79 5d2c 0a20 2020 206d  ..., Any],.    m
-00013d80: 6f64 756c 653a 204d 6f64 756c 652c 0a20  odule: Module,. 
-00013d90: 2020 206d 7574 6162 6c65 3a20 436f 6c6c     mutable: Coll
-00013da0: 6563 7469 6f6e 4669 6c74 6572 203d 2046  ectionFilter = F
-00013db0: 616c 7365 2c0a 2020 2020 6361 7074 7572  alse,.    captur
-00013dc0: 655f 696e 7465 726d 6564 6961 7465 733a  e_intermediates:
-00013dd0: 2055 6e69 6f6e 5b62 6f6f 6c2c 2043 616c   Union[bool, Cal
-00013de0: 6c61 626c 655b 5b4d 6f64 756c 652c 2073  lable[[Module, s
-00013df0: 7472 5d2c 2062 6f6f 6c5d 5d20 3d20 4661  tr], bool]] = Fa
-00013e00: 6c73 652c 0a29 202d 3e20 4361 6c6c 6162  lse,.) -> Callab
-00013e10: 6c65 5b2e 2e2e 2c20 416e 795d 3a0a 2020  le[..., Any]:.  
-00013e20: 2222 2243 7265 6174 6573 2061 6e20 6170  """Creates an ap
-00013e30: 706c 7920 6675 6e63 7469 6f6e 2074 6f20  ply function to 
-00013e40: 6361 6c6c 2060 6066 6e60 6020 7769 7468  call ``fn`` with
-00013e50: 2061 2062 6f75 6e64 206d 6f64 756c 652e   a bound module.
-00013e60: 0a0a 2020 556e 6c69 6b65 2060 604d 6f64  ..  Unlike ``Mod
-00013e70: 756c 652e 6170 706c 7960 6020 7468 6973  ule.apply`` this
-00013e80: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
-00013e90: 7320 6120 6e65 7720 6675 6e63 7469 6f6e  s a new function
-00013ea0: 2077 6974 6820 7468 6520 7369 676e 6174   with the signat
-00013eb0: 7572 650a 2020 6060 2876 6172 6961 626c  ure.  ``(variabl
-00013ec0: 6573 2c20 2a61 7267 732c 2072 6e67 733d  es, *args, rngs=
-00013ed0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 2920  None, **kwargs) 
-00013ee0: 2d3e 2054 6060 2077 6865 7265 2060 5460  -> T`` where `T`
-00013ef0: 2069 7320 7468 6520 7265 7475 726e 2074   is the return t
-00013f00: 7970 650a 2020 6f66 2060 6066 6e60 602e  ype.  of ``fn``.
-00013f10: 2049 6620 6060 6d75 7461 626c 6560 6020   If ``mutable`` 
-00013f20: 6973 206e 6f74 2060 6046 616c 7365 6060  is not ``False``
-00013f30: 2074 6865 2072 6574 7572 6e20 7479 7065   the return type
-00013f40: 2069 7320 6120 7475 706c 6520 7768 6572   is a tuple wher
-00013f50: 6520 7468 650a 2020 7365 636f 6e64 2069  e the.  second i
-00013f60: 7465 6d20 6973 2061 2060 6046 726f 7a65  tem is a ``Froze
-00013f70: 6e44 6963 7460 6020 7769 7468 2074 6865  nDict`` with the
-00013f80: 206d 7574 6174 6564 2076 6172 6961 626c   mutated variabl
-00013f90: 6573 2e0a 0a20 2054 6865 2061 7070 6c79  es...  The apply
-00013fa0: 2066 756e 6374 696f 6e20 7468 6174 2069   function that i
-00013fb0: 7320 7265 7475 726e 6564 2063 616e 2062  s returned can b
-00013fc0: 6520 6469 7265 6374 6c79 2063 6f6d 706f  e directly compo
-00013fd0: 7365 6420 7769 7468 0a20 204a 4158 2074  sed with.  JAX t
-00013fe0: 7261 6e73 666f 726d 6174 696f 6e73 206c  ransformations l
-00013ff0: 696b 6520 6060 6a61 782e 6a69 7460 603a  ike ``jax.jit``:
-00014000: 3a0a 0a20 2020 2064 6566 2066 2866 6f6f  :..    def f(foo
-00014010: 2c20 7829 3a0a 2020 2020 2020 7a20 3d20  , x):.      z = 
-00014020: 666f 6f2e 656e 636f 6465 2878 290a 2020  foo.encode(x).  
-00014030: 2020 2020 7920 3d20 666f 6f2e 6465 636f      y = foo.deco
-00014040: 6465 287a 290a 2020 2020 2020 2320 2e2e  de(z).      # ..
-00014050: 2e0a 2020 2020 2020 7265 7475 726e 2079  ..      return y
-00014060: 0a0a 2020 2020 666f 6f20 3d20 466f 6f28  ..    foo = Foo(
-00014070: 290a 2020 2020 665f 6a69 7474 6564 203d  ).    f_jitted =
-00014080: 206a 6178 2e6a 6974 286e 6e2e 6170 706c   jax.jit(nn.appl
-00014090: 7928 662c 2066 6f6f 2929 0a20 2020 2066  y(f, foo)).    f
-000140a0: 5f6a 6974 7465 6428 7661 7269 6162 6c65  _jitted(variable
-000140b0: 732c 2078 290a 0a20 2041 7267 733a 0a20  s, x)..  Args:. 
-000140c0: 2020 2066 6e3a 2054 6865 2066 756e 6374     fn: The funct
-000140d0: 696f 6e20 7468 6174 2073 686f 756c 6420  ion that should 
-000140e0: 6265 2061 7070 6c69 6564 2e20 5468 6520  be applied. The 
-000140f0: 6669 7273 7420 6172 6775 6d65 6e74 2070  first argument p
-00014100: 6173 7365 6420 7769 6c6c 0a20 2020 2020  assed will.     
-00014110: 2062 6520 616e 206d 6f64 756c 6520 696e   be an module in
-00014120: 7374 616e 6365 206f 6620 7468 6520 6060  stance of the ``
-00014130: 6d6f 6475 6c65 6060 2077 6974 6820 7661  module`` with va
-00014140: 7269 6162 6c65 7320 616e 6420 524e 4773  riables and RNGs
-00014150: 2062 6f75 6e64 0a20 2020 2020 2074 6f20   bound.      to 
-00014160: 6974 2e0a 2020 2020 6d6f 6475 6c65 3a20  it..    module: 
-00014170: 5468 6520 6060 4d6f 6475 6c65 6060 2074  The ``Module`` t
-00014180: 6861 7420 7769 6c6c 2062 6520 7573 6564  hat will be used
-00014190: 2074 6f20 6269 6e64 2076 6172 6961 626c   to bind variabl
-000141a0: 6573 2061 6e64 2052 4e47 7320 746f 2e0a  es and RNGs to..
-000141b0: 2020 2020 2020 5468 6520 6060 4d6f 6475        The ``Modu
-000141c0: 6c65 6060 2070 6173 7365 6420 6173 2074  le`` passed as t
-000141d0: 6865 2066 6972 7374 2061 7267 756d 656e  he first argumen
-000141e0: 7420 746f 2060 6066 6e60 6020 7769 6c6c  t to ``fn`` will
-000141f0: 2062 6520 6120 636c 6f6e 650a 2020 2020   be a clone.    
-00014200: 2020 6f66 206d 6f64 756c 652e 0a20 2020    of module..   
-00014210: 206d 7574 6162 6c65 3a20 4361 6e20 6265   mutable: Can be
-00014220: 2062 6f6f 6c2c 2073 7472 2c20 6f72 206c   bool, str, or l
-00014230: 6973 742e 2053 7065 6369 6669 6573 2077  ist. Specifies w
-00014240: 6869 6368 2063 6f6c 6c65 6374 696f 6e73  hich collections
-00014250: 2073 686f 756c 6420 6265 0a20 2020 2020   should be.     
-00014260: 2074 7265 6174 6564 2061 7320 6d75 7461   treated as muta
-00014270: 626c 653a 2060 6062 6f6f 6c60 603a 2061  ble: ``bool``: a
-00014280: 6c6c 2f6e 6f20 636f 6c6c 6563 7469 6f6e  ll/no collection
-00014290: 7320 6172 6520 6d75 7461 626c 652e 0a20  s are mutable.. 
-000142a0: 2020 2020 2060 6073 7472 6060 3a20 5468       ``str``: Th
-000142b0: 6520 6e61 6d65 206f 6620 6120 7369 6e67  e name of a sing
-000142c0: 6c65 206d 7574 6162 6c65 2063 6f6c 6c65  le mutable colle
-000142d0: 6374 696f 6e2e 2060 606c 6973 7460 603a  ction. ``list``:
-000142e0: 2041 0a20 2020 2020 206c 6973 7420 6f66   A.      list of
-000142f0: 206e 616d 6573 206f 6620 6d75 7461 626c   names of mutabl
-00014300: 6520 636f 6c6c 6563 7469 6f6e 732e 0a20  e collections.. 
-00014310: 2020 2063 6170 7475 7265 5f69 6e74 6572     capture_inter
-00014320: 6d65 6469 6174 6573 3a20 4966 2060 5472  mediates: If `Tr
-00014330: 7565 602c 2063 6170 7475 7265 7320 696e  ue`, captures in
-00014340: 7465 726d 6564 6961 7465 2072 6574 7572  termediate retur
-00014350: 6e20 7661 6c75 6573 0a20 2020 2020 206f  n values.      o
-00014360: 6620 616c 6c20 4d6f 6475 6c65 7320 696e  f all Modules in
-00014370: 7369 6465 2074 6865 2022 696e 7465 726d  side the "interm
-00014380: 6564 6961 7465 7322 2063 6f6c 6c65 6374  ediates" collect
-00014390: 696f 6e2e 2042 7920 6465 6661 756c 7420  ion. By default 
-000143a0: 6f6e 6c79 0a20 2020 2020 2074 6865 2072  only.      the r
-000143b0: 6574 7572 6e20 7661 6c75 6573 206f 6620  eturn values of 
-000143c0: 616c 6c20 605f 5f63 616c 6c5f 5f60 206d  all `__call__` m
-000143d0: 6574 686f 6473 2061 7265 2073 746f 7265  ethods are store
-000143e0: 642e 2041 2066 756e 6374 696f 6e20 6361  d. A function ca
-000143f0: 6e0a 2020 2020 2020 6265 2070 6173 7365  n.      be passe
-00014400: 6420 746f 2063 6861 6e67 6520 7468 6520  d to change the 
-00014410: 6669 6c74 6572 2062 6568 6176 696f 722e  filter behavior.
-00014420: 2054 6865 2066 696c 7465 7220 6675 6e63   The filter func
-00014430: 7469 6f6e 2074 616b 6573 0a20 2020 2020  tion takes.     
-00014440: 2074 6865 204d 6f64 756c 6520 696e 7374   the Module inst
-00014450: 616e 6365 2061 6e64 206d 6574 686f 6420  ance and method 
-00014460: 6e61 6d65 2061 6e64 2072 6574 7572 6e73  name and returns
-00014470: 2061 2062 6f6f 6c20 696e 6469 6361 7469   a bool indicati
-00014480: 6e67 0a20 2020 2020 2077 6865 7468 6572  ng.      whether
-00014490: 2074 6865 206f 7574 7075 7420 6f66 2074   the output of t
-000144a0: 6861 7420 6d65 7468 6f64 2069 6e76 6f63  hat method invoc
-000144b0: 6174 696f 6e20 7368 6f75 6c64 2062 6520  ation should be 
-000144c0: 7374 6f72 6564 2e0a 2020 5265 7475 726e  stored..  Return
-000144d0: 733a 0a20 2020 2054 6865 2061 7070 6c79  s:.    The apply
-000144e0: 2066 756e 6374 696f 6e20 7772 6170 7069   function wrappi
-000144f0: 6e67 2060 6066 6e60 602e 0a20 2022 2222  ng ``fn``..  """
-00014500: 0a0a 2020 4066 756e 6374 6f6f 6c73 2e77  ..  @functools.w
-00014510: 7261 7073 2866 6e29 0a20 2064 6566 2073  raps(fn).  def s
-00014520: 636f 7065 5f66 6e28 7363 6f70 652c 202a  cope_fn(scope, *
-00014530: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-00014540: 0a20 2020 205f 636f 6e74 6578 742e 6361  .    _context.ca
-00014550: 7074 7572 655f 7374 6163 6b2e 6170 7065  pture_stack.appe
-00014560: 6e64 2863 6170 7475 7265 5f69 6e74 6572  nd(capture_inter
-00014570: 6d65 6469 6174 6573 290a 2020 2020 7472  mediates).    tr
-00014580: 793a 0a20 2020 2020 2072 6574 7572 6e20  y:.      return 
-00014590: 666e 286d 6f64 756c 652e 636c 6f6e 6528  fn(module.clone(
-000145a0: 7061 7265 6e74 3d73 636f 7065 2c20 5f64  parent=scope, _d
-000145b0: 6565 705f 636c 6f6e 653d 5472 7565 292c  eep_clone=True),
-000145c0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-000145d0: 290a 2020 2020 6669 6e61 6c6c 793a 0a20  ).    finally:. 
-000145e0: 2020 2020 205f 636f 6e74 6578 742e 6361       _context.ca
-000145f0: 7074 7572 655f 7374 6163 6b2e 706f 7028  pture_stack.pop(
-00014600: 290a 0a20 2069 6620 6361 7074 7572 655f  )..  if capture_
-00014610: 696e 7465 726d 6564 6961 7465 7320 6973  intermediates is
-00014620: 2054 7275 653a 2020 2320 7079 6c69 6e74   True:  # pylint
-00014630: 3a20 6469 7361 626c 653d 672d 626f 6f6c  : disable=g-bool
-00014640: 2d69 642d 636f 6d70 6172 6973 6f6e 0a20  -id-comparison. 
-00014650: 2020 2063 6170 7475 7265 5f69 6e74 6572     capture_inter
-00014660: 6d65 6469 6174 6573 203d 2063 6170 7475  mediates = captu
-00014670: 7265 5f63 616c 6c5f 696e 7465 726d 6564  re_call_intermed
-00014680: 6961 7465 730a 2020 6966 2063 6170 7475  iates.  if captu
-00014690: 7265 5f69 6e74 6572 6d65 6469 6174 6573  re_intermediates
-000146a0: 3a0a 2020 2020 6d75 7461 626c 6520 3d20  :.    mutable = 
-000146b0: 756e 696f 6e5f 6669 6c74 6572 7328 6d75  union_filters(mu
-000146c0: 7461 626c 652c 2027 696e 7465 726d 6564  table, 'intermed
-000146d0: 6961 7465 7327 290a 2020 7265 7475 726e  iates').  return
-000146e0: 2063 6f72 652e 6170 706c 7928 7363 6f70   core.apply(scop
-000146f0: 655f 666e 2c20 6d75 7461 626c 653d 6d75  e_fn, mutable=mu
-00014700: 7461 626c 6529 0a0a 0a40 7472 6163 6562  table)...@traceb
-00014710: 6163 6b5f 7574 696c 2e61 7069 5f62 6f75  ack_util.api_bou
-00014720: 6e64 6172 790a 6465 6620 696e 6974 5f77  ndary.def init_w
-00014730: 6974 685f 6f75 7470 7574 280a 2020 2020  ith_output(.    
-00014740: 666e 3a20 4361 6c6c 6162 6c65 5b2e 2e2e  fn: Callable[...
-00014750: 2c20 416e 795d 2c0a 2020 2020 6d6f 6475  , Any],.    modu
-00014760: 6c65 3a20 4d6f 6475 6c65 2c0a 2020 2020  le: Module,.    
-00014770: 6d75 7461 626c 653a 2043 6f6c 6c65 6374  mutable: Collect
-00014780: 696f 6e46 696c 7465 7220 3d20 4465 6e79  ionFilter = Deny
-00014790: 4c69 7374 2827 696e 7465 726d 6564 6961  List('intermedia
-000147a0: 7465 7327 292c 0a20 2020 2063 6170 7475  tes'),.    captu
-000147b0: 7265 5f69 6e74 6572 6d65 6469 6174 6573  re_intermediates
-000147c0: 3a20 556e 696f 6e5b 626f 6f6c 2c20 4361  : Union[bool, Ca
-000147d0: 6c6c 6162 6c65 5b5b 4d6f 6475 6c65 2c20  llable[[Module, 
-000147e0: 7374 725d 2c20 626f 6f6c 5d5d 203d 2046  str], bool]] = F
-000147f0: 616c 7365 2c0a 2920 2d3e 2043 616c 6c61  alse,.) -> Calla
-00014800: 626c 655b 2e2e 2e2c 2054 7570 6c65 5b41  ble[..., Tuple[A
-00014810: 6e79 2c20 556e 696f 6e5b 4672 6f7a 656e  ny, Union[Frozen
-00014820: 5661 7269 6162 6c65 4469 6374 2c20 4469  VariableDict, Di
-00014830: 6374 5b73 7472 2c20 416e 795d 5d5d 5d3a  ct[str, Any]]]]:
-00014840: 0a20 2022 2222 4372 6561 7465 7320 616e  .  """Creates an
-00014850: 2069 6e69 7420 6675 6e63 7469 6f6e 2074   init function t
-00014860: 6f20 6361 6c6c 2060 6066 6e60 6020 7769  o call ``fn`` wi
-00014870: 7468 2061 2062 6f75 6e64 206d 6f64 756c  th a bound modul
-00014880: 6520 7468 6174 2061 6c73 6f20 7265 7475  e that also retu
-00014890: 726e 7320 7468 6520 6675 6e63 7469 6f6e  rns the function
-000148a0: 206f 7574 7075 7473 2e0a 0a20 2055 6e6c   outputs...  Unl
-000148b0: 696b 6520 6060 4d6f 6475 6c65 2e69 6e69  ike ``Module.ini
-000148c0: 745f 7769 7468 5f6f 7574 7075 7460 6020  t_with_output`` 
-000148d0: 7468 6973 2066 756e 6374 696f 6e20 7265  this function re
-000148e0: 7475 726e 7320 6120 6e65 7720 6675 6e63  turns a new func
-000148f0: 7469 6f6e 2077 6974 6820 7468 6520 7369  tion with the si
-00014900: 676e 6174 7572 650a 2020 6060 2872 6e67  gnature.  ``(rng
-00014910: 732c 202a 6172 6773 2c20 2a2a 6b77 6172  s, *args, **kwar
-00014920: 6773 2920 2d3e 2028 542c 2076 6172 6961  gs) -> (T, varia
-00014930: 626c 6573 2960 6020 7768 6572 6520 6054  bles)`` where `T
-00014940: 6020 6973 2074 6865 2072 6574 7572 6e20  ` is the return 
-00014950: 7479 7065 206f 6620 6060 666e 6060 2e0a  type of ``fn``..
-00014960: 2020 5468 6520 726e 6773 2063 616e 2062    The rngs can b
-00014970: 6520 6120 6469 6374 206f 6620 5052 4e47  e a dict of PRNG
-00014980: 4b65 7973 206f 7220 6120 7369 6e67 6c65  Keys or a single
-00014990: 2060 6060 5052 4e47 4b65 7960 6020 7768   ```PRNGKey`` wh
-000149a0: 6963 6820 6973 0a20 2065 7175 6976 616c  ich is.  equival
-000149b0: 656e 7420 746f 2070 6173 7369 6e67 2061  ent to passing a
-000149c0: 2064 6963 7420 7769 7468 206f 6e65 2050   dict with one P
-000149d0: 524e 474b 6579 2077 6974 6820 7468 6520  RNGKey with the 
-000149e0: 6e61 6d65 2022 7061 7261 6d73 222e 0a0a  name "params"...
-000149f0: 2020 5468 6520 696e 6974 2066 756e 6374    The init funct
-00014a00: 696f 6e20 7468 6174 2069 7320 7265 7475  ion that is retu
-00014a10: 726e 6564 2063 616e 2062 6520 6469 7265  rned can be dire
-00014a20: 6374 6c79 2063 6f6d 706f 7365 6420 7769  ctly composed wi
-00014a30: 7468 0a20 204a 4158 2074 7261 6e73 666f  th.  JAX transfo
-00014a40: 726d 6174 696f 6e73 206c 696b 6520 6060  rmations like ``
-00014a50: 6a61 782e 6a69 7460 603a 3a0a 0a20 2020  jax.jit``::..   
-00014a60: 2064 6566 2066 2866 6f6f 2c20 7829 3a0a   def f(foo, x):.
-00014a70: 2020 2020 2020 7a20 3d20 666f 6f2e 656e        z = foo.en
-00014a80: 636f 6465 2878 290a 2020 2020 2020 7920  code(x).      y 
-00014a90: 3d20 666f 6f2e 6465 636f 6465 287a 290a  = foo.decode(z).
-00014aa0: 2020 2020 2020 2320 2e2e 2e0a 2020 2020        # ....    
-00014ab0: 2020 7265 7475 726e 2079 0a0a 2020 2020    return y..    
-00014ac0: 666f 6f20 3d20 466f 6f28 290a 2020 2020  foo = Foo().    
-00014ad0: 665f 6a69 7474 6564 203d 206a 6178 2e6a  f_jitted = jax.j
-00014ae0: 6974 286e 6e2e 696e 6974 5f77 6974 685f  it(nn.init_with_
-00014af0: 6f75 7470 7574 2866 2c20 666f 6f29 290a  output(f, foo)).
-00014b00: 2020 2020 792c 2076 6172 6961 626c 6573      y, variables
-00014b10: 203d 2066 5f6a 6974 7465 6428 726e 672c   = f_jitted(rng,
-00014b20: 2078 290a 0a20 2041 7267 733a 0a20 2020   x)..  Args:.   
-00014b30: 2066 6e3a 2054 6865 2066 756e 6374 696f   fn: The functio
-00014b40: 6e20 7468 6174 2073 686f 756c 6420 6265  n that should be
-00014b50: 2061 7070 6c69 6564 2e20 5468 6520 6669   applied. The fi
-00014b60: 7273 7420 6172 6775 6d65 6e74 2070 6173  rst argument pas
-00014b70: 7365 6420 7769 6c6c 0a20 2020 2020 2062  sed will.      b
-00014b80: 6520 616e 206d 6f64 756c 6520 696e 7374  e an module inst
-00014b90: 616e 6365 206f 6620 7468 6520 6060 6d6f  ance of the ``mo
-00014ba0: 6475 6c65 6060 2077 6974 6820 7661 7269  dule`` with vari
-00014bb0: 6162 6c65 7320 616e 6420 524e 4773 2062  ables and RNGs b
-00014bc0: 6f75 6e64 0a20 2020 2020 2074 6f20 6974  ound.      to it
-00014bd0: 2e0a 2020 2020 6d6f 6475 6c65 3a20 5468  ..    module: Th
-00014be0: 6520 6060 4d6f 6475 6c65 6060 2074 6861  e ``Module`` tha
-00014bf0: 7420 7769 6c6c 2062 6520 7573 6564 2074  t will be used t
-00014c00: 6f20 6269 6e64 2076 6172 6961 626c 6573  o bind variables
-00014c10: 2061 6e64 2052 4e47 7320 746f 2e0a 2020   and RNGs to..  
-00014c20: 2020 2020 5468 6520 6060 4d6f 6475 6c65      The ``Module
-00014c30: 6060 2070 6173 7365 6420 6173 2074 6865  `` passed as the
-00014c40: 2066 6972 7374 2061 7267 756d 656e 7420   first argument 
-00014c50: 746f 2060 6066 6e60 6020 7769 6c6c 2062  to ``fn`` will b
-00014c60: 6520 6120 636c 6f6e 650a 2020 2020 2020  e a clone.      
-00014c70: 6f66 206d 6f64 756c 652e 0a20 2020 206d  of module..    m
-00014c80: 7574 6162 6c65 3a20 4361 6e20 6265 2062  utable: Can be b
-00014c90: 6f6f 6c2c 2073 7472 2c20 6f72 206c 6973  ool, str, or lis
-00014ca0: 742e 2053 7065 6369 6669 6573 2077 6869  t. Specifies whi
-00014cb0: 6368 2063 6f6c 6c65 6374 696f 6e73 2073  ch collections s
-00014cc0: 686f 756c 6420 6265 0a20 2020 2020 2074  hould be.      t
-00014cd0: 7265 6174 6564 2061 7320 6d75 7461 626c  reated as mutabl
-00014ce0: 653a 2060 6062 6f6f 6c60 603a 2061 6c6c  e: ``bool``: all
-00014cf0: 2f6e 6f20 636f 6c6c 6563 7469 6f6e 7320  /no collections 
-00014d00: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
-00014d10: 2020 2060 6073 7472 6060 3a20 5468 6520     ``str``: The 
-00014d20: 6e61 6d65 206f 6620 6120 7369 6e67 6c65  name of a single
-00014d30: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
-00014d40: 696f 6e2e 2060 606c 6973 7460 603a 2041  ion. ``list``: A
-00014d50: 0a20 2020 2020 206c 6973 7420 6f66 206e  .      list of n
-00014d60: 616d 6573 206f 6620 6d75 7461 626c 6520  ames of mutable 
-00014d70: 636f 6c6c 6563 7469 6f6e 732e 2042 7920  collections. By 
-00014d80: 6465 6661 756c 7420 616c 6c20 636f 6c6c  default all coll
-00014d90: 6563 7469 6f6e 730a 2020 2020 2020 6578  ections.      ex
-00014da0: 6365 7074 2022 696e 7465 726d 6564 6961  cept "intermedia
-00014db0: 7465 7322 2061 7265 206d 7574 6162 6c65  tes" are mutable
-00014dc0: 2e0a 2020 2020 6361 7074 7572 655f 696e  ..    capture_in
-00014dd0: 7465 726d 6564 6961 7465 733a 2049 6620  termediates: If 
-00014de0: 6054 7275 6560 2c20 6361 7074 7572 6573  `True`, captures
-00014df0: 2069 6e74 6572 6d65 6469 6174 6520 7265   intermediate re
-00014e00: 7475 726e 2076 616c 7565 730a 2020 2020  turn values.    
-00014e10: 2020 6f66 2061 6c6c 204d 6f64 756c 6573    of all Modules
-00014e20: 2069 6e73 6964 6520 7468 6520 2269 6e74   inside the "int
-00014e30: 6572 6d65 6469 6174 6573 2220 636f 6c6c  ermediates" coll
-00014e40: 6563 7469 6f6e 2e20 4279 2064 6566 6175  ection. By defau
-00014e50: 6c74 206f 6e6c 790a 2020 2020 2020 7468  lt only.      th
-00014e60: 6520 7265 7475 726e 2076 616c 7565 7320  e return values 
-00014e70: 6f66 2061 6c6c 2060 5f5f 6361 6c6c 5f5f  of all `__call__
-00014e80: 6020 6d65 7468 6f64 7320 6172 6520 7374  ` methods are st
-00014e90: 6f72 6564 2e20 4120 6675 6e63 7469 6f6e  ored. A function
-00014ea0: 2063 616e 0a20 2020 2020 2062 6520 7061   can.      be pa
-00014eb0: 7373 6564 2074 6f20 6368 616e 6765 2074  ssed to change t
-00014ec0: 6865 2066 696c 7465 7220 6265 6861 7669  he filter behavi
-00014ed0: 6f72 2e20 5468 6520 6669 6c74 6572 2066  or. The filter f
-00014ee0: 756e 6374 696f 6e20 7461 6b65 730a 2020  unction takes.  
-00014ef0: 2020 2020 7468 6520 4d6f 6475 6c65 2069      the Module i
-00014f00: 6e73 7461 6e63 6520 616e 6420 6d65 7468  nstance and meth
-00014f10: 6f64 206e 616d 6520 616e 6420 7265 7475  od name and retu
-00014f20: 726e 7320 6120 626f 6f6c 2069 6e64 6963  rns a bool indic
-00014f30: 6174 696e 670a 2020 2020 2020 7768 6574  ating.      whet
-00014f40: 6865 7220 7468 6520 6f75 7470 7574 206f  her the output o
-00014f50: 6620 7468 6174 206d 6574 686f 6420 696e  f that method in
-00014f60: 766f 6361 7469 6f6e 2073 686f 756c 6420  vocation should 
-00014f70: 6265 2073 746f 7265 642e 0a20 2052 6574  be stored..  Ret
-00014f80: 7572 6e73 3a0a 2020 2020 5468 6520 696e  urns:.    The in
-00014f90: 6974 2066 756e 6374 696f 6e20 7772 6170  it function wrap
-00014fa0: 7069 6e67 2060 6066 6e60 602e 0a20 2022  ping ``fn``..  "
-00014fb0: 2222 0a0a 2020 4066 756e 6374 6f6f 6c73  ""..  @functools
-00014fc0: 2e77 7261 7073 2866 6e29 0a20 2064 6566  .wraps(fn).  def
-00014fd0: 2073 636f 7065 5f66 6e28 7363 6f70 652c   scope_fn(scope,
-00014fe0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00014ff0: 293a 0a20 2020 205f 636f 6e74 6578 742e  ):.    _context.
-00015000: 6361 7074 7572 655f 7374 6163 6b2e 6170  capture_stack.ap
-00015010: 7065 6e64 2863 6170 7475 7265 5f69 6e74  pend(capture_int
-00015020: 6572 6d65 6469 6174 6573 290a 2020 2020  ermediates).    
-00015030: 7472 793a 0a20 2020 2020 2072 6574 7572  try:.      retur
-00015040: 6e20 666e 286d 6f64 756c 652e 636c 6f6e  n fn(module.clon
-00015050: 6528 7061 7265 6e74 3d73 636f 7065 2c20  e(parent=scope, 
-00015060: 5f64 6565 705f 636c 6f6e 653d 5472 7565  _deep_clone=True
-00015070: 292c 202a 6172 6773 2c20 2a2a 6b77 6172  ), *args, **kwar
-00015080: 6773 290a 2020 2020 6669 6e61 6c6c 793a  gs).    finally:
-00015090: 0a20 2020 2020 205f 636f 6e74 6578 742e  .      _context.
-000150a0: 6361 7074 7572 655f 7374 6163 6b2e 706f  capture_stack.po
-000150b0: 7028 290a 0a20 2069 6620 6361 7074 7572  p()..  if captur
-000150c0: 655f 696e 7465 726d 6564 6961 7465 7320  e_intermediates 
-000150d0: 6973 2054 7275 653a 2020 2320 7079 6c69  is True:  # pyli
-000150e0: 6e74 3a20 6469 7361 626c 653d 672d 626f  nt: disable=g-bo
-000150f0: 6f6c 2d69 642d 636f 6d70 6172 6973 6f6e  ol-id-comparison
-00015100: 0a20 2020 2063 6170 7475 7265 5f69 6e74  .    capture_int
-00015110: 6572 6d65 6469 6174 6573 203d 2063 6170  ermediates = cap
-00015120: 7475 7265 5f63 616c 6c5f 696e 7465 726d  ture_call_interm
-00015130: 6564 6961 7465 730a 2020 6966 2063 6170  ediates.  if cap
-00015140: 7475 7265 5f69 6e74 6572 6d65 6469 6174  ture_intermediat
-00015150: 6573 3a0a 2020 2020 6d75 7461 626c 6520  es:.    mutable 
-00015160: 3d20 756e 696f 6e5f 6669 6c74 6572 7328  = union_filters(
-00015170: 6d75 7461 626c 652c 2027 696e 7465 726d  mutable, 'interm
-00015180: 6564 6961 7465 7327 290a 2020 7265 7475  ediates').  retu
-00015190: 726e 2063 6f72 652e 696e 6974 2873 636f  rn core.init(sco
-000151a0: 7065 5f66 6e2c 206d 7574 6162 6c65 3d6d  pe_fn, mutable=m
-000151b0: 7574 6162 6c65 290a 0a0a 4074 7261 6365  utable)...@trace
-000151c0: 6261 636b 5f75 7469 6c2e 6170 695f 626f  back_util.api_bo
-000151d0: 756e 6461 7279 0a64 6566 2069 6e69 7428  undary.def init(
-000151e0: 0a20 2020 2066 6e3a 2043 616c 6c61 626c  .    fn: Callabl
-000151f0: 655b 2e2e 2e2c 2041 6e79 5d2c 0a20 2020  e[..., Any],.   
-00015200: 206d 6f64 756c 653a 204d 6f64 756c 652c   module: Module,
-00015210: 0a20 2020 206d 7574 6162 6c65 3a20 436f  .    mutable: Co
-00015220: 6c6c 6563 7469 6f6e 4669 6c74 6572 203d  llectionFilter =
-00015230: 2044 656e 794c 6973 7428 2769 6e74 6572   DenyList('inter
-00015240: 6d65 6469 6174 6573 2729 2c0a 2020 2020  mediates'),.    
-00015250: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
-00015260: 6961 7465 733a 2055 6e69 6f6e 5b62 6f6f  iates: Union[boo
-00015270: 6c2c 2043 616c 6c61 626c 655b 5b4d 6f64  l, Callable[[Mod
-00015280: 756c 652c 2073 7472 5d2c 2062 6f6f 6c5d  ule, str], bool]
-00015290: 5d20 3d20 4661 6c73 652c 0a29 202d 3e20  ] = False,.) -> 
-000152a0: 4361 6c6c 6162 6c65 5b2e 2e2e 2c20 556e  Callable[..., Un
-000152b0: 696f 6e5b 4672 6f7a 656e 5661 7269 6162  ion[FrozenVariab
-000152c0: 6c65 4469 6374 2c20 4469 6374 5b73 7472  leDict, Dict[str
-000152d0: 2c20 416e 795d 5d5d 3a0a 2020 2222 2243  , Any]]]:.  """C
-000152e0: 7265 6174 6573 2061 6e20 696e 6974 2066  reates an init f
-000152f0: 756e 6374 696f 6e20 746f 2063 616c 6c20  unction to call 
-00015300: 6060 666e 6060 2077 6974 6820 6120 626f  ``fn`` with a bo
-00015310: 756e 6420 6d6f 6475 6c65 2e0a 0a20 2055  und module...  U
-00015320: 6e6c 696b 6520 6060 4d6f 6475 6c65 2e69  nlike ``Module.i
-00015330: 6e69 7460 6020 7468 6973 2066 756e 6374  nit`` this funct
-00015340: 696f 6e20 7265 7475 726e 7320 6120 6e65  ion returns a ne
-00015350: 7720 6675 6e63 7469 6f6e 2077 6974 6820  w function with 
-00015360: 7468 6520 7369 676e 6174 7572 650a 2020  the signature.  
-00015370: 6060 2872 6e67 732c 202a 6172 6773 2c20  ``(rngs, *args, 
-00015380: 2a2a 6b77 6172 6773 2920 2d3e 2076 6172  **kwargs) -> var
-00015390: 6961 626c 6573 6060 2e0a 2020 5468 6520  iables``..  The 
-000153a0: 726e 6773 2063 616e 2062 6520 6120 6469  rngs can be a di
-000153b0: 6374 206f 6620 5052 4e47 4b65 7973 206f  ct of PRNGKeys o
-000153c0: 7220 6120 7369 6e67 6c65 2060 6060 5052  r a single ```PR
-000153d0: 4e47 4b65 7960 6020 7768 6963 6820 6973  NGKey`` which is
-000153e0: 0a20 2065 7175 6976 616c 656e 7420 746f  .  equivalent to
-000153f0: 2070 6173 7369 6e67 2061 2064 6963 7420   passing a dict 
-00015400: 7769 7468 206f 6e65 2050 524e 474b 6579  with one PRNGKey
-00015410: 2077 6974 6820 7468 6520 6e61 6d65 2022   with the name "
-00015420: 7061 7261 6d73 222e 0a0a 2020 5468 6520  params"...  The 
-00015430: 696e 6974 2066 756e 6374 696f 6e20 7468  init function th
-00015440: 6174 2069 7320 7265 7475 726e 6564 2063  at is returned c
-00015450: 616e 2062 6520 6469 7265 6374 6c79 2063  an be directly c
-00015460: 6f6d 706f 7365 6420 7769 7468 0a20 204a  omposed with.  J
-00015470: 4158 2074 7261 6e73 666f 726d 6174 696f  AX transformatio
-00015480: 6e73 206c 696b 6520 6060 6a61 782e 6a69  ns like ``jax.ji
-00015490: 7460 603a 3a0a 0a20 2020 2064 6566 2066  t``::..    def f
-000154a0: 2866 6f6f 2c20 7829 3a0a 2020 2020 2020  (foo, x):.      
-000154b0: 7a20 3d20 666f 6f2e 656e 636f 6465 2878  z = foo.encode(x
-000154c0: 290a 2020 2020 2020 7920 3d20 666f 6f2e  ).      y = foo.
-000154d0: 6465 636f 6465 287a 290a 2020 2020 2020  decode(z).      
-000154e0: 2320 2e2e 2e0a 2020 2020 2020 7265 7475  # ....      retu
-000154f0: 726e 2079 0a0a 2020 2020 666f 6f20 3d20  rn y..    foo = 
-00015500: 466f 6f28 290a 2020 2020 665f 6a69 7474  Foo().    f_jitt
-00015510: 6564 203d 206a 6178 2e6a 6974 286e 6e2e  ed = jax.jit(nn.
-00015520: 696e 6974 2866 2c20 666f 6f29 290a 2020  init(f, foo)).  
-00015530: 2020 7661 7269 6162 6c65 7320 3d20 665f    variables = f_
-00015540: 6a69 7474 6564 2872 6e67 2c20 7829 0a0a  jitted(rng, x)..
-00015550: 2020 4172 6773 3a0a 2020 2020 666e 3a20    Args:.    fn: 
-00015560: 5468 6520 6675 6e63 7469 6f6e 2074 6861  The function tha
-00015570: 7420 7368 6f75 6c64 2062 6520 6170 706c  t should be appl
-00015580: 6965 642e 2054 6865 2066 6972 7374 2061  ied. The first a
-00015590: 7267 756d 656e 7420 7061 7373 6564 2077  rgument passed w
-000155a0: 696c 6c0a 2020 2020 2020 6265 2061 6e20  ill.      be an 
-000155b0: 6d6f 6475 6c65 2069 6e73 7461 6e63 6520  module instance 
-000155c0: 6f66 2074 6865 2060 606d 6f64 756c 6560  of the ``module`
-000155d0: 6020 7769 7468 2076 6172 6961 626c 6573  ` with variables
-000155e0: 2061 6e64 2052 4e47 7320 626f 756e 640a   and RNGs bound.
-000155f0: 2020 2020 2020 746f 2069 742e 0a20 2020        to it..   
-00015600: 206d 6f64 756c 653a 2054 6865 2060 604d   module: The ``M
-00015610: 6f64 756c 6560 6020 7468 6174 2077 696c  odule`` that wil
-00015620: 6c20 6265 2075 7365 6420 746f 2062 696e  l be used to bin
-00015630: 6420 7661 7269 6162 6c65 7320 616e 6420  d variables and 
-00015640: 524e 4773 2074 6f2e 0a20 2020 2020 2054  RNGs to..      T
-00015650: 6865 2060 604d 6f64 756c 6560 6020 7061  he ``Module`` pa
-00015660: 7373 6564 2061 7320 7468 6520 6669 7273  ssed as the firs
-00015670: 7420 6172 6775 6d65 6e74 2074 6f20 6060  t argument to ``
-00015680: 666e 6060 2077 696c 6c20 6265 2061 2063  fn`` will be a c
-00015690: 6c6f 6e65 0a20 2020 2020 206f 6620 6d6f  lone.      of mo
-000156a0: 6475 6c65 2e0a 2020 2020 6d75 7461 626c  dule..    mutabl
-000156b0: 653a 2043 616e 2062 6520 626f 6f6c 2c20  e: Can be bool, 
-000156c0: 7374 722c 206f 7220 6c69 7374 2e20 5370  str, or list. Sp
-000156d0: 6563 6966 6965 7320 7768 6963 6820 636f  ecifies which co
-000156e0: 6c6c 6563 7469 6f6e 7320 7368 6f75 6c64  llections should
-000156f0: 2062 650a 2020 2020 2020 7472 6561 7465   be.      treate
-00015700: 6420 6173 206d 7574 6162 6c65 3a20 6060  d as mutable: ``
-00015710: 626f 6f6c 6060 3a20 616c 6c2f 6e6f 2063  bool``: all/no c
-00015720: 6f6c 6c65 6374 696f 6e73 2061 7265 206d  ollections are m
-00015730: 7574 6162 6c65 2e0a 2020 2020 2020 6060  utable..      ``
-00015740: 7374 7260 603a 2054 6865 206e 616d 6520  str``: The name 
-00015750: 6f66 2061 2073 696e 676c 6520 6d75 7461  of a single muta
-00015760: 626c 6520 636f 6c6c 6563 7469 6f6e 2e20  ble collection. 
-00015770: 6060 6c69 7374 6060 3a20 410a 2020 2020  ``list``: A.    
-00015780: 2020 6c69 7374 206f 6620 6e61 6d65 7320    list of names 
-00015790: 6f66 206d 7574 6162 6c65 2063 6f6c 6c65  of mutable colle
-000157a0: 6374 696f 6e73 2e20 4279 2064 6566 6175  ctions. By defau
-000157b0: 6c74 2061 6c6c 2063 6f6c 6c65 6374 696f  lt all collectio
-000157c0: 6e73 0a20 2020 2020 2065 7863 6570 7420  ns.      except 
-000157d0: 2269 6e74 6572 6d65 6469 6174 6573 2220  "intermediates" 
-000157e0: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
-000157f0: 2063 6170 7475 7265 5f69 6e74 6572 6d65   capture_interme
-00015800: 6469 6174 6573 3a20 4966 2060 5472 7565  diates: If `True
-00015810: 602c 2063 6170 7475 7265 7320 696e 7465  `, captures inte
-00015820: 726d 6564 6961 7465 2072 6574 7572 6e20  rmediate return 
-00015830: 7661 6c75 6573 0a20 2020 2020 206f 6620  values.      of 
-00015840: 616c 6c20 4d6f 6475 6c65 7320 696e 7369  all Modules insi
-00015850: 6465 2074 6865 2022 696e 7465 726d 6564  de the "intermed
-00015860: 6961 7465 7322 2063 6f6c 6c65 6374 696f  iates" collectio
-00015870: 6e2e 2042 7920 6465 6661 756c 7420 6f6e  n. By default on
-00015880: 6c79 0a20 2020 2020 2074 6865 2072 6574  ly.      the ret
-00015890: 7572 6e20 7661 6c75 6573 206f 6620 616c  urn values of al
-000158a0: 6c20 605f 5f63 616c 6c5f 5f60 206d 6574  l `__call__` met
-000158b0: 686f 6473 2061 7265 2073 746f 7265 642e  hods are stored.
-000158c0: 2041 2066 756e 6374 696f 6e20 6361 6e0a   A function can.
-000158d0: 2020 2020 2020 6265 2070 6173 7365 6420        be passed 
-000158e0: 746f 2063 6861 6e67 6520 7468 6520 6669  to change the fi
-000158f0: 6c74 6572 2062 6568 6176 696f 722e 2054  lter behavior. T
-00015900: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
-00015910: 6f6e 2074 616b 6573 0a20 2020 2020 2074  on takes.      t
-00015920: 6865 204d 6f64 756c 6520 696e 7374 616e  he Module instan
-00015930: 6365 2061 6e64 206d 6574 686f 6420 6e61  ce and method na
-00015940: 6d65 2061 6e64 2072 6574 7572 6e73 2061  me and returns a
-00015950: 2062 6f6f 6c20 696e 6469 6361 7469 6e67   bool indicating
-00015960: 0a20 2020 2020 2077 6865 7468 6572 2074  .      whether t
-00015970: 6865 206f 7574 7075 7420 6f66 2074 6861  he output of tha
-00015980: 7420 6d65 7468 6f64 2069 6e76 6f63 6174  t method invocat
-00015990: 696f 6e20 7368 6f75 6c64 2062 6520 7374  ion should be st
-000159a0: 6f72 6564 2e0a 2020 5265 7475 726e 733a  ored..  Returns:
-000159b0: 0a20 2020 2054 6865 2069 6e69 7420 6675  .    The init fu
-000159c0: 6e63 7469 6f6e 2077 7261 7070 696e 6720  nction wrapping 
-000159d0: 6060 666e 6060 2e0a 2020 2222 220a 2020  ``fn``..  """.  
-000159e0: 696e 6974 5f66 6e20 3d20 696e 6974 5f77  init_fn = init_w
-000159f0: 6974 685f 6f75 7470 7574 2866 6e2c 206d  ith_output(fn, m
-00015a00: 6f64 756c 652c 206d 7574 6162 6c65 2c20  odule, mutable, 
-00015a10: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
-00015a20: 6961 7465 7329 0a0a 2020 4066 756e 6374  iates)..  @funct
-00015a30: 6f6f 6c73 2e77 7261 7073 2869 6e69 745f  ools.wraps(init_
-00015a40: 666e 290a 2020 6465 6620 696e 6974 5f77  fn).  def init_w
-00015a50: 7261 7070 6572 282a 6172 6773 2c20 2a2a  rapper(*args, **
-00015a60: 6b77 6172 6773 293a 0a20 2020 2072 6574  kwargs):.    ret
-00015a70: 7572 6e20 696e 6974 5f66 6e28 2a61 7267  urn init_fn(*arg
-00015a80: 732c 202a 2a6b 7761 7267 7329 5b31 5d0a  s, **kwargs)[1].
-00015a90: 0a20 2072 6574 7572 6e20 696e 6974 5f77  .  return init_w
-00015aa0: 7261 7070 6572 0a                        rapper.
+00005480: 0a20 2020 206e 616d 653a 204f 7074 696f  .    name: Optio
+00005490: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000054a0: 2020 2020 7363 6f70 653a 204f 7074 696f      scope: Optio
+000054b0: 6e61 6c5b 5363 6f70 655d 0a20 2020 205f  nal[Scope].    _
+000054c0: 7374 6174 653a 205f 4d6f 6475 6c65 496e  state: _ModuleIn
+000054d0: 7465 726e 616c 5374 6174 650a 2020 2020  ternalState.    
+000054e0: 5f70 6172 656e 745f 7265 663a 2055 6e69  _parent_ref: Uni
+000054f0: 6f6e 5b27 4d6f 6475 6c65 272c 2077 6561  on['Module', wea
+00005500: 6b72 6566 2e52 6566 6572 656e 6365 5479  kref.ReferenceTy
+00005510: 7065 5b27 4d6f 6475 6c65 275d 2c20 4e6f  pe['Module'], No
+00005520: 6e65 5d0a 2020 2020 7061 7265 6e74 3a20  ne].    parent: 
+00005530: 556e 696f 6e5b 274d 6f64 756c 6527 2c20  Union['Module', 
+00005540: 5f53 656e 7469 6e65 6c2c 204e 6f6e 655d  _Sentinel, None]
+00005550: 0a20 2020 205f 5f64 6174 6163 6c61 7373  .    __dataclass
+00005560: 5f66 6965 6c64 735f 5f3a 2044 6963 745b  _fields__: Dict[
+00005570: 7374 722c 2064 6174 6163 6c61 7373 6573  str, dataclasses
+00005580: 2e46 6965 6c64 5d0a 0a0a 636c 6173 7320  .Field]...class 
+00005590: 4d6f 6475 6c65 284d 6f64 756c 6542 6173  Module(ModuleBas
+000055a0: 6529 3a0a 2020 2222 2242 6173 6520 636c  e):.  """Base cl
+000055b0: 6173 7320 666f 7220 616c 6c20 6e65 7572  ass for all neur
+000055c0: 616c 206e 6574 776f 726b 206d 6f64 756c  al network modul
+000055d0: 6573 2e20 4c61 7965 7273 2061 6e64 206d  es. Layers and m
+000055e0: 6f64 656c 7320 7368 6f75 6c64 2073 7562  odels should sub
+000055f0: 636c 6173 7320 7468 6973 2063 6c61 7373  class this class
+00005600: 2e0a 0a20 2041 6c6c 2046 6c61 7820 4d6f  ...  All Flax Mo
+00005610: 6475 6c65 7320 6172 6520 5079 7468 6f6e  dules are Python
+00005620: 2033 2e37 0a20 2060 6461 7461 636c 6173   3.7.  `dataclas
+00005630: 7365 7320 3c68 7474 7073 3a2f 2f64 6f63  ses <https://doc
+00005640: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+00005650: 6962 7261 7279 2f64 6174 6163 6c61 7373  ibrary/dataclass
+00005660: 6573 2e68 746d 6c3e 605f 2e20 5369 6e63  es.html>`_. Sinc
+00005670: 650a 2020 6461 7461 636c 6173 7365 7320  e.  dataclasses 
+00005680: 7461 6b65 206f 7665 7220 6060 5f5f 696e  take over ``__in
+00005690: 6974 5f5f 6060 2c20 796f 7520 7368 6f75  it__``, you shou
+000056a0: 6c64 2069 6e73 7465 6164 206f 7665 7272  ld instead overr
+000056b0: 6964 6520 3a6d 6574 683a 6073 6574 7570  ide :meth:`setup
+000056c0: 602c 0a20 2077 6869 6368 2069 7320 6175  `,.  which is au
+000056d0: 746f 6d61 7469 6361 6c6c 7920 6361 6c6c  tomatically call
+000056e0: 6564 2074 6f20 696e 6974 6961 6c69 7a65  ed to initialize
+000056f0: 2074 6865 206d 6f64 756c 652e 0a0a 2020   the module...  
+00005700: 4d6f 6475 6c65 7320 6361 6e20 636f 6e74  Modules can cont
+00005710: 6169 6e20 7375 626d 6f64 756c 6573 2c20  ain submodules, 
+00005720: 616e 6420 696e 2074 6869 7320 7761 7920  and in this way 
+00005730: 6361 6e20 6265 206e 6573 7465 6420 696e  can be nested in
+00005740: 2061 2074 7265 650a 2020 7374 7275 6374   a tree.  struct
+00005750: 7572 652e 2053 7562 6d6f 6465 6c73 2063  ure. Submodels c
+00005760: 616e 2062 6520 6173 7369 676e 6564 2061  an be assigned a
+00005770: 7320 7265 6775 6c61 7220 6174 7472 6962  s regular attrib
+00005780: 7574 6573 2069 6e73 6964 6520 7468 650a  utes inside the.
+00005790: 2020 3a6d 6574 683a 6073 6574 7570 6020    :meth:`setup` 
+000057a0: 6d65 7468 6f64 2e0a 0a20 2059 6f75 2063  method...  You c
+000057b0: 616e 2064 6566 696e 6520 6172 6269 7472  an define arbitr
+000057c0: 6172 7920 2266 6f72 7761 7264 2070 6173  ary "forward pas
+000057d0: 7322 206d 6574 686f 6473 206f 6e20 796f  s" methods on yo
+000057e0: 7572 204d 6f64 756c 6520 7375 6263 6c61  ur Module subcla
+000057f0: 7373 2e0a 2020 5768 696c 6520 6e6f 206d  ss..  While no m
+00005800: 6574 686f 6473 2061 7265 2073 7065 6369  ethods are speci
+00005810: 616c 2d63 6173 6564 2c20 6060 5f5f 6361  al-cased, ``__ca
+00005820: 6c6c 5f5f 6060 2069 7320 6120 706f 7075  ll__`` is a popu
+00005830: 6c61 7220 6368 6f69 6365 2062 6563 6175  lar choice becau
+00005840: 7365 0a20 2069 7420 616c 6c6f 7773 2079  se.  it allows y
+00005850: 6f75 2074 6f20 7573 6520 6d6f 6475 6c65  ou to use module
+00005860: 2069 6e73 7461 6e63 6573 2061 7320 6966   instances as if
+00005870: 2074 6865 7920 6172 6520 6675 6e63 7469   they are functi
+00005880: 6f6e 733a 3a0a 0a20 2020 2066 726f 6d20  ons::..    from 
+00005890: 666c 6178 2069 6d70 6f72 7420 6c69 6e65  flax import line
+000058a0: 6e20 6173 206e 6e0a 0a20 2020 2063 6c61  n as nn..    cla
+000058b0: 7373 204d 6f64 756c 6528 6e6e 2e4d 6f64  ss Module(nn.Mod
+000058c0: 756c 6529 3a0a 2020 2020 2020 6665 6174  ule):.      feat
+000058d0: 7572 6573 3a20 5475 706c 655b 696e 742c  ures: Tuple[int,
+000058e0: 202e 2e2e 5d20 3d20 2831 362c 2034 290a   ...] = (16, 4).
+000058f0: 0a20 2020 2020 2064 6566 2073 6574 7570  .      def setup
+00005900: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00005910: 7365 6c66 2e64 656e 7365 3120 3d20 4465  self.dense1 = De
+00005920: 6e73 6528 7365 6c66 2e66 6561 7475 7265  nse(self.feature
+00005930: 735b 305d 290a 2020 2020 2020 2020 7365  s[0]).        se
+00005940: 6c66 2e64 656e 7365 3220 3d20 4465 6e73  lf.dense2 = Dens
+00005950: 6528 7365 6c66 2e66 6561 7475 7265 735b  e(self.features[
+00005960: 315d 290a 0a20 2020 2020 2064 6566 205f  1])..      def _
+00005970: 5f63 616c 6c5f 5f28 7365 6c66 2c20 7829  _call__(self, x)
+00005980: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00005990: 2073 656c 662e 6465 6e73 6532 286e 6e2e   self.dense2(nn.
+000059a0: 7265 6c75 2873 656c 662e 6465 6e73 6531  relu(self.dense1
+000059b0: 2878 2929 290a 0a20 204f 7074 696f 6e61  (x)))..  Optiona
+000059c0: 6c6c 792c 2066 6f72 206d 6f72 6520 636f  lly, for more co
+000059d0: 6e63 6973 6520 6d6f 6475 6c65 2069 6d70  ncise module imp
+000059e0: 6c65 6d65 6e74 6174 696f 6e73 2077 6865  lementations whe
+000059f0: 7265 2073 7562 6d6f 6475 6c65 730a 2020  re submodules.  
+00005a00: 6465 6669 6e69 7469 6f6e 7320 6172 6520  definitions are 
+00005a10: 636f 2d6c 6f63 6174 6564 2077 6974 6820  co-located with 
+00005a20: 7468 6569 7220 7573 6167 652c 2079 6f75  their usage, you
+00005a30: 2063 616e 2075 7365 2074 6865 0a20 203a   can use the.  :
+00005a40: 6d65 7468 3a60 636f 6d70 6163 7460 2077  meth:`compact` w
+00005a50: 7261 7070 6572 2e0a 2020 2222 220a 0a20  rapper..  """.. 
+00005a60: 2069 6620 7479 7069 6e67 2e54 5950 455f   if typing.TYPE_
+00005a70: 4348 4543 4b49 4e47 3a0a 0a20 2020 2064  CHECKING:..    d
+00005a80: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00005a90: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00005aa0: 7329 3a0a 2020 2020 2020 2320 7468 6973  s):.      # this
+00005ab0: 2073 7475 6220 6d61 6b65 7320 7375 7265   stub makes sure
+00005ac0: 2070 7974 7970 6520 6163 6365 7074 7320   pytype accepts 
+00005ad0: 636f 6e73 7472 7563 746f 7220 6172 6775  constructor argu
+00005ae0: 6d65 6e74 732e 0a20 2020 2020 2070 6173  ments..      pas
+00005af0: 730a 0a20 2020 2064 6566 205f 5f63 616c  s..    def __cal
+00005b00: 6c5f 5f28 7365 6c66 2c20 2a61 7267 732c  l__(self, *args,
+00005b10: 202a 2a6b 7761 7267 7329 202d 3e20 416e   **kwargs) -> An
+00005b20: 793a 0a20 2020 2020 2023 2074 6869 7320  y:.      # this 
+00005b30: 7374 7562 2061 6c6c 6f77 7320 7079 7479  stub allows pyty
+00005b40: 7065 2074 6f20 6163 6365 7074 204d 6f64  pe to accept Mod
+00005b50: 756c 6573 2061 7320 4361 6c6c 6162 6c65  ules as Callable
+00005b60: 732e 0a20 2020 2020 2070 6173 730a 0a20  s..      pass.. 
+00005b70: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00005b80: 6465 6620 5f5f 696e 6974 5f73 7562 636c  def __init_subcl
+00005b90: 6173 735f 5f28 636c 732c 206b 775f 6f6e  ass__(cls, kw_on
+00005ba0: 6c79 3a20 626f 6f6c 203d 2046 616c 7365  ly: bool = False
+00005bb0: 2c20 2a2a 6b77 6172 6773 3a20 416e 7929  , **kwargs: Any)
+00005bc0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+00005bd0: 2241 7574 6f6d 6174 6963 616c 6c79 2069  "Automatically i
+00005be0: 6e69 7469 616c 697a 6573 2061 6c6c 2073  nitializes all s
+00005bf0: 7562 636c 6173 7365 7320 6173 2063 7573  ubclasses as cus
+00005c00: 746f 6d20 6461 7461 636c 6173 7365 732e  tom dataclasses.
+00005c10: 2222 220a 2020 2020 7375 7065 7228 292e  """.    super().
+00005c20: 5f5f 696e 6974 5f73 7562 636c 6173 735f  __init_subclass_
+00005c30: 5f28 2a2a 6b77 6172 6773 290a 2020 2020  _(**kwargs).    
+00005c40: 2320 416c 6c20 466c 6178 204d 6f64 756c  # All Flax Modul
+00005c50: 6573 2061 7265 2064 6174 6163 6c61 7373  es are dataclass
+00005c60: 6573 2e20 2057 6520 666f 7263 6520 7468  es.  We force th
+00005c70: 6973 2063 6f6e 7665 6e74 696f 6e20 7369  is convention si
+00005c80: 6e63 650a 2020 2020 2320 6974 2065 6e63  nce.    # it enc
+00005c90: 6f75 7261 6765 7320 7468 6520 7374 6174  ourages the stat
+00005ca0: 656c 6573 7320 6265 6861 7669 6f72 206e  eless behavior n
+00005cb0: 6565 6465 6420 746f 2063 6c6f 6e65 206d  eeded to clone m
+00005cc0: 6f64 756c 6520 696e 7374 616e 6365 7320  odule instances 
+00005cd0: 666f 720a 2020 2020 2320 6675 6e63 7469  for.    # functi
+00005ce0: 6f6e 616c 2074 7261 6e73 666f 726d 6174  onal transformat
+00005cf0: 696f 6e2e 2020 496e 7374 6561 6420 6f66  ion.  Instead of
+00005d00: 2075 7369 6e67 2061 2070 7974 686f 6e20   using a python 
+00005d10: 6d65 7461 636c 6173 732c 2077 650a 2020  metaclass, we.  
+00005d20: 2020 2320 6175 746f 6d61 7469 6361 6c6c    # automaticall
+00005d30: 7920 7472 616e 7366 6f72 6d20 4d6f 6475  y transform Modu
+00005d40: 6c65 7320 696e 746f 2064 6174 6163 6c61  les into datacla
+00005d50: 7373 6573 2061 7420 7375 6263 6c61 7373  sses at subclass
+00005d60: 2063 7265 6174 696f 6e0a 2020 2020 2320   creation.    # 
+00005d70: 7469 6d65 2c20 616e 6420 7765 2073 6574  time, and we set
+00005d80: 2074 6865 206c 6173 7420 6461 7461 636c   the last datacl
+00005d90: 6173 7320 6172 6775 6d65 6e74 7320 746f  ass arguments to
+00005da0: 2060 7061 7265 6e74 6020 616e 6420 606e   `parent` and `n
+00005db0: 616d 6560 2e0a 2020 2020 636c 732e 5f63  ame`..    cls._c
+00005dc0: 7573 746f 6d69 7a65 645f 6461 7461 636c  ustomized_datacl
+00005dd0: 6173 735f 7472 616e 7366 6f72 6d28 6b77  ass_transform(kw
+00005de0: 5f6f 6e6c 7929 0a20 2020 2023 2057 6520  _only).    # We 
+00005df0: 7772 6170 2075 7365 722d 6465 6669 6e65  wrap user-define
+00005e00: 6420 6d65 7468 6f64 7320 696e 636c 7564  d methods includ
+00005e10: 696e 6720 7365 7475 7020 616e 6420 5f5f  ing setup and __
+00005e20: 6361 6c6c 5f5f 2074 6f20 656e 666f 7263  call__ to enforc
+00005e30: 650a 2020 2020 2320 6120 6e75 6d62 6572  e.    # a number
+00005e40: 206f 6620 6469 6666 6572 656e 7420 6368   of different ch
+00005e50: 6563 6b73 2061 6e64 2074 6f20 7072 6f76  ecks and to prov
+00005e60: 6964 6520 636c 6561 7220 6572 726f 7220  ide clear error 
+00005e70: 6d65 7373 6167 6573 2e0a 2020 2020 636c  messages..    cl
+00005e80: 732e 5f76 6572 6966 795f 7369 6e67 6c65  s._verify_single
+00005e90: 5f6f 725f 6e6f 5f63 6f6d 7061 6374 2829  _or_no_compact()
+00005ea0: 0a20 2020 2063 6c73 2e5f 7772 6170 5f6d  .    cls._wrap_m
+00005eb0: 6f64 756c 655f 6174 7472 6962 7574 6573  odule_attributes
+00005ec0: 2829 0a20 2020 2023 2053 6574 2065 6d70  ().    # Set emp
+00005ed0: 7479 2063 6c61 7373 2064 6566 6175 6c74  ty class default
+00005ee0: 732e 0a20 2020 2063 6c73 2e5f 7374 6174  s..    cls._stat
+00005ef0: 6520 3d20 5f75 6e69 6e69 7469 616c 697a  e = _uninitializ
+00005f00: 6564 5f6d 6f64 756c 655f 696e 7465 726e  ed_module_intern
+00005f10: 616c 5f73 7461 7465 2020 2320 7479 7065  al_state  # type
+00005f20: 3a20 6967 6e6f 7265 5b61 7474 722d 6465  : ignore[attr-de
+00005f30: 6669 6e65 645d 0a20 2020 2063 6c73 2e73  fined].    cls.s
+00005f40: 636f 7065 3a20 4f70 7469 6f6e 616c 5b53  cope: Optional[S
+00005f50: 636f 7065 5d20 3d20 4e6f 6e65 2020 2320  cope] = None  # 
+00005f60: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00005f70: 2023 2048 616e 646c 6573 2077 6561 6b20   # Handles weak 
+00005f80: 7265 6665 7265 6e63 696e 6720 6f66 2070  referencing of p
+00005f90: 6172 656e 7420 4d6f 6475 6c65 7320 746f  arent Modules to
+00005fa0: 2070 7265 7665 6e74 2072 6566 6572 656e   prevent referen
+00005fb0: 6365 2063 7963 6c65 732e 0a20 2020 2063  ce cycles..    c
+00005fc0: 6c73 2e5f 7061 7265 6e74 5f72 6566 203d  ls._parent_ref =
+00005fd0: 204e 6f6e 6520 2023 2074 7970 653a 2069   None  # type: i
+00005fe0: 676e 6f72 655b 6174 7472 2d64 6566 696e  gnore[attr-defin
+00005ff0: 6564 5d0a 2020 2020 636c 732e 7061 7265  ed].    cls.pare
+00006000: 6e74 203d 2050 6172 656e 7444 6573 6372  nt = ParentDescr
+00006010: 6970 746f 7228 2920 2023 2074 7970 653a  iptor()  # type:
+00006020: 2069 676e 6f72 655b 6173 7369 676e 6d65   ignore[assignme
+00006030: 6e74 5d0a 0a20 2040 636c 6173 736d 6574  nt]..  @classmet
+00006040: 686f 640a 2020 6465 6620 5f63 7573 746f  hod.  def _custo
+00006050: 6d69 7a65 645f 6461 7461 636c 6173 735f  mized_dataclass_
+00006060: 7472 616e 7366 6f72 6d28 636c 732c 206b  transform(cls, k
+00006070: 775f 6f6e 6c79 3a20 626f 6f6c 293a 0a20  w_only: bool):. 
+00006080: 2020 2022 2222 5472 616e 7366 6f72 6d73     """Transforms
+00006090: 2060 636c 7360 2069 6e74 6f20 6120 6461   `cls` into a da
+000060a0: 7461 636c 6173 732c 2077 6974 6820 6375  taclass, with cu
+000060b0: 7374 6f6d 2061 6464 6974 696f 6e61 6c20  stom additional 
+000060c0: 6265 6861 7669 6f72 2e0a 0a20 2020 2031  behavior...    1
+000060d0: 2e20 496e 6a65 6374 2060 7061 7265 6e74  . Inject `parent
+000060e0: 6020 616e 6420 606e 616d 6560 2066 6965  ` and `name` fie
+000060f0: 6c64 732e 2020 2849 6620 7468 6579 2061  lds.  (If they a
+00006100: 7265 2061 6c72 6561 6479 2070 7265 7365  re already prese
+00006110: 6e74 2c0a 2020 2020 2020 2074 6865 6e20  nt,.       then 
+00006120: 6368 6563 6b20 7468 6174 2074 6865 7920  check that they 
+00006130: 6861 7665 2074 6865 2065 7870 6563 7465  have the expecte
+00006140: 6420 7479 7065 732e 290a 2020 2020 322e  d types.).    2.
+00006150: 2053 6574 2063 6f6d 7061 7265 2c20 6861   Set compare, ha
+00006160: 7368 2c20 616e 6420 7265 7072 2074 6f20  sh, and repr to 
+00006170: 4661 6c73 6520 666f 7220 6e6f 6e2d 696e  False for non-in
+00006180: 6974 2066 6965 6c64 732e 0a20 2020 2033  it fields..    3
+00006190: 2e20 4765 6e65 7261 7465 2061 2068 6173  . Generate a has
+000061a0: 6820 6675 6e63 7469 6f6e 2028 6966 206e  h function (if n
+000061b0: 6f74 2070 726f 7669 6465 6420 6279 2063  ot provided by c
+000061c0: 6c73 292e 0a20 2020 2022 2222 0a20 2020  ls)..    """.   
+000061d0: 2023 2043 6865 636b 2072 6573 6572 7665   # Check reserve
+000061e0: 6420 6174 7472 6962 7574 6573 2068 6176  d attributes hav
+000061f0: 6520 6578 7065 6374 6564 2074 7970 6520  e expected type 
+00006200: 616e 6e6f 7461 7469 6f6e 732e 0a20 2020  annotations..   
+00006210: 2061 6e6e 6f74 6174 696f 6e73 203d 2064   annotations = d
+00006220: 6963 7428 636c 732e 5f5f 6469 6374 5f5f  ict(cls.__dict__
+00006230: 2e67 6574 2827 5f5f 616e 6e6f 7461 7469  .get('__annotati
+00006240: 6f6e 735f 5f27 2c20 7b7d 2929 0a20 2020  ons__', {})).   
+00006250: 2069 6620 616e 6e6f 7461 7469 6f6e 732e   if annotations.
+00006260: 6765 7428 2770 6172 656e 7427 2c20 5f50  get('parent', _P
+00006270: 6172 656e 7454 7970 6529 2021 3d20 5f50  arentType) != _P
+00006280: 6172 656e 7454 7970 653a 0a20 2020 2020  arentType:.     
+00006290: 2072 6169 7365 2065 7272 6f72 732e 5265   raise errors.Re
+000062a0: 7365 7276 6564 4d6f 6475 6c65 4174 7472  servedModuleAttr
+000062b0: 6962 7574 6545 7272 6f72 2861 6e6e 6f74  ibuteError(annot
+000062c0: 6174 696f 6e73 290a 2020 2020 6966 2061  ations).    if a
+000062d0: 6e6e 6f74 6174 696f 6e73 2e67 6574 2827  nnotations.get('
+000062e0: 6e61 6d65 272c 2073 7472 2920 6e6f 7420  name', str) not 
+000062f0: 696e 2028 2773 7472 272c 2073 7472 2c20  in ('str', str, 
+00006300: 4f70 7469 6f6e 616c 5b73 7472 5d29 3a0a  Optional[str]):.
+00006310: 2020 2020 2020 7261 6973 6520 6572 726f        raise erro
+00006320: 7273 2e52 6573 6572 7665 644d 6f64 756c  rs.ReservedModul
+00006330: 6541 7474 7269 6275 7465 4572 726f 7228  eAttributeError(
+00006340: 616e 6e6f 7461 7469 6f6e 7329 0a0a 2020  annotations)..  
+00006350: 2020 2320 616e 7920 6e6f 6e2d 696e 6974    # any non-init
+00006360: 2066 6965 6c64 2077 696c 6c20 6f6e 6c79   field will only
+00006370: 2062 6520 7365 7420 696e 2073 6574 7570   be set in setup
+00006380: 0a20 2020 2023 2044 7572 696e 6720 5f5f  .    # During __
+00006390: 6861 7368 5f5f 2061 6e64 205f 5f65 715f  hash__ and __eq_
+000063a0: 5f20 7468 6520 6669 656c 6420 6973 206e  _ the field is n
+000063b0: 6f74 2073 6574 2079 6574 0a20 2020 2023  ot set yet.    #
+000063c0: 2073 6f20 6974 2073 686f 756c 6420 6e6f   so it should no
+000063d0: 7420 6265 2075 7365 6420 696e 2063 6f6d  t be used in com
+000063e0: 7061 7265 2c20 6861 7368 206f 7220 7265  pare, hash or re
+000063f0: 7072 2e0a 2020 2020 666f 7220 6669 656c  pr..    for fiel
+00006400: 6420 696e 2061 6e6e 6f74 6174 696f 6e73  d in annotations
+00006410: 3a0a 2020 2020 2020 6669 656c 645f 6d65  :.      field_me
+00006420: 7461 203d 2067 6574 6174 7472 2863 6c73  ta = getattr(cls
+00006430: 2c20 6669 656c 642c 204e 6f6e 6529 0a20  , field, None). 
+00006440: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00006450: 6365 2866 6965 6c64 5f6d 6574 612c 2064  ce(field_meta, d
+00006460: 6174 6163 6c61 7373 6573 2e46 6965 6c64  ataclasses.Field
+00006470: 2920 616e 6420 6e6f 7420 6669 656c 645f  ) and not field_
+00006480: 6d65 7461 2e69 6e69 743a 0a20 2020 2020  meta.init:.     
+00006490: 2020 2066 6965 6c64 5f6d 6574 612e 636f     field_meta.co
+000064a0: 6d70 6172 6520 3d20 4661 6c73 650a 2020  mpare = False.  
+000064b0: 2020 2020 2020 6669 656c 645f 6d65 7461        field_meta
+000064c0: 2e68 6173 6820 3d20 4661 6c73 650a 2020  .hash = False.  
+000064d0: 2020 2020 2020 6669 656c 645f 6d65 7461        field_meta
+000064e0: 2e72 6570 7220 3d20 4661 6c73 650a 0a20  .repr = False.. 
+000064f0: 2020 2065 7874 7261 5f66 6965 6c64 7320     extra_fields 
+00006500: 3d20 5b0a 2020 2020 2020 2020 280a 2020  = [.        (.  
+00006510: 2020 2020 2020 2020 2020 2770 6172 656e            'paren
+00006520: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+00006530: 5f50 6172 656e 7454 7970 652c 0a20 2020  _ParentType,.   
+00006540: 2020 2020 2020 2020 206b 775f 6f6e 6c79           kw_only
+00006550: 5f64 6174 6163 6c61 7373 6573 2e66 6965  _dataclasses.fie
+00006560: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00006570: 2020 2020 7265 7072 3d46 616c 7365 2c20      repr=False, 
+00006580: 6465 6661 756c 743d 5f75 6e73 7065 6369  default=_unspeci
+00006590: 6669 6564 5f70 6172 656e 742c 206b 775f  fied_parent, kw_
+000065a0: 6f6e 6c79 3d54 7275 650a 2020 2020 2020  only=True.      
+000065b0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+000065c0: 2029 2c0a 2020 2020 2020 2020 280a 2020   ),.        (.  
+000065d0: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+000065e0: 2c0a 2020 2020 2020 2020 2020 2020 4f70  ,.            Op
+000065f0: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
+00006600: 2020 2020 2020 2020 206b 775f 6f6e 6c79           kw_only
+00006610: 5f64 6174 6163 6c61 7373 6573 2e66 6965  _dataclasses.fie
+00006620: 6c64 2864 6566 6175 6c74 3d4e 6f6e 652c  ld(default=None,
+00006630: 206b 775f 6f6e 6c79 3d54 7275 6529 2c0a   kw_only=True),.
+00006640: 2020 2020 2020 2020 292c 0a20 2020 205d          ),.    ]
+00006650: 0a0a 2020 2020 6966 206b 775f 6f6e 6c79  ..    if kw_only
+00006660: 3a0a 2020 2020 2020 6966 2074 7570 6c65  :.      if tuple
+00006670: 2873 7973 2e76 6572 7369 6f6e 5f69 6e66  (sys.version_inf
+00006680: 6f29 5b3a 335d 203e 3d20 2833 2c20 3130  o)[:3] >= (3, 10
+00006690: 2c20 3029 3a0a 2020 2020 2020 2020 666f  , 0):.        fo
+000066a0: 7220 6e61 6d65 2c20 616e 6e6f 7461 7469  r name, annotati
+000066b0: 6f6e 2c20 6465 6661 756c 7420 696e 2065  on, default in e
+000066c0: 7874 7261 5f66 6965 6c64 733a 2020 2320  xtra_fields:  # 
+000066d0: 7079 7479 7065 3a20 6469 7361 626c 653d  pytype: disable=
+000066e0: 696e 7661 6c69 642d 616e 6e6f 7461 7469  invalid-annotati
+000066f0: 6f6e 0a20 2020 2020 2020 2020 2073 6574  on.          set
+00006700: 6174 7472 2863 6c73 2c20 6e61 6d65 2c20  attr(cls, name, 
+00006710: 6465 6661 756c 7429 0a20 2020 2020 2020  default).       
+00006720: 2020 2063 6c73 2e5f 5f61 6e6e 6f74 6174     cls.__annotat
+00006730: 696f 6e73 5f5f 5b6e 616d 655d 203d 2061  ions__[name] = a
+00006740: 6e6e 6f74 6174 696f 6e0a 2020 2020 2020  nnotation.      
+00006750: 2020 6461 7461 636c 6173 7365 732e 6461    dataclasses.da
+00006760: 7461 636c 6173 7328 2020 2320 7479 7065  taclass(  # type
+00006770: 3a20 6967 6e6f 7265 5b63 616c 6c2d 6f76  : ignore[call-ov
+00006780: 6572 6c6f 6164 5d0a 2020 2020 2020 2020  erload].        
+00006790: 2020 2020 756e 7361 6665 5f68 6173 683d      unsafe_hash=
+000067a0: 275f 5f68 6173 685f 5f27 206e 6f74 2069  '__hash__' not i
+000067b0: 6e20 636c 732e 5f5f 6469 6374 5f5f 2c0a  n cls.__dict__,.
+000067c0: 2020 2020 2020 2020 2020 2020 7265 7072              repr
+000067d0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+000067e0: 2020 2020 6b77 5f6f 6e6c 793d 5472 7565      kw_only=True
+000067f0: 2c0a 2020 2020 2020 2020 2928 636c 7329  ,.        )(cls)
+00006800: 0a20 2020 2020 2065 6c73 653a 0a20 2020  .      else:.   
+00006810: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00006820: 7272 6f72 2827 606b 775f 6f6e 6c79 6020  rror('`kw_only` 
+00006830: 6973 206e 6f74 2061 7661 696c 6162 6c65  is not available
+00006840: 2062 6566 6f72 6520 5079 2033 2e31 302e   before Py 3.10.
+00006850: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
+00006860: 2020 2023 204e 6f77 2061 7070 6c79 2064     # Now apply d
+00006870: 6174 6163 6c61 7373 2074 7261 6e73 666f  ataclass transfo
+00006880: 726d 2028 7768 6963 6820 6f70 6572 6174  rm (which operat
+00006890: 6573 2069 6e2d 706c 6163 6529 2e0a 2020  es in-place)..  
+000068a0: 2020 2020 2320 446f 2067 656e 6572 6174      # Do generat
+000068b0: 6520 6120 6861 7368 2066 756e 6374 696f  e a hash functio
+000068c0: 6e20 6f6e 6c79 2069 6620 6e6f 7420 7072  n only if not pr
+000068d0: 6f76 6964 6564 2062 7920 7468 6520 636c  ovided by the cl
+000068e0: 6173 732e 0a20 2020 2020 206b 775f 6f6e  ass..      kw_on
+000068f0: 6c79 5f64 6174 6163 6c61 7373 6573 2e64  ly_dataclasses.d
+00006900: 6174 6163 6c61 7373 280a 2020 2020 2020  ataclass(.      
+00006910: 2020 2020 636c 732c 0a20 2020 2020 2020      cls,.       
+00006920: 2020 2075 6e73 6166 655f 6861 7368 3d27     unsafe_hash='
+00006930: 5f5f 6861 7368 5f5f 2720 6e6f 7420 696e  __hash__' not in
+00006940: 2063 6c73 2e5f 5f64 6963 745f 5f2c 0a20   cls.__dict__,. 
+00006950: 2020 2020 2020 2020 2072 6570 723d 4661           repr=Fa
+00006960: 6c73 652c 0a20 2020 2020 2020 2020 2065  lse,.          e
+00006970: 7874 7261 5f66 6965 6c64 733d 6578 7472  xtra_fields=extr
+00006980: 615f 6669 656c 6473 2c0a 2020 2020 2020  a_fields,.      
+00006990: 2920 2023 2070 7974 7970 653a 2064 6973  )  # pytype: dis
+000069a0: 6162 6c65 3d77 726f 6e67 2d6b 6579 776f  able=wrong-keywo
+000069b0: 7264 2d61 7267 730a 0a20 2020 2063 6c73  rd-args..    cls
+000069c0: 2e5f 5f68 6173 685f 5f20 3d20 5f77 7261  .__hash__ = _wra
+000069d0: 705f 6861 7368 2863 6c73 2e5f 5f68 6173  p_hash(cls.__has
+000069e0: 685f 5f29 2020 2320 7479 7065 3a20 6967  h__)  # type: ig
+000069f0: 6e6f 7265 5b6d 6574 686f 642d 6173 7369  nore[method-assi
+00006a00: 676e 5d0a 0a20 2040 636c 6173 736d 6574  gn]..  @classmet
+00006a10: 686f 640a 2020 6465 6620 5f76 6572 6966  hod.  def _verif
+00006a20: 795f 7369 6e67 6c65 5f6f 725f 6e6f 5f63  y_single_or_no_c
+00006a30: 6f6d 7061 6374 2863 6c73 293a 0a20 2020  ompact(cls):.   
+00006a40: 2022 2222 5374 6174 6963 616c 6c79 2076   """Statically v
+00006a50: 6572 6966 6965 7320 7468 6174 2061 7420  erifies that at 
+00006a60: 6d6f 7374 2061 2073 696e 676c 6520 6d65  most a single me
+00006a70: 7468 6f64 2069 7320 6c61 6265 6c6c 6564  thod is labelled
+00006a80: 2063 6f6d 7061 6374 2e22 2222 0a20 2020   compact.""".   
+00006a90: 206d 6574 686f 6473 203d 205b 6d5b 305d   methods = [m[0]
+00006aa0: 2066 6f72 206d 2069 6e20 696e 7370 6563   for m in inspec
+00006ab0: 742e 6765 746d 656d 6265 7273 2863 6c73  t.getmembers(cls
+00006ac0: 2c20 7072 6564 6963 6174 653d 6361 6c6c  , predicate=call
+00006ad0: 6162 6c65 295d 0a20 2020 206e 5f63 6f6d  able)].    n_com
+00006ae0: 7061 6374 5f66 6e73 203d 206c 656e 280a  pact_fns = len(.
+00006af0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00006b00: 2020 2020 2020 6d65 7468 6f64 5f6e 616d        method_nam
+00006b10: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+00006b20: 7220 6d65 7468 6f64 5f6e 616d 6520 696e  r method_name in
+00006b30: 206d 6574 686f 6473 0a20 2020 2020 2020   methods.       
+00006b40: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00006b50: 6765 7461 7474 7228 636c 732c 206d 6574  getattr(cls, met
+00006b60: 686f 645f 6e61 6d65 292c 2027 636f 6d70  hod_name), 'comp
+00006b70: 6163 7427 290a 2020 2020 2020 2020 5d0a  act').        ].
+00006b80: 2020 2020 290a 2020 2020 6966 206e 5f63      ).    if n_c
+00006b90: 6f6d 7061 6374 5f66 6e73 203e 2031 3a0a  ompact_fns > 1:.
+00006ba0: 2020 2020 2020 7261 6973 6520 6572 726f        raise erro
+00006bb0: 7273 2e4d 756c 7469 706c 654d 6574 686f  rs.MultipleMetho
+00006bc0: 6473 436f 6d70 6163 7445 7272 6f72 2829  dsCompactError()
+00006bd0: 0a0a 2020 4063 6c61 7373 6d65 7468 6f64  ..  @classmethod
+00006be0: 0a20 2064 6566 205f 7772 6170 5f6d 6f64  .  def _wrap_mod
+00006bf0: 756c 655f 6174 7472 6962 7574 6573 2863  ule_attributes(c
+00006c00: 6c73 293a 0a20 2020 2022 2222 5772 6170  ls):.    """Wrap
+00006c10: 7320 7573 6572 2d64 6566 696e 6564 206e  s user-defined n
+00006c20: 6f6e 2d69 6e68 6572 6974 6564 206d 6574  on-inherited met
+00006c30: 686f 6473 2061 6e64 2064 6573 6372 6970  hods and descrip
+00006c40: 746f 7273 2077 6974 6820 7374 6174 650a  tors with state.
+00006c50: 2020 2020 6d61 6e61 6765 6d65 6e74 2066      management f
+00006c60: 756e 6374 696f 6e73 2e0a 2020 2020 2222  unctions..    ""
+00006c70: 220a 2020 2020 2320 7772 6170 206d 6574  ".    # wrap met
+00006c80: 686f 6473 0a20 2020 206d 6574 686f 645f  hods.    method_
+00006c90: 6578 636c 7573 696f 6e73 203d 205b 662e  exclusions = [f.
+00006ca0: 6e61 6d65 2066 6f72 2066 2069 6e20 6461  name for f in da
+00006cb0: 7461 636c 6173 7365 732e 6669 656c 6473  taclasses.fields
+00006cc0: 2863 6c73 295d 202b 205b 0a20 2020 2020  (cls)] + [.     
+00006cd0: 2020 2027 5f5f 6571 5f5f 272c 0a20 2020     '__eq__',.   
+00006ce0: 2020 2020 2027 5f5f 7265 7072 5f5f 272c       '__repr__',
+00006cf0: 0a20 2020 2020 2020 2027 5f5f 696e 6974  .        '__init
+00006d00: 5f5f 272c 0a20 2020 2020 2020 2027 5f5f  __',.        '__
+00006d10: 6861 7368 5f5f 272c 0a20 2020 2020 2020  hash__',.       
+00006d20: 2027 5f5f 706f 7374 5f69 6e69 745f 5f27   '__post_init__'
+00006d30: 2c0a 2020 2020 5d0a 2020 2020 666f 7220  ,.    ].    for 
+00006d40: 6b65 7920 696e 205f 6765 745f 6c6f 6361  key in _get_loca
+00006d50: 6c5f 6d65 7468 6f64 5f6e 616d 6573 2863  l_method_names(c
+00006d60: 6c73 2c20 6578 636c 7564 653d 6d65 7468  ls, exclude=meth
+00006d70: 6f64 5f65 7863 6c75 7369 6f6e 7329 3a0a  od_exclusions):.
+00006d80: 2020 2020 2020 6d65 7468 6f64 203d 2067        method = g
+00006d90: 6574 6174 7472 2863 6c73 2c20 6b65 7929  etattr(cls, key)
+00006da0: 0a20 2020 2020 2069 6620 6861 7361 7474  .      if hasatt
+00006db0: 7228 6d65 7468 6f64 2c20 276e 6f77 7261  r(method, 'nowra
+00006dc0: 7027 293a 0a20 2020 2020 2020 2063 6f6e  p'):.        con
+00006dd0: 7469 6e75 650a 2020 2020 2020 7365 7461  tinue.      seta
+00006de0: 7474 7228 636c 732c 206b 6579 2c20 7772  ttr(cls, key, wr
+00006df0: 6170 5f6d 6574 686f 645f 6f6e 6365 286d  ap_method_once(m
+00006e00: 6574 686f 6429 290a 0a20 2020 2023 2077  ethod))..    # w
+00006e10: 7261 7020 6465 7363 7269 7074 6f72 730a  rap descriptors.
+00006e20: 2020 2020 6465 7363 7269 7074 6f72 5f65      descriptor_e
+00006e30: 7863 6c75 7369 6f6e 7320 3d20 5b66 2e6e  xclusions = [f.n
+00006e40: 616d 6520 666f 7220 6620 696e 2064 6174  ame for f in dat
+00006e50: 6163 6c61 7373 6573 2e66 6965 6c64 7328  aclasses.fields(
+00006e60: 636c 7329 5d20 2b20 5b0a 2020 2020 2020  cls)] + [.      
+00006e70: 2020 2770 6172 656e 7427 2c0a 2020 2020    'parent',.    
+00006e80: 2020 2020 275f 5f64 6963 745f 5f27 2c0a      '__dict__',.
+00006e90: 2020 2020 5d0a 2020 2020 666f 7220 6b65      ].    for ke
+00006ea0: 7920 696e 205f 6765 745f 6c6f 6361 6c5f  y in _get_local_
+00006eb0: 6465 7363 7269 7074 6f72 5f6e 616d 6573  descriptor_names
+00006ec0: 2863 6c73 2c20 6465 7363 7269 7074 6f72  (cls, descriptor
+00006ed0: 5f65 7863 6c75 7369 6f6e 7329 3a0a 2020  _exclusions):.  
+00006ee0: 2020 2020 2320 646f 6e27 7420 7573 6520      # don't use 
+00006ef0: 6765 7461 7474 7220 6865 7265 2c20 7369  getattr here, si
+00006f00: 6e63 6520 6974 2077 696c 6c20 6361 6c6c  nce it will call
+00006f10: 2074 6865 2064 6573 6372 6970 746f 720a   the descriptor.
+00006f20: 2020 2020 2020 6465 7363 7269 7074 6f72        descriptor
+00006f30: 203d 2063 6c73 2e5f 5f64 6963 745f 5f5b   = cls.__dict__[
+00006f40: 6b65 795d 0a20 2020 2020 2069 6620 6861  key].      if ha
+00006f50: 7361 7474 7228 6465 7363 7269 7074 6f72  sattr(descriptor
+00006f60: 2c20 276e 6f77 7261 7027 293a 0a20 2020  , 'nowrap'):.   
+00006f70: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00006f80: 2020 2020 7365 7461 7474 7228 636c 732c      setattr(cls,
+00006f90: 206b 6579 2c20 7772 6170 5f64 6573 6372   key, wrap_descr
+00006fa0: 6970 746f 725f 6f6e 6365 2864 6573 6372  iptor_once(descr
+00006fb0: 6970 746f 7229 290a 2020 2020 7265 7475  iptor)).    retu
+00006fc0: 726e 2063 6c73 0a0a 2020 6465 6620 5f63  rn cls..  def _c
+00006fd0: 616c 6c5f 7772 6170 7065 645f 6d65 7468  all_wrapped_meth
+00006fe0: 6f64 2873 656c 662c 2066 756e 2c20 6172  od(self, fun, ar
+00006ff0: 6773 2c20 6b77 6172 6773 293a 0a20 2020  gs, kwargs):.   
+00007000: 2022 2222 2022 4361 6c6c 7320 6120 7772   """ "Calls a wr
+00007010: 6170 7065 6420 6d65 7468 6f64 2e0a 0a20  apped method... 
+00007020: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+00007030: 2069 7320 7265 7370 6f6e 7369 626c 6520   is responsible 
+00007040: 666f 7220 7365 7474 696e 6720 7570 2074  for setting up t
+00007050: 6865 2074 6872 6561 6420 6c6f 6361 6c20  he thread local 
+00007060: 7374 6174 650a 2020 2020 636f 7272 6563  state.    correc
+00007070: 746c 7920 6265 666f 7265 2063 616c 6c69  tly before calli
+00007080: 6e67 2074 6865 206d 6574 686f 6420 616e  ng the method an
+00007090: 6420 636c 6561 6e69 6e67 2075 7020 6166  d cleaning up af
+000070a0: 7465 7277 6172 6473 2e0a 2020 2020 5468  terwards..    Th
+000070b0: 6973 2069 6e63 6c75 6465 7320 7374 6f72  is includes stor
+000070c0: 696e 6720 696e 7465 726d 6564 6961 7465  ing intermediate
+000070d0: 732c 2073 6574 7570 206f 6620 7468 6520  s, setup of the 
+000070e0: 636f 6d70 6163 7420 7363 6f70 652c 0a20  compact scope,. 
+000070f0: 2020 2061 6e64 206d 616b 696e 6720 7375     and making su
+00007100: 7265 2073 6574 7570 2069 7320 6361 6c6c  re setup is call
+00007110: 6564 2062 6566 6f72 6520 616e 7920 6f74  ed before any ot
+00007120: 6865 7220 6d65 7468 6f64 2e0a 0a20 2020  her method...   
+00007130: 2041 7267 733a 0a20 2020 2020 2066 756e   Args:.      fun
+00007140: 3a20 5468 6520 7772 6170 7065 6420 6d65  : The wrapped me
+00007150: 7468 6f64 2e0a 2020 2020 2020 6172 6773  thod..      args
+00007160: 3a20 4e61 6d65 6420 6172 6775 6d65 6e74  : Named argument
+00007170: 7320 7061 7373 6564 2074 6f20 6060 6675  s passed to ``fu
+00007180: 6e60 602e 0a20 2020 2020 206b 7761 7267  n``..      kwarg
+00007190: 733a 204b 6579 776f 7264 2061 7267 756d  s: Keyword argum
+000071a0: 656e 7473 2070 6173 7365 6420 746f 2060  ents passed to `
+000071b0: 6066 756e 6060 2e0a 0a20 2020 2052 6574  `fun``...    Ret
+000071c0: 7572 6e73 3a0a 2020 2020 2020 5468 6520  urns:.      The 
+000071d0: 7265 7375 6c74 7320 6f66 2063 616c 6c69  results of calli
+000071e0: 6e67 2060 6066 756e 6060 2e0a 2020 2020  ng ``fun``..    
+000071f0: 2222 220a 2020 2020 6973 5f63 6f6d 7061  """.    is_compa
+00007200: 6374 5f6d 6574 686f 6420 3d20 6861 7361  ct_method = hasa
+00007210: 7474 7228 6675 6e2c 2027 636f 6d70 6163  ttr(fun, 'compac
+00007220: 7427 290a 2020 2020 6675 6e5f 6e61 6d65  t').    fun_name
+00007230: 203d 2067 6574 6174 7472 2866 756e 2c20   = getattr(fun, 
+00007240: 275f 5f6e 616d 655f 5f27 2c20 2775 6e6e  '__name__', 'unn
+00007250: 616d 6564 5f66 756e 6374 696f 6e27 290a  amed_function').
+00007260: 2020 2020 6973 5f73 6574 7570 5f6d 6574      is_setup_met
+00007270: 686f 6420 3d20 6675 6e5f 6e61 6d65 203d  hod = fun_name =
+00007280: 3d20 2773 6574 7570 270a 2020 2020 6164  = 'setup'.    ad
+00007290: 645f 6361 6c6c 5f69 6e66 6f20 3d20 6e6f  d_call_info = no
+000072a0: 7420 6973 5f73 6574 7570 5f6d 6574 686f  t is_setup_metho
+000072b0: 6420 616e 6420 6c65 6e28 5f63 6f6e 7465  d and len(_conte
+000072c0: 7874 2e63 616c 6c5f 696e 666f 5f73 7461  xt.call_info_sta
+000072d0: 636b 2920 3e20 300a 2020 2020 2320 5765  ck) > 0.    # We
+000072e0: 206c 617a 696c 7920 6361 6c6c 2073 6574   lazily call set
+000072f0: 7570 2829 206f 6e6c 7920 7768 656e 206e  up() only when n
+00007300: 6565 6465 642e 0a20 2020 2069 6620 6973  eeded..    if is
+00007310: 5f73 6574 7570 5f6d 6574 686f 643a 0a20  _setup_method:. 
+00007320: 2020 2020 2069 6620 7365 6c66 2e73 636f       if self.sco
+00007330: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+00007340: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
+00007350: 2e43 616c 6c53 6574 7570 556e 626f 756e  .CallSetupUnboun
+00007360: 644d 6f64 756c 6545 7272 6f72 2829 0a20  dModuleError(). 
+00007370: 2020 2020 2069 735f 7265 6375 7272 656e       is_recurren
+00007380: 7420 3d20 7365 6c66 2e5f 7374 6174 652e  t = self._state.
+00007390: 696e 5f73 6574 7570 0a20 2020 2020 2073  in_setup.      s
+000073a0: 656c 662e 5f73 7461 7465 2e69 6e5f 7365  elf._state.in_se
+000073b0: 7475 7020 3d20 5472 7565 0a20 2020 2065  tup = True.    e
+000073c0: 6c73 653a 0a20 2020 2020 2073 656c 662e  lse:.      self.
+000073d0: 5f74 7279 5f73 6574 7570 2829 0a0a 2020  _try_setup()..  
+000073e0: 2020 6966 2069 735f 636f 6d70 6163 745f    if is_compact_
+000073f0: 6d65 7468 6f64 3a0a 2020 2020 2020 6966  method:.      if
+00007400: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
+00007410: 6f6e 653a 0a20 2020 2020 2020 2072 6169  one:.        rai
+00007420: 7365 2065 7272 6f72 732e 4361 6c6c 436f  se errors.CallCo
+00007430: 6d70 6163 7455 6e62 6f75 6e64 4d6f 6475  mpactUnboundModu
+00007440: 6c65 4572 726f 7228 290a 2020 2020 2020  leError().      
+00007450: 6973 5f72 6563 7572 7265 6e74 203d 2073  is_recurrent = s
+00007460: 656c 662e 5f73 7461 7465 2e69 6e5f 636f  elf._state.in_co
+00007470: 6d70 6163 745f 6d65 7468 6f64 0a20 2020  mpact_method.   
+00007480: 2020 2073 656c 662e 5f73 7461 7465 2e69     self._state.i
+00007490: 6e5f 636f 6d70 6163 745f 6d65 7468 6f64  n_compact_method
+000074a0: 203d 2054 7275 650a 2020 2020 5f63 6f6e   = True.    _con
+000074b0: 7465 7874 2e6d 6f64 756c 655f 7374 6163  text.module_stac
+000074c0: 6b2e 6170 7065 6e64 2873 656c 6629 0a20  k.append(self). 
+000074d0: 2020 2074 7279 3a0a 2020 2020 2020 2320     try:.      # 
+000074e0: 6765 7420 6361 6c6c 2069 6e66 6f0a 2020  get call info.  
+000074f0: 2020 2020 6966 2061 6464 5f63 616c 6c5f      if add_call_
+00007500: 696e 666f 3a0a 2020 2020 2020 2020 6173  info:.        as
+00007510: 7365 7274 2073 656c 662e 7363 6f70 6520  sert self.scope 
+00007520: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00007530: 2020 2020 6361 6c6c 5f69 6e64 6578 203d      call_index =
+00007540: 205f 636f 6e74 6578 742e 6361 6c6c 5f69   _context.call_i
+00007550: 6e66 6f5f 7374 6163 6b5b 2d31 5d2e 6765  nfo_stack[-1].ge
+00007560: 745f 6361 6c6c 5f69 6e64 6578 2873 656c  t_call_index(sel
+00007570: 6629 0a20 2020 2020 2020 2073 636f 7065  f).        scope
+00007580: 5f70 6174 6820 3d20 6a61 782e 7472 6565  _path = jax.tree
+00007590: 5f75 7469 6c2e 7472 6565 5f6d 6170 285f  _util.tree_map(_
+000075a0: 6669 785f 7061 7468 5f70 6172 742c 2073  fix_path_part, s
+000075b0: 656c 662e 7363 6f70 652e 7061 7468 290a  elf.scope.path).
+000075c0: 0a20 2020 2020 2023 2063 616c 6c20 6d65  .      # call me
+000075d0: 7468 6f64 0a20 2020 2020 2069 6620 5f75  thod.      if _u
+000075e0: 7365 5f6e 616d 6564 5f63 616c 6c3a 0a20  se_named_call:. 
+000075f0: 2020 2020 2020 2077 6974 6820 6a61 782e         with jax.
+00007600: 6e61 6d65 645f 7363 6f70 6528 5f64 6572  named_scope(_der
+00007610: 6976 655f 7072 6f66 696c 696e 675f 6e61  ive_profiling_na
+00007620: 6d65 2873 656c 662c 2066 756e 2929 3a0a  me(self, fun)):.
+00007630: 2020 2020 2020 2020 2020 7920 3d20 6675            y = fu
+00007640: 6e28 7365 6c66 2c20 2a61 7267 732c 202a  n(self, *args, *
+00007650: 2a6b 7761 7267 7329 0a20 2020 2020 2065  *kwargs).      e
+00007660: 6c73 653a 0a20 2020 2020 2020 2079 203d  lse:.        y =
+00007670: 2066 756e 2873 656c 662c 202a 6172 6773   fun(self, *args
+00007680: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+00007690: 2020 2069 6620 5f63 6f6e 7465 7874 2e63     if _context.c
+000076a0: 6170 7475 7265 5f73 7461 636b 3a0a 2020  apture_stack:.  
+000076b0: 2020 2020 2020 6669 6c74 6572 5f66 6e20        filter_fn 
+000076c0: 3d20 5f63 6f6e 7465 7874 2e63 6170 7475  = _context.captu
+000076d0: 7265 5f73 7461 636b 5b2d 315d 0a20 2020  re_stack[-1].   
+000076e0: 2020 2020 2069 6620 6669 6c74 6572 5f66       if filter_f
+000076f0: 6e20 616e 6420 6669 6c74 6572 5f66 6e28  n and filter_fn(
+00007700: 7365 6c66 2c20 6675 6e5f 6e61 6d65 293a  self, fun_name):
+00007710: 0a20 2020 2020 2020 2020 2073 656c 662e  .          self.
+00007720: 736f 7728 2769 6e74 6572 6d65 6469 6174  sow('intermediat
+00007730: 6573 272c 2066 756e 5f6e 616d 652c 2079  es', fun_name, y
+00007740: 290a 2020 2020 2020 6966 2061 6464 5f63  ).      if add_c
+00007750: 616c 6c5f 696e 666f 3a0a 2020 2020 2020  all_info:.      
+00007760: 2020 5f61 7267 732c 205f 6b77 6172 6773    _args, _kwargs
+00007770: 2c20 5f79 203d 2066 6c61 782e 6c69 6e65  , _y = flax.line
+00007780: 6e2e 7375 6d6d 6172 792e 5f72 6570 7265  n.summary._repre
+00007790: 7365 6e74 5f74 7265 6528 0a20 2020 2020  sent_tree(.     
+000077a0: 2020 2020 2020 2028 6172 6773 2c20 6b77         (args, kw
+000077b0: 6172 6773 2c20 7929 0a20 2020 2020 2020  args, y).       
+000077c0: 2029 0a20 2020 2020 2020 205f 636f 6e74   ).        _cont
+000077d0: 6578 742e 6361 6c6c 5f69 6e66 6f5f 7374  ext.call_info_st
+000077e0: 6163 6b5b 2d31 5d2e 6361 6c6c 732e 6170  ack[-1].calls.ap
+000077f0: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00007800: 2020 5f43 616c 6c49 6e66 6f28 0a20 2020    _CallInfo(.   
+00007810: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+00007820: 6c5f 696e 6465 782c 0a20 2020 2020 2020  l_index,.       
+00007830: 2020 2020 2020 2020 2073 636f 7065 5f70           scope_p
+00007840: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+00007850: 2020 2020 2074 7970 6528 7365 6c66 292c       type(self),
+00007860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007870: 2066 756e 2e5f 5f6e 616d 655f 5f2c 0a20   fun.__name__,. 
+00007880: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00007890: 6172 6773 2c0a 2020 2020 2020 2020 2020  args,.          
+000078a0: 2020 2020 2020 5f6b 7761 7267 732c 0a20        _kwargs,. 
+000078b0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000078c0: 792c 0a20 2020 2020 2020 2020 2020 2029  y,.            )
+000078d0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000078e0: 2072 6574 7572 6e20 790a 2020 2020 6669   return y.    fi
+000078f0: 6e61 6c6c 793a 0a20 2020 2020 205f 636f  nally:.      _co
+00007900: 6e74 6578 742e 6d6f 6475 6c65 5f73 7461  ntext.module_sta
+00007910: 636b 2e70 6f70 2829 0a20 2020 2020 2069  ck.pop().      i
+00007920: 6620 6973 5f63 6f6d 7061 6374 5f6d 6574  f is_compact_met
+00007930: 686f 643a 0a20 2020 2020 2020 206f 626a  hod:.        obj
+00007940: 6563 742e 5f5f 7365 7461 7474 725f 5f28  ect.__setattr__(
+00007950: 7365 6c66 2c20 2773 636f 7065 272c 2073  self, 'scope', s
+00007960: 656c 662e 7363 6f70 652e 7265 776f 756e  elf.scope.rewoun
+00007970: 6428 2929 0a20 2020 2020 2023 2073 6574  d()).      # set
+00007980: 7570 206f 7220 636f 6d70 6163 7420 6361  up or compact ca
+00007990: 6c6c 7320 6361 6e20 6265 2072 6563 7572  lls can be recur
+000079a0: 7265 6e74 2066 6f72 2065 7861 6d70 6c65  rent for example
+000079b0: 2064 7565 2074 6f20 7375 7065 7220 6361   due to super ca
+000079c0: 6c6c 730a 2020 2020 2020 2320 7265 7365  lls.      # rese
+000079d0: 7474 696e 6720 7468 6520 7374 6174 6520  tting the state 
+000079e0: 776f 756c 6420 6361 7573 6520 6973 2063  would cause is c
+000079f0: 6f6d 7061 6374 2f73 6574 7570 206d 6574  ompact/setup met
+00007a00: 686f 640a 2020 2020 2020 2320 746f 2062  hod.      # to b
+00007a10: 6520 7365 7420 746f 2046 616c 7365 2070  e set to False p
+00007a20: 7265 6d61 7475 7265 6c79 2e0a 2020 2020  rematurely..    
+00007a30: 2020 6966 2028 6973 5f63 6f6d 7061 6374    if (is_compact
+00007a40: 5f6d 6574 686f 6420 6f72 2069 735f 7365  _method or is_se
+00007a50: 7475 705f 6d65 7468 6f64 2920 616e 6420  tup_method) and 
+00007a60: 6e6f 7420 6973 5f72 6563 7572 7265 6e74  not is_recurrent
+00007a70: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00007a80: 7374 6174 652e 7265 7365 7428 290a 0a20  state.reset().. 
+00007a90: 2064 6566 205f 5f73 6574 6174 7472 5f5f   def __setattr__
+00007aa0: 2873 656c 662c 206e 616d 653a 2073 7472  (self, name: str
+00007ab0: 2c20 7661 6c3a 2041 6e79 293a 0a20 2020  , val: Any):.   
+00007ac0: 2022 2222 5365 7473 2061 6e20 6174 7472   """Sets an attr
+00007ad0: 6962 7574 6520 6f6e 2074 6869 7320 4d6f  ibute on this Mo
+00007ae0: 6475 6c65 2e0a 0a20 2020 2057 6520 6f76  dule...    We ov
+00007af0: 6572 6c6f 6164 2073 6574 6174 7472 2073  erload setattr s
+00007b00: 6f6c 656c 7920 746f 2073 7570 706f 7274  olely to support
+00007b10: 2070 7974 686f 6e69 6320 6e61 6d69 6e67   pythonic naming
+00007b20: 2076 6961 2061 7373 6967 6e6d 656e 7420   via assignment 
+00007b30: 6f66 0a20 2020 2073 7562 6d6f 6475 6c65  of.    submodule
+00007b40: 7320 696e 2074 6865 2073 7065 6369 616c  s in the special
+00007b50: 203a 6d65 7468 3a60 7365 7475 7060 2066   :meth:`setup` f
+00007b60: 756e 6374 696f 6e3a 3a0a 0a20 2020 2020  unction::..     
+00007b70: 2073 656c 662e 7375 626d 6f64 756c 655f   self.submodule_
+00007b80: 6e61 6d65 203d 204d 794d 6f64 756c 6528  name = MyModule(
+00007b90: 2e2e 2e29 0a0a 2020 2020 5765 2061 6c73  ...)..    We als
+00007ba0: 6f20 7375 7070 6f72 7420 6c69 7374 7320  o support lists 
+00007bb0: 616e 6420 6f74 6865 7220 6765 6e65 7261  and other genera
+00007bc0: 6c20 7079 7472 6565 732c 2065 2e67 2e3a  l pytrees, e.g.:
+00007bd0: 3a0a 0a20 2020 2020 2073 656c 662e 7375  :..      self.su
+00007be0: 626d 6f64 756c 6573 203d 205b 4d79 4d6f  bmodules = [MyMo
+00007bf0: 6475 6c65 3028 2e2e 292c 204d 794d 6f64  dule0(..), MyMod
+00007c00: 756c 6531 282e 2e29 2c20 2e2e 2e5d 0a0a  ule1(..), ...]..
+00007c10: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00007c20: 6e61 6d65 3a20 4174 7472 6962 7574 6520  name: Attribute 
+00007c30: 746f 2073 6574 2e0a 2020 2020 2020 7661  to set..      va
+00007c40: 6c3a 2056 616c 7565 206f 6620 7468 6520  l: Value of the 
+00007c50: 6174 7472 6962 7574 652e 0a20 2020 2022  attribute..    "
+00007c60: 2222 0a20 2020 2066 6965 6c64 7320 3d20  "".    fields = 
+00007c70: 7365 6c66 2e5f 5f64 6174 6163 6c61 7373  self.__dataclass
+00007c80: 5f66 6965 6c64 735f 5f20 2023 2070 7974  _fields__  # pyt
+00007c90: 7970 653a 2064 6973 6162 6c65 3d61 7474  ype: disable=att
+00007ca0: 7269 6275 7465 2d65 7272 6f72 0a20 2020  ribute-error.   
+00007cb0: 2069 735f 6461 7461 636c 6173 735f 6174   is_dataclass_at
+00007cc0: 7472 203d 206e 616d 6520 696e 2066 6965  tr = name in fie
+00007cd0: 6c64 7320 616e 6420 6669 656c 6473 5b6e  lds and fields[n
+00007ce0: 616d 655d 2e69 6e69 740a 0a20 2020 2069  ame].init..    i
+00007cf0: 6620 6e6f 7420 7365 6c66 2e5f 7374 6174  f not self._stat
+00007d00: 652e 696e 5f73 6574 7570 3a0a 2020 2020  e.in_setup:.    
+00007d10: 2020 6966 206e 6f74 2073 656c 662e 5f73    if not self._s
+00007d20: 7461 7465 2e69 735f 696e 6974 6961 6c69  tate.is_initiali
+00007d30: 7a65 643a 0a20 2020 2020 2020 2023 2053  zed:.        # S
+00007d40: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
+00007d50: 7320 6265 666f 7265 2065 6e64 206f 6620  s before end of 
+00007d60: 4d6f 6475 6c65 2e5f 5f70 6f73 745f 696e  Module.__post_in
+00007d70: 6974 5f5f 2829 0a20 2020 2020 2020 206f  it__().        o
+00007d80: 626a 6563 742e 5f5f 7365 7461 7474 725f  bject.__setattr_
+00007d90: 5f28 7365 6c66 2c20 6e61 6d65 2c20 7661  _(self, name, va
+00007da0: 6c29 0a20 2020 2020 2020 2072 6574 7572  l).        retur
+00007db0: 6e0a 2020 2020 2020 656c 7365 3a0a 2020  n.      else:.  
+00007dc0: 2020 2020 2020 2320 5765 2772 6520 7061        # We're pa
+00007dd0: 7374 2061 6c6c 2069 6e69 7469 616c 697a  st all initializ
+00007de0: 6174 696f 6e20 616e 6420 7365 7475 7020  ation and setup 
+00007df0: 6c6f 6769 633a 0a20 2020 2020 2020 2023  logic:.        #
+00007e00: 2052 6169 7365 7320 6120 5479 7065 4572   Raises a TypeEr
+00007e10: 726f 7220 6a75 7374 206c 696b 6520 6672  ror just like fr
+00007e20: 6f7a 656e 2070 7974 686f 6e20 6461 7461  ozen python data
+00007e30: 636c 6173 7365 732e 0a20 2020 2020 2020  classes..       
+00007e40: 2072 6169 7365 2065 7272 6f72 732e 5365   raise errors.Se
+00007e50: 7441 7474 7269 6275 7465 4672 6f7a 656e  tAttributeFrozen
+00007e60: 4d6f 6475 6c65 4572 726f 7228 0a20 2020  ModuleError(.   
+00007e70: 2020 2020 2020 2020 2073 656c 662e 5f5f           self.__
+00007e80: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00007e90: 2c20 6e61 6d65 2c20 7661 6c0a 2020 2020  , name, val.    
+00007ea0: 2020 2020 290a 0a20 2020 2023 2057 6527      )..    # We'
+00007eb0: 7265 2069 6e73 6964 6520 7468 6520 7365  re inside the se
+00007ec0: 7475 7028 2920 6d65 7468 6f64 3a0a 2020  tup() method:.  
+00007ed0: 2020 6966 2069 735f 6461 7461 636c 6173    if is_dataclas
+00007ee0: 735f 6174 7472 3a0a 2020 2020 2020 2320  s_attr:.      # 
+00007ef0: 5468 6573 6520 6e61 6d65 7320 6172 6520  These names are 
+00007f00: 7370 6563 6966 6965 6420 6173 2064 6174  specified as dat
+00007f10: 6163 6c61 7373 2066 6965 6c64 732e 2054  aclass fields. T
+00007f20: 6865 7920 7368 6f75 6c64 206e 6f74 2062  hey should not b
+00007f30: 650a 2020 2020 2020 2320 696e 6974 6961  e.      # initia
+00007f40: 6c69 7a65 6420 7769 7468 696e 2074 6865  lized within the
+00007f50: 2073 6574 7570 2829 206d 6574 686f 642c   setup() method,
+00007f60: 2062 7574 2063 616e 2062 6520 6d6f 6469   but can be modi
+00007f70: 6669 6564 2066 7265 656c 790a 2020 2020  fied freely.    
+00007f80: 2020 2320 6265 666f 7265 2069 742e 0a20    # before it.. 
+00007f90: 2020 2020 2072 6169 7365 2065 7272 6f72       raise error
+00007fa0: 732e 5365 7441 7474 7269 6275 7465 496e  s.SetAttributeIn
+00007fb0: 4d6f 6475 6c65 5365 7475 7045 7272 6f72  ModuleSetupError
+00007fc0: 2829 0a0a 2020 2020 2320 5661 6c75 6573  ()..    # Values
+00007fd0: 2028 7468 6174 206d 6179 2062 6520 7661   (that may be va
+00007fe0: 7269 6162 6c65 7320 6f72 2073 7562 6d6f  riables or submo
+00007ff0: 6475 6c65 7329 2061 7265 2062 6569 6e67  dules) are being
+00008000: 2064 6566 696e 6564 2061 6e64 0a20 2020   defined and.   
+00008010: 2023 2061 7474 6163 6865 6420 696e 2073   # attached in s
+00008020: 6574 7570 2829 2c20 7765 2072 756e 2073  etup(), we run s
+00008030: 6f6d 6520 6578 7472 6120 6c6f 6769 6320  ome extra logic 
+00008040: 696e 2074 6861 7420 6361 7365 2e0a 2020  in that case..  
+00008050: 2020 7365 6c66 2e5f 7265 6769 7374 6572    self._register
+00008060: 5f73 7562 6d6f 6475 6c65 7328 6e61 6d65  _submodules(name
+00008070: 2c20 7661 6c29 0a0a 2020 6465 6620 5f5f  , val)..  def __
+00008080: 6765 7461 7474 725f 5f28 7365 6c66 2c20  getattr__(self, 
+00008090: 6e61 6d65 3a20 7374 7229 202d 3e20 416e  name: str) -> An
+000080a0: 793a 0a20 2020 2022 2222 4361 6c6c 2073  y:.    """Call s
+000080b0: 6574 7570 2829 2062 6566 6f72 6520 6765  etup() before ge
+000080c0: 7474 696e 6720 616e 7920 7365 7475 702d  tting any setup-
+000080d0: 6465 6669 6e65 6420 6174 7472 6962 7574  defined attribut
+000080e0: 6573 2e22 2222 0a20 2020 2023 2057 6520  es.""".    # We 
+000080f0: 646f 6e27 7420 7761 6e74 2074 6f20 7265  don't want to re
+00008100: 7475 726e 2061 6e79 7468 696e 6720 666f  turn anything fo
+00008110: 7220 7079 7468 6f6e 2063 6f70 7920 2f20  r python copy / 
+00008120: 7069 636b 6c65 206d 6574 686f 6473 2e0a  pickle methods..
+00008130: 2020 2020 6966 206e 616d 6520 696e 205f      if name in _
+00008140: 554e 4445 4649 4e45 445f 434f 5059 5f50  UNDEFINED_COPY_P
+00008150: 4943 4b4c 455f 4d45 5448 4f44 533a 0a20  ICKLE_METHODS:. 
+00008160: 2020 2020 2072 6169 7365 2041 7474 7269       raise Attri
+00008170: 6275 7465 4572 726f 7228 290a 2020 2020  buteError().    
+00008180: 7365 6c66 2e5f 7472 795f 7365 7475 7028  self._try_setup(
+00008190: 290a 2020 2020 6966 206e 616d 6520 696e  ).    if name in
+000081a0: 2073 656c 662e 5f5f 6469 6374 5f5f 3a0a   self.__dict__:.
+000081b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000081c0: 662e 5f5f 6469 6374 5f5f 5b6e 616d 655d  f.__dict__[name]
+000081d0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000081e0: 206d 7367 203d 2066 2722 7b73 656c 662e   msg = f'"{self.
+000081f0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
+00008200: 5f5f 7d22 206f 626a 6563 7420 6861 7320  __}" object has 
+00008210: 6e6f 2061 7474 7269 6275 7465 2022 7b6e  no attribute "{n
+00008220: 616d 657d 222e 270a 2020 2020 2020 6966  ame}".'.      if
+00008230: 2073 656c 662e 7363 6f70 6520 6973 204e   self.scope is N
+00008240: 6f6e 653a 0a20 2020 2020 2020 206d 7367  one:.        msg
+00008250: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
+00008260: 2020 6627 2049 6620 227b 6e61 6d65 7d22    f' If "{name}"
+00008270: 2069 7320 6465 6669 6e65 6420 696e 205c   is defined in \
+00008280: 272e 7365 7475 7028 295c 272c 2072 656d  '.setup()\', rem
+00008290: 656d 6265 7220 7468 6573 6520 6669 656c  ember these fiel
+000082a0: 6473 2027 0a20 2020 2020 2020 2020 2020  ds '.           
+000082b0: 2022 6172 6520 6f6e 6c79 2061 6363 6573   "are only acces
+000082c0: 7369 626c 6520 6672 6f6d 2069 6e73 6964  sible from insid
+000082d0: 6520 2769 6e69 7427 206f 7220 2761 7070  e 'init' or 'app
+000082e0: 6c79 272e 220a 2020 2020 2020 2020 290a  ly'.".        ).
+000082f0: 2020 2020 2020 7261 6973 6520 4174 7472        raise Attr
+00008300: 6962 7574 6545 7272 6f72 286d 7367 290a  ibuteError(msg).
+00008310: 0a20 2064 6566 205f 5f64 6972 5f5f 2873  .  def __dir__(s
+00008320: 656c 6629 202d 3e20 4c69 7374 5b73 7472  elf) -> List[str
+00008330: 5d3a 0a20 2020 2022 2222 4361 6c6c 2073  ]:.    """Call s
+00008340: 6574 7570 2829 2062 6566 6f72 6520 6c69  etup() before li
+00008350: 7374 696e 6720 6174 7472 6962 7574 6573  sting attributes
+00008360: 2e22 2222 0a20 2020 2073 656c 662e 5f74  .""".    self._t
+00008370: 7279 5f73 6574 7570 2829 0a20 2020 2072  ry_setup().    r
+00008380: 6574 7572 6e20 6f62 6a65 6374 2e5f 5f64  eturn object.__d
+00008390: 6972 5f5f 2873 656c 6629 2020 2320 7479  ir__(self)  # ty
+000083a0: 7065 3a20 6967 6e6f 7265 0a0a 2020 6465  pe: ignore..  de
+000083b0: 6620 5f5f 706f 7374 5f69 6e69 745f 5f28  f __post_init__(
+000083c0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000083d0: 2020 2023 2044 4f20 4e4f 5420 5245 4d4f     # DO NOT REMO
+000083e0: 5645 202d 204d 6172 6b65 7220 666f 7220  VE - Marker for 
+000083f0: 696e 7465 726e 616c 206c 6f67 6769 6e67  internal logging
+00008400: 2e0a 2020 2020 2320 496e 2064 6174 6163  ..    # In datac
+00008410: 6c61 7373 6573 2c20 5f5f 696e 6974 5f5f  lasses, __init__
+00008420: 2069 7320 6f76 6572 7269 6464 656e 2074   is overridden t
+00008430: 6f20 7072 6f63 6573 7320 6461 7461 636c  o process datacl
+00008440: 6173 7320 6172 6775 6d65 6e74 732c 0a20  ass arguments,. 
+00008450: 2020 2023 2061 6e64 205f 5f70 6f73 745f     # and __post_
+00008460: 696e 6974 5f5f 2069 7320 6361 6c6c 6564  init__ is called
+00008470: 2069 6d6d 6564 6961 7465 6c79 2061 6674   immediately aft
+00008480: 6572 7761 7264 732e 2048 6572 652c 2064  erwards. Here, d
+00008490: 6570 656e 6469 6e67 206f 6e20 7468 650a  epending on the.
+000084a0: 2020 2020 2320 7479 7065 206f 6620 6070      # type of `p
+000084b0: 6172 656e 7460 2070 6173 7365 6420 746f  arent` passed to
+000084c0: 2069 6e69 7469 616c 697a 6520 7468 6520   initialize the 
+000084d0: 4d6f 6475 6c65 2c20 7765 2065 6974 6865  Module, we eithe
+000084e0: 7220 6465 6665 720a 2020 2020 2320 696e  r defer.    # in
+000084f0: 6974 6961 6c69 7a61 7469 6f6e 2c20 6174  itialization, at
+00008500: 7461 6368 2074 6869 7320 4d6f 6475 6c65  tach this Module
+00008510: 2061 7320 6120 7375 626d 6f64 756c 6520   as a submodule 
+00008520: 6f66 2061 2070 6172 656e 742c 206f 7220  of a parent, or 
+00008530: 6269 6e64 0a20 2020 2023 2074 6869 7320  bind.    # this 
+00008540: 4d6f 6475 6c65 2061 7420 7468 6520 746f  Module at the to
+00008550: 702d 6c65 7665 6c20 746f 2076 6172 6961  p-level to varia
+00008560: 626c 6573 2061 6e64 2072 6e67 732e 0a0a  bles and rngs...
+00008570: 2020 2020 6f62 6a65 6374 2e5f 5f73 6574      object.__set
+00008580: 6174 7472 5f5f 2873 656c 662c 2027 5f69  attr__(self, '_i
+00008590: 6427 2c20 7575 6964 2829 290a 2020 2020  d', uuid()).    
+000085a0: 6f62 6a65 6374 2e5f 5f73 6574 6174 7472  object.__setattr
+000085b0: 5f5f 2873 656c 662c 2027 5f73 7461 7465  __(self, '_state
+000085c0: 272c 205f 4d6f 6475 6c65 496e 7465 726e  ', _ModuleIntern
+000085d0: 616c 5374 6174 6528 2929 0a0a 2020 2020  alState())..    
+000085e0: 2320 5479 7069 6361 6c6c 7920 7765 2073  # Typically we s
+000085f0: 6574 2074 6865 2070 6172 656e 7420 6261  et the parent ba
+00008600: 7365 6420 6f6e 2074 6865 2064 796e 616d  sed on the dynam
+00008610: 6963 206d 6f64 756c 6520 636f 6e74 6578  ic module contex
+00008620: 742e 0a20 2020 2069 6620 7365 6c66 2e70  t..    if self.p
+00008630: 6172 656e 7420 6973 205f 756e 7370 6563  arent is _unspec
+00008640: 6966 6965 645f 7061 7265 6e74 3a20 2023  ified_parent:  #
+00008650: 2070 7974 7970 653a 2064 6973 6162 6c65   pytype: disable
+00008660: 3d61 7474 7269 6275 7465 2d65 7272 6f72  =attribute-error
+00008670: 0a20 2020 2020 206f 626a 6563 742e 5f5f  .      object.__
+00008680: 7365 7461 7474 725f 5f28 7365 6c66 2c20  setattr__(self, 
+00008690: 2770 6172 656e 7427 2c20 5f63 6f6e 7465  'parent', _conte
+000086a0: 7874 2e6d 6f64 756c 655f 7374 6163 6b5b  xt.module_stack[
+000086b0: 2d31 5d29 0a0a 2020 2020 2320 496e 6974  -1])..    # Init
+000086c0: 6961 6c69 7a61 7469 6f6e 2069 7320 6465  ialization is de
+000086d0: 6665 7272 6564 2066 6f72 2074 6f70 206c  ferred for top l
+000086e0: 6576 656c 204d 6f64 756c 6573 206f 7220  evel Modules or 
+000086f0: 616e 7920 6f74 6865 7220 226f 7270 6861  any other "orpha
+00008700: 6e22 0a20 2020 2023 204d 6f64 756c 6573  n".    # Modules
+00008710: 2075 6e74 696c 2061 7474 6163 686d 656e   until attachmen
+00008720: 7420 6279 205f 5f73 6574 6174 7472 5f5f  t by __setattr__
+00008730: 2069 2e65 2e20 4d79 4d6f 6475 6c65 282e   i.e. MyModule(.
+00008740: 2e2e 2c20 7061 7265 6e74 3d4e 6f6e 6529  .., parent=None)
+00008750: 0a20 2020 2069 6620 7365 6c66 2e70 6172  .    if self.par
+00008760: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
+00008770: 2020 2072 6574 7572 6e0a 0a20 2020 2023     return..    #
+00008780: 2052 6567 6973 7465 7220 7375 626d 6f64   Register submod
+00008790: 756c 6520 6f6e 2070 6172 656e 7420 4d6f  ule on parent Mo
+000087a0: 6475 6c65 2e0a 2020 2020 6966 2069 7369  dule..    if isi
+000087b0: 6e73 7461 6e63 6528 7365 6c66 2e70 6172  nstance(self.par
+000087c0: 656e 742c 204d 6f64 756c 6529 3a0a 2020  ent, Module):.  
+000087d0: 2020 2020 2320 5768 656e 2069 6e69 7469      # When initi
+000087e0: 616c 697a 696e 6720 616e 2075 6e6e 616d  alizing an unnam
+000087f0: 6564 204d 6f64 756c 6520 696e 7369 6465  ed Module inside
+00008800: 2073 6574 7570 2829 0a20 2020 2020 2023   setup().      #
+00008810: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
+00008820: 6973 2064 6566 6572 7265 6420 756e 7469  is deferred unti
+00008830: 6c20 6174 7461 6368 6d65 6e74 2062 7920  l attachment by 
+00008840: 5f5f 7365 7461 7474 725f 5f0a 2020 2020  __setattr__.    
+00008850: 2020 2320 692e 652e 2073 656c 662e 6d79    # i.e. self.my
+00008860: 6d6f 6475 6c65 203d 204d 794d 6f64 756c  module = MyModul
+00008870: 6528 2e2e 2e29 0a20 2020 2020 2073 656c  e(...).      sel
+00008880: 662e 6e61 6d65 3a20 4f70 7469 6f6e 616c  f.name: Optional
+00008890: 5b73 7472 5d0a 2020 2020 2020 6966 2073  [str].      if s
+000088a0: 656c 662e 7061 7265 6e74 2e5f 7374 6174  elf.parent._stat
+000088b0: 652e 696e 5f73 6574 7570 2061 6e64 2073  e.in_setup and s
+000088c0: 656c 662e 6e61 6d65 2069 7320 4e6f 6e65  elf.name is None
+000088d0: 3a20 2023 2070 7974 7970 653a 2064 6973  :  # pytype: dis
+000088e0: 6162 6c65 3d61 7474 7269 6275 7465 2d65  able=attribute-e
+000088f0: 7272 6f72 0a20 2020 2020 2020 2072 6574  rror.        ret
+00008900: 7572 6e0a 2020 2020 2020 6966 206e 6f74  urn.      if not
+00008910: 2073 656c 662e 7061 7265 6e74 2e5f 696e   self.parent._in
+00008920: 6974 6961 6c69 7a61 7469 6f6e 5f61 6c6c  itialization_all
+00008930: 6f77 6564 3a0a 2020 2020 2020 2020 7261  owed:.        ra
+00008940: 6973 6520 6572 726f 7273 2e41 7373 6967  ise errors.Assig
+00008950: 6e53 7562 4d6f 6475 6c65 4572 726f 7228  nSubModuleError(
+00008960: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
+00008970: 5f6e 616d 655f 5f29 0a20 2020 2020 2023  _name__).      #
+00008980: 2041 7574 6f6e 616d 696e 6720 6f66 2073   Autonaming of s
+00008990: 7562 6d6f 6475 6c65 732e 0a20 2020 2020  ubmodules..     
+000089a0: 2069 6620 7365 6c66 2e6e 616d 6520 6973   if self.name is
+000089b0: 204e 6f6e 653a 2020 2320 7079 7479 7065   None:  # pytype
+000089c0: 3a20 6469 7361 626c 653d 6174 7472 6962  : disable=attrib
+000089d0: 7574 652d 6572 726f 720a 2020 2020 2020  ute-error.      
+000089e0: 2020 7072 6566 6978 203d 2066 277b 7365    prefix = f'{se
+000089f0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+00008a00: 616d 655f 5f7d 270a 2020 2020 2020 2020  ame__}'.        
+00008a10: 6375 7273 6f72 203d 2073 656c 662e 7061  cursor = self.pa
+00008a20: 7265 6e74 2e5f 7374 6174 652e 6175 746f  rent._state.auto
+00008a30: 6e61 6d65 5f63 7572 736f 722e 6765 7428  name_cursor.get(
+00008a40: 7072 6566 6978 2c20 3029 0a20 2020 2020  prefix, 0).     
+00008a50: 2020 2073 656c 662e 6e61 6d65 203d 2066     self.name = f
+00008a60: 277b 7072 6566 6978 7d5f 7b63 7572 736f  '{prefix}_{curso
+00008a70: 727d 270a 2020 2020 2020 2020 7365 6c66  r}'.        self
+00008a80: 2e70 6172 656e 742e 5f73 7461 7465 2e61  .parent._state.a
+00008a90: 7574 6f6e 616d 655f 6375 7273 6f72 5b70  utoname_cursor[p
+00008aa0: 7265 6669 785d 203d 2063 7572 736f 7220  refix] = cursor 
+00008ab0: 2b20 310a 2020 2020 2020 2320 416c 6c6f  + 1.      # Allo
+00008ac0: 7720 7363 6f70 6520 616c 6961 7369 6e67  w scope aliasing
+00008ad0: 2075 6e64 6572 2074 7261 6e73 666f 726d   under transform
+00008ae0: 7320 666f 7220 7375 626d 6f64 756c 6573  s for submodules
+00008af0: 2064 6566 696e 6564 2069 6e20 7365 7475   defined in setu
+00008b00: 702e 0a20 2020 2020 2072 6575 7365 5f73  p..      reuse_s
+00008b10: 636f 7065 7320 3d20 280a 2020 2020 2020  copes = (.      
+00008b20: 2020 2020 7365 6c66 2e70 6172 656e 742e      self.parent.
+00008b30: 5f73 7461 7465 2e69 6e5f 7365 7475 700a  _state.in_setup.
+00008b40: 2020 2020 2020 2020 2020 616e 6420 7365            and se
+00008b50: 6c66 2e70 6172 656e 742e 5f73 7461 7465  lf.parent._state
+00008b60: 2e73 6574 7570 5f63 616c 6c65 6420 3d3d  .setup_called ==
+00008b70: 2053 6574 7570 5374 6174 652e 5452 414e   SetupState.TRAN
+00008b80: 5346 4f52 4d45 440a 2020 2020 2020 290a  SFORMED.      ).
+00008b90: 2020 2020 2020 2320 5065 7266 6f72 6d20        # Perform 
+00008ba0: 6e61 6d65 2d63 6f6c 6c69 7369 6f6e 2063  name-collision c
+00008bb0: 6865 636b 2e0a 2020 2020 2020 6966 2073  heck..      if s
+00008bc0: 656c 662e 7061 7265 6e74 2e5f 6e61 6d65  elf.parent._name
+00008bd0: 5f74 616b 656e 2873 656c 662e 6e61 6d65  _taken(self.name
+00008be0: 2c20 7365 6c66 2c20 7265 7573 655f 7363  , self, reuse_sc
+00008bf0: 6f70 6573 3d72 6575 7365 5f73 636f 7065  opes=reuse_scope
+00008c00: 7329 3a0a 2020 2020 2020 2020 7061 7265  s):.        pare
+00008c10: 6e74 5f63 6c61 7373 203d 2073 656c 662e  nt_class = self.
+00008c20: 7061 7265 6e74 2e5f 5f63 6c61 7373 5f5f  parent.__class__
+00008c30: 2e5f 5f6e 616d 655f 5f0a 2020 2020 2020  .__name__.      
+00008c40: 2020 7261 6973 6520 6572 726f 7273 2e4e    raise errors.N
+00008c50: 616d 6549 6e55 7365 4572 726f 7228 2773  ameInUseError('s
+00008c60: 7562 6d6f 6475 6c65 272c 2073 656c 662e  ubmodule', self.
+00008c70: 6e61 6d65 2c20 7061 7265 6e74 5f63 6c61  name, parent_cla
+00008c80: 7373 290a 2020 2020 2020 2320 4669 6e61  ss).      # Fina
+00008c90: 6c69 7a65 2061 7474 6163 686d 656e 7420  lize attachment 
+00008ca0: 746f 2070 6172 656e 7420 616e 6420 7363  to parent and sc
+00008cb0: 6f70 6520 696e 6974 6961 6c69 7a61 7469  ope initializati
+00008cc0: 6f6e 2e0a 2020 2020 2020 7365 6c66 2e70  on..      self.p
+00008cd0: 6172 656e 742e 5f73 7461 7465 2e63 6869  arent._state.chi
+00008ce0: 6c64 7265 6e5b 7365 6c66 2e6e 616d 655d  ldren[self.name]
+00008cf0: 203d 2073 656c 660a 2020 2020 2020 6173   = self.      as
+00008d00: 7365 7274 2073 656c 662e 7061 7265 6e74  sert self.parent
+00008d10: 2e73 636f 7065 2069 7320 6e6f 7420 4e6f  .scope is not No
+00008d20: 6e65 0a20 2020 2020 206f 626a 6563 742e  ne.      object.
+00008d30: 5f5f 7365 7461 7474 725f 5f28 0a20 2020  __setattr__(.   
+00008d40: 2020 2020 2020 2073 656c 662c 2027 7363         self, 'sc
+00008d50: 6f70 6527 2c20 7365 6c66 2e70 6172 656e  ope', self.paren
+00008d60: 742e 7363 6f70 652e 7075 7368 2873 656c  t.scope.push(sel
+00008d70: 662e 6e61 6d65 2c20 7265 7573 653d 7265  f.name, reuse=re
+00008d80: 7573 655f 7363 6f70 6573 290a 2020 2020  use_scopes).    
+00008d90: 2020 290a 0a20 2020 2023 2054 6f70 2d6c    )..    # Top-l
+00008da0: 6576 656c 2069 6e76 6f63 6174 696f 6e20  evel invocation 
+00008db0: 7769 7468 2061 2066 756e 6374 696f 6e61  with a functiona
+00008dc0: 6c20 5363 6f70 652e 0a20 2020 2065 6c69  l Scope..    eli
+00008dd0: 6620 6973 696e 7374 616e 6365 2873 656c  f isinstance(sel
+00008de0: 662e 7061 7265 6e74 2c20 5363 6f70 6529  f.parent, Scope)
+00008df0: 3a0a 2020 2020 2020 6f62 6a65 6374 2e5f  :.      object._
+00008e00: 5f73 6574 6174 7472 5f5f 2873 656c 662c  _setattr__(self,
+00008e10: 2027 7363 6f70 6527 2c20 7365 6c66 2e70   'scope', self.p
+00008e20: 6172 656e 7429 0a20 2020 2065 6c73 653a  arent).    else:
+00008e30: 0a20 2020 2020 2072 6169 7365 2056 616c  .      raise Val
+00008e40: 7565 4572 726f 7228 2770 6172 656e 7420  ueError('parent 
+00008e50: 6d75 7374 2062 6520 4e6f 6e65 2c20 4d6f  must be None, Mo
+00008e60: 6475 6c65 206f 7220 5363 6f70 6527 290a  dule or Scope').
+00008e70: 0a20 2020 2023 2065 6167 6572 6c79 2062  .    # eagerly b
+00008e80: 696e 6420 7375 626d 6f64 756c 6573 2069  ind submodules i
+00008e90: 6620 7363 6f70 6520 6973 2061 7661 696c  f scope is avail
+00008ea0: 6162 6c65 0a20 2020 2069 6620 7365 6c66  able.    if self
+00008eb0: 2e73 636f 7065 2069 7320 6e6f 7420 4e6f  .scope is not No
+00008ec0: 6e65 3a0a 2020 2020 2020 666f 7220 6669  ne:.      for fi
+00008ed0: 656c 6420 696e 2064 6174 6163 6c61 7373  eld in dataclass
+00008ee0: 6573 2e66 6965 6c64 7328 7365 6c66 293a  es.fields(self):
+00008ef0: 0a20 2020 2020 2020 2069 6620 6669 656c  .        if fiel
+00008f00: 642e 6e61 6d65 206e 6f74 2069 6e20 2827  d.name not in ('
+00008f10: 7061 7265 6e74 272c 2027 6e61 6d65 2729  parent', 'name')
+00008f20: 2061 6e64 2066 6965 6c64 2e69 6e69 743a   and field.init:
+00008f30: 0a20 2020 2020 2020 2020 2073 656c 662e  .          self.
+00008f40: 5f72 6567 6973 7465 725f 7375 626d 6f64  _register_submod
+00008f50: 756c 6573 2866 6965 6c64 2e6e 616d 652c  ules(field.name,
+00008f60: 2067 6574 6174 7472 2873 656c 662c 2066   getattr(self, f
+00008f70: 6965 6c64 2e6e 616d 6529 290a 0a20 2020  ield.name))..   
+00008f80: 2073 656c 662e 5f73 7461 7465 2e69 735f   self._state.is_
+00008f90: 696e 6974 6961 6c69 7a65 6420 3d20 5472  initialized = Tr
+00008fa0: 7565 0a0a 2020 6465 6620 5f5f 7265 7072  ue..  def __repr
+00008fb0: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
+00008fc0: 0a20 2020 2072 6574 7572 6e20 5f6d 6f64  .    return _mod
+00008fd0: 756c 655f 7265 7072 2873 656c 6629 0a0a  ule_repr(self)..
+00008fe0: 2020 6465 6620 7365 7475 7028 7365 6c66    def setup(self
+00008ff0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+00009000: 2222 496e 6974 6961 6c69 7a65 7320 6120  ""Initializes a 
+00009010: 4d6f 6475 6c65 206c 617a 696c 7920 2873  Module lazily (s
+00009020: 696d 696c 6172 2074 6f20 6120 6c61 7a79  imilar to a lazy
+00009030: 2060 605f 5f69 6e69 745f 5f60 6029 2e0a   ``__init__``)..
+00009040: 0a20 2020 2060 6073 6574 7570 6060 2069  .    ``setup`` i
+00009050: 7320 6361 6c6c 6564 206f 6e63 6520 6c61  s called once la
+00009060: 7a69 6c79 206f 6e20 6120 6d6f 6475 6c65  zily on a module
+00009070: 2069 6e73 7461 6e63 6520 7768 656e 2061   instance when a
+00009080: 206d 6f64 756c 650a 2020 2020 6973 2062   module.    is b
+00009090: 6f75 6e64 2c20 696d 6d65 6469 6174 656c  ound, immediatel
+000090a0: 7920 6265 666f 7265 2061 6e79 206f 7468  y before any oth
+000090b0: 6572 206d 6574 686f 6473 206c 696b 6520  er methods like 
+000090c0: 6060 5f5f 6361 6c6c 5f5f 6060 2061 7265  ``__call__`` are
+000090d0: 0a20 2020 2069 6e76 6f6b 6564 2c20 6f72  .    invoked, or
+000090e0: 2062 6566 6f72 6520 6120 6060 7365 7475   before a ``setu
+000090f0: 7060 602d 6465 6669 6e65 6420 6174 7472  p``-defined attr
+00009100: 6962 7574 6520 6f6e 2060 7365 6c66 6020  ibute on `self` 
+00009110: 6973 2061 6363 6573 7365 642e 0a0a 2020  is accessed...  
+00009120: 2020 5468 6973 2063 616e 2068 6170 7065    This can happe
+00009130: 6e20 696e 2074 6872 6565 2063 6173 6573  n in three cases
+00009140: 3a0a 0a20 2020 2020 2031 2e20 496d 6d65  :..      1. Imme
+00009150: 6469 6174 656c 7920 7768 656e 2069 6e76  diately when inv
+00009160: 6f6b 696e 6720 3a6d 6574 683a 6061 7070  oking :meth:`app
+00009170: 6c79 602c 203a 6d65 7468 3a60 696e 6974  ly`, :meth:`init
+00009180: 6020 6f72 0a20 2020 2020 2020 2020 3a6d  ` or.         :m
+00009190: 6574 683a 6069 6e69 745f 616e 645f 6f75  eth:`init_and_ou
+000091a0: 7470 7574 602e 0a0a 2020 2020 2020 322e  tput`...      2.
+000091b0: 204f 6e63 6520 7468 6520 6d6f 6475 6c65   Once the module
+000091c0: 2069 7320 6769 7665 6e20 6120 6e61 6d65   is given a name
+000091d0: 2062 7920 6265 696e 6720 6173 7369 676e   by being assign
+000091e0: 6564 2074 6f20 616e 2061 7474 7269 6275  ed to an attribu
+000091f0: 7465 206f 660a 2020 2020 2020 2020 2061  te of.         a
+00009200: 6e6f 7468 6572 206d 6f64 756c 6520 696e  nother module in
+00009210: 7369 6465 2074 6865 206f 7468 6572 206d  side the other m
+00009220: 6f64 756c 6527 7320 6060 7365 7475 7060  odule's ``setup`
+00009230: 6020 6d65 7468 6f64 0a20 2020 2020 2020  ` method.       
+00009240: 2020 2873 6565 203a 6d65 7468 3a60 5f5f    (see :meth:`__
+00009250: 7365 7461 7474 725f 5f60 293a 3a0a 0a20  setattr__`)::.. 
+00009260: 2020 2020 2020 2020 2020 636c 6173 7320            class 
+00009270: 4d79 4d6f 6475 6c65 286e 6e2e 4d6f 6475  MyModule(nn.Modu
+00009280: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00009290: 2020 6465 6620 7365 7475 7028 7365 6c66    def setup(self
+000092a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000092b0: 2020 7375 626d 6f64 756c 6520 3d20 436f    submodule = Co
+000092c0: 6e76 282e 2e2e 290a 0a20 2020 2020 2020  nv(...)..       
+000092d0: 2020 2020 2020 2020 2320 4163 6365 7373          # Access
+000092e0: 696e 6720 6073 7562 6d6f 6475 6c65 6020  ing `submodule` 
+000092f0: 6174 7472 6962 7574 6573 2064 6f65 7320  attributes does 
+00009300: 6e6f 7420 7965 7420 776f 726b 2068 6572  not yet work her
+00009310: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00009320: 2020 2023 2054 6865 2066 6f6c 6c6f 7769     # The followi
+00009330: 6e67 206c 696e 6520 696e 766f 6b65 7320  ng line invokes 
+00009340: 6073 656c 662e 5f5f 7365 7461 7474 725f  `self.__setattr_
+00009350: 5f60 2c20 7768 6963 6820 6769 7665 730a  _`, which gives.
+00009360: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00009370: 2060 7375 626d 6f64 756c 6560 2074 6865   `submodule` the
+00009380: 206e 616d 6520 2263 6f6e 7631 222e 0a20   name "conv1".. 
+00009390: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000093a0: 6c66 2e63 6f6e 7631 203d 2073 7562 6d6f  lf.conv1 = submo
+000093b0: 6475 6c65 0a0a 2020 2020 2020 2020 2020  dule..          
+000093c0: 2020 2020 2023 2041 6363 6573 7369 6e67       # Accessing
+000093d0: 2060 7375 626d 6f64 756c 6560 2061 7474   `submodule` att
+000093e0: 7269 6275 7465 7320 6f72 206d 6574 686f  ributes or metho
+000093f0: 6473 2069 7320 6e6f 7720 7361 6665 2061  ds is now safe a
+00009400: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00009410: 2020 2320 6569 7468 6572 2063 6175 7365    # either cause
+00009420: 7320 7365 7475 7028 2920 746f 2062 6520  s setup() to be 
+00009430: 6361 6c6c 6564 206f 6e63 652e 0a0a 2020  called once...  
+00009440: 2020 2020 332e 204f 6e63 6520 6120 6d6f      3. Once a mo
+00009450: 6475 6c65 2069 7320 636f 6e73 7472 7563  dule is construc
+00009460: 7465 6420 696e 7369 6465 2061 206d 6574  ted inside a met
+00009470: 686f 6420 7772 6170 7065 6420 7769 7468  hod wrapped with
+00009480: 0a20 2020 2020 2020 2020 3a6d 6574 683a  .         :meth:
+00009490: 6063 6f6d 7061 6374 602c 2069 6d6d 6564  `compact`, immed
+000094a0: 6961 7465 6c79 2062 6566 6f72 6520 616e  iately before an
+000094b0: 6f74 6865 7220 6d65 7468 6f64 2069 7320  other method is 
+000094c0: 6361 6c6c 6564 206f 720a 2020 2020 2020  called or.      
+000094d0: 2020 2060 6073 6574 7570 6060 2064 6566     ``setup`` def
+000094e0: 696e 6564 2061 7474 7269 6275 7465 2069  ined attribute i
+000094f0: 7320 6163 6365 7373 6564 2e0a 2020 2020  s accessed..    
+00009500: 2222 220a 2020 2020 7061 7373 0a0a 2020  """.    pass..  
+00009510: 6465 6620 5f72 6567 6973 7465 725f 7375  def _register_su
+00009520: 626d 6f64 756c 6573 2873 656c 662c 206e  bmodules(self, n
+00009530: 616d 652c 2076 616c 293a 0a20 2020 2022  ame, val):.    "
+00009540: 2222 5265 6769 7374 6572 7320 6120 7375  ""Registers a su
+00009550: 626d 6f64 756c 652e 2222 220a 2020 2020  bmodule.""".    
+00009560: 6173 7365 7274 2073 656c 662e 7363 6f70  assert self.scop
+00009570: 652c 2027 5472 7969 6e67 2074 6f20 7265  e, 'Trying to re
+00009580: 6769 7374 6572 2073 7562 6d6f 6475 6c65  gister submodule
+00009590: 7320 6f6e 2075 6e62 6f75 6e64 2073 636f  s on unbound sco
+000095a0: 7065 2e27 0a20 2020 2072 6f6f 7420 3d20  pe.'.    root = 
+000095b0: 7365 6c66 2e73 636f 7065 2e72 6f6f 740a  self.scope.root.
+000095c0: 2020 2020 6361 6368 6520 3d20 5f63 6163      cache = _cac
+000095d0: 6865 732e 6765 7428 726f 6f74 2c20 7765  hes.get(root, we
+000095e0: 616b 7265 662e 5765 616b 5661 6c75 6544  akref.WeakValueD
+000095f0: 6963 7469 6f6e 6172 7928 2929 0a20 2020  ictionary()).   
+00009600: 205f 6361 6368 6573 5b72 6f6f 745d 203d   _caches[root] =
+00009610: 2063 6163 6865 0a20 2020 2071 7565 7565   cache.    queue
+00009620: 203d 205b 5d0a 2020 2020 7072 6573 6572   = [].    preser
+00009630: 7665 5f61 646f 7074 6564 5f6e 616d 6573  ve_adopted_names
+00009640: 203d 2063 6f6e 6669 672e 666c 6178 5f70   = config.flax_p
+00009650: 7265 7365 7276 655f 6164 6f70 7465 645f  reserve_adopted_
+00009660: 6e61 6d65 730a 2020 2020 6966 2068 6173  names.    if has
+00009670: 6174 7472 2874 7970 6528 7365 6c66 292c  attr(type(self),
+00009680: 2027 7072 6573 6572 7665 5f61 646f 7074   'preserve_adopt
+00009690: 6564 5f6e 616d 6573 2729 3a0a 2020 2020  ed_names'):.    
+000096a0: 2020 7072 6573 6572 7665 5f61 646f 7074    preserve_adopt
+000096b0: 6564 5f6e 616d 6573 203d 2074 7970 6528  ed_names = type(
+000096c0: 7365 6c66 292e 7072 6573 6572 7665 5f61  self).preserve_a
+000096d0: 646f 7074 6564 5f6e 616d 6573 0a0a 2020  dopted_names..  
+000096e0: 2020 6465 6620 6164 6f70 745f 6174 7472    def adopt_attr
+000096f0: 5f6d 6f64 756c 6573 2863 6163 6865 2c20  _modules(cache, 
+00009700: 7175 6575 652c 2073 7566 6669 782c 2073  queue, suffix, s
+00009710: 7562 7661 6c75 6529 3a0a 2020 2020 2020  ubvalue):.      
+00009720: 6966 2069 7369 6e73 7461 6e63 6528 7375  if isinstance(su
+00009730: 6276 616c 7565 2c20 4d6f 6475 6c65 293a  bvalue, Module):
+00009740: 0a20 2020 2020 2020 2061 646f 7074 6564  .        adopted
+00009750: 5f6e 616d 6520 3d20 4e6f 6e65 0a20 2020  _name = None.   
+00009760: 2020 2020 2069 6620 7375 6276 616c 7565       if subvalue
+00009770: 2e70 6172 656e 7420 6973 204e 6f6e 653a  .parent is None:
+00009780: 0a20 2020 2020 2020 2020 2023 2050 7265  .          # Pre
+00009790: 7365 7276 6520 7368 6172 696e 672d 6279  serve sharing-by
+000097a0: 2d72 6566 6572 656e 6365 2072 656c 6174  -reference relat
+000097b0: 696f 6e73 6869 7073 2064 7572 696e 6720  ionships during 
+000097c0: 6164 6f70 7469 6f6e 0a20 2020 2020 2020  adoption.       
+000097d0: 2020 2023 2076 6961 2063 6163 6865 206b     # via cache k
+000097e0: 6579 6564 206f 6e20 756e 6971 7565 2069  eyed on unique i
+000097f0: 6e73 7461 6e63 6520 6964 732e 0a20 2020  nstance ids..   
+00009800: 2020 2020 2020 206b 6579 203d 2073 7562         key = sub
+00009810: 7661 6c75 652e 5f69 640a 2020 2020 2020  value._id.      
+00009820: 2020 2020 2320 4d6f 6475 6c65 2077 6173      # Module was
+00009830: 2070 6173 7365 6420 6672 6f6d 206f 7574   passed from out
+00009840: 7369 6465 2e20 4974 206e 6565 6473 2074  side. It needs t
+00009850: 6f20 6265 2063 6c6f 6e65 642e 0a20 2020  o be cloned..   
+00009860: 2020 2020 2020 2023 204f 7574 7369 6465         # Outside
+00009870: 206d 6f64 756c 6573 2061 7265 206e 616d   modules are nam
+00009880: 6564 2062 7920 6174 7461 6368 6d65 6e74  ed by attachment
+00009890: 2c20 6e6f 7420 616e 206f 7574 6572 206e  , not an outer n
+000098a0: 616d 652c 0a20 2020 2020 2020 2020 2023  ame,.          #
+000098b0: 2055 4e4c 4553 5320 7765 2772 6520 7573   UNLESS we're us
+000098c0: 696e 6720 6e65 7720 6164 6f70 7465 6420  ing new adopted 
+000098d0: 6e61 6d65 2070 6f6c 6963 792c 2069 6e20  name policy, in 
+000098e0: 7768 6963 6820 6361 7365 2061 6e20 6578  which case an ex
+000098f0: 6973 7469 6e67 0a20 2020 2020 2020 2020  isting.         
+00009900: 2023 206e 616d 6520 7769 6c6c 2062 6520   # name will be 
+00009910: 7573 6564 2c20 6173 2069 7320 6f66 7465  used, as is ofte
+00009920: 6e20 7375 7070 6c69 6564 2062 7920 636f  n supplied by co
+00009930: 6e66 6967 2073 7973 7465 6d73 2e0a 2020  nfig systems..  
+00009940: 2020 2020 2020 2020 6966 2070 7265 7365          if prese
+00009950: 7276 655f 6164 6f70 7465 645f 6e61 6d65  rve_adopted_name
+00009960: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00009970: 646f 7074 6564 5f6e 616d 6520 3d20 6f62  dopted_name = ob
+00009980: 6a65 6374 2e5f 5f67 6574 6174 7472 6962  ject.__getattrib
+00009990: 7574 655f 5f28 7375 6276 616c 7565 2c20  ute__(subvalue, 
+000099a0: 276e 616d 6527 290a 2020 2020 2020 2020  'name').        
+000099b0: 2020 6966 206b 6579 2069 6e20 6361 6368    if key in cach
+000099c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000099d0: 7562 7661 6c75 6520 3d20 6361 6368 655b  ubvalue = cache[
+000099e0: 6b65 795d 0a20 2020 2020 2020 2020 2065  key].          e
+000099f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00009a00: 2073 7562 7661 6c75 6520 3d20 7375 6276   subvalue = subv
+00009a10: 616c 7565 2e63 6c6f 6e65 286e 616d 653d  alue.clone(name=
+00009a20: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
+00009a30: 2020 6361 6368 655b 6b65 795d 203d 2073    cache[key] = s
+00009a40: 7562 7661 6c75 650a 2020 2020 2020 2020  ubvalue.        
+00009a50: 6966 2073 7562 7661 6c75 652e 6e61 6d65  if subvalue.name
+00009a60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00009a70: 2020 2020 6f62 6a65 6374 2e5f 5f73 6574      object.__set
+00009a80: 6174 7472 5f5f 2873 7562 7661 6c75 652c  attr__(subvalue,
+00009a90: 2027 7061 7265 6e74 272c 2073 656c 6629   'parent', self)
+00009aa0: 0a20 2020 2020 2020 2020 2069 6620 6164  .          if ad
+00009ab0: 6f70 7465 645f 6e61 6d65 2069 7320 4e6f  opted_name is No
+00009ac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009ad0: 6164 6f70 7465 645f 6e61 6d65 203d 2066  adopted_name = f
+00009ae0: 277b 6e61 6d65 7d7b 7375 6666 6978 7d27  '{name}{suffix}'
+00009af0: 0a20 2020 2020 2020 2020 206f 626a 6563  .          objec
+00009b00: 742e 5f5f 7365 7461 7474 725f 5f28 7375  t.__setattr__(su
+00009b10: 6276 616c 7565 2c20 276e 616d 6527 2c20  bvalue, 'name', 
+00009b20: 6164 6f70 7465 645f 6e61 6d65 290a 2020  adopted_name).  
+00009b30: 2020 2020 2020 2020 7175 6575 652e 6170          queue.ap
+00009b40: 7065 6e64 2873 7562 7661 6c75 6529 0a20  pend(subvalue). 
+00009b50: 2020 2020 2072 6574 7572 6e20 7375 6276       return subv
+00009b60: 616c 7565 0a0a 2020 2020 7661 6c20 3d20  alue..    val = 
+00009b70: 5f66 7265 657a 655f 6174 7472 280a 2020  _freeze_attr(.  
+00009b80: 2020 2020 2020 5f6d 6170 5f6f 7665 725f        _map_over_
+00009b90: 6d6f 6475 6c65 735f 696e 5f74 7265 6528  modules_in_tree(
+00009ba0: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
+00009bb0: 6374 6f6f 6c73 2e70 6172 7469 616c 2861  ctools.partial(a
+00009bc0: 646f 7074 5f61 7474 725f 6d6f 6475 6c65  dopt_attr_module
+00009bd0: 732c 2063 6163 6865 2c20 7175 6575 6529  s, cache, queue)
+00009be0: 2c20 7661 6c0a 2020 2020 2020 2020 290a  , val.        ).
+00009bf0: 2020 2020 290a 2020 2020 6f62 6a65 6374      ).    object
+00009c00: 2e5f 5f73 6574 6174 7472 5f5f 2873 656c  .__setattr__(sel
+00009c10: 662c 206e 616d 652c 2076 616c 290a 2020  f, name, val).  
+00009c20: 2020 666f 7220 7820 696e 2071 7565 7565    for x in queue
+00009c30: 3a0a 2020 2020 2020 782e 5f5f 706f 7374  :.      x.__post
+00009c40: 5f69 6e69 745f 5f28 290a 0a20 2064 6566  _init__()..  def
+00009c50: 205f 7472 795f 7365 7475 7028 7365 6c66   _try_setup(self
+00009c60: 2c20 7368 616c 6c6f 773a 2062 6f6f 6c20  , shallow: bool 
+00009c70: 3d20 4661 6c73 6529 202d 3e20 4e6f 6e65  = False) -> None
+00009c80: 3a0a 2020 2020 2222 2254 7269 6573 2074  :.    """Tries t
+00009c90: 6f20 7365 7475 7020 6d6f 6475 6c65 2069  o setup module i
+00009ca0: 6620 7363 6f70 6520 6973 2061 7661 696c  f scope is avail
+00009cb0: 6162 6c65 2061 6e64 2073 6574 7570 2068  able and setup h
+00009cc0: 6173 206e 6f74 2062 6565 6e20 6361 6c6c  as not been call
+00009cd0: 6564 2079 6574 2e22 2222 0a20 2020 2069  ed yet.""".    i
+00009ce0: 6620 280a 2020 2020 2020 2020 7365 6c66  f (.        self
+00009cf0: 2e73 636f 7065 0a20 2020 2020 2020 2061  .scope.        a
+00009d00: 6e64 206e 6f74 2073 656c 662e 5f73 7461  nd not self._sta
+00009d10: 7465 2e69 6e5f 7365 7475 700a 2020 2020  te.in_setup.    
+00009d20: 2020 2020 616e 6420 7365 6c66 2e5f 7374      and self._st
+00009d30: 6174 652e 7365 7475 705f 6361 6c6c 6564  ate.setup_called
+00009d40: 2021 3d20 5365 7475 7053 7461 7465 2e44   != SetupState.D
+00009d50: 4f4e 450a 2020 2020 293a 0a20 2020 2020  ONE.    ):.     
+00009d60: 2074 7279 3a0a 2020 2020 2020 2020 7365   try:.        se
+00009d70: 6c66 2e5f 7374 6174 652e 696e 5f73 6574  lf._state.in_set
+00009d80: 7570 203d 2054 7275 650a 2020 2020 2020  up = True.      
+00009d90: 2020 2320 4120 7368 616c 6c6f 7720 7365    # A shallow se
+00009da0: 7475 7020 7769 6c6c 206f 6e6c 7920 7265  tup will only re
+00009db0: 6769 7374 6572 2061 7474 7269 6275 7465  gister attribute
+00009dc0: 2073 7562 6d6f 6475 6c65 7320 6275 7420   submodules but 
+00009dd0: 6974 2064 6f65 730a 2020 2020 2020 2020  it does.        
+00009de0: 2320 6e6f 7420 6361 6c6c 2074 6865 2075  # not call the u
+00009df0: 7365 7227 7320 7365 7475 702e 2054 6869  ser's setup. Thi
+00009e00: 7320 6176 6f69 6473 2072 756e 6e69 6e67  s avoids running
+00009e10: 2062 6566 6f72 6520 610a 2020 2020 2020   before a.      
+00009e20: 2020 2320 7472 616e 7366 6f72 6d61 7469    # transformati
+00009e30: 6f6e 2e0a 2020 2020 2020 2020 666f 7220  on..        for 
+00009e40: 6669 656c 6420 696e 2064 6174 6163 6c61  field in datacla
+00009e50: 7373 6573 2e66 6965 6c64 7328 7365 6c66  sses.fields(self
+00009e60: 293a 0a20 2020 2020 2020 2020 2069 6620  ):.          if 
+00009e70: 6669 656c 642e 6e61 6d65 206e 6f74 2069  field.name not i
+00009e80: 6e20 2827 7061 7265 6e74 272c 2027 6e61  n ('parent', 'na
+00009e90: 6d65 2729 2061 6e64 2066 6965 6c64 2e69  me') and field.i
+00009ea0: 6e69 743a 0a20 2020 2020 2020 2020 2020  nit:.           
+00009eb0: 2073 656c 662e 5f72 6567 6973 7465 725f   self._register_
+00009ec0: 7375 626d 6f64 756c 6573 2866 6965 6c64  submodules(field
+00009ed0: 2e6e 616d 652c 2067 6574 6174 7472 2873  .name, getattr(s
+00009ee0: 656c 662c 2066 6965 6c64 2e6e 616d 6529  elf, field.name)
+00009ef0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00009f00: 2073 6861 6c6c 6f77 3a0a 2020 2020 2020   shallow:.      
+00009f10: 2020 2020 7365 6c66 2e73 6574 7570 2829      self.setup()
+00009f20: 0a20 2020 2020 2020 2023 2057 6520 7275  .        # We ru
+00009f30: 6e20 7374 6174 6963 2063 6865 636b 7320  n static checks 
+00009f40: 6162 7374 7261 6374 6c79 206f 6e63 6520  abstractly once 
+00009f50: 666f 7220 7365 7475 7020 6265 666f 7265  for setup before
+00009f60: 2061 6e79 2074 7261 6e73 666f 726d 730a   any transforms.
+00009f70: 2020 2020 2020 2020 2320 746f 2064 6574          # to det
+00009f80: 6563 7420 6e61 6d65 2063 6f6c 6c69 7369  ect name collisi
+00009f90: 6f6e 7320 616e 6420 6f74 6865 7220 7079  ons and other py
+00009fa0: 7468 6f6e 2065 7272 6f72 732e 0a20 2020  thon errors..   
+00009fb0: 2020 2020 2065 6c69 6620 7365 6c66 2e5f       elif self._
+00009fc0: 7374 6174 652e 7365 7475 705f 6361 6c6c  state.setup_call
+00009fd0: 6564 203d 3d20 5365 7475 7053 7461 7465  ed == SetupState
+00009fe0: 2e4e 4557 3a0a 2020 2020 2020 2020 2020  .NEW:.          
+00009ff0: 7365 6c66 2e5f 7661 6c69 6461 7465 5f73  self._validate_s
+0000a000: 6574 7570 2829 0a20 2020 2020 2066 696e  etup().      fin
+0000a010: 616c 6c79 3a0a 2020 2020 2020 2020 7365  ally:.        se
+0000a020: 6c66 2e5f 7374 6174 652e 696e 5f73 6574  lf._state.in_set
+0000a030: 7570 203d 2046 616c 7365 0a20 2020 2020  up = False.     
+0000a040: 2020 2069 6620 6e6f 7420 7368 616c 6c6f     if not shallo
+0000a050: 773a 0a20 2020 2020 2020 2020 2073 656c  w:.          sel
+0000a060: 662e 5f73 7461 7465 2e73 6574 7570 5f63  f._state.setup_c
+0000a070: 616c 6c65 6420 3d20 5365 7475 7053 7461  alled = SetupSta
+0000a080: 7465 2e44 4f4e 450a 0a20 2064 6566 205f  te.DONE..  def _
+0000a090: 7661 6c69 6461 7465 5f73 6574 7570 2873  validate_setup(s
+0000a0a0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000a0b0: 2020 2222 2241 6273 7472 6163 746c 7920    """Abstractly 
+0000a0c0: 6576 616c 7561 7465 7320 7365 7475 7020  evaluates setup 
+0000a0d0: 6f6e 6c79 2074 6f20 7275 6e20 7374 6174  only to run stat
+0000a0e0: 6963 2063 6865 636b 732e 2222 220a 0a20  ic checks.""".. 
+0000a0f0: 2020 2064 6566 2072 756e 5f73 6574 7570     def run_setup
+0000a100: 5f6f 6e6c 7928 7829 3a0a 2020 2020 2020  _only(x):.      
+0000a110: 7772 6170 7065 645f 6964 203d 2077 7261  wrapped_id = wra
+0000a120: 705f 6d65 7468 6f64 5f6f 6e63 6528 6c61  p_method_once(la
+0000a130: 6d62 6461 206d 2c20 783a 2078 290a 2020  mbda m, x: x).  
+0000a140: 2020 2020 7769 7468 2054 6573 7453 636f      with TestSco
+0000a150: 7065 287b 7d2c 2072 6e67 733d 7b7d 2c20  pe({}, rngs={}, 
+0000a160: 6d75 7461 626c 653d 5472 7565 292e 7465  mutable=True).te
+0000a170: 6d70 6f72 6172 7928 2920 6173 2072 6f6f  mporary() as roo
+0000a180: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+0000a190: 6e20 7772 6170 7065 645f 6964 2873 656c  n wrapped_id(sel
+0000a1a0: 662e 636c 6f6e 6528 7061 7265 6e74 3d72  f.clone(parent=r
+0000a1b0: 6f6f 7429 2c20 7829 0a0a 2020 2020 5f20  oot), x)..    _ 
+0000a1c0: 3d20 6a61 782e 6576 616c 5f73 6861 7065  = jax.eval_shape
+0000a1d0: 2872 756e 5f73 6574 7570 5f6f 6e6c 792c  (run_setup_only,
+0000a1e0: 2030 290a 0a20 2064 6566 205f 6e61 6d65   0)..  def _name
+0000a1f0: 5f74 616b 656e 280a 2020 2020 2020 7365  _taken(.      se
+0000a200: 6c66 2c0a 2020 2020 2020 6e61 6d65 3a20  lf,.      name: 
+0000a210: 7374 722c 0a20 2020 2020 206d 6f64 756c  str,.      modul
+0000a220: 653a 204f 7074 696f 6e61 6c5b 274d 6f64  e: Optional['Mod
+0000a230: 756c 6527 5d20 3d20 4e6f 6e65 2c0a 2020  ule'] = None,.  
+0000a240: 2020 2020 7265 7573 655f 7363 6f70 6573      reuse_scopes
+0000a250: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0000a260: 2020 2020 2020 636f 6c6c 6563 7469 6f6e        collection
+0000a270: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000a280: 3d20 4e6f 6e65 2c0a 2020 2920 2d3e 2062  = None,.  ) -> b
+0000a290: 6f6f 6c3a 0a20 2020 2061 7373 6572 7420  ool:.    assert 
+0000a2a0: 7365 6c66 2e73 636f 7065 2069 7320 6e6f  self.scope is no
+0000a2b0: 7420 4e6f 6e65 0a20 2020 2069 6620 7265  t None.    if re
+0000a2c0: 7573 655f 7363 6f70 6573 3a0a 2020 2020  use_scopes:.    
+0000a2d0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0000a2e0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+0000a2f0: 636f 7065 2e6e 616d 655f 7265 7365 7276  cope.name_reserv
+0000a300: 6564 286e 616d 652c 2063 6f6c 6c65 6374  ed(name, collect
+0000a310: 696f 6e29 0a0a 2020 4070 726f 7065 7274  ion)..  @propert
+0000a320: 790a 2020 6465 6620 5f69 6e69 7469 616c  y.  def _initial
+0000a330: 697a 6174 696f 6e5f 616c 6c6f 7765 6428  ization_allowed(
+0000a340: 7365 6c66 293a 0a20 2020 2072 6574 7572  self):.    retur
+0000a350: 6e20 280a 2020 2020 2020 2020 6e6f 7420  n (.        not 
+0000a360: 7365 6c66 2e5f 7374 6174 652e 6973 5f69  self._state.is_i
+0000a370: 6e69 7469 616c 697a 6564 2020 2320 616c  nitialized  # al
+0000a380: 6c6f 7720 6561 6765 7220 6174 7461 6368  low eager attach
+0000a390: 6d65 6e74 2069 6e20 706f 7374 2d69 6e69  ment in post-ini
+0000a3a0: 740a 2020 2020 2020 2020 6f72 2073 656c  t.        or sel
+0000a3b0: 662e 5f73 7461 7465 2e69 6e5f 7365 7475  f._state.in_setu
+0000a3c0: 700a 2020 2020 2020 2020 6f72 2073 656c  p.        or sel
+0000a3d0: 662e 5f73 7461 7465 2e69 6e5f 636f 6d70  f._state.in_comp
+0000a3e0: 6163 745f 6d65 7468 6f64 0a20 2020 2029  act_method.    )
+0000a3f0: 0a0a 2020 6465 6620 636c 6f6e 6528 0a20  ..  def clone(. 
+0000a400: 2020 2020 2073 656c 663a 204d 2c0a 2020       self: M,.  
+0000a410: 2020 2020 2a2c 0a20 2020 2020 2070 6172      *,.      par
+0000a420: 656e 743a 204f 7074 696f 6e61 6c5b 556e  ent: Optional[Un
+0000a430: 696f 6e5b 5363 6f70 652c 2027 4d6f 6475  ion[Scope, 'Modu
+0000a440: 6c65 275d 5d20 3d20 4e6f 6e65 2c0a 2020  le']] = None,.  
+0000a450: 2020 2020 5f64 6565 705f 636c 6f6e 653a      _deep_clone:
+0000a460: 2055 6e69 6f6e 5b62 6f6f 6c2c 2077 6561   Union[bool, wea
+0000a470: 6b72 6566 2e57 6561 6b56 616c 7565 4469  kref.WeakValueDi
+0000a480: 6374 696f 6e61 7279 5d20 3d20 4661 6c73  ctionary] = Fals
+0000a490: 652c 0a20 2020 2020 202a 2a75 7064 6174  e,.      **updat
+0000a4a0: 6573 2c0a 2020 2920 2d3e 204d 3a0a 2020  es,.  ) -> M:.  
+0000a4b0: 2020 2222 2243 7265 6174 6573 2061 2063    """Creates a c
+0000a4c0: 6c6f 6e65 206f 6620 7468 6973 204d 6f64  lone of this Mod
+0000a4d0: 756c 652c 2077 6974 6820 6f70 7469 6f6e  ule, with option
+0000a4e0: 616c 6c79 2075 7064 6174 6564 2061 7267  ally updated arg
+0000a4f0: 756d 656e 7473 2e0a 0a20 2020 2041 7267  uments...    Arg
+0000a500: 733a 0a20 2020 2020 2070 6172 656e 743a  s:.      parent:
+0000a510: 2054 6865 2070 6172 656e 7420 6f66 2074   The parent of t
+0000a520: 6865 2063 6c6f 6e65 2e20 5468 6520 636c  he clone. The cl
+0000a530: 6f6e 6520 7769 6c6c 2068 6176 6520 6e6f  one will have no
+0000a540: 2070 6172 656e 7420 6966 206e 6f0a 2020   parent if no.  
+0000a550: 2020 2020 2020 6578 706c 6963 6974 2070        explicit p
+0000a560: 6172 656e 7420 6973 2073 7065 6369 6669  arent is specifi
+0000a570: 6564 2e0a 2020 2020 2020 5f64 6565 705f  ed..      _deep_
+0000a580: 636c 6f6e 653a 2041 2062 6f6f 6c65 616e  clone: A boolean
+0000a590: 206f 7220 6120 7765 616b 2076 616c 7565   or a weak value
+0000a5a0: 2064 6963 7469 6f6e 6172 7920 746f 2063   dictionary to c
+0000a5b0: 6f6e 7472 6f6c 2064 6565 7020 636c 6f6e  ontrol deep clon
+0000a5c0: 696e 670a 2020 2020 2020 2020 6f66 2073  ing.        of s
+0000a5d0: 7562 6d6f 6475 6c65 732e 2049 6620 5472  ubmodules. If Tr
+0000a5e0: 7565 2c20 7375 626d 6f64 756c 6573 2077  ue, submodules w
+0000a5f0: 696c 6c20 6265 2063 6c6f 6e65 6420 7265  ill be cloned re
+0000a600: 6375 7273 6976 656c 792e 2049 6620 610a  cursively. If a.
+0000a610: 2020 2020 2020 2020 7765 616b 2076 616c          weak val
+0000a620: 7565 2064 6963 7469 6f6e 6172 7920 6973  ue dictionary is
+0000a630: 2070 6173 7365 642c 2069 7420 7769 6c6c   passed, it will
+0000a640: 2062 6520 7573 6564 2074 6f20 6361 6368   be used to cach
+0000a650: 6520 636c 6f6e 6564 0a20 2020 2020 2020  e cloned.       
+0000a660: 2073 7562 6d6f 6475 6c65 732e 2054 6869   submodules. Thi
+0000a670: 7320 666c 6167 2069 7320 7573 6564 2062  s flag is used b
+0000a680: 7920 696e 6974 2f61 7070 6c79 2f62 696e  y init/apply/bin
+0000a690: 6420 746f 2061 766f 6964 2073 636f 7065  d to avoid scope
+0000a6a0: 0a20 2020 2020 2020 206c 6561 6b61 6765  .        leakage
+0000a6b0: 2e0a 2020 2020 2020 2a2a 7570 6461 7465  ..      **update
+0000a6c0: 733a 2041 7474 7269 6275 7465 2075 7064  s: Attribute upd
+0000a6d0: 6174 6573 2e0a 2020 2020 5265 7475 726e  ates..    Return
+0000a6e0: 733a 0a20 2020 2020 2041 2063 6c6f 6e65  s:.      A clone
+0000a6f0: 206f 6620 7468 6520 7468 6973 204d 6f64   of the this Mod
+0000a700: 756c 6520 7769 7468 2074 6865 2075 7064  ule with the upd
+0000a710: 6174 6564 2061 7474 7269 6275 7465 7320  ated attributes 
+0000a720: 616e 6420 7061 7265 6e74 2e0a 2020 2020  and parent..    
+0000a730: 2222 220a 2020 2020 6174 7472 7320 3d20  """.    attrs = 
+0000a740: 7b0a 2020 2020 2020 2020 662e 6e61 6d65  {.        f.name
+0000a750: 3a20 6765 7461 7474 7228 7365 6c66 2c20  : getattr(self, 
+0000a760: 662e 6e61 6d65 290a 2020 2020 2020 2020  f.name).        
+0000a770: 666f 7220 6620 696e 2064 6174 6163 6c61  for f in datacla
+0000a780: 7373 6573 2e66 6965 6c64 7328 7365 6c66  sses.fields(self
+0000a790: 290a 2020 2020 2020 2020 6966 2066 2e69  ).        if f.i
+0000a7a0: 6e69 740a 2020 2020 7d0a 0a20 2020 2061  nit.    }..    a
+0000a7b0: 7474 7273 2e75 7064 6174 6528 7061 7265  ttrs.update(pare
+0000a7c0: 6e74 3d70 6172 656e 742c 202a 2a75 7064  nt=parent, **upd
+0000a7d0: 6174 6573 290a 0a20 2020 2023 2048 6572  ates)..    # Her
+0000a7e0: 6520 7765 2069 6d70 6c65 6d65 6e74 2064  e we implement d
+0000a7f0: 6565 7020 636c 6f6e 696e 6720 6f66 2073  eep cloning of s
+0000a800: 7562 6d6f 6475 6c65 732c 2074 6869 7320  ubmodules, this 
+0000a810: 6973 206e 6563 6573 7361 7279 2074 6f20  is necessary to 
+0000a820: 6176 6f69 6420 7363 6f70 6520 6c65 616b  avoid scope leak
+0000a830: 6167 650a 2020 2020 2320 6672 6f6d 2065  age.    # from e
+0000a840: 7874 6572 6e61 6c20 7375 626d 6f64 756c  xternal submodul
+0000a850: 6573 2069 6e74 6f20 696e 6974 2f61 7070  es into init/app
+0000a860: 6c79 2f62 696e 6420 7768 696c 6520 7072  ly/bind while pr
+0000a870: 6573 6572 7669 6e67 2073 6861 7269 6e67  eserving sharing
+0000a880: 2d62 792d 7265 6665 7265 6e63 650a 2020  -by-reference.  
+0000a890: 2020 2320 7265 6c61 7469 6f6e 7368 6970    # relationship
+0000a8a0: 7320 6265 7477 6565 6e20 7375 626d 6f64  s between submod
+0000a8b0: 756c 6573 2e0a 2020 2020 6966 205f 6465  ules..    if _de
+0000a8c0: 6570 5f63 6c6f 6e65 2021 3d20 4661 6c73  ep_clone != Fals
+0000a8d0: 653a 0a20 2020 2020 2023 2057 6520 7573  e:.      # We us
+0000a8e0: 6520 6120 7765 616b 2076 616c 7565 2064  e a weak value d
+0000a8f0: 6963 7469 6f6e 6172 7920 746f 2063 6163  ictionary to cac
+0000a900: 6865 2063 6c6f 6e65 6420 7375 626d 6f64  he cloned submod
+0000a910: 756c 6573 2e20 5768 656e 2061 2073 6861  ules. When a sha
+0000a920: 7265 640a 2020 2020 2020 2320 7375 626d  red.      # subm
+0000a930: 6f64 756c 6520 6973 2063 6c6f 6e65 642c  odule is cloned,
+0000a940: 2069 7473 206f 6e6c 7920 636c 6f6e 6564   its only cloned
+0000a950: 206f 6e63 6520 656c 7365 2069 7473 2066   once else its f
+0000a960: 6574 6368 6564 2066 726f 6d20 7468 6520  etched from the 
+0000a970: 6361 6368 652e 0a20 2020 2020 2063 6163  cache..      cac
+0000a980: 6865 203d 2028 0a20 2020 2020 2020 2020  he = (.         
+0000a990: 2077 6561 6b72 6566 2e57 6561 6b56 616c   weakref.WeakVal
+0000a9a0: 7565 4469 6374 696f 6e61 7279 2829 0a20  ueDictionary(). 
+0000a9b0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000a9c0: 7374 616e 6365 285f 6465 6570 5f63 6c6f  stance(_deep_clo
+0000a9d0: 6e65 2c20 626f 6f6c 290a 2020 2020 2020  ne, bool).      
+0000a9e0: 2020 2020 656c 7365 205f 6465 6570 5f63      else _deep_c
+0000a9f0: 6c6f 6e65 0a20 2020 2020 2029 0a0a 2020  lone.      )..  
+0000aa00: 2020 2020 6465 6620 636c 6f6e 655f 666e      def clone_fn
+0000aa10: 286d 3a20 4d6f 6475 6c65 2920 2d3e 204d  (m: Module) -> M
+0000aa20: 6f64 756c 653a 0a20 2020 2020 2020 2069  odule:.        i
+0000aa30: 6620 6861 7361 7474 7228 6d2c 2027 5f69  f hasattr(m, '_i
+0000aa40: 6427 293a 0a20 2020 2020 2020 2020 206b  d'):.          k
+0000aa50: 6579 203d 206d 2e5f 6964 0a20 2020 2020  ey = m._id.     
+0000aa60: 2020 2020 2069 6620 6b65 7920 696e 2063       if key in c
+0000aa70: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
+0000aa80: 2020 7265 7475 726e 2063 6163 6865 5b6b    return cache[k
+0000aa90: 6579 5d0a 2020 2020 2020 2020 2020 656c  ey].          el
+0000aaa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000aab0: 636c 6f6e 6520 3d20 6d2e 636c 6f6e 6528  clone = m.clone(
+0000aac0: 5f64 6565 705f 636c 6f6e 653d 6361 6368  _deep_clone=cach
+0000aad0: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
+0000aae0: 6163 6865 5b6b 6579 5d20 3d20 636c 6f6e  ache[key] = clon
+0000aaf0: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
+0000ab00: 7475 726e 2063 6c6f 6e65 0a20 2020 2020  turn clone.     
+0000ab10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000ab20: 2020 2023 2049 6620 7468 6520 6d6f 6475     # If the modu
+0000ab30: 6c65 2064 6f65 736e 2774 2068 6176 6520  le doesn't have 
+0000ab40: 616e 205f 6964 2061 7474 7269 6275 7465  an _id attribute
+0000ab50: 2069 7420 636f 756c 6420 6265 2061 206d   it could be a m
+0000ab60: 6f63 6b20 6f62 6a65 6374 0a20 2020 2020  ock object.     
+0000ab70: 2020 2020 2023 2073 6f20 7765 2072 6574       # so we ret
+0000ab80: 7572 6e20 6974 2061 7320 6973 2e0a 2020  urn it as is..  
+0000ab90: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+0000aba0: 0a0a 2020 2020 2020 2320 5f6d 6170 5f73  ..      # _map_s
+0000abb0: 7562 6d6f 6475 6c65 7320 7769 6c6c 206d  ubmodules will m
+0000abc0: 6170 206f 7665 7220 616c 6c20 7375 626d  ap over all subm
+0000abd0: 6f64 756c 6573 2069 6e73 6964 6520 6174  odules inside at
+0000abe0: 7472 730a 2020 2020 2020 2320 7661 6c75  trs.      # valu
+0000abf0: 6520 6865 7265 2063 616e 2062 6520 616e  e here can be an
+0000ac00: 7920 7079 7472 6565 2c20 6e6f 6e2d 6d6f  y pytree, non-mo
+0000ac10: 6475 6c65 2076 616c 7565 7320 6172 6520  dule values are 
+0000ac20: 6967 6e6f 7265 640a 2020 2020 2020 666f  ignored.      fo
+0000ac30: 7220 6669 656c 645f 6e61 6d65 2c20 7661  r field_name, va
+0000ac40: 6c75 6520 696e 2061 7474 7273 2e69 7465  lue in attrs.ite
+0000ac50: 6d73 2829 3a0a 2020 2020 2020 2020 6174  ms():.        at
+0000ac60: 7472 735b 6669 656c 645f 6e61 6d65 5d20  trs[field_name] 
+0000ac70: 3d20 5f6d 6170 5f73 7562 6d6f 6475 6c65  = _map_submodule
+0000ac80: 7328 636c 6f6e 655f 666e 2c20 7661 6c75  s(clone_fn, valu
+0000ac90: 6529 0a0a 2020 2020 6d6f 6475 6c65 203d  e)..    module =
+0000aca0: 2073 656c 662e 5f5f 636c 6173 735f 5f28   self.__class__(
+0000acb0: 2a2a 6174 7472 7329 0a0a 2020 2020 7265  **attrs)..    re
+0000acc0: 7475 726e 206d 6f64 756c 650a 0a20 2064  turn module..  d
+0000acd0: 6566 2076 6172 6961 626c 6528 0a20 2020  ef variable(.   
+0000ace0: 2020 2073 656c 662c 0a20 2020 2020 2063     self,.      c
+0000acf0: 6f6c 3a20 7374 722c 0a20 2020 2020 206e  ol: str,.      n
+0000ad00: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
+0000ad10: 696e 6974 5f66 6e3a 204f 7074 696f 6e61  init_fn: Optiona
+0000ad20: 6c5b 4361 6c6c 6162 6c65 5b2e 2e2e 2c20  l[Callable[..., 
+0000ad30: 416e 795d 5d20 3d20 4e6f 6e65 2c0a 2020  Any]] = None,.  
+0000ad40: 2020 2020 2a69 6e69 745f 6172 6773 2c0a      *init_args,.
+0000ad50: 2020 2020 2020 756e 626f 783a 2062 6f6f        unbox: boo
+0000ad60: 6c20 3d20 5472 7565 2c0a 2020 2920 2d3e  l = True,.  ) ->
+0000ad70: 2056 6172 6961 626c 653a 0a20 2020 2022   Variable:.    "
+0000ad80: 2222 4465 636c 6172 6573 2061 6e64 2072  ""Declares and r
+0000ad90: 6574 7572 6e73 2061 2076 6172 6961 626c  eturns a variabl
+0000ada0: 6520 696e 2074 6869 7320 4d6f 6475 6c65  e in this Module
+0000adb0: 2e0a 0a20 2020 2053 6565 203a 6d6f 643a  ...    See :mod:
+0000adc0: 6066 6c61 782e 636f 7265 2e76 6172 6961  `flax.core.varia
+0000add0: 626c 6573 6020 666f 7220 6d6f 7265 2069  bles` for more i
+0000ade0: 6e66 6f72 6d61 7469 6f6e 2e20 5365 6520  nformation. See 
+0000adf0: 616c 736f 203a 6d65 7468 3a60 7061 7261  also :meth:`para
+0000ae00: 6d60 0a20 2020 2066 6f72 2061 2073 686f  m`.    for a sho
+0000ae10: 7274 6861 6e64 2077 6179 2074 6f20 6465  rthand way to de
+0000ae20: 6669 6e65 2072 6561 642d 6f6e 6c79 2076  fine read-only v
+0000ae30: 6172 6961 626c 6573 2069 6e20 7468 6520  ariables in the 
+0000ae40: 2270 6172 616d 7322 0a20 2020 2063 6f6c  "params".    col
+0000ae50: 6c65 6374 696f 6e2e 0a0a 2020 2020 436f  lection...    Co
+0000ae60: 6e74 7261 7279 2074 6f20 3a6d 6574 683a  ntrary to :meth:
+0000ae70: 6070 6172 616d 602c 2061 6c6c 2061 7267  `param`, all arg
+0000ae80: 756d 656e 7473 2070 6173 7369 6e67 2075  uments passing u
+0000ae90: 7369 6e67 2060 696e 6974 5f66 6e60 2073  sing `init_fn` s
+0000aea0: 686f 756c 6420 6265 0a20 2020 2070 6173  hould be.    pas
+0000aeb0: 7365 6420 6f6e 2065 7870 6c69 6369 746c  sed on explicitl
+0000aec0: 793a 3a0a 0a20 2020 2020 206b 6579 203d  y::..      key =
+0000aed0: 2073 656c 662e 6d61 6b65 5f72 6e67 2827   self.make_rng('
+0000aee0: 7374 6174 7327 290a 2020 2020 2020 6d65  stats').      me
+0000aef0: 616e 203d 2073 656c 662e 7661 7269 6162  an = self.variab
+0000af00: 6c65 2827 7374 6174 7327 2c20 276d 6561  le('stats', 'mea
+0000af10: 6e27 2c20 6c65 6375 6e5f 6e6f 726d 616c  n', lecun_normal
+0000af20: 2829 2c20 6b65 792c 2028 322c 2032 2929  (), key, (2, 2))
+0000af30: 0a0a 2020 2020 496e 2074 6865 2065 7861  ..    In the exa
+0000af40: 6d70 6c65 2061 626f 7665 2c20 7468 6520  mple above, the 
+0000af50: 6675 6e63 7469 6f6e 2060 6c65 6375 6e5f  function `lecun_
+0000af60: 6e6f 726d 616c 6020 6578 7065 6374 7320  normal` expects 
+0000af70: 7477 6f20 6172 6775 6d65 6e74 733a 0a20  two arguments:. 
+0000af80: 2020 2060 6b65 7960 2061 6e64 2060 7368     `key` and `sh
+0000af90: 6170 6560 2c20 616e 6420 626f 7468 2068  ape`, and both h
+0000afa0: 6176 6520 746f 2062 6520 7061 7373 6564  ave to be passed
+0000afb0: 206f 6e2e 2054 6865 2050 524e 4720 666f   on. The PRNG fo
+0000afc0: 7220 6073 7461 7473 6020 6861 730a 2020  r `stats` has.  
+0000afd0: 2020 746f 2062 6520 7072 6f76 6964 6564    to be provided
+0000afe0: 2065 7870 6c69 6369 746c 7920 7768 656e   explicitly when
+0000aff0: 2063 616c 6c69 6e67 203a 6d65 7468 3a60   calling :meth:`
+0000b000: 696e 6974 6020 616e 6420 3a6d 6574 683a  init` and :meth:
+0000b010: 6061 7070 6c79 602e 0a0a 2020 2020 4172  `apply`...    Ar
+0000b020: 6773 3a0a 2020 2020 2020 636f 6c3a 2054  gs:.      col: T
+0000b030: 6865 2076 6172 6961 626c 6520 636f 6c6c  he variable coll
+0000b040: 6563 7469 6f6e 206e 616d 652e 0a20 2020  ection name..   
+0000b050: 2020 206e 616d 653a 2054 6865 2076 6172     name: The var
+0000b060: 6961 626c 6520 6e61 6d65 2e0a 2020 2020  iable name..    
+0000b070: 2020 696e 6974 5f66 6e3a 2054 6865 2066    init_fn: The f
+0000b080: 756e 6374 696f 6e20 7468 6174 2077 696c  unction that wil
+0000b090: 6c20 6265 2063 616c 6c65 6420 746f 2063  l be called to c
+0000b0a0: 6f6d 7075 7465 2074 6865 2069 6e69 7469  ompute the initi
+0000b0b0: 616c 2076 616c 7565 0a20 2020 2020 2020  al value.       
+0000b0c0: 206f 6620 7468 6973 2076 6172 6961 626c   of this variabl
+0000b0d0: 652e 2054 6869 7320 6675 6e63 7469 6f6e  e. This function
+0000b0e0: 2077 696c 6c20 6f6e 6c79 2062 6520 6361   will only be ca
+0000b0f0: 6c6c 6564 2074 6865 2066 6972 7374 2074  lled the first t
+0000b100: 696d 650a 2020 2020 2020 2020 7468 6973  ime.        this
+0000b110: 2076 6172 6961 626c 6520 6973 2075 7365   variable is use
+0000b120: 6420 696e 2074 6869 7320 6d6f 6475 6c65  d in this module
+0000b130: 2e20 4966 204e 6f6e 652c 2074 6865 2076  . If None, the v
+0000b140: 6172 6961 626c 6520 6d75 7374 0a20 2020  ariable must.   
+0000b150: 2020 2020 2061 6c72 6561 6479 2062 6520       already be 
+0000b160: 696e 6974 6961 6c69 7a65 6420 6f74 6865  initialized othe
+0000b170: 7277 6973 6520 616e 2065 7272 6f72 2069  rwise an error i
+0000b180: 7320 7261 6973 6564 2e0a 2020 2020 2020  s raised..      
+0000b190: 2a69 6e69 745f 6172 6773 3a20 5468 6520  *init_args: The 
+0000b1a0: 6172 6775 6d65 6e74 7320 746f 2070 6173  arguments to pas
+0000b1b0: 7320 746f 2069 6e69 745f 666e 2e0a 2020  s to init_fn..  
+0000b1c0: 2020 2020 756e 626f 783a 2049 6620 5472      unbox: If Tr
+0000b1d0: 7565 2c20 6060 4178 6973 4d65 7461 6461  ue, ``AxisMetada
+0000b1e0: 7461 6060 2069 6e73 7461 6e63 6573 2061  ta`` instances a
+0000b1f0: 7265 2072 6570 6c61 6365 6420 6279 2074  re replaced by t
+0000b200: 6865 6972 2075 6e62 6f78 6564 0a20 2020  heir unboxed.   
+0000b210: 2020 2020 2076 616c 7565 2c20 7365 6520       value, see 
+0000b220: 6060 666c 6178 2e6e 6e2e 6d65 7461 2e75  ``flax.nn.meta.u
+0000b230: 6e62 6f78 6060 2028 6465 6661 756c 743a  nbox`` (default:
+0000b240: 2054 7275 6529 2e0a 0a20 2020 2052 6574   True)...    Ret
+0000b250: 7572 6e73 3a0a 2020 2020 2020 4120 3a63  urns:.      A :c
+0000b260: 6c61 7373 3a60 666c 6178 2e63 6f72 652e  lass:`flax.core.
+0000b270: 7661 7269 6162 6c65 732e 5661 7269 6162  variables.Variab
+0000b280: 6c65 6020 7468 6174 2063 616e 2062 6520  le` that can be 
+0000b290: 7265 6164 206f 7220 7365 7420 7669 610a  read or set via.
+0000b2a0: 2020 2020 2020 222e 7661 6c75 6522 2061        ".value" a
+0000b2b0: 7474 7269 6275 7465 2e20 5468 726f 7773  ttribute. Throws
+0000b2c0: 2061 6e20 6572 726f 7220 6966 2074 6865   an error if the
+0000b2d0: 2076 6172 6961 626c 6520 6578 6973 7473   variable exists
+0000b2e0: 2061 6c72 6561 6479 2e0a 2020 2020 2222   already..    ""
+0000b2f0: 220a 2020 2020 6966 206e 6f74 2073 656c  ".    if not sel
+0000b300: 662e 5f69 6e69 7469 616c 697a 6174 696f  f._initializatio
+0000b310: 6e5f 616c 6c6f 7765 643a 0a20 2020 2020  n_allowed:.     
+0000b320: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000b330: 7228 0a20 2020 2020 2020 2020 2027 5661  r(.          'Va
+0000b340: 7269 6162 6c65 7320 6d75 7374 2062 6520  riables must be 
+0000b350: 696e 6974 6961 6c69 7a65 6420 696e 2060  initialized in `
+0000b360: 7365 7475 7028 2960 206f 7220 696e 2061  setup()` or in a
+0000b370: 206d 6574 686f 6420 270a 2020 2020 2020   method '.      
+0000b380: 2020 2020 2777 7261 7070 6564 2069 6e20      'wrapped in 
+0000b390: 6040 636f 6d70 6163 7460 270a 2020 2020  `@compact`'.    
+0000b3a0: 2020 290a 2020 2020 6966 2073 656c 662e    ).    if self.
+0000b3b0: 5f6e 616d 655f 7461 6b65 6e28 6e61 6d65  _name_taken(name
+0000b3c0: 2c20 636f 6c6c 6563 7469 6f6e 3d63 6f6c  , collection=col
+0000b3d0: 293a 0a20 2020 2020 2072 6169 7365 2065  ):.      raise e
+0000b3e0: 7272 6f72 732e 4e61 6d65 496e 5573 6545  rrors.NameInUseE
+0000b3f0: 7272 6f72 2827 7661 7269 6162 6c65 272c  rror('variable',
+0000b400: 206e 616d 652c 2073 656c 662e 5f5f 636c   name, self.__cl
+0000b410: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 290a  ass__.__name__).
+0000b420: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+0000b430: 7363 6f70 6520 6973 206e 6f74 204e 6f6e  scope is not Non
+0000b440: 650a 2020 2020 7620 3d20 7365 6c66 2e73  e.    v = self.s
+0000b450: 636f 7065 2e76 6172 6961 626c 6528 636f  cope.variable(co
+0000b460: 6c2c 206e 616d 652c 2069 6e69 745f 666e  l, name, init_fn
+0000b470: 2c20 2a69 6e69 745f 6172 6773 2c20 756e  , *init_args, un
+0000b480: 626f 783d 756e 626f 7829 0a20 2020 2073  box=unbox).    s
+0000b490: 656c 662e 5f73 7461 7465 2e63 6869 6c64  elf._state.child
+0000b4a0: 7265 6e5b 6e61 6d65 5d20 3d20 636f 6c0a  ren[name] = col.
+0000b4b0: 2020 2020 7265 7475 726e 2076 0a0a 2020      return v..  
+0000b4c0: 6465 6620 7061 7261 6d28 0a20 2020 2020  def param(.     
+0000b4d0: 2073 656c 662c 206e 616d 653a 2073 7472   self, name: str
+0000b4e0: 2c20 696e 6974 5f66 6e3a 2043 616c 6c61  , init_fn: Calla
+0000b4f0: 626c 655b 2e2e 2e2c 2054 5d2c 202a 696e  ble[..., T], *in
+0000b500: 6974 5f61 7267 732c 2075 6e62 6f78 3a20  it_args, unbox: 
+0000b510: 626f 6f6c 203d 2054 7275 650a 2020 2920  bool = True.  ) 
+0000b520: 2d3e 2054 3a0a 2020 2020 2222 2244 6563  -> T:.    """Dec
+0000b530: 6c61 7265 7320 616e 6420 7265 7475 726e  lares and return
+0000b540: 7320 6120 7061 7261 6d65 7465 7220 696e  s a parameter in
+0000b550: 2074 6869 7320 4d6f 6475 6c65 2e0a 0a20   this Module... 
+0000b560: 2020 2050 6172 616d 6574 6572 7320 6172     Parameters ar
+0000b570: 6520 7265 6164 2d6f 6e6c 7920 7661 7269  e read-only vari
+0000b580: 6162 6c65 7320 696e 2074 6865 2063 6f6c  ables in the col
+0000b590: 6c65 6374 696f 6e20 6e61 6d65 6420 2270  lection named "p
+0000b5a0: 6172 616d 7322 2e20 5365 650a 2020 2020  arams". See.    
+0000b5b0: 3a6d 6f64 3a60 666c 6178 2e63 6f72 652e  :mod:`flax.core.
+0000b5c0: 7661 7269 6162 6c65 7360 2066 6f72 206d  variables` for m
+0000b5d0: 6f72 6520 6465 7461 696c 7320 6f6e 2076  ore details on v
+0000b5e0: 6172 6961 626c 6573 2e0a 0a20 2020 2054  ariables...    T
+0000b5f0: 6865 2066 6972 7374 2061 7267 756d 656e  he first argumen
+0000b600: 7420 6f66 2060 696e 6974 5f66 6e60 2069  t of `init_fn` i
+0000b610: 7320 6173 7375 6d65 6420 746f 2062 6520  s assumed to be 
+0000b620: 6120 5052 4e47 206b 6579 2c20 7768 6963  a PRNG key, whic
+0000b630: 6820 6973 0a20 2020 2070 726f 7669 6465  h is.    provide
+0000b640: 6420 6175 746f 6d61 7469 6361 6c6c 7920  d automatically 
+0000b650: 616e 6420 646f 6573 206e 6f74 2068 6176  and does not hav
+0000b660: 6520 746f 2062 6520 7061 7373 6564 2075  e to be passed u
+0000b670: 7369 6e67 2060 696e 6974 5f61 7267 7360  sing `init_args`
+0000b680: 3a3a 0a0a 2020 2020 2020 6d65 616e 203d  ::..      mean =
+0000b690: 2073 656c 662e 7061 7261 6d28 276d 6561   self.param('mea
+0000b6a0: 6e27 2c20 6c65 6375 6e5f 6e6f 726d 616c  n', lecun_normal
+0000b6b0: 2829 2c20 2832 2c20 3229 290a 0a20 2020  (), (2, 2))..   
+0000b6c0: 2049 6e20 7468 6520 6578 616d 706c 6520   In the example 
+0000b6d0: 6162 6f76 652c 2074 6865 2066 756e 6374  above, the funct
+0000b6e0: 696f 6e20 606c 6563 756e 5f6e 6f72 6d61  ion `lecun_norma
+0000b6f0: 6c60 2065 7870 6563 7473 2074 776f 2061  l` expects two a
+0000b700: 7267 756d 656e 7473 3a0a 2020 2020 606b  rguments:.    `k
+0000b710: 6579 6020 616e 6420 6073 6861 7065 602c  ey` and `shape`,
+0000b720: 2062 7574 206f 6e6c 7920 6073 6861 7065   but only `shape
+0000b730: 6020 6861 7320 746f 2062 6520 7072 6f76  ` has to be prov
+0000b740: 6964 6564 2065 7870 6c69 6369 746c 793b  ided explicitly;
+0000b750: 2060 6b65 7960 0a20 2020 2069 7320 7365   `key`.    is se
+0000b760: 7420 6175 746f 6d61 7469 6361 6c6c 7920  t automatically 
+0000b770: 7573 696e 6720 7468 6520 5052 4e47 2066  using the PRNG f
+0000b780: 6f72 2060 7061 7261 6d73 6020 7468 6174  or `params` that
+0000b790: 2069 7320 7061 7373 6564 2077 6865 6e0a   is passed when.
+0000b7a0: 2020 2020 696e 6974 6961 6c69 7a69 6e67      initializing
+0000b7b0: 2074 6865 206d 6f64 756c 6520 7573 696e   the module usin
+0000b7c0: 6720 3a6d 6574 683a 6069 6e69 7460 2e0a  g :meth:`init`..
+0000b7d0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000b7e0: 206e 616d 653a 2054 6865 2070 6172 616d   name: The param
+0000b7f0: 6574 6572 206e 616d 652e 0a20 2020 2020  eter name..     
+0000b800: 2069 6e69 745f 666e 3a20 5468 6520 6675   init_fn: The fu
+0000b810: 6e63 7469 6f6e 2074 6861 7420 7769 6c6c  nction that will
+0000b820: 2062 6520 6361 6c6c 6564 2074 6f20 636f   be called to co
+0000b830: 6d70 7574 6520 7468 6520 696e 6974 6961  mpute the initia
+0000b840: 6c20 7661 6c75 650a 2020 2020 2020 2020  l value.        
+0000b850: 6f66 2074 6869 7320 7661 7269 6162 6c65  of this variable
+0000b860: 2e20 5468 6973 2066 756e 6374 696f 6e20  . This function 
+0000b870: 7769 6c6c 206f 6e6c 7920 6265 2063 616c  will only be cal
+0000b880: 6c65 6420 7468 6520 6669 7273 7420 7469  led the first ti
+0000b890: 6d65 0a20 2020 2020 2020 2074 6869 7320  me.        this 
+0000b8a0: 7061 7261 6d65 7465 7220 6973 2075 7365  parameter is use
+0000b8b0: 6420 696e 2074 6869 7320 6d6f 6475 6c65  d in this module
+0000b8c0: 2e0a 2020 2020 2020 2a69 6e69 745f 6172  ..      *init_ar
+0000b8d0: 6773 3a20 5468 6520 6172 6775 6d65 6e74  gs: The argument
+0000b8e0: 7320 746f 2070 6173 7320 746f 2069 6e69  s to pass to ini
+0000b8f0: 745f 666e 2e0a 2020 2020 2020 756e 626f  t_fn..      unbo
+0000b900: 783a 2049 6620 5472 7565 2c20 6060 4178  x: If True, ``Ax
+0000b910: 6973 4d65 7461 6461 7461 6060 2069 6e73  isMetadata`` ins
+0000b920: 7461 6e63 6573 2061 7265 2072 6570 6c61  tances are repla
+0000b930: 6365 6420 6279 2074 6865 6972 2075 6e62  ced by their unb
+0000b940: 6f78 6564 0a20 2020 2020 2020 2076 616c  oxed.        val
+0000b950: 7565 2c20 7365 6520 6060 666c 6178 2e6e  ue, see ``flax.n
+0000b960: 6e2e 6d65 7461 2e75 6e62 6f78 6060 2028  n.meta.unbox`` (
+0000b970: 6465 6661 756c 743a 2054 7275 6529 2e0a  default: True)..
+0000b980: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000b990: 2020 2020 5468 6520 7661 6c75 6520 6f66      The value of
+0000b9a0: 2074 6865 2069 6e69 7469 616c 697a 6564   the initialized
+0000b9b0: 2070 6172 616d 6574 6572 2e20 5468 726f   parameter. Thro
+0000b9c0: 7773 2061 6e20 6572 726f 7220 6966 2074  ws an error if t
+0000b9d0: 6865 2070 6172 616d 6574 6572 0a20 2020  he parameter.   
+0000b9e0: 2020 2065 7869 7374 7320 616c 7265 6164     exists alread
+0000b9f0: 792e 0a20 2020 2022 2222 0a20 2020 2069  y..    """.    i
+0000ba00: 6620 6e6f 7420 7365 6c66 2e5f 696e 6974  f not self._init
+0000ba10: 6961 6c69 7a61 7469 6f6e 5f61 6c6c 6f77  ialization_allow
+0000ba20: 6564 3a0a 2020 2020 2020 7261 6973 6520  ed:.      raise 
+0000ba30: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+0000ba40: 2020 2020 2020 2750 6172 616d 6574 6572        'Parameter
+0000ba50: 7320 6d75 7374 2062 6520 696e 6974 6961  s must be initia
+0000ba60: 6c69 7a65 6420 696e 2060 7365 7475 7028  lized in `setup(
+0000ba70: 2960 206f 7220 696e 2061 206d 6574 686f  )` or in a metho
+0000ba80: 6420 270a 2020 2020 2020 2020 2020 2777  d '.          'w
+0000ba90: 7261 7070 6564 2069 6e20 6040 636f 6d70  rapped in `@comp
+0000baa0: 6163 7460 270a 2020 2020 2020 290a 2020  act`'.      ).  
+0000bab0: 2020 6966 2073 656c 662e 5f6e 616d 655f    if self._name_
+0000bac0: 7461 6b65 6e28 6e61 6d65 2c20 636f 6c6c  taken(name, coll
+0000bad0: 6563 7469 6f6e 3d27 7061 7261 6d73 2729  ection='params')
+0000bae0: 3a0a 2020 2020 2020 7261 6973 6520 6572  :.      raise er
+0000baf0: 726f 7273 2e4e 616d 6549 6e55 7365 4572  rors.NameInUseEr
+0000bb00: 726f 7228 2770 6172 616d 272c 206e 616d  ror('param', nam
+0000bb10: 652c 2073 656c 662e 5f5f 636c 6173 735f  e, self.__class_
+0000bb20: 5f2e 5f5f 6e61 6d65 5f5f 290a 2020 2020  _.__name__).    
+0000bb30: 6173 7365 7274 2073 656c 662e 7363 6f70  assert self.scop
+0000bb40: 6520 6973 206e 6f74 204e 6f6e 650a 2020  e is not None.  
+0000bb50: 2020 7620 3d20 7365 6c66 2e73 636f 7065    v = self.scope
+0000bb60: 2e70 6172 616d 286e 616d 652c 2069 6e69  .param(name, ini
+0000bb70: 745f 666e 2c20 2a69 6e69 745f 6172 6773  t_fn, *init_args
+0000bb80: 2c20 756e 626f 783d 756e 626f 7829 0a20  , unbox=unbox). 
+0000bb90: 2020 2073 656c 662e 5f73 7461 7465 2e63     self._state.c
+0000bba0: 6869 6c64 7265 6e5b 6e61 6d65 5d20 3d20  hildren[name] = 
+0000bbb0: 2770 6172 616d 7327 0a20 2020 2072 6574  'params'.    ret
+0000bbc0: 7572 6e20 760a 0a20 2064 6566 2068 6173  urn v..  def has
+0000bbd0: 5f76 6172 6961 626c 6528 7365 6c66 2c20  _variable(self, 
+0000bbe0: 636f 6c3a 2073 7472 2c20 6e61 6d65 3a20  col: str, name: 
+0000bbf0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+0000bc00: 2020 2222 2243 6865 636b 7320 6966 2061    """Checks if a
+0000bc10: 2076 6172 6961 626c 6520 6f66 2067 6976   variable of giv
+0000bc20: 656e 2063 6f6c 6c65 6374 696f 6e20 616e  en collection an
+0000bc30: 6420 6e61 6d65 2065 7869 7374 7320 696e  d name exists in
+0000bc40: 2074 6869 7320 4d6f 6475 6c65 2e0a 0a20   this Module... 
+0000bc50: 2020 2053 6565 203a 6d6f 643a 6066 6c61     See :mod:`fla
+0000bc60: 782e 636f 7265 2e76 6172 6961 626c 6573  x.core.variables
+0000bc70: 6020 666f 7220 6d6f 7265 2065 7870 6c61  ` for more expla
+0000bc80: 6e61 7469 6f6e 206f 6e20 7661 7269 6162  nation on variab
+0000bc90: 6c65 7320 616e 640a 2020 2020 636f 6c6c  les and.    coll
+0000bca0: 6563 7469 6f6e 732e 0a0a 2020 2020 4172  ections...    Ar
+0000bcb0: 6773 3a0a 2020 2020 2020 636f 6c3a 2054  gs:.      col: T
+0000bcc0: 6865 2076 6172 6961 626c 6520 636f 6c6c  he variable coll
+0000bcd0: 6563 7469 6f6e 206e 616d 652e 0a20 2020  ection name..   
+0000bce0: 2020 206e 616d 653a 2054 6865 206e 616d     name: The nam
+0000bcf0: 6520 6f66 2074 6865 2076 6172 6961 626c  e of the variabl
+0000bd00: 652e 0a20 2020 2052 6574 7572 6e73 3a0a  e..    Returns:.
+0000bd10: 2020 2020 2020 5472 7565 2069 6620 7468        True if th
+0000bd20: 6520 7661 7269 6162 6c65 2065 7869 7374  e variable exist
+0000bd30: 732e 0a20 2020 2022 2222 0a20 2020 2069  s..    """.    i
+0000bd40: 6620 7365 6c66 2e73 636f 7065 2069 7320  f self.scope is 
+0000bd50: 4e6f 6e65 3a0a 2020 2020 2020 7261 6973  None:.      rais
+0000bd60: 6520 5661 6c75 6545 7272 6f72 2822 4361  e ValueError("Ca
+0000bd70: 6e27 7420 6163 6365 7373 2076 6172 6961  n't access varia
+0000bd80: 626c 6573 206f 6e20 756e 626f 756e 6420  bles on unbound 
+0000bd90: 6d6f 6475 6c65 7322 290a 2020 2020 7265  modules").    re
+0000bda0: 7475 726e 2073 656c 662e 7363 6f70 652e  turn self.scope.
+0000bdb0: 6861 735f 7661 7269 6162 6c65 2863 6f6c  has_variable(col
+0000bdc0: 2c20 6e61 6d65 290a 0a20 2064 6566 2069  , name)..  def i
+0000bdd0: 735f 6d75 7461 626c 655f 636f 6c6c 6563  s_mutable_collec
+0000bde0: 7469 6f6e 2873 656c 662c 2063 6f6c 3a20  tion(self, col: 
+0000bdf0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+0000be00: 2020 2222 2252 6574 7572 6e73 2074 7275    """Returns tru
+0000be10: 6520 6966 2074 6865 2063 6f6c 6c65 6374  e if the collect
+0000be20: 696f 6e20 6063 6f6c 6020 6973 206d 7574  ion `col` is mut
+0000be30: 6162 6c65 2e22 2222 0a20 2020 2069 6620  able.""".    if 
+0000be40: 7365 6c66 2e73 636f 7065 2069 7320 4e6f  self.scope is No
+0000be50: 6e65 3a0a 2020 2020 2020 7261 6973 6520  ne:.      raise 
+0000be60: 5661 6c75 6545 7272 6f72 2822 4361 6e27  ValueError("Can'
+0000be70: 7420 6368 6563 6b20 6d75 7461 6269 6c69  t check mutabili
+0000be80: 7479 206f 6e20 756e 626f 756e 6420 6d6f  ty on unbound mo
+0000be90: 6475 6c65 7322 290a 2020 2020 7265 7475  dules").    retu
+0000bea0: 726e 2073 656c 662e 7363 6f70 652e 6973  rn self.scope.is
+0000beb0: 5f6d 7574 6162 6c65 5f63 6f6c 6c65 6374  _mutable_collect
+0000bec0: 696f 6e28 636f 6c29 0a0a 2020 6465 6620  ion(col)..  def 
+0000bed0: 6861 735f 726e 6728 7365 6c66 2c20 6e61  has_rng(self, na
+0000bee0: 6d65 3a20 7374 7229 202d 3e20 626f 6f6c  me: str) -> bool
+0000bef0: 3a0a 2020 2020 2222 2252 6574 7572 6e73  :.    """Returns
+0000bf00: 2074 7275 6520 6966 2061 2050 524e 4753   true if a PRNGS
+0000bf10: 6571 7565 6e63 6520 7769 7468 206e 616d  equence with nam
+0000bf20: 6520 606e 616d 6560 2065 7869 7374 732e  e `name` exists.
+0000bf30: 2222 220a 2020 2020 6966 2073 656c 662e  """.    if self.
+0000bf40: 7363 6f70 6520 6973 204e 6f6e 653a 0a20  scope is None:. 
+0000bf50: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000bf60: 4572 726f 7228 2243 616e 2774 2071 7565  Error("Can't que
+0000bf70: 7279 2066 6f72 2052 4e47 7320 6f6e 2075  ry for RNGs on u
+0000bf80: 6e62 6f75 6e64 206d 6f64 756c 6573 2229  nbound modules")
+0000bf90: 0a20 2020 2072 6574 7572 6e20 7365 6c66  .    return self
+0000bfa0: 2e73 636f 7065 2e68 6173 5f72 6e67 286e  .scope.has_rng(n
+0000bfb0: 616d 6529 0a0a 2020 6465 6620 6d61 6b65  ame)..  def make
+0000bfc0: 5f72 6e67 2873 656c 662c 206e 616d 653a  _rng(self, name:
+0000bfd0: 2073 7472 2920 2d3e 204b 6579 4172 7261   str) -> KeyArra
+0000bfe0: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
+0000bff0: 7320 6120 6e65 7720 524e 4720 6b65 7920  s a new RNG key 
+0000c000: 6672 6f6d 2061 2067 6976 656e 2052 4e47  from a given RNG
+0000c010: 2073 6571 7565 6e63 6520 666f 7220 7468   sequence for th
+0000c020: 6973 204d 6f64 756c 652e 0a0a 2020 2020  is Module...    
+0000c030: 5468 6520 6e65 7720 524e 4720 6b65 7920  The new RNG key 
+0000c040: 6973 2073 706c 6974 2066 726f 6d20 7468  is split from th
+0000c050: 6520 7072 6576 696f 7573 206f 6e65 2e20  e previous one. 
+0000c060: 5468 7573 2c20 6576 6572 7920 6361 6c6c  Thus, every call
+0000c070: 2074 6f0a 2020 2020 606d 616b 655f 726e   to.    `make_rn
+0000c080: 6760 2072 6574 7572 6e73 2061 206e 6577  g` returns a new
+0000c090: 2052 4e47 206b 6579 2c20 7768 696c 6520   RNG key, while 
+0000c0a0: 7374 696c 6c20 6775 6172 616e 7465 6569  still guaranteei
+0000c0b0: 6e67 2066 756c 6c0a 2020 2020 7265 7072  ng full.    repr
+0000c0c0: 6f64 7563 6962 696c 6974 792e 0a0a 2020  oducibility...  
+0000c0d0: 2020 544f 444f 3a20 4c69 6e6b 2074 6f20    TODO: Link to 
+0000c0e0: 466c 6178 2052 4e47 2064 6573 6967 6e20  Flax RNG design 
+0000c0f0: 6e6f 7465 2e0a 0a20 2020 2041 7267 733a  note...    Args:
+0000c100: 0a20 2020 2020 206e 616d 653a 2054 6865  .      name: The
+0000c110: 2052 4e47 2073 6571 7565 6e63 6520 6e61   RNG sequence na
+0000c120: 6d65 2e0a 2020 2020 5265 7475 726e 733a  me..    Returns:
+0000c130: 0a20 2020 2020 2054 6865 206e 6577 6c79  .      The newly
+0000c140: 2067 656e 6572 6174 6564 2052 4e47 206b   generated RNG k
+0000c150: 6579 2e0a 2020 2020 2222 220a 2020 2020  ey..    """.    
+0000c160: 6966 2073 656c 662e 7363 6f70 6520 6973  if self.scope is
+0000c170: 204e 6f6e 653a 0a20 2020 2020 2072 6169   None:.      rai
+0000c180: 7365 2056 616c 7565 4572 726f 7228 2243  se ValueError("C
+0000c190: 616e 2774 2075 7365 2052 4e47 7320 6f6e  an't use RNGs on
+0000c1a0: 2075 6e62 6f75 6e64 206d 6f64 756c 6573   unbound modules
+0000c1b0: 2229 0a20 2020 2072 6574 7572 6e20 7365  ").    return se
+0000c1c0: 6c66 2e73 636f 7065 2e6d 616b 655f 726e  lf.scope.make_rn
+0000c1d0: 6728 6e61 6d65 290a 0a20 2064 6566 2069  g(name)..  def i
+0000c1e0: 735f 696e 6974 6961 6c69 7a69 6e67 2873  s_initializing(s
+0000c1f0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0000c200: 2020 2222 2252 6574 7572 6e73 2054 7275    """Returns Tru
+0000c210: 6520 6966 2072 756e 6e69 6e67 2075 6e64  e if running und
+0000c220: 6572 2073 656c 662e 696e 6974 282e 2e2e  er self.init(...
+0000c230: 2920 6f72 206e 6e2e 696e 6974 282e 2e2e  ) or nn.init(...
+0000c240: 2928 292e 0a0a 2020 2020 5468 6973 2069  )()...    This i
+0000c250: 7320 6120 6865 6c70 6572 206d 6574 686f  s a helper metho
+0000c260: 6420 746f 2068 616e 646c 6520 7468 6520  d to handle the 
+0000c270: 636f 6d6d 6f6e 2063 6173 6520 6f66 2073  common case of s
+0000c280: 696d 706c 6520 696e 6974 6961 6c69 7a61  imple initializa
+0000c290: 7469 6f6e 0a20 2020 2077 6865 7265 2077  tion.    where w
+0000c2a0: 6520 7769 7368 2074 6f20 6861 7665 2073  e wish to have s
+0000c2b0: 6574 7570 206c 6f67 6963 206f 6363 7572  etup logic occur
+0000c2c0: 2077 6865 6e20 6f6e 6c79 2063 616c 6c65   when only calle
+0000c2d0: 6420 756e 6465 720a 2020 2020 6060 6d6f  d under.    ``mo
+0000c2e0: 6475 6c65 2e69 6e69 7460 6020 6f72 2060  dule.init`` or `
+0000c2f0: 606e 6e2e 696e 6974 6060 2e20 2046 6f72  `nn.init``.  For
+0000c300: 206d 6f72 6520 636f 6d70 6c69 6361 7465   more complicate
+0000c310: 6420 6d75 6c74 692d 7068 6173 650a 2020  d multi-phase.  
+0000c320: 2020 696e 6974 6961 6c69 7a61 7469 6f6e    initialization
+0000c330: 2073 6365 6e61 7269 6f73 2069 7420 6973   scenarios it is
+0000c340: 2062 6574 7465 7220 746f 2074 6573 7420   better to test 
+0000c350: 666f 7220 7468 6520 6d75 7461 6269 6c69  for the mutabili
+0000c360: 7479 206f 660a 2020 2020 7061 7274 6963  ty of.    partic
+0000c370: 756c 6172 2076 6172 6961 626c 6520 636f  ular variable co
+0000c380: 6c6c 6563 7469 6f6e 7320 6f72 2066 6f72  llections or for
+0000c390: 2074 6865 2070 7265 7365 6e63 6520 6f66   the presence of
+0000c3a0: 2070 6172 7469 6375 6c61 720a 2020 2020   particular.    
+0000c3b0: 7661 7269 6162 6c65 7320 7468 6174 2070  variables that p
+0000c3c0: 6f74 656e 7469 616c 6c79 206e 6565 6420  otentially need 
+0000c3d0: 746f 2062 6520 696e 6974 6961 6c69 7a65  to be initialize
+0000c3e0: 642e 0a20 2020 2022 2222 0a20 2020 2069  d..    """.    i
+0000c3f0: 6620 7365 6c66 2e73 636f 7065 2069 7320  f self.scope is 
+0000c400: 4e6f 6e65 3a0a 2020 2020 2020 7261 6973  None:.      rais
+0000c410: 6520 5661 6c75 6545 7272 6f72 2822 4361  e ValueError("Ca
+0000c420: 6e27 7420 6368 6563 6b20 6966 2072 756e  n't check if run
+0000c430: 6e69 6e67 2075 6e64 6572 2069 6e69 7428  ning under init(
+0000c440: 2920 6f6e 2075 6e62 6f75 6e64 206d 6f64  ) on unbound mod
+0000c450: 756c 6573 2229 0a20 2020 2072 6574 7572  ules").    retur
+0000c460: 6e20 7365 6c66 2e73 636f 7065 2e67 6574  n self.scope.get
+0000c470: 5f66 6c61 6728 2769 6e69 7469 616c 697a  _flag('initializ
+0000c480: 696e 6727 2c20 4661 6c73 6529 0a0a 2020  ing', False)..  
+0000c490: 6465 6620 5f6d 6f64 756c 655f 6368 6563  def _module_chec
+0000c4a0: 6b73 2873 656c 6629 3a0a 2020 2020 2222  ks(self):.    ""
+0000c4b0: 2252 756e 2073 7461 6e64 6172 6420 7275  "Run standard ru
+0000c4c0: 6e74 696d 6520 6368 6563 6b73 2e22 2222  ntime checks."""
+0000c4d0: 0a0a 2020 2020 6966 206e 6f74 2069 7369  ..    if not isi
+0000c4e0: 6e73 7461 6e63 6528 7365 6c66 2c20 4d6f  nstance(self, Mo
+0000c4f0: 6475 6c65 293a 0a20 2020 2020 2072 6169  dule):.      rai
+0000c500: 7365 2065 7272 6f72 732e 496e 7661 6c69  se errors.Invali
+0000c510: 6449 6e73 7461 6e63 654d 6f64 756c 6545  dInstanceModuleE
+0000c520: 7272 6f72 2829 0a0a 2020 2020 6f76 6572  rror()..    over
+0000c530: 7269 6464 656e 5f70 6f73 745f 696e 6974  ridden_post_init
+0000c540: 203d 2073 656c 662e 5f5f 706f 7374 5f69   = self.__post_i
+0000c550: 6e69 745f 5f20 213d 204d 6f64 756c 652e  nit__ != Module.
+0000c560: 5f5f 706f 7374 5f69 6e69 745f 5f0a 2020  __post_init__.  
+0000c570: 2020 6966 206f 7665 7272 6964 6465 6e5f    if overridden_
+0000c580: 706f 7374 5f69 6e69 7420 616e 6420 6e6f  post_init and no
+0000c590: 7420 6861 7361 7474 7228 7365 6c66 2c20  t hasattr(self, 
+0000c5a0: 275f 6964 2729 3a0a 2020 2020 2020 7261  '_id'):.      ra
+0000c5b0: 6973 6520 6572 726f 7273 2e49 6e63 6f72  ise errors.Incor
+0000c5c0: 7265 6374 506f 7374 496e 6974 4f76 6572  rectPostInitOver
+0000c5d0: 7269 6465 4572 726f 7228 290a 0a20 2040  rideError()..  @
+0000c5e0: 7472 6163 6562 6163 6b5f 7574 696c 2e61  traceback_util.a
+0000c5f0: 7069 5f62 6f75 6e64 6172 790a 2020 6465  pi_boundary.  de
+0000c600: 6620 6269 6e64 280a 2020 2020 2020 7365  f bind(.      se
+0000c610: 6c66 3a20 4d2c 0a20 2020 2020 2076 6172  lf: M,.      var
+0000c620: 6961 626c 6573 3a20 5661 7269 6162 6c65  iables: Variable
+0000c630: 4469 6374 2c0a 2020 2020 2020 2a61 7267  Dict,.      *arg
+0000c640: 732c 0a20 2020 2020 2072 6e67 733a 204f  s,.      rngs: O
+0000c650: 7074 696f 6e61 6c5b 524e 4753 6571 7565  ptional[RNGSeque
+0000c660: 6e63 6573 5d20 3d20 4e6f 6e65 2c0a 2020  nces] = None,.  
+0000c670: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
+0000c680: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
+0000c690: 4661 6c73 652c 0a20 2029 202d 3e20 4d3a  False,.  ) -> M:
+0000c6a0: 0a20 2020 2022 2222 4372 6561 7465 7320  .    """Creates 
+0000c6b0: 616e 2069 6e74 6572 6163 7469 7665 204d  an interactive M
+0000c6c0: 6f64 756c 6520 696e 7374 616e 6365 2062  odule instance b
+0000c6d0: 7920 6269 6e64 696e 6720 7661 7269 6162  y binding variab
+0000c6e0: 6c65 7320 616e 6420 524e 4773 2e0a 0a20  les and RNGs... 
+0000c6f0: 2020 2060 6062 696e 6460 6020 7072 6f76     ``bind`` prov
+0000c700: 6964 6573 2061 6e20 2269 6e74 6572 6163  ides an "interac
+0000c710: 7469 7665 2220 696e 7374 616e 6365 206f  tive" instance o
+0000c720: 6620 6120 4d6f 6475 6c65 2064 6972 6563  f a Module direc
+0000c730: 746c 7920 7769 7468 6f75 740a 2020 2020  tly without.    
+0000c740: 7472 616e 7366 6f72 6d69 6e67 2061 2066  transforming a f
+0000c750: 756e 6374 696f 6e20 7769 7468 2060 6061  unction with ``a
+0000c760: 7070 6c79 6060 2e20 5468 6973 2069 7320  pply``. This is 
+0000c770: 7061 7274 6963 756c 6172 6c79 2075 7365  particularly use
+0000c780: 6675 6c20 666f 720a 2020 2020 6465 6275  ful for.    debu
+0000c790: 6767 696e 6720 616e 6420 696e 7465 7261  gging and intera
+0000c7a0: 6374 6976 6520 7573 6520 6361 7365 7320  ctive use cases 
+0000c7b0: 6c69 6b65 206e 6f74 6562 6f6f 6b73 2077  like notebooks w
+0000c7c0: 6865 7265 2061 2066 756e 6374 696f 6e20  here a function 
+0000c7d0: 776f 756c 640a 2020 2020 6c69 6d69 7420  would.    limit 
+0000c7e0: 7468 6520 6162 696c 6974 7920 746f 2073  the ability to s
+0000c7f0: 706c 6974 2075 7020 636f 6465 2069 6e74  plit up code int
+0000c800: 6f20 6469 6666 6572 656e 7420 6365 6c6c  o different cell
+0000c810: 732e 0a0a 2020 2020 4f6e 6365 2074 6865  s...    Once the
+0000c820: 2076 6172 6961 626c 6573 2028 616e 6420   variables (and 
+0000c830: 6f70 7469 6f6e 616c 6c79 2052 4e47 7329  optionally RNGs)
+0000c840: 2061 7265 2062 6f75 6e64 2074 6f20 6120   are bound to a 
+0000c850: 6060 4d6f 6475 6c65 6060 2069 740a 2020  ``Module`` it.  
+0000c860: 2020 6265 636f 6d65 7320 6120 7374 6174    becomes a stat
+0000c870: 6566 756c 206f 626a 6563 742e 204e 6f74  eful object. Not
+0000c880: 6520 7468 6174 2069 6469 6f6d 6174 6963  e that idiomatic
+0000c890: 204a 4158 2069 7320 6675 6e63 7469 6f6e   JAX is function
+0000c8a0: 616c 2061 6e64 0a20 2020 2074 6865 7265  al and.    there
+0000c8b0: 666f 7265 2061 6e20 696e 7465 7261 6374  fore an interact
+0000c8c0: 6976 6520 696e 7374 616e 6365 2064 6f65  ive instance doe
+0000c8d0: 7320 6e6f 7420 6d69 7820 7765 6c6c 2077  s not mix well w
+0000c8e0: 6974 6820 7661 6e69 6c6c 6120 4a41 5820  ith vanilla JAX 
+0000c8f0: 4150 4973 2e0a 2020 2020 6060 6269 6e64  APIs..    ``bind
+0000c900: 2829 6060 2073 686f 756c 6420 6f6e 6c79  ()`` should only
+0000c910: 2062 6520 7573 6564 2066 6f72 2069 6e74   be used for int
+0000c920: 6572 6163 7469 7665 2065 7870 6572 696d  eractive experim
+0000c930: 656e 7461 7469 6f6e 2c20 616e 6420 696e  entation, and in
+0000c940: 2061 6c6c 0a20 2020 206f 7468 6572 2063   all.    other c
+0000c950: 6173 6573 2077 6520 7374 726f 6e67 6c79  ases we strongly
+0000c960: 2065 6e63 6f75 7261 6765 2075 7365 7273   encourage users
+0000c970: 2074 6f20 7573 6520 6060 6170 706c 7928   to use ``apply(
+0000c980: 2960 6020 696e 7374 6561 642e 0a0a 2020  )`` instead...  
+0000c990: 2020 4578 616d 706c 653a 3a0a 0a20 2020    Example::..   
+0000c9a0: 2020 2069 6d70 6f72 7420 6a61 780a 2020     import jax.  
+0000c9b0: 2020 2020 696d 706f 7274 206a 6178 2e6e      import jax.n
+0000c9c0: 756d 7079 2061 7320 6a6e 700a 2020 2020  umpy as jnp.    
+0000c9d0: 2020 696d 706f 7274 2066 6c61 782e 6c69    import flax.li
+0000c9e0: 6e65 6e20 6173 206e 6e0a 0a20 2020 2020  nen as nn..     
+0000c9f0: 2063 6c61 7373 2041 7574 6f45 6e63 6f64   class AutoEncod
+0000ca00: 6572 286e 6e2e 4d6f 6475 6c65 293a 0a20  er(nn.Module):. 
+0000ca10: 2020 2020 2020 2064 6566 2073 6574 7570         def setup
+0000ca20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ca30: 2020 7365 6c66 2e65 6e63 6f64 6572 203d    self.encoder =
+0000ca40: 206e 6e2e 4465 6e73 6528 3329 0a20 2020   nn.Dense(3).   
+0000ca50: 2020 2020 2020 2073 656c 662e 6465 636f         self.deco
+0000ca60: 6465 7220 3d20 6e6e 2e44 656e 7365 2835  der = nn.Dense(5
+0000ca70: 290a 0a20 2020 2020 2020 2064 6566 205f  )..        def _
+0000ca80: 5f63 616c 6c5f 5f28 7365 6c66 2c20 7829  _call__(self, x)
+0000ca90: 3a0a 2020 2020 2020 2020 2020 7265 7475  :.          retu
+0000caa0: 726e 2073 656c 662e 6465 636f 6465 7228  rn self.decoder(
+0000cab0: 7365 6c66 2e65 6e63 6f64 6572 2878 2929  self.encoder(x))
+0000cac0: 0a0a 2020 2020 2020 7820 3d20 6a6e 702e  ..      x = jnp.
+0000cad0: 6f6e 6573 2828 3136 2c20 3929 290a 2020  ones((16, 9)).  
+0000cae0: 2020 2020 6165 203d 2041 7574 6f45 6e63      ae = AutoEnc
+0000caf0: 6f64 6572 2829 0a20 2020 2020 2076 6172  oder().      var
+0000cb00: 6961 626c 6573 203d 2061 652e 696e 6974  iables = ae.init
+0000cb10: 286a 6178 2e72 616e 646f 6d2e 5052 4e47  (jax.random.PRNG
+0000cb20: 4b65 7928 3029 2c20 7829 0a20 2020 2020  Key(0), x).     
+0000cb30: 206d 6f64 656c 203d 2061 652e 6269 6e64   model = ae.bind
+0000cb40: 2876 6172 6961 626c 6573 290a 2020 2020  (variables).    
+0000cb50: 2020 7a20 3d20 6d6f 6465 6c2e 656e 636f    z = model.enco
+0000cb60: 6465 7228 7829 0a20 2020 2020 2078 5f72  der(x).      x_r
+0000cb70: 6563 6f6e 7374 7275 6374 6564 203d 206d  econstructed = m
+0000cb80: 6f64 656c 2e64 6563 6f64 6572 287a 290a  odel.decoder(z).
+0000cb90: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000cba0: 2076 6172 6961 626c 6573 3a20 4120 6469   variables: A di
+0000cbb0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+0000cbc0: 696e 6720 7661 7269 6162 6c65 7320 6b65  ing variables ke
+0000cbd0: 7965 6420 6279 2076 6172 6961 626c 650a  yed by variable.
+0000cbe0: 2020 2020 2020 2020 636f 6c6c 6563 7469          collecti
+0000cbf0: 6f6e 732e 2053 6565 203a 6d6f 643a 6066  ons. See :mod:`f
+0000cc00: 6c61 782e 636f 7265 2e76 6172 6961 626c  lax.core.variabl
+0000cc10: 6573 6020 666f 7220 6d6f 7265 2064 6574  es` for more det
+0000cc20: 6169 6c73 0a20 2020 2020 2020 2061 626f  ails.        abo
+0000cc30: 7574 2076 6172 6961 626c 6573 2e0a 2020  ut variables..  
+0000cc40: 2020 2020 2a61 7267 733a 204e 616d 6564      *args: Named
+0000cc50: 2061 7267 756d 656e 7473 2028 6e6f 7420   arguments (not 
+0000cc60: 7573 6564 292e 0a20 2020 2020 2072 6e67  used)..      rng
+0000cc70: 733a 2061 2064 6963 7420 6f66 2050 524e  s: a dict of PRN
+0000cc80: 474b 6579 7320 746f 2069 6e69 7469 616c  GKeys to initial
+0000cc90: 697a 6520 7468 6520 5052 4e47 2073 6571  ize the PRNG seq
+0000cca0: 7565 6e63 6573 2e0a 2020 2020 2020 6d75  uences..      mu
+0000ccb0: 7461 626c 653a 2043 616e 2062 6520 626f  table: Can be bo
+0000ccc0: 6f6c 2c20 7374 722c 206f 7220 6c69 7374  ol, str, or list
+0000ccd0: 2e20 5370 6563 6966 6965 7320 7768 6963  . Specifies whic
+0000cce0: 6820 636f 6c6c 6563 7469 6f6e 7320 7368  h collections sh
+0000ccf0: 6f75 6c64 2062 650a 2020 2020 2020 2020  ould be.        
+0000cd00: 7472 6561 7465 6420 6173 206d 7574 6162  treated as mutab
+0000cd10: 6c65 3a0a 2020 2020 2020 2020 2020 6060  le:.          ``
+0000cd20: 626f 6f6c 6060 3a20 616c 6c2f 6e6f 2063  bool``: all/no c
+0000cd30: 6f6c 6c65 6374 696f 6e73 2061 7265 206d  ollections are m
+0000cd40: 7574 6162 6c65 2e0a 2020 2020 2020 2020  utable..        
+0000cd50: 2020 6060 7374 7260 603a 2054 6865 206e    ``str``: The n
+0000cd60: 616d 6520 6f66 2061 2073 696e 676c 6520  ame of a single 
+0000cd70: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
+0000cd80: 6f6e 2e0a 2020 2020 2020 2020 2020 6060  on..          ``
+0000cd90: 6c69 7374 6060 3a20 4120 6c69 7374 206f  list``: A list o
+0000cda0: 6620 6e61 6d65 7320 6f66 206d 7574 6162  f names of mutab
+0000cdb0: 6c65 2063 6f6c 6c65 6374 696f 6e73 2e0a  le collections..
+0000cdc0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000cdd0: 2020 2020 4120 636f 7079 206f 6620 7468      A copy of th
+0000cde0: 6973 2069 6e73 7461 6e63 6520 7769 7468  is instance with
+0000cdf0: 2062 6f75 6e64 2076 6172 6961 626c 6573   bound variables
+0000ce00: 2061 6e64 2052 4e47 732e 0a20 2020 2022   and RNGs..    "
+0000ce10: 2222 0a20 2020 204d 6f64 756c 652e 5f6d  "".    Module._m
+0000ce20: 6f64 756c 655f 6368 6563 6b73 2873 656c  odule_checks(sel
+0000ce30: 6629 0a0a 2020 2020 6465 6c20 6172 6773  f)..    del args
+0000ce40: 0a20 2020 2073 636f 7065 203d 2063 6f72  .    scope = cor
+0000ce50: 652e 6269 6e64 2876 6172 6961 626c 6573  e.bind(variables
+0000ce60: 2c20 726e 6773 3d72 6e67 732c 206d 7574  , rngs=rngs, mut
+0000ce70: 6162 6c65 3d6d 7574 6162 6c65 290a 2020  able=mutable).  
+0000ce80: 2020 7265 7475 726e 2073 656c 662e 636c    return self.cl
+0000ce90: 6f6e 6528 7061 7265 6e74 3d73 636f 7065  one(parent=scope
+0000cea0: 2c20 5f64 6565 705f 636c 6f6e 653d 5472  , _deep_clone=Tr
+0000ceb0: 7565 290a 0a20 2064 6566 2075 6e62 696e  ue)..  def unbin
+0000cec0: 6428 7365 6c66 3a20 4d29 202d 3e20 5475  d(self: M) -> Tu
+0000ced0: 706c 655b 4d2c 2056 6172 6961 626c 6544  ple[M, VariableD
+0000cee0: 6963 745d 3a0a 2020 2020 2222 2252 6574  ict]:.    """Ret
+0000cef0: 7572 6e73 2061 6e20 756e 626f 756e 6420  urns an unbound 
+0000cf00: 636f 7079 206f 6620 6120 4d6f 6475 6c65  copy of a Module
+0000cf10: 2061 6e64 2069 7473 2076 6172 6961 626c   and its variabl
+0000cf20: 6573 2e0a 0a20 2020 2060 6075 6e62 696e  es...    ``unbin
+0000cf30: 6460 6020 6865 6c70 7320 6372 6561 7465  d`` helps create
+0000cf40: 2061 2073 7461 7465 6c65 7373 2076 6572   a stateless ver
+0000cf50: 7369 6f6e 206f 6620 6120 626f 756e 6420  sion of a bound 
+0000cf60: 4d6f 6475 6c65 2e0a 0a20 2020 2041 6e20  Module...    An 
+0000cf70: 6578 616d 706c 6520 6f66 2061 2063 6f6d  example of a com
+0000cf80: 6d6f 6e20 7573 6520 6361 7365 3a20 746f  mon use case: to
+0000cf90: 2065 7874 7261 6374 2061 2073 7562 2d4d   extract a sub-M
+0000cfa0: 6f64 756c 6520 6465 6669 6e65 6420 696e  odule defined in
+0000cfb0: 7369 6465 0a20 2020 2060 6073 6574 7570  side.    ``setup
+0000cfc0: 2829 6060 2061 6e64 2069 7473 2063 6f72  ()`` and its cor
+0000cfd0: 7265 7370 6f6e 6469 6e67 2076 6172 6961  responding varia
+0000cfe0: 626c 6573 3a20 3129 2074 656d 706f 7261  bles: 1) tempora
+0000cff0: 7269 6c79 2060 6062 696e 6460 6020 7468  rily ``bind`` th
+0000d000: 6520 7061 7265 6e74 0a20 2020 204d 6f64  e parent.    Mod
+0000d010: 756c 653b 2061 6e64 2074 6865 6e20 3229  ule; and then 2)
+0000d020: 2060 6075 6e62 696e 6460 6020 7468 6520   ``unbind`` the 
+0000d030: 6465 7369 7265 6420 7375 622d 4d6f 6475  desired sub-Modu
+0000d040: 6c65 2e20 2852 6563 616c 6c20 7468 6174  le. (Recall that
+0000d050: 2060 6073 6574 7570 2829 6060 0a20 2020   ``setup()``.   
+0000d060: 2069 7320 6f6e 6c79 2063 616c 6c65 6420   is only called 
+0000d070: 7768 656e 2074 6865 204d 6f64 756c 6520  when the Module 
+0000d080: 6973 2062 6f75 6e64 2e29 3a3a 0a0a 2020  is bound.)::..  
+0000d090: 2020 2020 636c 6173 7320 4175 746f 456e      class AutoEn
+0000d0a0: 636f 6465 7228 6e6e 2e4d 6f64 756c 6529  coder(nn.Module)
+0000d0b0: 3a0a 2020 2020 2020 2020 6465 6620 7365  :.        def se
+0000d0c0: 7475 7028 7365 6c66 293a 0a20 2020 2020  tup(self):.     
+0000d0d0: 2020 2020 2073 656c 662e 656e 636f 6465       self.encode
+0000d0e0: 7220 3d20 456e 636f 6465 7228 290a 2020  r = Encoder().  
+0000d0f0: 2020 2020 2020 2020 7365 6c66 2e64 6563          self.dec
+0000d100: 6f64 6572 203d 2044 6563 6f64 6572 2829  oder = Decoder()
+0000d110: 0a0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
+0000d120: 6361 6c6c 5f5f 2873 656c 662c 2078 293a  call__(self, x):
+0000d130: 0a20 2020 2020 2020 2020 2072 6574 7572  .          retur
+0000d140: 6e20 7365 6c66 2e64 6563 6f64 6572 2873  n self.decoder(s
+0000d150: 656c 662e 656e 636f 6465 7228 7829 290a  elf.encoder(x)).
+0000d160: 0a20 2020 2020 206d 6f64 756c 6520 3d20  .      module = 
+0000d170: 4175 746f 456e 636f 6465 7228 290a 2020  AutoEncoder().  
+0000d180: 2020 2020 7661 7269 6162 6c65 7320 3d20      variables = 
+0000d190: 6d6f 6475 6c65 2e69 6e69 7428 6a61 782e  module.init(jax.
+0000d1a0: 7261 6e64 6f6d 2e50 524e 474b 6579 2830  random.PRNGKey(0
+0000d1b0: 292c 206a 6e70 2e6f 6e65 7328 2831 2c20  ), jnp.ones((1, 
+0000d1c0: 3738 3429 2929 0a20 2020 2020 202e 2e2e  784))).      ...
+0000d1d0: 0a20 2020 2020 2023 2045 7874 7261 6374  .      # Extract
+0000d1e0: 2074 6865 2045 6e63 6f64 6572 2073 7562   the Encoder sub
+0000d1f0: 2d4d 6f64 756c 6520 616e 6420 6974 7320  -Module and its 
+0000d200: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
+0000d210: 656e 636f 6465 722c 2065 6e63 6f64 6572  encoder, encoder
+0000d220: 5f76 6172 7320 3d20 6d6f 6475 6c65 2e62  _vars = module.b
+0000d230: 696e 6428 7661 7269 6162 6c65 7329 2e65  ind(variables).e
+0000d240: 6e63 6f64 6572 2e75 6e62 696e 6428 290a  ncoder.unbind().
+0000d250: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000d260: 2020 2020 4120 7475 706c 6520 7769 7468      A tuple with
+0000d270: 2061 6e20 756e 626f 756e 6420 636f 7079   an unbound copy
+0000d280: 206f 6620 7468 6973 204d 6f64 756c 6520   of this Module 
+0000d290: 616e 6420 6974 7320 7661 7269 6162 6c65  and its variable
+0000d2a0: 732e 0a20 2020 2022 2222 0a20 2020 204d  s..    """.    M
+0000d2b0: 6f64 756c 652e 5f6d 6f64 756c 655f 6368  odule._module_ch
+0000d2c0: 6563 6b73 2873 656c 6629 0a0a 2020 2020  ecks(self)..    
+0000d2d0: 6966 2073 656c 662e 7363 6f70 6520 6973  if self.scope is
+0000d2e0: 204e 6f6e 653a 0a20 2020 2020 2072 6169   None:.      rai
+0000d2f0: 7365 2065 7272 6f72 732e 4361 6c6c 556e  se errors.CallUn
+0000d300: 6269 6e64 4f6e 556e 626f 756e 644d 6f64  bindOnUnboundMod
+0000d310: 756c 6545 7272 6f72 2829 0a0a 2020 2020  uleError()..    
+0000d320: 7661 7269 6162 6c65 7320 3d20 7365 6c66  variables = self
+0000d330: 2e76 6172 6961 626c 6573 0a20 2020 206d  .variables.    m
+0000d340: 6f64 756c 6520 3d20 7365 6c66 2e63 6c6f  odule = self.clo
+0000d350: 6e65 2829 0a20 2020 2072 6574 7572 6e20  ne().    return 
+0000d360: 6d6f 6475 6c65 2c20 7661 7269 6162 6c65  module, variable
+0000d370: 730a 0a20 2040 7472 6163 6562 6163 6b5f  s..  @traceback_
+0000d380: 7574 696c 2e61 7069 5f62 6f75 6e64 6172  util.api_boundar
+0000d390: 790a 2020 6465 6620 6170 706c 7928 0a20  y.  def apply(. 
+0000d3a0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000d3b0: 2076 6172 6961 626c 6573 3a20 5661 7269   variables: Vari
+0000d3c0: 6162 6c65 4469 6374 2c0a 2020 2020 2020  ableDict,.      
+0000d3d0: 2a61 7267 732c 0a20 2020 2020 2072 6e67  *args,.      rng
+0000d3e0: 733a 204f 7074 696f 6e61 6c5b 524e 4753  s: Optional[RNGS
+0000d3f0: 6571 7565 6e63 6573 5d20 3d20 4e6f 6e65  equences] = None
+0000d400: 2c0a 2020 2020 2020 6d65 7468 6f64 3a20  ,.      method: 
+0000d410: 556e 696f 6e5b 4361 6c6c 6162 6c65 5b2e  Union[Callable[.
+0000d420: 2e2e 2c20 416e 795d 2c20 7374 722c 204e  .., Any], str, N
+0000d430: 6f6e 655d 203d 204e 6f6e 652c 0a20 2020  one] = None,.   
+0000d440: 2020 206d 7574 6162 6c65 3a20 436f 6c6c     mutable: Coll
+0000d450: 6563 7469 6f6e 4669 6c74 6572 203d 2046  ectionFilter = F
+0000d460: 616c 7365 2c0a 2020 2020 2020 6361 7074  alse,.      capt
+0000d470: 7572 655f 696e 7465 726d 6564 6961 7465  ure_intermediate
+0000d480: 733a 2055 6e69 6f6e 5b0a 2020 2020 2020  s: Union[.      
+0000d490: 2020 2020 626f 6f6c 2c20 4361 6c6c 6162      bool, Callab
+0000d4a0: 6c65 5b5b 274d 6f64 756c 6527 2c20 7374  le[['Module', st
+0000d4b0: 725d 2c20 626f 6f6c 5d0a 2020 2020 2020  r], bool].      
+0000d4c0: 5d20 3d20 4661 6c73 652c 0a20 2020 2020  ] = False,.     
+0000d4d0: 202a 2a6b 7761 7267 732c 0a20 2029 202d   **kwargs,.  ) -
+0000d4e0: 3e20 556e 696f 6e5b 416e 792c 2054 7570  > Union[Any, Tup
+0000d4f0: 6c65 5b41 6e79 2c20 556e 696f 6e5b 4672  le[Any, Union[Fr
+0000d500: 6f7a 656e 5661 7269 6162 6c65 4469 6374  ozenVariableDict
+0000d510: 2c20 4469 6374 5b73 7472 2c20 416e 795d  , Dict[str, Any]
+0000d520: 5d5d 5d3a 0a20 2020 2022 2222 4170 706c  ]]]:.    """Appl
+0000d530: 6965 7320 6120 6d6f 6475 6c65 206d 6574  ies a module met
+0000d540: 686f 6420 746f 2076 6172 6961 626c 6573  hod to variables
+0000d550: 2061 6e64 2072 6574 7572 6e73 206f 7574   and returns out
+0000d560: 7075 7420 616e 6420 6d6f 6469 6669 6564  put and modified
+0000d570: 2076 6172 6961 626c 6573 2e0a 0a20 2020   variables...   
+0000d580: 204e 6f74 6520 7468 6174 2060 6d65 7468   Note that `meth
+0000d590: 6f64 6020 7368 6f75 6c64 2062 6520 7365  od` should be se
+0000d5a0: 7420 6966 206f 6e65 2077 6f75 6c64 206c  t if one would l
+0000d5b0: 696b 6520 746f 2063 616c 6c20 6061 7070  ike to call `app
+0000d5c0: 6c79 6020 6f6e 2061 0a20 2020 2064 6966  ly` on a.    dif
+0000d5d0: 6665 7265 6e74 2063 6c61 7373 206d 6574  ferent class met
+0000d5e0: 686f 6420 7468 616e 2060 605f 5f63 616c  hod than ``__cal
+0000d5f0: 6c5f 5f60 602e 2046 6f72 2069 6e73 7461  l__``. For insta
+0000d600: 6e63 652c 2073 7570 706f 7365 2061 0a20  nce, suppose a. 
+0000d610: 2020 2054 7261 6e73 666f 726d 6572 206d     Transformer m
+0000d620: 6f64 756c 6573 2068 6173 2061 206d 6574  odules has a met
+0000d630: 686f 6420 6361 6c6c 6564 2060 656e 636f  hod called `enco
+0000d640: 6465 602c 2074 6865 6e20 7468 6520 666f  de`, then the fo
+0000d650: 6c6c 6f77 696e 6720 6361 6c6c 730a 2020  llowing calls.  
+0000d660: 2020 6061 7070 6c79 6020 6f6e 2074 6861    `apply` on tha
+0000d670: 7420 6d65 7468 6f64 3a3a 0a0a 2020 2020  t method::..    
+0000d680: 2020 6d6f 6465 6c20 3d20 5472 616e 7366    model = Transf
+0000d690: 6f72 6d65 7228 290a 2020 2020 2020 656e  ormer().      en
+0000d6a0: 636f 6465 6420 3d20 6d6f 6465 6c2e 6170  coded = model.ap
+0000d6b0: 706c 7928 7b27 7061 7261 6d73 273a 2070  ply({'params': p
+0000d6c0: 6172 616d 737d 2c20 782c 206d 6574 686f  arams}, x, metho
+0000d6d0: 643d 5472 616e 7366 6f72 6d65 722e 656e  d=Transformer.en
+0000d6e0: 636f 6465 290a 0a20 2020 2049 6620 6120  code)..    If a 
+0000d6f0: 6675 6e63 7469 6f6e 2069 6e73 7461 6e63  function instanc
+0000d700: 6520 6973 2070 726f 7669 6465 642c 2074  e is provided, t
+0000d710: 6865 2075 6e62 6f75 6e64 2066 756e 6374  he unbound funct
+0000d720: 696f 6e20 6973 2075 7365 642e 2046 6f72  ion is used. For
+0000d730: 0a20 2020 2069 6e73 7461 6e63 652c 2074  .    instance, t
+0000d740: 6865 2065 7861 6d70 6c65 2062 656c 6f77  he example below
+0000d750: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
+0000d760: 6f20 7468 6520 6f6e 6520 6162 6f76 653a  o the one above:
+0000d770: 3a0a 0a20 2020 2020 2065 6e63 6f64 6564  :..      encoded
+0000d780: 203d 206d 6f64 656c 2e61 7070 6c79 287b   = model.apply({
+0000d790: 2770 6172 616d 7327 3a20 7061 7261 6d73  'params': params
+0000d7a0: 7d2c 2078 2c20 6d65 7468 6f64 3d6d 6f64  }, x, method=mod
+0000d7b0: 656c 2e65 6e63 6f64 6529 0a0a 2020 2020  el.encode)..    
+0000d7c0: 596f 7520 6361 6e20 616c 736f 2070 6173  You can also pas
+0000d7d0: 7320 6120 7374 7269 6e67 2074 6f20 6120  s a string to a 
+0000d7e0: 6361 6c6c 6162 6c65 2061 7474 7269 6275  callable attribu
+0000d7f0: 7465 206f 6620 7468 6520 6d6f 6475 6c65  te of the module
+0000d800: 2e20 466f 720a 2020 2020 6578 616d 706c  . For.    exampl
+0000d810: 652c 2074 6865 2070 7265 7669 6f75 7320  e, the previous 
+0000d820: 6361 6e20 6265 2077 7269 7474 656e 2061  can be written a
+0000d830: 733a 3a0a 0a20 2020 2020 2065 6e63 6f64  s::..      encod
+0000d840: 6564 203d 206d 6f64 656c 2e61 7070 6c79  ed = model.apply
+0000d850: 287b 2770 6172 616d 7327 3a20 7061 7261  ({'params': para
+0000d860: 6d73 7d2c 2078 2c20 6d65 7468 6f64 3d27  ms}, x, method='
+0000d870: 656e 636f 6465 2729 0a0a 2020 2020 4e6f  encode')..    No
+0000d880: 7465 2060 606d 6574 686f 6460 6020 6361  te ``method`` ca
+0000d890: 6e20 616c 736f 2062 6520 6120 6675 6e63  n also be a func
+0000d8a0: 7469 6f6e 2074 6861 7420 6973 206e 6f74  tion that is not
+0000d8b0: 2064 6566 696e 6564 2069 6e0a 2020 2020   defined in.    
+0000d8c0: 6060 5472 616e 7366 6f72 6d65 7260 602e  ``Transformer``.
+0000d8d0: 2049 6e20 7468 6174 2063 6173 652c 2074   In that case, t
+0000d8e0: 6865 2066 756e 6374 696f 6e20 7368 6f75  he function shou
+0000d8f0: 6c64 2068 6176 6520 6174 206c 6561 7374  ld have at least
+0000d900: 206f 6e65 0a20 2020 2061 7267 756d 656e   one.    argumen
+0000d910: 7420 7265 7072 6573 656e 7469 6e67 2061  t representing a
+0000d920: 6e20 696e 7374 616e 6365 206f 6620 7468  n instance of th
+0000d930: 6520 4d6f 6475 6c65 2063 6c61 7373 3a3a  e Module class::
+0000d940: 0a0a 2020 2020 2020 6465 6620 6f74 6865  ..      def othe
+0000d950: 725f 666e 2869 6e73 7461 6e63 652c 202e  r_fn(instance, .
+0000d960: 2e2e 293a 0a20 2020 2020 2020 2069 6e73  ..):.        ins
+0000d970: 7461 6e63 652e 736f 6d65 5f6d 6f64 756c  tance.some_modul
+0000d980: 655f 6174 7472 282e 2e2e 290a 2020 2020  e_attr(...).    
+0000d990: 2020 2020 2e2e 2e0a 0a20 2020 2020 206d      .....      m
+0000d9a0: 6f64 656c 2e61 7070 6c79 287b 2770 6172  odel.apply({'par
+0000d9b0: 616d 7327 3a20 7061 7261 6d73 7d2c 2078  ams': params}, x
+0000d9c0: 2c20 6d65 7468 6f64 3d6f 7468 6572 5f66  , method=other_f
+0000d9d0: 6e29 0a0a 2020 2020 4172 6773 3a0a 2020  n)..    Args:.  
+0000d9e0: 2020 2020 7661 7269 6162 6c65 733a 2041      variables: A
+0000d9f0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
+0000da00: 6169 6e69 6e67 2076 6172 6961 626c 6573  aining variables
+0000da10: 206b 6579 6564 2062 7920 7661 7269 6162   keyed by variab
+0000da20: 6c65 0a20 2020 2020 2020 2063 6f6c 6c65  le.        colle
+0000da30: 6374 696f 6e73 2e20 5365 6520 3a6d 6f64  ctions. See :mod
+0000da40: 3a60 666c 6178 2e63 6f72 652e 7661 7269  :`flax.core.vari
+0000da50: 6162 6c65 7360 2066 6f72 206d 6f72 6520  ables` for more 
+0000da60: 6465 7461 696c 730a 2020 2020 2020 2020  details.        
+0000da70: 6162 6f75 7420 7661 7269 6162 6c65 732e  about variables.
+0000da80: 0a20 2020 2020 202a 6172 6773 3a20 4e61  .      *args: Na
+0000da90: 6d65 6420 6172 6775 6d65 6e74 7320 7061  med arguments pa
+0000daa0: 7373 6564 2074 6f20 7468 6520 7370 6563  ssed to the spec
+0000dab0: 6966 6965 6420 6170 706c 7920 6d65 7468  ified apply meth
+0000dac0: 6f64 2e0a 2020 2020 2020 726e 6773 3a20  od..      rngs: 
+0000dad0: 6120 6469 6374 206f 6620 5052 4e47 4b65  a dict of PRNGKe
+0000dae0: 7973 2074 6f20 696e 6974 6961 6c69 7a65  ys to initialize
+0000daf0: 2074 6865 2050 524e 4720 7365 7175 656e   the PRNG sequen
+0000db00: 6365 732e 0a20 2020 2020 2020 2054 6865  ces..        The
+0000db10: 2022 7061 7261 6d73 2220 5052 4e47 2073   "params" PRNG s
+0000db20: 6571 7565 6e63 6520 6973 2075 7365 6420  equence is used 
+0000db30: 746f 2069 6e69 7469 616c 697a 6520 7061  to initialize pa
+0000db40: 7261 6d65 7465 7273 2e0a 2020 2020 2020  rameters..      
+0000db50: 6d65 7468 6f64 3a20 4120 6675 6e63 7469  method: A functi
+0000db60: 6f6e 2074 6f20 6361 6c6c 2061 7070 6c79  on to call apply
+0000db70: 206f 6e2e 2054 6869 7320 6973 2067 656e   on. This is gen
+0000db80: 6572 616c 6c79 2061 2066 756e 6374 696f  erally a functio
+0000db90: 6e20 696e 2074 6865 0a20 2020 2020 2020  n in the.       
+0000dba0: 206d 6f64 756c 652e 2049 6620 7072 6f76   module. If prov
+0000dbb0: 6964 6564 2c20 6170 706c 6965 7320 7468  ided, applies th
+0000dbc0: 6973 206d 6574 686f 642e 2049 6620 6e6f  is method. If no
+0000dbd0: 7420 7072 6f76 6964 6564 2c20 6170 706c  t provided, appl
+0000dbe0: 6965 7320 7468 650a 2020 2020 2020 2020  ies the.        
+0000dbf0: 6060 5f5f 6361 6c6c 5f5f 6060 206d 6574  ``__call__`` met
+0000dc00: 686f 6420 6f66 2074 6865 206d 6f64 756c  hod of the modul
+0000dc10: 652e 2041 2073 7472 696e 6720 6361 6e20  e. A string can 
+0000dc20: 616c 736f 2062 6520 7072 6f76 6964 6564  also be provided
+0000dc30: 2074 6f0a 2020 2020 2020 2020 7370 6563   to.        spec
+0000dc40: 6966 7920 6120 6d65 7468 6f64 2062 7920  ify a method by 
+0000dc50: 6e61 6d65 2e0a 2020 2020 2020 6d75 7461  name..      muta
+0000dc60: 626c 653a 2043 616e 2062 6520 626f 6f6c  ble: Can be bool
+0000dc70: 2c20 7374 722c 206f 7220 6c69 7374 2e20  , str, or list. 
+0000dc80: 5370 6563 6966 6965 7320 7768 6963 6820  Specifies which 
+0000dc90: 636f 6c6c 6563 7469 6f6e 7320 7368 6f75  collections shou
+0000dca0: 6c64 2062 650a 2020 2020 2020 2020 2020  ld be.          
+0000dcb0: 2020 2020 2074 7265 6174 6564 2061 7320       treated as 
+0000dcc0: 6d75 7461 626c 653a 2060 6062 6f6f 6c60  mutable: ``bool`
+0000dcd0: 603a 2061 6c6c 2f6e 6f20 636f 6c6c 6563  `: all/no collec
+0000dce0: 7469 6f6e 7320 6172 6520 6d75 7461 626c  tions are mutabl
+0000dcf0: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000dd00: 2020 6060 7374 7260 603a 2054 6865 206e    ``str``: The n
+0000dd10: 616d 6520 6f66 2061 2073 696e 676c 6520  ame of a single 
+0000dd20: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
+0000dd30: 6f6e 2e20 6060 6c69 7374 6060 3a20 410a  on. ``list``: A.
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dd50: 6973 7420 6f66 206e 616d 6573 206f 6620  ist of names of 
+0000dd60: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
+0000dd70: 6f6e 732e 0a20 2020 2020 2063 6170 7475  ons..      captu
+0000dd80: 7265 5f69 6e74 6572 6d65 6469 6174 6573  re_intermediates
+0000dd90: 3a20 4966 2060 5472 7565 602c 2063 6170  : If `True`, cap
+0000dda0: 7475 7265 7320 696e 7465 726d 6564 6961  tures intermedia
+0000ddb0: 7465 2072 6574 7572 6e20 7661 6c75 6573  te return values
+0000ddc0: 0a20 2020 2020 2020 206f 6620 616c 6c20  .        of all 
+0000ddd0: 4d6f 6475 6c65 7320 696e 7369 6465 2074  Modules inside t
+0000dde0: 6865 2022 696e 7465 726d 6564 6961 7465  he "intermediate
+0000ddf0: 7322 2063 6f6c 6c65 6374 696f 6e2e 2042  s" collection. B
+0000de00: 7920 6465 6661 756c 7420 6f6e 6c79 0a20  y default only. 
+0000de10: 2020 2020 2020 2074 6865 2072 6574 7572         the retur
+0000de20: 6e20 7661 6c75 6573 206f 6620 616c 6c20  n values of all 
+0000de30: 6060 5f5f 6361 6c6c 5f5f 6060 206d 6574  ``__call__`` met
+0000de40: 686f 6473 2061 7265 2073 746f 7265 642e  hods are stored.
+0000de50: 2041 2066 756e 6374 696f 6e20 6361 6e0a   A function can.
+0000de60: 2020 2020 2020 2020 6265 2070 6173 7365          be passe
+0000de70: 6420 746f 2063 6861 6e67 6520 7468 6520  d to change the 
+0000de80: 6669 6c74 6572 2062 6568 6176 696f 722e  filter behavior.
+0000de90: 2054 6865 2066 696c 7465 7220 6675 6e63   The filter func
+0000dea0: 7469 6f6e 2074 616b 6573 0a20 2020 2020  tion takes.     
+0000deb0: 2020 2074 6865 204d 6f64 756c 6520 696e     the Module in
+0000dec0: 7374 616e 6365 2061 6e64 206d 6574 686f  stance and metho
+0000ded0: 6420 6e61 6d65 2061 6e64 2072 6574 7572  d name and retur
+0000dee0: 6e73 2061 2062 6f6f 6c20 696e 6469 6361  ns a bool indica
+0000def0: 7469 6e67 0a20 2020 2020 2020 2077 6865  ting.        whe
+0000df00: 7468 6572 2074 6865 206f 7574 7075 7420  ther the output 
+0000df10: 6f66 2074 6861 7420 6d65 7468 6f64 2069  of that method i
+0000df20: 6e76 6f63 6174 696f 6e20 7368 6f75 6c64  nvocation should
+0000df30: 2062 6520 7374 6f72 6564 2e0a 2020 2020   be stored..    
+0000df40: 2020 2a2a 6b77 6172 6773 3a20 4b65 7977    **kwargs: Keyw
+0000df50: 6f72 6420 6172 6775 6d65 6e74 7320 7061  ord arguments pa
+0000df60: 7373 6564 2074 6f20 7468 6520 7370 6563  ssed to the spec
+0000df70: 6966 6965 6420 6170 706c 7920 6d65 7468  ified apply meth
+0000df80: 6f64 2e0a 2020 2020 5265 7475 726e 733a  od..    Returns:
+0000df90: 0a20 2020 2020 2049 6620 6060 6d75 7461  .      If ``muta
+0000dfa0: 626c 6560 6020 6973 2046 616c 7365 2c20  ble`` is False, 
+0000dfb0: 7265 7475 726e 7320 6f75 7470 7574 2e20  returns output. 
+0000dfc0: 4966 2061 6e79 2063 6f6c 6c65 6374 696f  If any collectio
+0000dfd0: 6e73 2061 7265 0a20 2020 2020 206d 7574  ns are.      mut
+0000dfe0: 6162 6c65 2c20 7265 7475 726e 7320 6060  able, returns ``
+0000dff0: 286f 7574 7075 742c 2076 6172 7329 6060  (output, vars)``
+0000e000: 2c20 7768 6572 6520 6060 7661 7273 6060  , where ``vars``
+0000e010: 2061 7265 2069 7320 6120 6469 6374 0a20   are is a dict. 
+0000e020: 2020 2020 206f 6620 7468 6520 6d6f 6469       of the modi
+0000e030: 6669 6564 2063 6f6c 6c65 6374 696f 6e73  fied collections
+0000e040: 2e0a 2020 2020 2222 220a 2020 2020 4d6f  ..    """.    Mo
+0000e050: 6475 6c65 2e5f 6d6f 6475 6c65 5f63 6865  dule._module_che
+0000e060: 636b 7328 7365 6c66 290a 0a20 2020 2069  cks(self)..    i
+0000e070: 6620 6973 696e 7374 616e 6365 286d 6574  f isinstance(met
+0000e080: 686f 642c 2073 7472 293a 0a20 2020 2020  hod, str):.     
+0000e090: 2061 7474 7269 6275 7465 5f6e 616d 6520   attribute_name 
+0000e0a0: 3d20 6d65 7468 6f64 0a20 2020 2020 206d  = method.      m
+0000e0b0: 6574 686f 6420 3d20 6765 7461 7474 7228  ethod = getattr(
+0000e0c0: 7365 6c66 2c20 6174 7472 6962 7574 655f  self, attribute_
+0000e0d0: 6e61 6d65 290a 2020 2020 2020 6966 206e  name).      if n
+0000e0e0: 6f74 2063 616c 6c61 626c 6528 6d65 7468  ot callable(meth
+0000e0f0: 6f64 293a 0a20 2020 2020 2020 2063 6c61  od):.        cla
+0000e100: 7373 5f6e 616d 6520 3d20 7479 7065 2873  ss_name = type(s
+0000e110: 656c 6629 2e5f 5f6e 616d 655f 5f0a 2020  elf).__name__.  
+0000e120: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+0000e130: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000e140: 2020 2066 2227 7b63 6c61 7373 5f6e 616d     f"'{class_nam
+0000e150: 657d 2e7b 6174 7472 6962 7574 655f 6e61  e}.{attribute_na
+0000e160: 6d65 7d27 206d 7573 7420 6265 2061 2063  me}' must be a c
+0000e170: 616c 6c61 626c 652c 2067 6f74 220a 2020  allable, got".  
+0000e180: 2020 2020 2020 2020 2020 6627 207b 7479            f' {ty
+0000e190: 7065 286d 6574 686f 6429 7d2e 270a 2020  pe(method)}.'.  
+0000e1a0: 2020 2020 2020 290a 2020 2020 656c 6966        ).    elif
+0000e1b0: 206d 6574 686f 6420 6973 204e 6f6e 653a   method is None:
+0000e1c0: 0a20 2020 2020 206d 6574 686f 6420 3d20  .      method = 
+0000e1d0: 7365 6c66 2e5f 5f63 616c 6c5f 5f0a 2020  self.__call__.  
+0000e1e0: 2020 6d65 7468 6f64 203d 205f 6765 745f    method = _get_
+0000e1f0: 756e 626f 756e 645f 666e 286d 6574 686f  unbound_fn(metho
+0000e200: 6429 0a20 2020 2072 6574 7572 6e20 6170  d).    return ap
+0000e210: 706c 7928 0a20 2020 2020 2020 206d 6574  ply(.        met
+0000e220: 686f 642c 0a20 2020 2020 2020 2073 656c  hod,.        sel
+0000e230: 662c 0a20 2020 2020 2020 206d 7574 6162  f,.        mutab
+0000e240: 6c65 3d6d 7574 6162 6c65 2c0a 2020 2020  le=mutable,.    
+0000e250: 2020 2020 6361 7074 7572 655f 696e 7465      capture_inte
+0000e260: 726d 6564 6961 7465 733d 6361 7074 7572  rmediates=captur
+0000e270: 655f 696e 7465 726d 6564 6961 7465 732c  e_intermediates,
+0000e280: 0a20 2020 2029 2876 6172 6961 626c 6573  .    )(variables
+0000e290: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+0000e2a0: 732c 2072 6e67 733d 726e 6773 290a 0a20  s, rngs=rngs).. 
+0000e2b0: 2040 7472 6163 6562 6163 6b5f 7574 696c   @traceback_util
+0000e2c0: 2e61 7069 5f62 6f75 6e64 6172 790a 2020  .api_boundary.  
+0000e2d0: 6465 6620 696e 6974 5f77 6974 685f 6f75  def init_with_ou
+0000e2e0: 7470 7574 280a 2020 2020 2020 7365 6c66  tput(.      self
+0000e2f0: 2c0a 2020 2020 2020 726e 6773 3a20 556e  ,.      rngs: Un
+0000e300: 696f 6e5b 4b65 7941 7272 6179 2c20 524e  ion[KeyArray, RN
+0000e310: 4753 6571 7565 6e63 6573 5d2c 0a20 2020  GSequences],.   
+0000e320: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
+0000e330: 6d65 7468 6f64 3a20 556e 696f 6e5b 4361  method: Union[Ca
+0000e340: 6c6c 6162 6c65 5b2e 2e2e 2c20 416e 795d  llable[..., Any]
+0000e350: 2c20 7374 722c 204e 6f6e 655d 203d 204e  , str, None] = N
+0000e360: 6f6e 652c 0a20 2020 2020 206d 7574 6162  one,.      mutab
+0000e370: 6c65 3a20 436f 6c6c 6563 7469 6f6e 4669  le: CollectionFi
+0000e380: 6c74 6572 203d 2044 656e 794c 6973 7428  lter = DenyList(
+0000e390: 2769 6e74 6572 6d65 6469 6174 6573 2729  'intermediates')
+0000e3a0: 2c0a 2020 2020 2020 6361 7074 7572 655f  ,.      capture_
+0000e3b0: 696e 7465 726d 6564 6961 7465 733a 2055  intermediates: U
+0000e3c0: 6e69 6f6e 5b0a 2020 2020 2020 2020 2020  nion[.          
+0000e3d0: 626f 6f6c 2c20 4361 6c6c 6162 6c65 5b5b  bool, Callable[[
+0000e3e0: 274d 6f64 756c 6527 2c20 7374 725d 2c20  'Module', str], 
+0000e3f0: 626f 6f6c 5d0a 2020 2020 2020 5d20 3d20  bool].      ] = 
+0000e400: 4661 6c73 652c 0a20 2020 2020 202a 2a6b  False,.      **k
+0000e410: 7761 7267 732c 0a20 2029 202d 3e20 5475  wargs,.  ) -> Tu
+0000e420: 706c 655b 416e 792c 2055 6e69 6f6e 5b46  ple[Any, Union[F
+0000e430: 726f 7a65 6e56 6172 6961 626c 6544 6963  rozenVariableDic
+0000e440: 742c 2044 6963 745b 7374 722c 2041 6e79  t, Dict[str, Any
+0000e450: 5d5d 5d3a 0a20 2020 2022 2222 496e 6974  ]]]:.    """Init
+0000e460: 6961 6c69 7a65 7320 6120 6d6f 6475 6c65  ializes a module
+0000e470: 206d 6574 686f 6420 7769 7468 2076 6172   method with var
+0000e480: 6961 626c 6573 2061 6e64 2072 6574 7572  iables and retur
+0000e490: 6e73 206f 7574 7075 7420 616e 6420 6d6f  ns output and mo
+0000e4a0: 6469 6669 6564 2076 6172 6961 626c 6573  dified variables
+0000e4b0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+0000e4c0: 2020 2072 6e67 733a 2054 6865 2072 6e67     rngs: The rng
+0000e4d0: 7320 666f 7220 7468 6520 7661 7269 6162  s for the variab
+0000e4e0: 6c65 2063 6f6c 6c65 6374 696f 6e73 2e0a  le collections..
+0000e4f0: 2020 2020 2020 2a61 7267 733a 204e 616d        *args: Nam
+0000e500: 6564 2061 7267 756d 656e 7473 2070 6173  ed arguments pas
+0000e510: 7365 6420 746f 2074 6865 2069 6e69 7420  sed to the init 
+0000e520: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
+0000e530: 6d65 7468 6f64 3a20 416e 206f 7074 696f  method: An optio
+0000e540: 6e61 6c20 6d65 7468 6f64 2e20 4966 2070  nal method. If p
+0000e550: 726f 7669 6465 642c 2061 7070 6c69 6573  rovided, applies
+0000e560: 2074 6869 7320 6d65 7468 6f64 2e20 4966   this method. If
+0000e570: 206e 6f74 0a20 2020 2020 2020 2070 726f   not.        pro
+0000e580: 7669 6465 642c 2061 7070 6c69 6573 2074  vided, applies t
+0000e590: 6865 2060 605f 5f63 616c 6c5f 5f60 6020  he ``__call__`` 
+0000e5a0: 6d65 7468 6f64 2e20 4120 7374 7269 6e67  method. A string
+0000e5b0: 2063 616e 2061 6c73 6f20 6265 270a 2020   can also be'.  
+0000e5c0: 2020 2020 2020 7072 6f76 6964 6564 2074        provided t
+0000e5d0: 6f20 7370 6563 6966 7920 6120 6d65 7468  o specify a meth
+0000e5e0: 6f64 2062 7920 6e61 6d65 2e0a 2020 2020  od by name..    
+0000e5f0: 2020 6d75 7461 626c 653a 2043 616e 2062    mutable: Can b
+0000e600: 6520 626f 6f6c 2c20 7374 722c 206f 7220  e bool, str, or 
+0000e610: 6c69 7374 2e20 5370 6563 6966 6965 7320  list. Specifies 
+0000e620: 7768 6963 6820 636f 6c6c 6563 7469 6f6e  which collection
+0000e630: 7320 7368 6f75 6c64 2062 650a 2020 2020  s should be.    
+0000e640: 2020 2020 7472 6561 7465 6420 6173 206d      treated as m
+0000e650: 7574 6162 6c65 3a20 6060 626f 6f6c 6060  utable: ``bool``
+0000e660: 3a20 616c 6c2f 6e6f 2063 6f6c 6c65 6374  : all/no collect
+0000e670: 696f 6e73 2061 7265 206d 7574 6162 6c65  ions are mutable
+0000e680: 2e0a 2020 2020 2020 2020 6060 7374 7260  ..        ``str`
+0000e690: 603a 2054 6865 206e 616d 6520 6f66 2061  `: The name of a
+0000e6a0: 2073 696e 676c 6520 6d75 7461 626c 6520   single mutable 
+0000e6b0: 636f 6c6c 6563 7469 6f6e 2e20 6060 6c69  collection. ``li
+0000e6c0: 7374 6060 3a20 410a 2020 2020 2020 2020  st``: A.        
+0000e6d0: 6c69 7374 206f 6620 6e61 6d65 7320 6f66  list of names of
+0000e6e0: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
+0000e6f0: 696f 6e73 2e20 4279 2064 6566 6175 6c74  ions. By default
+0000e700: 2061 6c6c 2063 6f6c 6c65 6374 696f 6e73   all collections
+0000e710: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000e720: 2269 6e74 6572 6d65 6469 6174 6573 2220  "intermediates" 
+0000e730: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
+0000e740: 2020 2063 6170 7475 7265 5f69 6e74 6572     capture_inter
+0000e750: 6d65 6469 6174 6573 3a20 4966 2060 5472  mediates: If `Tr
+0000e760: 7565 602c 2063 6170 7475 7265 7320 696e  ue`, captures in
+0000e770: 7465 726d 6564 6961 7465 2072 6574 7572  termediate retur
+0000e780: 6e20 7661 6c75 6573 0a20 2020 2020 2020  n values.       
+0000e790: 206f 6620 616c 6c20 4d6f 6475 6c65 7320   of all Modules 
+0000e7a0: 696e 7369 6465 2074 6865 2022 696e 7465  inside the "inte
+0000e7b0: 726d 6564 6961 7465 7322 2063 6f6c 6c65  rmediates" colle
+0000e7c0: 6374 696f 6e2e 2042 7920 6465 6661 756c  ction. By defaul
+0000e7d0: 7420 6f6e 6c79 0a20 2020 2020 2020 2074  t only.        t
+0000e7e0: 6865 2072 6574 7572 6e20 7661 6c75 6573  he return values
+0000e7f0: 206f 6620 616c 6c20 6060 5f5f 6361 6c6c   of all ``__call
+0000e800: 5f5f 6060 206d 6574 686f 6473 2061 7265  __`` methods are
+0000e810: 2073 746f 7265 642e 2041 2066 756e 6374   stored. A funct
+0000e820: 696f 6e20 6361 6e0a 2020 2020 2020 2020  ion can.        
+0000e830: 6265 2070 6173 7365 6420 746f 2063 6861  be passed to cha
+0000e840: 6e67 6520 7468 6520 6669 6c74 6572 2062  nge the filter b
+0000e850: 6568 6176 696f 722e 2054 6865 2066 696c  ehavior. The fil
+0000e860: 7465 7220 6675 6e63 7469 6f6e 2074 616b  ter function tak
+0000e870: 6573 0a20 2020 2020 2020 2074 6865 204d  es.        the M
+0000e880: 6f64 756c 6520 696e 7374 616e 6365 2061  odule instance a
+0000e890: 6e64 206d 6574 686f 6420 6e61 6d65 2061  nd method name a
+0000e8a0: 6e64 2072 6574 7572 6e73 2061 2062 6f6f  nd returns a boo
+0000e8b0: 6c20 696e 6469 6361 7469 6e67 0a20 2020  l indicating.   
+0000e8c0: 2020 2020 2077 6865 7468 6572 2074 6865       whether the
+0000e8d0: 206f 7574 7075 7420 6f66 2074 6861 7420   output of that 
+0000e8e0: 6d65 7468 6f64 2069 6e76 6f63 6174 696f  method invocatio
+0000e8f0: 6e20 7368 6f75 6c64 2062 6520 7374 6f72  n should be stor
+0000e900: 6564 2e0a 2020 2020 2020 2a2a 6b77 6172  ed..      **kwar
+0000e910: 6773 3a20 4b65 7977 6f72 6420 6172 6775  gs: Keyword argu
+0000e920: 6d65 6e74 7320 7061 7373 6564 2074 6f20  ments passed to 
+0000e930: 7468 6520 696e 6974 2066 756e 6374 696f  the init functio
+0000e940: 6e2e 0a20 2020 2052 6574 7572 6e73 3a0a  n..    Returns:.
+0000e950: 2020 2020 2020 6028 6f75 7470 7574 2c20        `(output, 
+0000e960: 7661 7273 2960 602c 2077 6865 7265 2060  vars)``, where `
+0000e970: 6076 6172 7360 6020 6172 6520 6973 2061  `vars`` are is a
+0000e980: 2064 6963 7420 6f66 2074 6865 206d 6f64   dict of the mod
+0000e990: 6966 6965 640a 2020 2020 2020 636f 6c6c  ified.      coll
+0000e9a0: 6563 7469 6f6e 732e 0a20 2020 2022 2222  ections..    """
+0000e9b0: 0a20 2020 204d 6f64 756c 652e 5f6d 6f64  .    Module._mod
+0000e9c0: 756c 655f 6368 6563 6b73 2873 656c 6629  ule_checks(self)
+0000e9d0: 0a0a 2020 2020 6966 206e 6f74 2069 7369  ..    if not isi
+0000e9e0: 6e73 7461 6e63 6528 726e 6773 2c20 6469  nstance(rngs, di
+0000e9f0: 6374 293a 0a20 2020 2020 2069 6620 6e6f  ct):.      if no
+0000ea00: 7420 636f 7265 2e73 636f 7065 2e5f 6973  t core.scope._is
+0000ea10: 5f76 616c 6964 5f72 6e67 2872 6e67 7329  _valid_rng(rngs)
+0000ea20: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+0000ea30: 6572 726f 7273 2e49 6e76 616c 6964 526e  errors.InvalidRn
+0000ea40: 6745 7272 6f72 280a 2020 2020 2020 2020  gError(.        
+0000ea50: 2020 2020 2752 4e47 7320 7368 6f75 6c64      'RNGs should
+0000ea60: 2062 6520 6f66 2073 6861 7065 2028 322c   be of shape (2,
+0000ea70: 2920 6f72 204b 6579 4172 7261 7920 696e  ) or KeyArray in
+0000ea80: 204d 6f64 756c 6520 270a 2020 2020 2020   Module '.      
+0000ea90: 2020 2020 2020 6627 7b73 656c 662e 5f5f        f'{self.__
+0000eaa0: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+0000eab0: 7d2c 2062 7574 2072 6e67 7320 6172 653a  }, but rngs are:
+0000eac0: 207b 726e 6773 7d27 0a20 2020 2020 2020   {rngs}'.       
+0000ead0: 2029 0a20 2020 2020 2072 6e67 7320 3d20   ).      rngs = 
+0000eae0: 7b27 7061 7261 6d73 273a 2072 6e67 737d  {'params': rngs}
+0000eaf0: 0a0a 2020 2020 6966 2069 7369 6e73 7461  ..    if isinsta
+0000eb00: 6e63 6528 6d65 7468 6f64 2c20 7374 7229  nce(method, str)
+0000eb10: 3a0a 2020 2020 2020 6174 7472 6962 7574  :.      attribut
+0000eb20: 655f 6e61 6d65 203d 206d 6574 686f 640a  e_name = method.
+0000eb30: 2020 2020 2020 6d65 7468 6f64 203d 2067        method = g
+0000eb40: 6574 6174 7472 2873 656c 662c 2061 7474  etattr(self, att
+0000eb50: 7269 6275 7465 5f6e 616d 6529 0a20 2020  ribute_name).   
+0000eb60: 2020 2069 6620 6e6f 7420 6361 6c6c 6162     if not callab
+0000eb70: 6c65 286d 6574 686f 6429 3a0a 2020 2020  le(method):.    
+0000eb80: 2020 2020 636c 6173 735f 6e61 6d65 203d      class_name =
+0000eb90: 2074 7970 6528 7365 6c66 292e 5f5f 6e61   type(self).__na
+0000eba0: 6d65 5f5f 0a20 2020 2020 2020 2072 6169  me__.        rai
+0000ebb0: 7365 2054 7970 6545 7272 6f72 280a 2020  se TypeError(.  
+0000ebc0: 2020 2020 2020 2020 2020 6622 277b 636c            f"'{cl
+0000ebd0: 6173 735f 6e61 6d65 7d2e 7b61 7474 7269  ass_name}.{attri
+0000ebe0: 6275 7465 5f6e 616d 657d 2720 6d75 7374  bute_name}' must
+0000ebf0: 2062 6520 6120 6361 6c6c 6162 6c65 2c20   be a callable, 
+0000ec00: 676f 7422 0a20 2020 2020 2020 2020 2020  got".           
+0000ec10: 2066 2720 7b74 7970 6528 6d65 7468 6f64   f' {type(method
+0000ec20: 297d 2e27 0a20 2020 2020 2020 2029 0a20  )}.'.        ). 
+0000ec30: 2020 2065 6c69 6620 6d65 7468 6f64 2069     elif method i
+0000ec40: 7320 4e6f 6e65 3a0a 2020 2020 2020 6d65  s None:.      me
+0000ec50: 7468 6f64 203d 2073 656c 662e 5f5f 6361  thod = self.__ca
+0000ec60: 6c6c 5f5f 0a20 2020 206d 6574 686f 6420  ll__.    method 
+0000ec70: 3d20 5f67 6574 5f75 6e62 6f75 6e64 5f66  = _get_unbound_f
+0000ec80: 6e28 6d65 7468 6f64 290a 2020 2020 7265  n(method).    re
+0000ec90: 7475 726e 2069 6e69 745f 7769 7468 5f6f  turn init_with_o
+0000eca0: 7574 7075 7428 0a20 2020 2020 2020 206d  utput(.        m
+0000ecb0: 6574 686f 642c 0a20 2020 2020 2020 2073  ethod,.        s
+0000ecc0: 656c 662c 0a20 2020 2020 2020 206d 7574  elf,.        mut
+0000ecd0: 6162 6c65 3d6d 7574 6162 6c65 2c0a 2020  able=mutable,.  
+0000ece0: 2020 2020 2020 6361 7074 7572 655f 696e        capture_in
+0000ecf0: 7465 726d 6564 6961 7465 733d 6361 7074  termediates=capt
+0000ed00: 7572 655f 696e 7465 726d 6564 6961 7465  ure_intermediate
+0000ed10: 732c 0a20 2020 2029 2872 6e67 732c 202a  s,.    )(rngs, *
+0000ed20: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+0000ed30: 0a20 2040 7472 6163 6562 6163 6b5f 7574  .  @traceback_ut
+0000ed40: 696c 2e61 7069 5f62 6f75 6e64 6172 790a  il.api_boundary.
+0000ed50: 2020 6465 6620 696e 6974 280a 2020 2020    def init(.    
+0000ed60: 2020 7365 6c66 2c0a 2020 2020 2020 726e    self,.      rn
+0000ed70: 6773 3a20 556e 696f 6e5b 4b65 7941 7272  gs: Union[KeyArr
+0000ed80: 6179 2c20 524e 4753 6571 7565 6e63 6573  ay, RNGSequences
+0000ed90: 5d2c 0a20 2020 2020 202a 6172 6773 2c0a  ],.      *args,.
+0000eda0: 2020 2020 2020 6d65 7468 6f64 3a20 556e        method: Un
+0000edb0: 696f 6e5b 4361 6c6c 6162 6c65 5b2e 2e2e  ion[Callable[...
+0000edc0: 2c20 416e 795d 2c20 7374 722c 204e 6f6e  , Any], str, Non
+0000edd0: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
+0000ede0: 206d 7574 6162 6c65 3a20 436f 6c6c 6563   mutable: Collec
+0000edf0: 7469 6f6e 4669 6c74 6572 203d 2044 656e  tionFilter = Den
+0000ee00: 794c 6973 7428 2769 6e74 6572 6d65 6469  yList('intermedi
+0000ee10: 6174 6573 2729 2c0a 2020 2020 2020 6361  ates'),.      ca
+0000ee20: 7074 7572 655f 696e 7465 726d 6564 6961  pture_intermedia
+0000ee30: 7465 733a 2055 6e69 6f6e 5b0a 2020 2020  tes: Union[.    
+0000ee40: 2020 2020 2020 626f 6f6c 2c20 4361 6c6c        bool, Call
+0000ee50: 6162 6c65 5b5b 274d 6f64 756c 6527 2c20  able[['Module', 
+0000ee60: 7374 725d 2c20 626f 6f6c 5d0a 2020 2020  str], bool].    
+0000ee70: 2020 5d20 3d20 4661 6c73 652c 0a20 2020    ] = False,.   
+0000ee80: 2020 202a 2a6b 7761 7267 732c 0a20 2029     **kwargs,.  )
+0000ee90: 202d 3e20 556e 696f 6e5b 4672 6f7a 656e   -> Union[Frozen
+0000eea0: 5661 7269 6162 6c65 4469 6374 2c20 4469  VariableDict, Di
+0000eeb0: 6374 5b73 7472 2c20 416e 795d 5d3a 0a20  ct[str, Any]]:. 
+0000eec0: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
+0000eed0: 7320 6120 6d6f 6475 6c65 206d 6574 686f  s a module metho
+0000eee0: 6420 7769 7468 2076 6172 6961 626c 6573  d with variables
+0000eef0: 2061 6e64 2072 6574 7572 6e73 206d 6f64   and returns mod
+0000ef00: 6966 6965 6420 7661 7269 6162 6c65 732e  ified variables.
+0000ef10: 0a0a 2020 2020 6060 696e 6974 6060 2074  ..    ``init`` t
+0000ef20: 616b 6573 2061 7320 6669 7273 7420 6172  akes as first ar
+0000ef30: 6775 6d65 6e74 2065 6974 6865 7220 6120  gument either a 
+0000ef40: 7369 6e67 6c65 2060 6050 524e 474b 6579  single ``PRNGKey
+0000ef50: 6060 2c20 6f72 2061 2064 6963 7469 6f6e  ``, or a diction
+0000ef60: 6172 7920 6d61 7070 696e 6720 7661 7269  ary mapping vari
+0000ef70: 6162 6c65 2063 6f6c 6c65 6374 696f 6e73  able collections
+0000ef80: 206e 616d 6573 2074 6f20 7468 6569 7220   names to their 
+0000ef90: 6060 5052 4e47 4b65 7973 6060 2c20 616e  ``PRNGKeys``, an
+0000efa0: 6420 7769 6c6c 2063 616c 6c20 6060 6d65  d will call ``me
+0000efb0: 7468 6f64 6060 2028 7768 6963 6820 6973  thod`` (which is
+0000efc0: 2074 6865 206d 6f64 756c 6527 7320 6060   the module's ``
+0000efd0: 5f5f 6361 6c6c 5f5f 6060 2066 756e 6374  __call__`` funct
+0000efe0: 696f 6e20 6279 2064 6566 6175 6c74 2920  ion by default) 
+0000eff0: 7061 7373 696e 6720 6060 2a61 7267 7360  passing ``*args`
+0000f000: 6020 616e 6420 6060 2a2a 6b77 6172 6773  ` and ``**kwargs
+0000f010: 6060 2c20 616e 6420 7265 7475 726e 730a  ``, and returns.
+0000f020: 2020 2020 6120 6469 6374 696f 6e61 7279      a dictionary
+0000f030: 206f 6620 696e 6974 6961 6c69 7a65 6420   of initialized 
+0000f040: 7661 7269 6162 6c65 732e 0a0a 2020 2020  variables...    
+0000f050: 4578 616d 706c 653a 3a0a 0a20 2020 2020  Example::..     
+0000f060: 203e 3e3e 2069 6d70 6f72 7420 666c 6178   >>> import flax
+0000f070: 2e6c 696e 656e 2061 7320 6e6e 0a20 2020  .linen as nn.   
+0000f080: 2020 203e 3e3e 2069 6d70 6f72 7420 6a61     >>> import ja
+0000f090: 782e 6e75 6d70 7920 6173 206a 6e70 0a20  x.numpy as jnp. 
+0000f0a0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+0000f0b0: 6a61 780a 2020 2020 2020 2e2e 2e0a 2020  jax.      ....  
+0000f0c0: 2020 2020 3e3e 3e20 636c 6173 7320 466f      >>> class Fo
+0000f0d0: 6f28 6e6e 2e4d 6f64 756c 6529 3a0a 2020  o(nn.Module):.  
+0000f0e0: 2020 2020 2e2e 2e20 2020 406e 6e2e 636f      ...   @nn.co
+0000f0f0: 6d70 6163 740a 2020 2020 2020 2e2e 2e20  mpact.      ... 
+0000f100: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+0000f110: 656c 662c 2078 2c20 7472 6169 6e29 3a0a  elf, x, train):.
+0000f120: 2020 2020 2020 2e2e 2e20 2020 2020 7820        ...     x 
+0000f130: 3d20 6e6e 2e44 656e 7365 2831 3629 2878  = nn.Dense(16)(x
+0000f140: 290a 2020 2020 2020 2e2e 2e20 2020 2020  ).      ...     
+0000f150: 7820 3d20 6e6e 2e42 6174 6368 4e6f 726d  x = nn.BatchNorm
+0000f160: 2875 7365 5f72 756e 6e69 6e67 5f61 7665  (use_running_ave
+0000f170: 7261 6765 3d6e 6f74 2074 7261 696e 2928  rage=not train)(
+0000f180: 7829 0a20 2020 2020 202e 2e2e 2020 2020  x).      ...    
+0000f190: 2078 203d 206e 6e2e 7265 6c75 2878 290a   x = nn.relu(x).
+0000f1a0: 2020 2020 2020 2e2e 2e20 2020 2020 7265        ...     re
+0000f1b0: 7475 726e 206e 6e2e 4465 6e73 6528 3129  turn nn.Dense(1)
+0000f1c0: 2878 290a 2020 2020 2020 2e2e 2e0a 2020  (x).      ....  
+0000f1d0: 2020 2020 3e3e 3e20 6d6f 6475 6c65 203d      >>> module =
+0000f1e0: 2046 6f6f 2829 0a20 2020 2020 203e 3e3e   Foo().      >>>
+0000f1f0: 206b 6579 203d 206a 6178 2e72 616e 646f   key = jax.rando
+0000f200: 6d2e 5052 4e47 4b65 7928 3029 0a20 2020  m.PRNGKey(0).   
+0000f210: 2020 203e 3e3e 2076 6172 6961 626c 6573     >>> variables
+0000f220: 203d 206d 6f64 756c 652e 696e 6974 286b   = module.init(k
+0000f230: 6579 2c20 6a6e 702e 656d 7074 7928 2831  ey, jnp.empty((1
+0000f240: 2c20 3729 292c 2074 7261 696e 3d46 616c  , 7)), train=Fal
+0000f250: 7365 290a 0a20 2020 2049 6620 796f 7520  se)..    If you 
+0000f260: 7061 7373 2061 2073 696e 676c 6520 6060  pass a single ``
+0000f270: 5052 4e47 4b65 7960 602c 2046 6c61 7820  PRNGKey``, Flax 
+0000f280: 7769 6c6c 2075 7365 2069 7420 746f 2066  will use it to f
+0000f290: 6565 6420 7468 6520 6060 2770 6172 616d  eed the ``'param
+0000f2a0: 7327 6060 2052 4e47 2073 7472 6561 6d2e  s'`` RNG stream.
+0000f2b0: 0a20 2020 2049 6620 796f 7520 7761 6e74  .    If you want
+0000f2c0: 2074 6f20 7573 6520 6120 6469 6666 6572   to use a differ
+0000f2d0: 656e 7420 524e 4720 7374 7265 616d 206f  ent RNG stream o
+0000f2e0: 7220 6e65 6564 2074 6f20 7573 6520 6d75  r need to use mu
+0000f2f0: 6c74 6970 6c65 2073 7472 6561 6d73 2c20  ltiple streams, 
+0000f300: 796f 7520 6d75 7374 2070 6173 7320 610a  you must pass a.
+0000f310: 2020 2020 6469 6374 696f 6e61 7279 206d      dictionary m
+0000f320: 6170 7069 6e67 2065 6163 6820 524e 4720  apping each RNG 
+0000f330: 7374 7265 616d 206e 616d 6520 746f 2069  stream name to i
+0000f340: 7473 2063 6f72 7265 7370 6f6e 6469 6e67  ts corresponding
+0000f350: 2060 6050 524e 474b 6579 6060 2074 6f20   ``PRNGKey`` to 
+0000f360: 6060 696e 6974 6060 2e0a 0a20 2020 2045  ``init``...    E
+0000f370: 7861 6d70 6c65 3a3a 0a0a 2020 2020 2020  xample::..      
+0000f380: 3e3e 3e20 636c 6173 7320 466f 6f28 6e6e  >>> class Foo(nn
+0000f390: 2e4d 6f64 756c 6529 3a0a 2020 2020 2020  .Module):.      
+0000f3a0: 2e2e 2e20 2020 406e 6e2e 636f 6d70 6163  ...   @nn.compac
+0000f3b0: 740a 2020 2020 2020 2e2e 2e20 2020 6465  t.      ...   de
+0000f3c0: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
+0000f3d0: 2078 2c20 7472 6169 6e29 3a0a 2020 2020   x, train):.    
+0000f3e0: 2020 2e2e 2e20 2020 2020 7820 3d20 6e6e    ...     x = nn
+0000f3f0: 2e44 656e 7365 2831 3629 2878 290a 2020  .Dense(16)(x).  
+0000f400: 2020 2020 2e2e 2e20 2020 2020 7820 3d20      ...     x = 
+0000f410: 6e6e 2e42 6174 6368 4e6f 726d 2875 7365  nn.BatchNorm(use
+0000f420: 5f72 756e 6e69 6e67 5f61 7665 7261 6765  _running_average
+0000f430: 3d6e 6f74 2074 7261 696e 2928 7829 0a20  =not train)(x). 
+0000f440: 2020 2020 202e 2e2e 2020 2020 2078 203d       ...     x =
+0000f450: 206e 6e2e 7265 6c75 2878 290a 2020 2020   nn.relu(x).    
+0000f460: 2020 2e2e 2e0a 2020 2020 2020 2e2e 2e20    ....      ... 
+0000f470: 2020 2020 2320 4164 6420 6761 7573 7369      # Add gaussi
+0000f480: 616e 206e 6f69 7365 0a20 2020 2020 202e  an noise.      .
+0000f490: 2e2e 2020 2020 206e 6f69 7365 5f6b 6579  ..     noise_key
+0000f4a0: 203d 2073 656c 662e 6d61 6b65 5f72 6e67   = self.make_rng
+0000f4b0: 2827 6e6f 6973 6527 290a 2020 2020 2020  ('noise').      
+0000f4c0: 2e2e 2e20 2020 2020 7820 3d20 7820 2b20  ...     x = x + 
+0000f4d0: 6a61 782e 7261 6e64 6f6d 2e6e 6f72 6d61  jax.random.norma
+0000f4e0: 6c28 6e6f 6973 655f 6b65 792c 2078 2e73  l(noise_key, x.s
+0000f4f0: 6861 7065 290a 2020 2020 2020 2e2e 2e0a  hape).      ....
+0000f500: 2020 2020 2020 2e2e 2e20 2020 2020 7265        ...     re
+0000f510: 7475 726e 206e 6e2e 4465 6e73 6528 3129  turn nn.Dense(1)
+0000f520: 2878 290a 2020 2020 2020 2e2e 2e0a 2020  (x).      ....  
+0000f530: 2020 2020 3e3e 3e20 6d6f 6475 6c65 203d      >>> module =
+0000f540: 2046 6f6f 2829 0a20 2020 2020 203e 3e3e   Foo().      >>>
+0000f550: 2072 6e67 7320 3d20 7b27 7061 7261 6d73   rngs = {'params
+0000f560: 273a 206a 6178 2e72 616e 646f 6d2e 5052  ': jax.random.PR
+0000f570: 4e47 4b65 7928 3029 2c20 276e 6f69 7365  NGKey(0), 'noise
+0000f580: 273a 206a 6178 2e72 616e 646f 6d2e 5052  ': jax.random.PR
+0000f590: 4e47 4b65 7928 3129 7d0a 2020 2020 2020  NGKey(1)}.      
+0000f5a0: 3e3e 3e20 7661 7269 6162 6c65 7320 3d20  >>> variables = 
+0000f5b0: 6d6f 6475 6c65 2e69 6e69 7428 726e 6773  module.init(rngs
+0000f5c0: 2c20 6a6e 702e 656d 7074 7928 2831 2c20  , jnp.empty((1, 
+0000f5d0: 3729 292c 2074 7261 696e 3d46 616c 7365  7)), train=False
+0000f5e0: 290a 0a20 2020 204a 6974 7469 6e67 2060  )..    Jitting `
+0000f5f0: 696e 6974 6020 696e 6974 6961 6c69 7a65  init` initialize
+0000f600: 7320 6120 6d6f 6465 6c20 6c61 7a69 6c79  s a model lazily
+0000f610: 2075 7369 6e67 206f 6e6c 7920 7468 6520   using only the 
+0000f620: 7368 6170 6573 206f 6620 7468 650a 2020  shapes of the.  
+0000f630: 2020 7072 6f76 6964 6564 2061 7267 756d    provided argum
+0000f640: 656e 7473 2c20 616e 6420 6176 6f69 6473  ents, and avoids
+0000f650: 2063 6f6d 7075 7469 6e67 2074 6865 2066   computing the f
+0000f660: 6f72 7761 7264 2070 6173 7320 7769 7468  orward pass with
+0000f670: 2061 6374 7561 6c0a 2020 2020 7661 6c75   actual.    valu
+0000f680: 6573 2e20 4578 616d 706c 653a 3a0a 0a20  es. Example::.. 
+0000f690: 2020 2020 203e 3e3e 206d 6f64 756c 6520       >>> module 
+0000f6a0: 3d20 6e6e 2e44 656e 7365 2831 290a 2020  = nn.Dense(1).  
+0000f6b0: 2020 2020 3e3e 3e20 696e 6974 5f6a 6974      >>> init_jit
+0000f6c0: 203d 206a 6178 2e6a 6974 286d 6f64 756c   = jax.jit(modul
+0000f6d0: 652e 696e 6974 290a 2020 2020 2020 3e3e  e.init).      >>
+0000f6e0: 3e20 7661 7269 6162 6c65 7320 3d20 696e  > variables = in
+0000f6f0: 6974 5f6a 6974 286a 6178 2e72 616e 646f  it_jit(jax.rando
+0000f700: 6d2e 5052 4e47 4b65 7928 3029 2c20 6a6e  m.PRNGKey(0), jn
+0000f710: 702e 656d 7074 7928 2831 2c20 3729 2929  p.empty((1, 7)))
+0000f720: 0a0a 2020 2020 6060 696e 6974 6060 2069  ..    ``init`` i
+0000f730: 7320 6120 6c69 6768 7420 7772 6170 7065  s a light wrappe
+0000f740: 7220 6f76 6572 2060 6061 7070 6c79 6060  r over ``apply``
+0000f750: 2c20 736f 206f 7468 6572 2060 6061 7070  , so other ``app
+0000f760: 6c79 6060 2061 7267 756d 656e 7473 206c  ly`` arguments l
+0000f770: 696b 650a 2020 2020 6060 6d65 7468 6f64  ike.    ``method
+0000f780: 6060 2c20 6060 6d75 7461 626c 6560 602c  ``, ``mutable``,
+0000f790: 2061 6e64 2060 6063 6170 7475 7265 5f69   and ``capture_i
+0000f7a0: 6e74 6572 6d65 6469 6174 6573 6060 2061  ntermediates`` a
+0000f7b0: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
+0000f7c0: 652e 0a0a 2020 2020 4172 6773 3a0a 2020  e...    Args:.  
+0000f7d0: 2020 2020 726e 6773 3a20 5468 6520 726e      rngs: The rn
+0000f7e0: 6773 2066 6f72 2074 6865 2076 6172 6961  gs for the varia
+0000f7f0: 626c 6520 636f 6c6c 6563 7469 6f6e 732e  ble collections.
+0000f800: 0a20 2020 2020 202a 6172 6773 3a20 4e61  .      *args: Na
+0000f810: 6d65 6420 6172 6775 6d65 6e74 7320 7061  med arguments pa
+0000f820: 7373 6564 2074 6f20 7468 6520 696e 6974  ssed to the init
+0000f830: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
+0000f840: 206d 6574 686f 643a 2041 6e20 6f70 7469   method: An opti
+0000f850: 6f6e 616c 206d 6574 686f 642e 2049 6620  onal method. If 
+0000f860: 7072 6f76 6964 6564 2c20 6170 706c 6965  provided, applie
+0000f870: 7320 7468 6973 206d 6574 686f 642e 2049  s this method. I
+0000f880: 6620 6e6f 740a 2020 2020 2020 2020 7072  f not.        pr
+0000f890: 6f76 6964 6564 2c20 6170 706c 6965 7320  ovided, applies 
+0000f8a0: 7468 6520 6060 5f5f 6361 6c6c 5f5f 6060  the ``__call__``
+0000f8b0: 206d 6574 686f 642e 2041 2073 7472 696e   method. A strin
+0000f8c0: 6720 6361 6e20 616c 736f 2062 650a 2020  g can also be.  
+0000f8d0: 2020 2020 2020 7072 6f76 6964 6564 2074        provided t
+0000f8e0: 6f20 7370 6563 6966 7920 6120 6d65 7468  o specify a meth
+0000f8f0: 6f64 2062 7920 6e61 6d65 2e0a 2020 2020  od by name..    
+0000f900: 2020 6d75 7461 626c 653a 2043 616e 2062    mutable: Can b
+0000f910: 6520 626f 6f6c 2c20 7374 722c 206f 7220  e bool, str, or 
+0000f920: 6c69 7374 2e20 5370 6563 6966 6965 7320  list. Specifies 
+0000f930: 7768 6963 6820 636f 6c6c 6563 7469 6f6e  which collection
+0000f940: 7320 7368 6f75 6c64 2062 650a 2020 2020  s should be.    
+0000f950: 2020 2020 7472 6561 7465 6420 6173 206d      treated as m
+0000f960: 7574 6162 6c65 3a20 6060 626f 6f6c 6060  utable: ``bool``
+0000f970: 3a20 616c 6c2f 6e6f 2063 6f6c 6c65 6374  : all/no collect
+0000f980: 696f 6e73 2061 7265 206d 7574 6162 6c65  ions are mutable
+0000f990: 2e0a 2020 2020 2020 2020 6060 7374 7260  ..        ``str`
+0000f9a0: 603a 2054 6865 206e 616d 6520 6f66 2061  `: The name of a
+0000f9b0: 2073 696e 676c 6520 6d75 7461 626c 6520   single mutable 
+0000f9c0: 636f 6c6c 6563 7469 6f6e 2e20 6060 6c69  collection. ``li
+0000f9d0: 7374 6060 3a20 410a 2020 2020 2020 2020  st``: A.        
+0000f9e0: 6c69 7374 206f 6620 6e61 6d65 7320 6f66  list of names of
+0000f9f0: 206d 7574 6162 6c65 2063 6f6c 6c65 6374   mutable collect
+0000fa00: 696f 6e73 2e20 4279 2064 6566 6175 6c74  ions. By default
+0000fa10: 2061 6c6c 2063 6f6c 6c65 6374 696f 6e73   all collections
+0000fa20: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000fa30: 2269 6e74 6572 6d65 6469 6174 6573 2220  "intermediates" 
+0000fa40: 6172 6520 6d75 7461 626c 652e 0a20 2020  are mutable..   
+0000fa50: 2020 2063 6170 7475 7265 5f69 6e74 6572     capture_inter
+0000fa60: 6d65 6469 6174 6573 3a20 4966 2060 5472  mediates: If `Tr
+0000fa70: 7565 602c 2063 6170 7475 7265 7320 696e  ue`, captures in
+0000fa80: 7465 726d 6564 6961 7465 2072 6574 7572  termediate retur
+0000fa90: 6e20 7661 6c75 6573 0a20 2020 2020 2020  n values.       
+0000faa0: 206f 6620 616c 6c20 4d6f 6475 6c65 7320   of all Modules 
+0000fab0: 696e 7369 6465 2074 6865 2022 696e 7465  inside the "inte
+0000fac0: 726d 6564 6961 7465 7322 2063 6f6c 6c65  rmediates" colle
+0000fad0: 6374 696f 6e2e 2042 7920 6465 6661 756c  ction. By defaul
+0000fae0: 7420 6f6e 6c79 0a20 2020 2020 2020 2074  t only.        t
+0000faf0: 6865 2072 6574 7572 6e20 7661 6c75 6573  he return values
+0000fb00: 206f 6620 616c 6c20 6060 5f5f 6361 6c6c   of all ``__call
+0000fb10: 5f5f 6060 206d 6574 686f 6473 2061 7265  __`` methods are
+0000fb20: 2073 746f 7265 642e 2041 2066 756e 6374   stored. A funct
+0000fb30: 696f 6e20 6361 6e0a 2020 2020 2020 2020  ion can.        
+0000fb40: 6265 2070 6173 7365 6420 746f 2063 6861  be passed to cha
+0000fb50: 6e67 6520 7468 6520 6669 6c74 6572 2062  nge the filter b
+0000fb60: 6568 6176 696f 722e 2054 6865 2066 696c  ehavior. The fil
+0000fb70: 7465 7220 6675 6e63 7469 6f6e 2074 616b  ter function tak
+0000fb80: 6573 0a20 2020 2020 2020 2074 6865 204d  es.        the M
+0000fb90: 6f64 756c 6520 696e 7374 616e 6365 2061  odule instance a
+0000fba0: 6e64 206d 6574 686f 6420 6e61 6d65 2061  nd method name a
+0000fbb0: 6e64 2072 6574 7572 6e73 2061 2062 6f6f  nd returns a boo
+0000fbc0: 6c20 696e 6469 6361 7469 6e67 0a20 2020  l indicating.   
+0000fbd0: 2020 2020 2077 6865 7468 6572 2074 6865       whether the
+0000fbe0: 206f 7574 7075 7420 6f66 2074 6861 7420   output of that 
+0000fbf0: 6d65 7468 6f64 2069 6e76 6f63 6174 696f  method invocatio
+0000fc00: 6e20 7368 6f75 6c64 2062 6520 7374 6f72  n should be stor
+0000fc10: 6564 2e0a 2020 2020 2020 2a2a 6b77 6172  ed..      **kwar
+0000fc20: 6773 3a20 4b65 7977 6f72 6420 6172 6775  gs: Keyword argu
+0000fc30: 6d65 6e74 7320 7061 7373 6564 2074 6f20  ments passed to 
+0000fc40: 7468 6520 696e 6974 2066 756e 6374 696f  the init functio
+0000fc50: 6e2e 0a20 2020 2052 6574 7572 6e73 3a0a  n..    Returns:.
+0000fc60: 2020 2020 2020 5468 6520 696e 6974 6961        The initia
+0000fc70: 6c69 7a65 6420 7661 7269 6162 6c65 2064  lized variable d
+0000fc80: 6963 742e 0a20 2020 2022 2222 0a20 2020  ict..    """.   
+0000fc90: 204d 6f64 756c 652e 5f6d 6f64 756c 655f   Module._module_
+0000fca0: 6368 6563 6b73 2873 656c 6629 0a0a 2020  checks(self)..  
+0000fcb0: 2020 5f2c 2076 5f6f 7574 203d 2073 656c    _, v_out = sel
+0000fcc0: 662e 696e 6974 5f77 6974 685f 6f75 7470  f.init_with_outp
+0000fcd0: 7574 280a 2020 2020 2020 2020 726e 6773  ut(.        rngs
+0000fce0: 2c0a 2020 2020 2020 2020 2a61 7267 732c  ,.        *args,
+0000fcf0: 0a20 2020 2020 2020 206d 6574 686f 643d  .        method=
+0000fd00: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
+0000fd10: 6d75 7461 626c 653d 6d75 7461 626c 652c  mutable=mutable,
+0000fd20: 0a20 2020 2020 2020 2063 6170 7475 7265  .        capture
+0000fd30: 5f69 6e74 6572 6d65 6469 6174 6573 3d63  _intermediates=c
+0000fd40: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
+0000fd50: 6174 6573 2c0a 2020 2020 2020 2020 2a2a  ates,.        **
+0000fd60: 6b77 6172 6773 2c0a 2020 2020 290a 2020  kwargs,.    ).  
+0000fd70: 2020 7265 7475 726e 2076 5f6f 7574 0a0a    return v_out..
+0000fd80: 2020 4074 7261 6365 6261 636b 5f75 7469    @traceback_uti
+0000fd90: 6c2e 6170 695f 626f 756e 6461 7279 0a20  l.api_boundary. 
+0000fda0: 2064 6566 206c 617a 795f 696e 6974 280a   def lazy_init(.
+0000fdb0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000fdc0: 2020 726e 6773 3a20 556e 696f 6e5b 4b65    rngs: Union[Ke
+0000fdd0: 7941 7272 6179 2c20 524e 4753 6571 7565  yArray, RNGSeque
+0000fde0: 6e63 6573 5d2c 0a20 2020 2020 202a 6172  nces],.      *ar
+0000fdf0: 6773 2c0a 2020 2020 2020 6d65 7468 6f64  gs,.      method
+0000fe00: 3a20 4f70 7469 6f6e 616c 5b43 616c 6c61  : Optional[Calla
+0000fe10: 626c 655b 2e2e 2e2c 2041 6e79 5d5d 203d  ble[..., Any]] =
+0000fe20: 204e 6f6e 652c 0a20 2020 2020 206d 7574   None,.      mut
+0000fe30: 6162 6c65 3a20 436f 6c6c 6563 7469 6f6e  able: Collection
+0000fe40: 4669 6c74 6572 203d 2044 656e 794c 6973  Filter = DenyLis
+0000fe50: 7428 2769 6e74 6572 6d65 6469 6174 6573  t('intermediates
+0000fe60: 2729 2c0a 2020 2020 2020 2a2a 6b77 6172  '),.      **kwar
+0000fe70: 6773 2c0a 2020 2920 2d3e 2046 726f 7a65  gs,.  ) -> Froze
+0000fe80: 6e56 6172 6961 626c 6544 6963 743a 0a20  nVariableDict:. 
+0000fe90: 2020 2022 2222 496e 6974 6961 6c69 7a65     """Initialize
+0000fea0: 7320 6120 6d6f 6475 6c65 2077 6974 686f  s a module witho
+0000feb0: 7574 2063 6f6d 7075 7469 6e67 206f 6e20  ut computing on 
+0000fec0: 616e 2061 6374 7561 6c20 696e 7075 742e  an actual input.
+0000fed0: 0a0a 2020 2020 6c61 7a79 5f69 6e69 7420  ..    lazy_init 
+0000fee0: 7769 6c6c 2069 6e69 7469 616c 697a 6520  will initialize 
+0000fef0: 7468 6520 7661 7269 6162 6c65 7320 7769  the variables wi
+0000ff00: 7468 6f75 7420 646f 696e 6720 756e 6e65  thout doing unne
+0000ff10: 6365 7373 6172 7920 636f 6d70 7574 652e  cessary compute.
+0000ff20: 0a20 2020 2054 6865 2069 6e70 7574 2064  .    The input d
+0000ff30: 6174 6120 7368 6f75 6c64 2062 6520 7061  ata should be pa
+0000ff40: 7373 6564 2061 7320 6120 6060 6a61 782e  ssed as a ``jax.
+0000ff50: 5368 6170 6544 7479 7065 5374 7275 6374  ShapeDtypeStruct
+0000ff60: 6060 2077 6869 6368 2073 7065 6369 6669  `` which specifi
+0000ff70: 6573 0a20 2020 2074 6865 2073 6861 7065  es.    the shape
+0000ff80: 2061 6e64 2064 7479 7065 206f 6620 7468   and dtype of th
+0000ff90: 6520 696e 7075 7420 6275 7420 6e6f 2063  e input but no c
+0000ffa0: 6f6e 6372 6574 6520 6461 7461 2e0a 0a20  oncrete data... 
+0000ffb0: 2020 2045 7861 6d70 6c65 3a3a 0a0a 2020     Example::..  
+0000ffc0: 2020 2020 6d6f 6465 6c20 3d20 6e6e 2e44      model = nn.D
+0000ffd0: 656e 7365 2866 6561 7475 7265 733d 3235  ense(features=25
+0000ffe0: 3629 0a20 2020 2020 2076 6172 6961 626c  6).      variabl
+0000fff0: 6573 203d 206d 6f64 656c 2e6c 617a 795f  es = model.lazy_
+00010000: 696e 6974 2872 6e67 2c20 6a61 782e 5368  init(rng, jax.Sh
+00010010: 6170 6544 7479 7065 5374 7275 6374 2828  apeDtypeStruct((
+00010020: 312c 2031 3238 292c 206a 6e70 2e66 6c6f  1, 128), jnp.flo
+00010030: 6174 3332 2929 0a0a 2020 2020 5468 6520  at32))..    The 
+00010040: 6172 6773 2061 6e64 206b 7761 7267 7320  args and kwargs 
+00010050: 6172 6773 2070 6173 7365 6420 746f 2060  args passed to `
+00010060: 606c 617a 795f 696e 6974 6060 2063 616e  `lazy_init`` can
+00010070: 2062 6520 6120 6d69 7820 6f66 0a20 2020   be a mix of.   
+00010080: 2063 6f6e 6372 6574 6520 286a 6178 2061   concrete (jax a
+00010090: 7272 6179 732c 2073 6361 6c61 7273 2c20  rrays, scalars, 
+000100a0: 626f 6f6c 7329 2061 6e64 2061 6273 7472  bools) and abstr
+000100b0: 6163 7420 2853 6861 7065 4474 7970 6553  act (ShapeDtypeS
+000100c0: 7472 7563 7429 2076 616c 7565 732e 0a20  truct) values.. 
+000100d0: 2020 2043 6f6e 6372 6574 6520 7661 6c75     Concrete valu
+000100e0: 6573 2061 7265 206f 6e6c 7920 6e65 6365  es are only nece
+000100f0: 7373 6172 7920 666f 7220 6172 6775 6d65  ssary for argume
+00010100: 6e74 7320 7468 6174 2061 6666 6563 740a  nts that affect.
+00010110: 2020 2020 7468 6520 696e 6974 6961 6c69      the initiali
+00010120: 7a61 7469 6f6e 206f 6620 7661 7269 6162  zation of variab
+00010130: 6c65 732e 2046 6f72 2065 7861 6d70 6c65  les. For example
+00010140: 2c20 7468 6520 6d6f 6465 6c20 6d69 6768  , the model migh
+00010150: 7420 6578 7065 6374 0a20 2020 2061 206b  t expect.    a k
+00010160: 6579 776f 7264 2061 7267 2074 6861 7420  eyword arg that 
+00010170: 656e 6162 6c65 732f 6469 7361 626c 6573  enables/disables
+00010180: 2061 2073 7562 7061 7274 206f 6620 7468   a subpart of th
+00010190: 6520 6d6f 6465 6c2e 0a20 2020 2049 6e20  e model..    In 
+000101a0: 7468 6973 2063 6173 652c 2061 6e20 6578  this case, an ex
+000101b0: 706c 6963 6974 2076 616c 7565 2028 5472  plicit value (Tr
+000101c0: 7565 2f46 6c61 7365 2920 7368 6f75 6c64  ue/Flase) should
+000101d0: 2062 6520 7061 7373 6564 206f 7468 6572   be passed other
+000101e0: 7769 7365 0a20 2020 2060 606c 617a 795f  wise.    ``lazy_
+000101f0: 696e 6974 6060 2063 616e 6e6f 7420 696e  init`` cannot in
+00010200: 6665 7220 7768 6963 6820 7661 7269 6162  fer which variab
+00010210: 6c65 7320 7368 6f75 6c64 2062 6520 696e  les should be in
+00010220: 6974 6961 6c69 7a65 642e 0a0a 2020 2020  itialized...    
+00010230: 4172 6773 3a0a 2020 2020 2020 726e 6773  Args:.      rngs
+00010240: 3a20 5468 6520 726e 6773 2066 6f72 2074  : The rngs for t
+00010250: 6865 2076 6172 6961 626c 6520 636f 6c6c  he variable coll
+00010260: 6563 7469 6f6e 732e 0a20 2020 2020 202a  ections..      *
+00010270: 6172 6773 3a20 6172 6775 6d65 6e74 7320  args: arguments 
+00010280: 7061 7373 6564 2074 6f20 7468 6520 696e  passed to the in
+00010290: 6974 2066 756e 6374 696f 6e2e 0a20 2020  it function..   
+000102a0: 2020 206d 6574 686f 643a 2041 6e20 6f70     method: An op
+000102b0: 7469 6f6e 616c 206d 6574 686f 642e 2049  tional method. I
+000102c0: 6620 7072 6f76 6964 6564 2c20 6170 706c  f provided, appl
+000102d0: 6965 7320 7468 6973 206d 6574 686f 642e  ies this method.
+000102e0: 2049 6620 6e6f 740a 2020 2020 2020 2020   If not.        
+000102f0: 7072 6f76 6964 6564 2c20 6170 706c 6965  provided, applie
+00010300: 7320 7468 6520 6060 5f5f 6361 6c6c 5f5f  s the ``__call__
+00010310: 6060 206d 6574 686f 642e 0a20 2020 2020  `` method..     
+00010320: 206d 7574 6162 6c65 3a20 4361 6e20 6265   mutable: Can be
+00010330: 2062 6f6f 6c2c 2073 7472 2c20 6f72 206c   bool, str, or l
+00010340: 6973 742e 2053 7065 6369 6669 6573 2077  ist. Specifies w
+00010350: 6869 6368 2063 6f6c 6c65 6374 696f 6e73  hich collections
+00010360: 2073 686f 756c 6420 6265 0a20 2020 2020   should be.     
+00010370: 2020 2074 7265 6174 6564 2061 7320 6d75     treated as mu
+00010380: 7461 626c 653a 2060 6062 6f6f 6c60 603a  table: ``bool``:
+00010390: 2061 6c6c 2f6e 6f20 636f 6c6c 6563 7469   all/no collecti
+000103a0: 6f6e 7320 6172 6520 6d75 7461 626c 652e  ons are mutable.
+000103b0: 0a20 2020 2020 2020 2060 6073 7472 6060  .        ``str``
+000103c0: 3a20 5468 6520 6e61 6d65 206f 6620 6120  : The name of a 
+000103d0: 7369 6e67 6c65 206d 7574 6162 6c65 2063  single mutable c
+000103e0: 6f6c 6c65 6374 696f 6e2e 2060 606c 6973  ollection. ``lis
+000103f0: 7460 603a 2041 0a20 2020 2020 2020 206c  t``: A.        l
+00010400: 6973 7420 6f66 206e 616d 6573 206f 6620  ist of names of 
+00010410: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
+00010420: 6f6e 732e 2042 7920 6465 6661 756c 7420  ons. By default 
+00010430: 616c 6c20 636f 6c6c 6563 7469 6f6e 730a  all collections.
+00010440: 2020 2020 2020 2020 6578 6365 7074 2022          except "
+00010450: 696e 7465 726d 6564 6961 7465 7322 2061  intermediates" a
+00010460: 7265 206d 7574 6162 6c65 2e0a 2020 2020  re mutable..    
+00010470: 2020 2a2a 6b77 6172 6773 3a20 4b65 7977    **kwargs: Keyw
+00010480: 6f72 6420 6172 6775 6d65 6e74 7320 7061  ord arguments pa
+00010490: 7373 6564 2074 6f20 7468 6520 696e 6974  ssed to the init
+000104a0: 2066 756e 6374 696f 6e2e 0a20 2020 2052   function..    R
+000104b0: 6574 7572 6e73 3a0a 2020 2020 2020 5468  eturns:.      Th
+000104c0: 6520 696e 6974 6961 6c69 7a65 6420 7661  e initialized va
+000104d0: 7269 6162 6c65 2064 6963 742e 0a20 2020  riable dict..   
+000104e0: 2022 2222 0a20 2020 204d 6f64 756c 652e   """.    Module.
+000104f0: 5f6d 6f64 756c 655f 6368 6563 6b73 2873  _module_checks(s
+00010500: 656c 6629 0a0a 2020 2020 6465 6620 6c61  elf)..    def la
+00010510: 7a79 5f77 7261 7070 6572 2872 6e67 732c  zy_wrapper(rngs,
+00010520: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00010530: 293a 0a20 2020 2020 2072 6574 7572 6e20  ):.      return 
+00010540: 7365 6c66 2e69 6e69 7428 726e 6773 2c20  self.init(rngs, 
+00010550: 2a61 7267 732c 206d 6574 686f 643d 6d65  *args, method=me
+00010560: 7468 6f64 2c20 6d75 7461 626c 653d 6d75  thod, mutable=mu
+00010570: 7461 626c 652c 202a 2a6b 7761 7267 7329  table, **kwargs)
+00010580: 0a0a 2020 2020 7265 7475 726e 2070 6172  ..    return par
+00010590: 7469 616c 5f65 7661 6c2e 6c61 7a79 5f69  tial_eval.lazy_i
+000105a0: 6e69 7428 6c61 7a79 5f77 7261 7070 6572  nit(lazy_wrapper
+000105b0: 2928 726e 6773 2c20 2a61 7267 732c 202a  )(rngs, *args, *
+000105c0: 2a6b 7761 7267 7329 0a0a 2020 4070 726f  *kwargs)..  @pro
+000105d0: 7065 7274 790a 2020 6465 6620 7661 7269  perty.  def vari
+000105e0: 6162 6c65 7328 7365 6c66 2920 2d3e 2056  ables(self) -> V
+000105f0: 6172 6961 626c 6544 6963 743a 0a20 2020  ariableDict:.   
+00010600: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
+00010610: 7661 7269 6162 6c65 7320 696e 2074 6869  variables in thi
+00010620: 7320 6d6f 6475 6c65 2e22 2222 0a20 2020  s module.""".   
+00010630: 2069 6620 7365 6c66 2e73 636f 7065 2069   if self.scope i
+00010640: 7320 4e6f 6e65 3a0a 2020 2020 2020 7261  s None:.      ra
+00010650: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00010660: 4361 6e27 7420 6163 6365 7373 2076 6172  Can't access var
+00010670: 6961 626c 6573 206f 6e20 756e 626f 756e  iables on unboun
+00010680: 6420 6d6f 6475 6c65 7322 290a 2020 2020  d modules").    
+00010690: 7265 7475 726e 2073 656c 662e 7363 6f70  return self.scop
+000106a0: 652e 7661 7269 6162 6c65 7328 290a 0a20  e.variables().. 
+000106b0: 2064 6566 2067 6574 5f76 6172 6961 626c   def get_variabl
+000106c0: 6528 7365 6c66 2c20 636f 6c3a 2073 7472  e(self, col: str
+000106d0: 2c20 6e61 6d65 3a20 7374 722c 2064 6566  , name: str, def
+000106e0: 6175 6c74 3a20 4f70 7469 6f6e 616c 5b54  ault: Optional[T
+000106f0: 5d20 3d20 4e6f 6e65 2920 2d3e 2054 3a0a  ] = None) -> T:.
+00010700: 2020 2020 2222 2252 6574 7269 6576 6573      """Retrieves
+00010710: 2074 6865 2076 616c 7565 206f 6620 6120   the value of a 
+00010720: 5661 7269 6162 6c65 2e0a 0a20 2020 2041  Variable...    A
+00010730: 7267 733a 0a20 2020 2020 2063 6f6c 3a20  rgs:.      col: 
+00010740: 7468 6520 7661 7269 6162 6c65 2063 6f6c  the variable col
+00010750: 6c65 6374 696f 6e2e 0a20 2020 2020 206e  lection..      n
+00010760: 616d 653a 2074 6865 206e 616d 6520 6f66  ame: the name of
+00010770: 2074 6865 2076 6172 6961 626c 652e 0a20   the variable.. 
+00010780: 2020 2020 2064 6566 6175 6c74 3a20 7468       default: th
+00010790: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+000107a0: 746f 2072 6574 7572 6e20 6966 2074 6865  to return if the
+000107b0: 2076 6172 6961 626c 6520 646f 6573 206e   variable does n
+000107c0: 6f74 2065 7869 7374 2069 6e0a 2020 2020  ot exist in.    
+000107d0: 2020 2020 7468 6973 2073 636f 7065 2e0a      this scope..
+000107e0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+000107f0: 2020 2020 5468 6520 7661 6c75 6520 6f66      The value of
+00010800: 2074 6865 2069 6e70 7574 2076 6172 6961   the input varia
+00010810: 626c 652c 206f 6620 7468 6520 6465 6661  ble, of the defa
+00010820: 756c 7420 7661 6c75 6520 6966 2074 6865  ult value if the
+00010830: 2076 6172 6961 626c 650a 2020 2020 2020   variable.      
+00010840: 646f 6573 6e27 7420 6578 6973 7420 696e  doesn't exist in
+00010850: 2074 6869 7320 7363 6f70 652e 0a20 2020   this scope..   
+00010860: 2022 2222 0a20 2020 2069 6620 7365 6c66   """.    if self
+00010870: 2e73 636f 7065 2069 7320 4e6f 6e65 3a0a  .scope is None:.
+00010880: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00010890: 6545 7272 6f72 2822 4361 6e27 7420 6163  eError("Can't ac
+000108a0: 6365 7373 2076 6172 6961 626c 6573 206f  cess variables o
+000108b0: 6e20 756e 626f 756e 6420 6d6f 6475 6c65  n unbound module
+000108c0: 7322 290a 2020 2020 7265 7475 726e 2073  s").    return s
+000108d0: 656c 662e 7363 6f70 652e 6765 745f 7661  elf.scope.get_va
+000108e0: 7269 6162 6c65 2863 6f6c 2c20 6e61 6d65  riable(col, name
+000108f0: 2c20 6465 6661 756c 7429 0a0a 2020 6465  , default)..  de
+00010900: 6620 7075 745f 7661 7269 6162 6c65 2873  f put_variable(s
+00010910: 656c 662c 2063 6f6c 3a20 7374 722c 206e  elf, col: str, n
+00010920: 616d 653a 2073 7472 2c20 7661 6c75 653a  ame: str, value:
+00010930: 2041 6e79 293a 0a20 2020 2022 2222 5570   Any):.    """Up
+00010940: 6461 7465 7320 7468 6520 7661 6c75 6520  dates the value 
+00010950: 6f66 2074 6865 2067 6976 656e 2076 6172  of the given var
+00010960: 6961 626c 6520 6966 2069 7420 6973 206d  iable if it is m
+00010970: 7574 6162 6c65 2c20 6f72 2061 6e20 6572  utable, or an er
+00010980: 726f 7220 6f74 6865 7277 6973 652e 0a0a  ror otherwise...
+00010990: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000109a0: 636f 6c3a 2074 6865 2076 6172 6961 626c  col: the variabl
+000109b0: 6520 636f 6c6c 6563 7469 6f6e 2e0a 2020  e collection..  
+000109c0: 2020 2020 6e61 6d65 3a20 7468 6520 6e61      name: the na
+000109d0: 6d65 206f 6620 7468 6520 7661 7269 6162  me of the variab
+000109e0: 6c65 2e0a 2020 2020 2020 7661 6c75 653a  le..      value:
+000109f0: 2074 6865 206e 6577 2076 616c 7565 206f   the new value o
+00010a00: 6620 7468 6520 7661 7269 6162 6c65 2e0a  f the variable..
+00010a10: 2020 2020 2222 220a 2020 2020 6966 2073      """.    if s
+00010a20: 656c 662e 7363 6f70 6520 6973 204e 6f6e  elf.scope is Non
+00010a30: 653a 0a20 2020 2020 2072 6169 7365 2056  e:.      raise V
+00010a40: 616c 7565 4572 726f 7228 2243 616e 2774  alueError("Can't
+00010a50: 2061 6363 6573 7320 7661 7269 6162 6c65   access variable
+00010a60: 7320 6f6e 2075 6e62 6f75 6e64 206d 6f64  s on unbound mod
+00010a70: 756c 6573 2229 0a20 2020 2073 656c 662e  ules").    self.
+00010a80: 7363 6f70 652e 7075 745f 7661 7269 6162  scope.put_variab
+00010a90: 6c65 2863 6f6c 2c20 6e61 6d65 2c20 7661  le(col, name, va
+00010aa0: 6c75 6529 0a0a 2020 406f 7665 726c 6f61  lue)..  @overloa
+00010ab0: 640a 2020 6465 6620 736f 7728 7365 6c66  d.  def sow(self
+00010ac0: 2c20 636f 6c3a 2073 7472 2c20 6e61 6d65  , col: str, name
+00010ad0: 3a20 7374 722c 2076 616c 7565 3a20 416e  : str, value: An
+00010ae0: 7929 202d 3e20 626f 6f6c 3a0a 2020 2020  y) -> bool:.    
+00010af0: 2e2e 2e0a 0a20 2040 6f76 6572 6c6f 6164  .....  @overload
+00010b00: 0a20 2064 6566 2073 6f77 280a 2020 2020  .  def sow(.    
+00010b10: 2020 7365 6c66 2c0a 2020 2020 2020 636f    self,.      co
+00010b20: 6c3a 2073 7472 2c0a 2020 2020 2020 6e61  l: str,.      na
+00010b30: 6d65 3a20 7374 722c 0a20 2020 2020 2076  me: str,.      v
+00010b40: 616c 7565 3a20 542c 0a20 2020 2020 2072  alue: T,.      r
+00010b50: 6564 7563 655f 666e 3a20 4361 6c6c 6162  educe_fn: Callab
+00010b60: 6c65 5b5b 4b2c 2054 5d2c 204b 5d20 3d20  le[[K, T], K] = 
+00010b70: 7475 706c 655f 7265 6475 6365 2c0a 2020  tuple_reduce,.  
+00010b80: 2020 2020 696e 6974 5f66 6e3a 2043 616c      init_fn: Cal
+00010b90: 6c61 626c 655b 5b5d 2c20 4b5d 203d 2074  lable[[], K] = t
+00010ba0: 7570 6c65 5f69 6e69 742c 2020 2320 7479  uple_init,  # ty
+00010bb0: 7065 3a20 6967 6e6f 7265 0a20 2029 202d  pe: ignore.  ) -
+00010bc0: 3e20 626f 6f6c 3a0a 2020 2020 2e2e 2e0a  > bool:.    ....
+00010bd0: 0a20 2064 6566 2073 6f77 280a 2020 2020  .  def sow(.    
+00010be0: 2020 7365 6c66 2c0a 2020 2020 2020 636f    self,.      co
+00010bf0: 6c3a 2073 7472 2c0a 2020 2020 2020 6e61  l: str,.      na
+00010c00: 6d65 3a20 7374 722c 0a20 2020 2020 2076  me: str,.      v
+00010c10: 616c 7565 3a20 542c 0a20 2020 2020 2072  alue: T,.      r
+00010c20: 6564 7563 655f 666e 3a20 4361 6c6c 6162  educe_fn: Callab
+00010c30: 6c65 5b5b 4b2c 2054 5d2c 204b 5d20 3d20  le[[K, T], K] = 
+00010c40: 7475 706c 655f 7265 6475 6365 2c0a 2020  tuple_reduce,.  
+00010c50: 2020 2020 696e 6974 5f66 6e3a 2043 616c      init_fn: Cal
+00010c60: 6c61 626c 655b 5b5d 2c20 4b5d 203d 2074  lable[[], K] = t
+00010c70: 7570 6c65 5f69 6e69 742c 2020 2320 7479  uple_init,  # ty
+00010c80: 7065 3a20 6967 6e6f 7265 0a20 2029 202d  pe: ignore.  ) -
+00010c90: 3e20 626f 6f6c 3a0a 2020 2020 2222 2253  > bool:.    """S
+00010ca0: 746f 7265 7320 6120 7661 6c75 6520 696e  tores a value in
+00010cb0: 2061 2063 6f6c 6c65 6374 696f 6e2e 0a0a   a collection...
+00010cc0: 2020 2020 436f 6c6c 6563 7469 6f6e 7320      Collections 
+00010cd0: 6361 6e20 6265 2075 7365 6420 746f 2063  can be used to c
+00010ce0: 6f6c 6c65 6374 2069 6e74 6572 6d65 6469  ollect intermedi
+00010cf0: 6174 6520 7661 6c75 6573 2077 6974 686f  ate values witho
+00010d00: 7574 0a20 2020 2074 6865 206f 7665 7268  ut.    the overh
+00010d10: 6561 6420 6f66 2065 7870 6c69 6369 746c  ead of explicitl
+00010d20: 7920 7061 7373 696e 6720 6120 636f 6e74  y passing a cont
+00010d30: 6169 6e65 7220 7468 726f 7567 6820 6561  ainer through ea
+00010d40: 6368 204d 6f64 756c 6520 6361 6c6c 2e0a  ch Module call..
+00010d50: 0a20 2020 2049 6620 7468 6520 7461 7267  .    If the targ
+00010d60: 6574 2063 6f6c 6c65 6374 696f 6e20 6973  et collection is
+00010d70: 206e 6f74 206d 7574 6162 6c65 2060 736f   not mutable `so
+00010d80: 7760 2062 6568 6176 6573 206c 696b 6520  w` behaves like 
+00010d90: 6120 6e6f 2d6f 700a 2020 2020 616e 6420  a no-op.    and 
+00010da0: 7265 7475 726e 7320 6046 616c 7365 602e  returns `False`.
+00010db0: 0a0a 2020 2020 4578 616d 706c 653a 3a0a  ..    Example::.
+00010dc0: 0a20 2020 2020 2069 6d70 6f72 7420 6a61  .      import ja
+00010dd0: 780a 2020 2020 2020 696d 706f 7274 206a  x.      import j
+00010de0: 6178 2e6e 756d 7079 2061 7320 6a6e 700a  ax.numpy as jnp.
+00010df0: 2020 2020 2020 696d 706f 7274 2066 6c61        import fla
+00010e00: 782e 6c69 6e65 6e20 6173 206e 6e0a 0a20  x.linen as nn.. 
+00010e10: 2020 2020 2063 6c61 7373 2046 6f6f 286e       class Foo(n
+00010e20: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2020  n.Module):.     
+00010e30: 2020 2040 6e6e 2e63 6f6d 7061 6374 0a20     @nn.compact. 
+00010e40: 2020 2020 2020 2064 6566 205f 5f63 616c         def __cal
+00010e50: 6c5f 5f28 7365 6c66 2c20 7829 3a0a 2020  l__(self, x):.  
+00010e60: 2020 2020 2020 2020 6820 3d20 6e6e 2e44          h = nn.D
+00010e70: 656e 7365 2834 2928 7829 0a20 2020 2020  ense(4)(x).     
+00010e80: 2020 2020 2073 656c 662e 736f 7728 2769       self.sow('i
+00010e90: 6e74 6572 6d65 6469 6174 6573 272c 2027  ntermediates', '
+00010ea0: 6827 2c20 6829 0a20 2020 2020 2020 2020  h', h).         
+00010eb0: 2072 6574 7572 6e20 6e6e 2e44 656e 7365   return nn.Dense
+00010ec0: 2832 2928 6829 0a0a 2020 2020 2020 7820  (2)(h)..      x 
+00010ed0: 3d20 6a6e 702e 6f6e 6573 2828 3136 2c20  = jnp.ones((16, 
+00010ee0: 3929 290a 2020 2020 2020 6d6f 6465 6c20  9)).      model 
+00010ef0: 3d20 466f 6f28 290a 2020 2020 2020 7661  = Foo().      va
+00010f00: 7269 6162 6c65 7320 3d20 6d6f 6465 6c2e  riables = model.
+00010f10: 696e 6974 286a 6178 2e72 616e 646f 6d2e  init(jax.random.
+00010f20: 5052 4e47 4b65 7928 3029 2c20 7829 0a20  PRNGKey(0), x). 
+00010f30: 2020 2020 2079 2c20 7374 6174 6520 3d20       y, state = 
+00010f40: 6d6f 6465 6c2e 6170 706c 7928 7661 7269  model.apply(vari
+00010f50: 6162 6c65 732c 2078 2c20 6d75 7461 626c  ables, x, mutabl
+00010f60: 653d 5b27 696e 7465 726d 6564 6961 7465  e=['intermediate
+00010f70: 7327 5d29 0a20 2020 2020 2070 7269 6e74  s']).      print
+00010f80: 2873 7461 7465 5b27 696e 7465 726d 6564  (state['intermed
+00010f90: 6961 7465 7327 5d29 2020 2320 7b27 6827  iates'])  # {'h'
+00010fa0: 3a20 282e 2e2e 2c29 7d0a 0a20 2020 2042  : (...,)}..    B
+00010fb0: 7920 6465 6661 756c 7420 7468 6520 7661  y default the va
+00010fc0: 6c75 6573 2061 7265 2073 746f 7265 6420  lues are stored 
+00010fd0: 696e 2061 2074 7570 6c65 2061 6e64 2065  in a tuple and e
+00010fe0: 6163 6820 7374 6f72 6564 2076 616c 7565  ach stored value
+00010ff0: 0a20 2020 2069 7320 6170 7065 6e64 6564  .    is appended
+00011000: 2061 7420 7468 6520 656e 642e 2054 6869   at the end. Thi
+00011010: 7320 7761 7920 616c 6c20 696e 7465 726d  s way all interm
+00011020: 6564 6961 7465 7320 6361 6e20 6265 2074  ediates can be t
+00011030: 7261 636b 6564 2077 6865 6e0a 2020 2020  racked when.    
+00011040: 7468 6520 7361 6d65 206d 6f64 756c 6520  the same module 
+00011050: 6973 2063 616c 6c65 6420 6d75 6c74 6970  is called multip
+00011060: 6c65 2074 696d 6573 2e20 416c 7465 726e  le times. Altern
+00011070: 6174 6976 656c 792c 2061 2063 7573 746f  atively, a custo
+00011080: 6d0a 2020 2020 696e 6974 2f72 6564 7563  m.    init/reduc
+00011090: 6520 6675 6e63 7469 6f6e 2063 616e 2062  e function can b
+000110a0: 6520 7061 7373 6564 3a3a 0a0a 2020 2020  e passed::..    
+000110b0: 2020 636c 6173 7320 466f 6f32 286e 6e2e    class Foo2(nn.
+000110c0: 4d6f 6475 6c65 293a 0a20 2020 2020 2020  Module):.       
+000110d0: 2040 6e6e 2e63 6f6d 7061 6374 0a20 2020   @nn.compact.   
+000110e0: 2020 2020 2064 6566 205f 5f63 616c 6c5f       def __call_
+000110f0: 5f28 7365 6c66 2c20 7829 3a0a 2020 2020  _(self, x):.    
+00011100: 2020 2020 2020 696e 6974 5f66 6e20 3d20        init_fn = 
+00011110: 6c61 6d62 6461 3a20 300a 2020 2020 2020  lambda: 0.      
+00011120: 2020 2020 7265 6475 6365 5f66 6e20 3d20      reduce_fn = 
+00011130: 6c61 6d62 6461 2061 2c20 623a 2061 202b  lambda a, b: a +
+00011140: 2062 0a20 2020 2020 2020 2020 2073 656c   b.          sel
+00011150: 662e 736f 7728 2769 6e74 6572 6d65 6469  f.sow('intermedi
+00011160: 6174 6573 272c 2027 6827 2c20 782c 0a20  ates', 'h', x,. 
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 696e 6974 5f66 6e3d 696e 6974 5f66    init_fn=init_f
+00011190: 6e2c 2072 6564 7563 655f 666e 3d72 6564  n, reduce_fn=red
+000111a0: 7563 655f 666e 290a 2020 2020 2020 2020  uce_fn).        
+000111b0: 2020 7365 6c66 2e73 6f77 2827 696e 7465    self.sow('inte
+000111c0: 726d 6564 6961 7465 7327 2c20 2768 272c  rmediates', 'h',
+000111d0: 2078 202a 2032 2c0a 2020 2020 2020 2020   x * 2,.        
+000111e0: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
+000111f0: 666e 3d69 6e69 745f 666e 2c20 7265 6475  fn=init_fn, redu
+00011200: 6365 5f66 6e3d 7265 6475 6365 5f66 6e29  ce_fn=reduce_fn)
+00011210: 0a20 2020 2020 2020 2020 2072 6574 7572  .          retur
+00011220: 6e20 780a 0a20 2020 2020 206d 6f64 656c  n x..      model
+00011230: 203d 2046 6f6f 3228 290a 2020 2020 2020   = Foo2().      
+00011240: 7661 7269 6162 6c65 7320 3d20 6d6f 6465  variables = mode
+00011250: 6c2e 696e 6974 286a 6178 2e72 616e 646f  l.init(jax.rando
+00011260: 6d2e 5052 4e47 4b65 7928 3029 2c20 7829  m.PRNGKey(0), x)
+00011270: 0a20 2020 2020 2079 2c20 7374 6174 6520  .      y, state 
+00011280: 3d20 6d6f 6465 6c2e 6170 706c 7928 7661  = model.apply(va
+00011290: 7269 6162 6c65 732c 206a 6e70 2e6f 6e65  riables, jnp.one
+000112a0: 7328 2831 2c20 3129 292c 206d 7574 6162  s((1, 1)), mutab
+000112b0: 6c65 3d5b 2769 6e74 6572 6d65 6469 6174  le=['intermediat
+000112c0: 6573 275d 290a 2020 2020 2020 7072 696e  es']).      prin
+000112d0: 7428 7374 6174 655b 2769 6e74 6572 6d65  t(state['interme
+000112e0: 6469 6174 6573 275d 2920 2023 203d 3d3e  diates'])  # ==>
+000112f0: 207b 2768 273a 205b 5b33 2e5d 5d7d 0a0a   {'h': [[3.]]}..
+00011300: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00011310: 636f 6c3a 2054 6865 206e 616d 6520 6f66  col: The name of
+00011320: 2074 6865 2076 6172 6961 626c 6520 636f   the variable co
+00011330: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
+00011340: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
+00011350: 6620 7468 6520 7661 7269 6162 6c65 2e0a  f the variable..
+00011360: 2020 2020 2020 7661 6c75 653a 2054 6865        value: The
+00011370: 2076 616c 7565 206f 6620 7468 6520 7661   value of the va
+00011380: 7269 6162 6c65 2e0a 2020 2020 2020 7265  riable..      re
+00011390: 6475 6365 5f66 6e3a 2054 6865 2066 756e  duce_fn: The fun
+000113a0: 6374 696f 6e20 7573 6564 2074 6f20 636f  ction used to co
+000113b0: 6d62 696e 6520 7468 6520 6578 6973 7469  mbine the existi
+000113c0: 6e67 2076 616c 7565 2077 6974 680a 2020  ng value with.  
+000113d0: 2020 2020 2020 7468 6520 6e65 7720 7661        the new va
+000113e0: 6c75 652e 2054 6865 2064 6566 6175 6c74  lue. The default
+000113f0: 2069 7320 746f 2061 7070 656e 6420 7468   is to append th
+00011400: 6520 7661 6c75 6520 746f 2061 2074 7570  e value to a tup
+00011410: 6c65 2e0a 2020 2020 2020 696e 6974 5f66  le..      init_f
+00011420: 6e3a 2046 6f72 2074 6865 2066 6972 7374  n: For the first
+00011430: 2076 616c 7565 2073 746f 7265 642c 2060   value stored, `
+00011440: 7265 6475 6365 5f66 6e60 2077 696c 6c20  reduce_fn` will 
+00011450: 6265 2070 6173 7365 640a 2020 2020 2020  be passed.      
+00011460: 2020 7468 6520 7265 7375 6c74 206f 6620    the result of 
+00011470: 6069 6e69 745f 666e 6020 746f 6765 7468  `init_fn` togeth
+00011480: 6572 2077 6974 6820 7468 6520 7661 6c75  er with the valu
+00011490: 6520 746f 2062 6520 7374 6f72 6564 2e0a  e to be stored..
+000114a0: 2020 2020 2020 2020 5468 6520 6465 6661          The defa
+000114b0: 756c 7420 6973 2061 6e20 656d 7074 7920  ult is an empty 
+000114c0: 7475 706c 652e 0a0a 2020 2020 5265 7475  tuple...    Retu
+000114d0: 726e 733a 0a20 2020 2020 2060 5472 7565  rns:.      `True
+000114e0: 6020 6966 2074 6865 2076 616c 7565 2068  ` if the value h
+000114f0: 6173 2062 6565 6e20 7374 6f72 6564 2073  as been stored s
+00011500: 7563 6365 7373 6675 6c6c 792c 2060 4661  uccessfully, `Fa
+00011510: 6c73 6560 206f 7468 6572 7769 7365 2e0a  lse` otherwise..
+00011520: 2020 2020 2222 220a 2020 2020 6966 2073      """.    if s
+00011530: 656c 662e 7363 6f70 6520 6973 204e 6f6e  elf.scope is Non
+00011540: 653a 0a20 2020 2020 2072 6169 7365 2056  e:.      raise V
+00011550: 616c 7565 4572 726f 7228 2243 616e 2774  alueError("Can't
+00011560: 2073 746f 7265 2076 6172 6961 626c 6573   store variables
+00011570: 206f 6e20 756e 626f 756e 6420 6d6f 6475   on unbound modu
+00011580: 6c65 7322 290a 2020 2020 6966 206e 6f74  les").    if not
+00011590: 2073 656c 662e 7363 6f70 652e 6973 5f6d   self.scope.is_m
+000115a0: 7574 6162 6c65 5f63 6f6c 6c65 6374 696f  utable_collectio
+000115b0: 6e28 636f 6c29 3a0a 2020 2020 2020 7265  n(col):.      re
+000115c0: 7475 726e 2046 616c 7365 0a20 2020 2069  turn False.    i
+000115d0: 6620 7365 6c66 2e73 636f 7065 2e68 6173  f self.scope.has
+000115e0: 5f76 6172 6961 626c 6528 636f 6c2c 206e  _variable(col, n
+000115f0: 616d 6529 3a0a 2020 2020 2020 7873 203d  ame):.      xs =
+00011600: 2073 656c 662e 7363 6f70 652e 6765 745f   self.scope.get_
+00011610: 7661 7269 6162 6c65 2863 6f6c 2c20 6e61  variable(col, na
+00011620: 6d65 290a 2020 2020 656c 7365 3a0a 2020  me).    else:.  
+00011630: 2020 2020 7365 6c66 2e73 636f 7065 2e72      self.scope.r
+00011640: 6573 6572 7665 286e 616d 652c 2063 6f6c  eserve(name, col
+00011650: 290a 2020 2020 2020 7365 6c66 2e5f 7374  ).      self._st
+00011660: 6174 652e 6368 696c 6472 656e 5b6e 616d  ate.children[nam
+00011670: 655d 203d 2063 6f6c 0a20 2020 2020 2078  e] = col.      x
+00011680: 7320 3d20 696e 6974 5f66 6e28 290a 2020  s = init_fn().  
+00011690: 2020 7873 203d 2072 6564 7563 655f 666e    xs = reduce_fn
+000116a0: 2878 732c 2076 616c 7565 290a 2020 2020  (xs, value).    
+000116b0: 7365 6c66 2e73 636f 7065 2e70 7574 5f76  self.scope.put_v
+000116c0: 6172 6961 626c 6528 636f 6c2c 206e 616d  ariable(col, nam
+000116d0: 652c 2078 7329 0a20 2020 2072 6574 7572  e, xs).    retur
+000116e0: 6e20 5472 7565 0a0a 2020 6465 6620 7065  n True..  def pe
+000116f0: 7274 7572 6228 0a20 2020 2020 2073 656c  rturb(.      sel
+00011700: 662c 206e 616d 653a 2073 7472 2c20 7661  f, name: str, va
+00011710: 6c75 653a 2054 2c20 636f 6c6c 6563 7469  lue: T, collecti
+00011720: 6f6e 3a20 7374 7220 3d20 2770 6572 7475  on: str = 'pertu
+00011730: 7262 6174 696f 6e73 270a 2020 2920 2d3e  rbations'.  ) ->
+00011740: 2054 3a0a 2020 2020 2222 2241 6464 2061   T:.    """Add a
+00011750: 6e20 7a65 726f 2d76 616c 7565 2076 6172  n zero-value var
+00011760: 6961 626c 6520 2827 7065 7274 7572 6261  iable ('perturba
+00011770: 7469 6f6e 2729 2074 6f20 7468 6520 696e  tion') to the in
+00011780: 7465 726d 6564 6961 7465 2076 616c 7565  termediate value
+00011790: 2e0a 0a20 2020 2054 6865 2067 7261 6469  ...    The gradi
+000117a0: 656e 7420 6f66 2060 7661 6c75 6560 2077  ent of `value` w
+000117b0: 6f75 6c64 2062 6520 7468 6520 7361 6d65  ould be the same
+000117c0: 2061 7320 7468 6520 6772 6164 6965 6e74   as the gradient
+000117d0: 206f 6620 7468 6973 0a20 2020 2070 6572   of this.    per
+000117e0: 7475 7262 6174 696f 6e20 7661 7269 6162  turbation variab
+000117f0: 6c65 2e20 5468 6572 6566 6f72 652c 2069  le. Therefore, i
+00011800: 6620 796f 7520 6465 6669 6e65 2079 6f75  f you define you
+00011810: 7220 6c6f 7373 2066 756e 6374 696f 6e20  r loss function 
+00011820: 7769 7468 0a20 2020 2062 6f74 6820 7061  with.    both pa
+00011830: 7261 6d73 2061 6e64 2070 6572 7475 7262  rams and perturb
+00011840: 6174 696f 6e73 2061 7320 7374 616e 6461  ations as standa
+00011850: 6c6f 6e65 2061 7267 756d 656e 7473 2c20  lone arguments, 
+00011860: 796f 7520 6361 6e20 6765 7420 7468 650a  you can get the.
+00011870: 2020 2020 696e 7465 726d 6564 6961 7465      intermediate
+00011880: 2067 7261 6469 656e 7473 206f 6620 6076   gradients of `v
+00011890: 616c 7565 6020 6279 2072 756e 6e69 6e67  alue` by running
+000118a0: 2060 6a61 782e 6772 6164 6020 6f6e 2074   `jax.grad` on t
+000118b0: 6865 2070 6572 7475 7262 6174 696f 6e0a  he perturbation.
+000118c0: 2020 2020 6172 6775 6d65 6e74 2e0a 0a20      argument... 
+000118d0: 2020 204e 6f74 653a 2074 6869 7320 6973     Note: this is
+000118e0: 2061 6e20 6578 7065 7269 6d65 6e74 616c   an experimental
+000118f0: 2041 5049 2061 6e64 206d 6179 2062 6520   API and may be 
+00011900: 7477 6561 6b65 6420 6c61 7465 7220 666f  tweaked later fo
+00011910: 7220 6265 7474 6572 0a20 2020 2070 6572  r better.    per
+00011920: 666f 726d 616e 6365 2061 6e64 2075 7361  formance and usa
+00011930: 6269 6c69 7479 2e0a 2020 2020 4174 2069  bility..    At i
+00011940: 7473 2063 7572 7265 6e74 2073 7461 6765  ts current stage
+00011950: 2c20 6974 2063 7265 6174 6573 2065 7874  , it creates ext
+00011960: 7261 2064 756d 6d79 2076 6172 6961 626c  ra dummy variabl
+00011970: 6573 2074 6861 7420 6f63 6375 7069 6573  es that occupies
+00011980: 2065 7874 7261 0a20 2020 206d 656d 6f72   extra.    memor
+00011990: 7920 7370 6163 652e 2055 7365 2069 7420  y space. Use it 
+000119a0: 6f6e 6c79 2074 6f20 6465 6275 6720 6772  only to debug gr
+000119b0: 6164 6965 6e74 7320 696e 2074 7261 696e  adients in train
+000119c0: 696e 672e 0a0a 2020 2020 4578 616d 706c  ing...    Exampl
+000119d0: 653a 3a0a 0a20 2020 2020 2069 6d70 6f72  e::..      impor
+000119e0: 7420 6a61 780a 2020 2020 2020 696d 706f  t jax.      impo
+000119f0: 7274 206a 6178 2e6e 756d 7079 2061 7320  rt jax.numpy as 
+00011a00: 6a6e 700a 2020 2020 2020 696d 706f 7274  jnp.      import
+00011a10: 2066 6c61 782e 6c69 6e65 6e20 6173 206e   flax.linen as n
+00011a20: 6e0a 0a20 2020 2020 2063 6c61 7373 2046  n..      class F
+00011a30: 6f6f 286e 6e2e 4d6f 6475 6c65 293a 0a20  oo(nn.Module):. 
+00011a40: 2020 2020 2020 2020 2040 6e6e 2e63 6f6d           @nn.com
+00011a50: 7061 6374 0a20 2020 2020 2020 2020 2064  pact.          d
+00011a60: 6566 205f 5f63 616c 6c5f 5f28 7365 6c66  ef __call__(self
+00011a70: 2c20 7829 3a0a 2020 2020 2020 2020 2020  , x):.          
+00011a80: 2020 2020 7820 3d20 6e6e 2e44 656e 7365      x = nn.Dense
+00011a90: 2833 2928 7829 0a20 2020 2020 2020 2020  (3)(x).         
+00011aa0: 2020 2020 2078 203d 2073 656c 662e 7065       x = self.pe
+00011ab0: 7274 7572 6228 2764 656e 7365 3327 2c20  rturb('dense3', 
+00011ac0: 7829 0a20 2020 2020 2020 2020 2020 2020  x).             
+00011ad0: 2072 6574 7572 6e20 6e6e 2e44 656e 7365   return nn.Dense
+00011ae0: 2832 2928 7829 0a0a 2020 2020 2020 6465  (2)(x)..      de
+00011af0: 6620 6c6f 7373 2870 6172 616d 732c 2070  f loss(params, p
+00011b00: 6572 7475 7262 6174 696f 6e73 2c20 696e  erturbations, in
+00011b10: 7075 7473 2c20 7461 7267 6574 7329 3a0a  puts, targets):.
+00011b20: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+00011b30: 7320 3d20 7b27 7061 7261 6d73 273a 2070  s = {'params': p
+00011b40: 6172 616d 732c 2027 7065 7274 7572 6261  arams, 'perturba
+00011b50: 7469 6f6e 7327 3a20 7065 7274 7572 6261  tions': perturba
+00011b60: 7469 6f6e 737d 0a20 2020 2020 2020 2070  tions}.        p
+00011b70: 7265 6473 203d 206d 6f64 656c 2e61 7070  reds = model.app
+00011b80: 6c79 2876 6172 6961 626c 6573 2c20 696e  ly(variables, in
+00011b90: 7075 7473 290a 2020 2020 2020 2020 7265  puts).        re
+00011ba0: 7475 726e 206a 6e70 2e73 7175 6172 6528  turn jnp.square(
+00011bb0: 7072 6564 7320 2d20 7461 7267 6574 7329  preds - targets)
+00011bc0: 2e6d 6561 6e28 290a 0a20 2020 2020 2078  .mean()..      x
+00011bd0: 203d 206a 6e70 2e6f 6e65 7328 2832 2c20   = jnp.ones((2, 
+00011be0: 3929 290a 2020 2020 2020 7920 3d20 6a6e  9)).      y = jn
+00011bf0: 702e 6f6e 6573 2828 322c 2032 2929 0a20  p.ones((2, 2)). 
+00011c00: 2020 2020 206d 6f64 656c 203d 2046 6f6f       model = Foo
+00011c10: 2829 0a20 2020 2020 2076 6172 6961 626c  ().      variabl
+00011c20: 6573 203d 206d 6f64 656c 2e69 6e69 7428  es = model.init(
+00011c30: 6a61 782e 7261 6e64 6f6d 2e50 524e 474b  jax.random.PRNGK
+00011c40: 6579 2830 292c 2078 290a 2020 2020 2020  ey(0), x).      
+00011c50: 696e 746d 5f67 7261 6473 203d 206a 6178  intm_grads = jax
+00011c60: 2e67 7261 6428 6c6f 7373 2c20 6172 676e  .grad(loss, argn
+00011c70: 756d 733d 3129 2876 6172 6961 626c 6573  ums=1)(variables
+00011c80: 5b27 7061 7261 6d73 275d 2c20 7661 7269  ['params'], vari
+00011c90: 6162 6c65 735b 2770 6572 7475 7262 6174  ables['perturbat
+00011ca0: 696f 6e73 275d 2c20 782c 2079 290a 2020  ions'], x, y).  
+00011cb0: 2020 2020 7072 696e 7428 696e 746d 5f67      print(intm_g
+00011cc0: 7261 6473 5b27 6465 6e73 6533 275d 2920  rads['dense3']) 
+00011cd0: 2320 3d3d 3e20 5b5b 2d31 2e34 3536 3932  # ==> [[-1.45692
+00011ce0: 3420 2020 2d30 2e34 3433 3332 3533 3720  4   -0.44332537 
+00011cf0: 2030 2e30 3234 3232 3834 375d 0a20 2020   0.02422847].   
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00011d20: 2020 2020 2020 5b2d 312e 3435 3639 3234        [-1.456924
+00011d30: 2020 202d 302e 3434 3333 3235 3337 2020     -0.44332537  
+00011d40: 302e 3032 3432 3238 3437 5d5d 0a0a 2020  0.02422847]]..  
+00011d50: 2020 4966 2070 6572 7475 7262 6174 696f    If perturbatio
+00011d60: 6e73 2061 7265 206e 6f74 2070 6173 7365  ns are not passe
+00011d70: 6420 746f 2060 6170 706c 7960 2c20 6070  d to `apply`, `p
+00011d80: 6572 7475 7262 6020 6265 6861 7665 7320  erturb` behaves 
+00011d90: 6c69 6b65 2061 206e 6f2d 6f70 0a20 2020  like a no-op.   
+00011da0: 2073 6f20 796f 7520 6361 6e20 6561 7369   so you can easi
+00011db0: 6c79 2064 6973 6162 6c65 2074 6865 2062  ly disable the b
+00011dc0: 6568 6176 696f 7220 7768 656e 206e 6f74  ehavior when not
+00011dd0: 206e 6565 6465 643a 3a0a 0a20 2020 2020   needed::..     
+00011de0: 206d 6f64 656c 2e61 7070 6c79 287b 2770   model.apply({'p
+00011df0: 6172 616d 7327 3a20 7061 7261 6d73 2c20  arams': params, 
+00011e00: 2770 6572 7475 7262 6174 696f 6e73 273a  'perturbations':
+00011e10: 2070 6572 7475 7262 6174 696f 6e73 7d2c   perturbations},
+00011e20: 2078 2920 2320 776f 726b 7320 6173 2065   x) # works as e
+00011e30: 7870 6563 7465 640a 2020 2020 2020 6d6f  xpected.      mo
+00011e40: 6465 6c2e 6170 706c 7928 7b27 7061 7261  del.apply({'para
+00011e50: 6d73 273a 2070 6172 616d 737d 2c20 7829  ms': params}, x)
+00011e60: 2023 2062 6568 6176 6573 206c 696b 6520   # behaves like 
+00011e70: 6120 6e6f 2d6f 700a 0a20 2020 2022 2222  a no-op..    """
+00011e80: 0a0a 2020 2020 6465 6620 5f72 6f6f 745f  ..    def _root_
+00011e90: 6861 735f 636f 6c6c 6563 7469 6f6e 2829  has_collection()
+00011ea0: 3a0a 2020 2020 2020 2222 2252 6574 7572  :.      """Retur
+00011eb0: 6e73 2054 7275 6520 6966 2074 6865 2072  ns True if the r
+00011ec0: 6f6f 7420 7363 6f70 6520 6861 7320 7468  oot scope has th
+00011ed0: 6520 636f 6c6c 6563 7469 6f6e 2e22 2222  e collection."""
+00011ee0: 0a20 2020 2020 2061 7373 6572 7420 7365  .      assert se
+00011ef0: 6c66 2e73 636f 7065 2069 7320 6e6f 7420  lf.scope is not 
+00011f00: 4e6f 6e65 0a20 2020 2020 2072 6574 7572  None.      retur
+00011f10: 6e20 636f 6c6c 6563 7469 6f6e 2069 6e20  n collection in 
+00011f20: 7365 6c66 2e73 636f 7065 2e72 6f6f 742e  self.scope.root.
+00011f30: 5f76 6172 6961 626c 6573 0a0a 2020 2020  _variables..    
+00011f40: 2320 7765 2077 696c 6c20 6f6e 6c79 2061  # we will only a
+00011f50: 6464 2074 6865 2070 6572 7475 7262 6174  dd the perturbat
+00011f60: 696f 6e20 7661 7269 6162 6c65 2069 6620  ion variable if 
+00011f70: 7468 6520 636f 6c6c 6563 7469 6f6e 2069  the collection i
+00011f80: 7320 6d75 7461 626c 650a 2020 2020 2320  s mutable.    # 
+00011f90: 2865 2e67 2e20 6475 7269 6e67 2060 696e  (e.g. during `in
+00011fa0: 6974 6029 206f 7220 6966 2074 6865 2063  it`) or if the c
+00011fb0: 6f6c 6c65 6374 696f 6e20 7761 7320 7061  ollection was pa
+00011fc0: 7373 6564 2074 6f20 6061 7070 6c79 6020  ssed to `apply` 
+00011fd0: 2863 6f6e 7461 696e 6564 2069 6e0a 2020  (contained in.  
+00011fe0: 2020 2320 7468 6520 726f 6f74 2073 636f    # the root sco
+00011ff0: 7065 292e 0a20 2020 2069 6620 7365 6c66  pe)..    if self
+00012000: 2e69 735f 6d75 7461 626c 655f 636f 6c6c  .is_mutable_coll
+00012010: 6563 7469 6f6e 2863 6f6c 6c65 6374 696f  ection(collectio
+00012020: 6e29 206f 7220 5f72 6f6f 745f 6861 735f  n) or _root_has_
+00012030: 636f 6c6c 6563 7469 6f6e 2829 3a0a 2020  collection():.  
+00012040: 2020 2020 7661 6c75 6520 2b3d 2073 656c      value += sel
+00012050: 662e 7661 7269 6162 6c65 2863 6f6c 6c65  f.variable(colle
+00012060: 6374 696f 6e2c 206e 616d 652c 206c 616d  ction, name, lam
+00012070: 6264 613a 206a 6e70 2e7a 6572 6f73 5f6c  bda: jnp.zeros_l
+00012080: 696b 6528 7661 6c75 6529 292e 7661 6c75  ike(value)).valu
+00012090: 6520 2023 2074 7970 653a 2069 676e 6f72  e  # type: ignor
+000120a0: 650a 2020 2020 7265 7475 726e 2076 616c  e.    return val
+000120b0: 7565 0a0a 2020 6465 6620 7461 6275 6c61  ue..  def tabula
+000120c0: 7465 280a 2020 2020 2020 7365 6c66 2c0a  te(.      self,.
+000120d0: 2020 2020 2020 726e 6773 3a20 556e 696f        rngs: Unio
+000120e0: 6e5b 4b65 7941 7272 6179 2c20 524e 4753  n[KeyArray, RNGS
+000120f0: 6571 7565 6e63 6573 5d2c 0a20 2020 2020  equences],.     
+00012100: 202a 6172 6773 2c0a 2020 2020 2020 6465   *args,.      de
+00012110: 7074 683a 204f 7074 696f 6e61 6c5b 696e  pth: Optional[in
+00012120: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+00012130: 2073 686f 775f 7265 7065 6174 6564 3a20   show_repeated: 
+00012140: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00012150: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
+00012160: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
+00012170: 5472 7565 2c0a 2020 2020 2020 636f 6e73  True,.      cons
+00012180: 6f6c 655f 6b77 6172 6773 3a20 4f70 7469  ole_kwargs: Opti
+00012190: 6f6e 616c 5b4d 6170 7069 6e67 5b73 7472  onal[Mapping[str
+000121a0: 2c20 416e 795d 5d20 3d20 4e6f 6e65 2c0a  , Any]] = None,.
+000121b0: 2020 2020 2020 7461 626c 655f 6b77 6172        table_kwar
+000121c0: 6773 3a20 4d61 7070 696e 675b 7374 722c  gs: Mapping[str,
+000121d0: 2041 6e79 5d20 3d20 4d61 7070 696e 6750   Any] = MappingP
+000121e0: 726f 7879 5479 7065 287b 7d29 2c0a 2020  roxyType({}),.  
+000121f0: 2020 2020 636f 6c75 6d6e 5f6b 7761 7267      column_kwarg
+00012200: 733a 204d 6170 7069 6e67 5b73 7472 2c20  s: Mapping[str, 
+00012210: 416e 795d 203d 204d 6170 7069 6e67 5072  Any] = MappingPr
+00012220: 6f78 7954 7970 6528 7b7d 292c 0a20 2020  oxyType({}),.   
+00012230: 2020 202a 2a6b 7761 7267 732c 0a20 2029     **kwargs,.  )
+00012240: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
+00012250: 4372 6561 7465 7320 6120 7375 6d6d 6172  Creates a summar
+00012260: 7920 6f66 2074 6865 204d 6f64 756c 6520  y of the Module 
+00012270: 7265 7072 6573 656e 7465 6420 6173 2061  represented as a
+00012280: 2074 6162 6c65 2e0a 0a20 2020 2054 6869   table...    Thi
+00012290: 7320 6d65 7468 6f64 2068 6173 2074 6865  s method has the
+000122a0: 2073 616d 6520 7369 676e 6174 7572 6520   same signature 
+000122b0: 616e 6420 696e 7465 726e 616c 6c79 2063  and internally c
+000122c0: 616c 6c73 2060 4d6f 6475 6c65 2e69 6e69  alls `Module.ini
+000122d0: 7460 2c0a 2020 2020 6275 7420 696e 7374  t`,.    but inst
+000122e0: 6561 6420 6f66 2072 6574 7572 6e69 6e67  ead of returning
+000122f0: 2074 6865 2076 6172 6961 626c 6573 2c20   the variables, 
+00012300: 6974 2072 6574 7572 6e73 2074 6865 2073  it returns the s
+00012310: 7472 696e 6720 7375 6d6d 6172 697a 696e  tring summarizin
+00012320: 670a 2020 2020 7468 6520 4d6f 6475 6c65  g.    the Module
+00012330: 2069 6e20 6120 7461 626c 652e 2060 7461   in a table. `ta
+00012340: 6275 6c61 7465 6020 7573 6573 2060 6a61  bulate` uses `ja
+00012350: 782e 6576 616c 5f73 6861 7065 6020 746f  x.eval_shape` to
+00012360: 2072 756e 2074 6865 2066 6f72 7761 7264   run the forward
+00012370: 0a20 2020 2063 6f6d 7075 7461 7469 6f6e  .    computation
+00012380: 2077 6974 686f 7574 2063 6f6e 7375 6d69   without consumi
+00012390: 6e67 2061 6e79 2046 4c4f 5073 206f 7220  ng any FLOPs or 
+000123a0: 616c 6c6f 6361 7469 6e67 206d 656d 6f72  allocating memor
+000123b0: 792e 0a0a 2020 2020 4164 6469 7469 6f6e  y...    Addition
+000123c0: 616c 2061 7267 756d 656e 7473 2063 616e  al arguments can
+000123d0: 2062 6520 7061 7373 6564 2069 6e74 6f20   be passed into 
+000123e0: 7468 6520 6063 6f6e 736f 6c65 5f6b 7761  the `console_kwa
+000123f0: 7267 7360 2061 7267 756d 656e 742c 2066  rgs` argument, f
+00012400: 6f72 2065 7861 6d70 6c65 2c0a 2020 2020  or example,.    
+00012410: 607b 2777 6964 7468 273a 2031 3230 7d60  `{'width': 120}`
+00012420: 2e20 466f 7220 6120 6675 6c6c 206c 6973  . For a full lis
+00012430: 7420 6f66 2060 636f 6e73 6f6c 655f 6b77  t of `console_kw
+00012440: 6172 6773 6020 6172 6775 6d65 6e74 732c  args` arguments,
+00012450: 2073 6565 3a0a 2020 2020 6874 7470 733a   see:.    https:
+00012460: 2f2f 7269 6368 2e72 6561 6474 6865 646f  //rich.readthedo
+00012470: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+00012480: 7265 6665 7265 6e63 652f 636f 6e73 6f6c  reference/consol
+00012490: 652e 6874 6d6c 2372 6963 682e 636f 6e73  e.html#rich.cons
+000124a0: 6f6c 652e 436f 6e73 6f6c 650a 0a20 2020  ole.Console..   
+000124b0: 2045 7861 6d70 6c65 3a3a 0a0a 2020 2020   Example::..    
+000124c0: 2020 696d 706f 7274 206a 6178 0a20 2020    import jax.   
+000124d0: 2020 2069 6d70 6f72 7420 6a61 782e 6e75     import jax.nu
+000124e0: 6d70 7920 6173 206a 6e70 0a20 2020 2020  mpy as jnp.     
+000124f0: 2069 6d70 6f72 7420 666c 6178 2e6c 696e   import flax.lin
+00012500: 656e 2061 7320 6e6e 0a0a 2020 2020 2020  en as nn..      
+00012510: 636c 6173 7320 466f 6f28 6e6e 2e4d 6f64  class Foo(nn.Mod
+00012520: 756c 6529 3a0a 2020 2020 2020 2020 2020  ule):.          
+00012530: 406e 6e2e 636f 6d70 6163 740a 2020 2020  @nn.compact.    
+00012540: 2020 2020 2020 6465 6620 5f5f 6361 6c6c        def __call
+00012550: 5f5f 2873 656c 662c 2078 293a 0a20 2020  __(self, x):.   
+00012560: 2020 2020 2020 2020 2020 2068 203d 206e             h = n
+00012570: 6e2e 4465 6e73 6528 3429 2878 290a 2020  n.Dense(4)(x).  
+00012580: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012590: 726e 206e 6e2e 4465 6e73 6528 3229 2868  rn nn.Dense(2)(h
+000125a0: 290a 0a20 2020 2020 2078 203d 206a 6e70  )..      x = jnp
+000125b0: 2e6f 6e65 7328 2831 362c 2039 2929 0a0a  .ones((16, 9))..
+000125c0: 2020 2020 2020 7072 696e 7428 466f 6f28        print(Foo(
+000125d0: 292e 7461 6275 6c61 7465 286a 6178 2e72  ).tabulate(jax.r
+000125e0: 616e 646f 6d2e 5052 4e47 4b65 7928 3029  andom.PRNGKey(0)
+000125f0: 2c20 7829 290a 0a0a 2020 2020 5468 6973  , x))...    This
+00012600: 2067 6976 6573 2074 6865 2066 6f6c 6c6f   gives the follo
+00012610: 7769 6e67 206f 7574 7075 743a 3a0a 0a20  wing output::.. 
+00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 2020 2020 2046 6f6f 2053 756d 6d61 7279       Foo Summary
+00012650: 0a20 2020 2020 20e2 948f e294 81e2 9481  .      .........
+00012660: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00012670: 9481 e294 81e2 94b3 e294 81e2 9481 e294  ................
+00012680: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00012690: e294 b3e2 9481 e294 81e2 9481 e294 81e2  ................
+000126a0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000126b0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000126c0: e294 b3e2 9481 e294 81e2 9481 e294 81e2  ................
+000126d0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000126e0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000126f0: e294 b3e2 9481 e294 81e2 9481 e294 81e2  ................
+00012700: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00012710: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00012720: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00012730: 9481 e294 81e2 9493 0a20 2020 2020 20e2  .........      .
+00012740: 9483 2070 6174 6820 2020 20e2 9483 206d  .. path    ... m
+00012750: 6f64 756c 6520 e294 8320 696e 7075 7473  odule ... inputs
+00012760: 2020 2020 2020 2020 e294 8320 6f75 7470          ... outp
+00012770: 7574 7320 2020 2020 2020 e294 8320 7061  uts       ... pa
+00012780: 7261 6d73 2020 2020 2020 2020 2020 2020  rams            
+00012790: 2020 20e2 9483 0a20 2020 2020 20e2 94a1     ....      ...
+000127a0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+000127b0: 9481 e294 81e2 9481 e294 81e2 9587 e294  ................
+000127c0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+000127d0: e294 81e2 9481 e295 87e2 9481 e294 81e2  ................
+000127e0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+000127f0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00012800: e294 81e2 9481 e295 87e2 9481 e294 81e2  ................
+00012810: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00012820: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00012830: e294 81e2 9481 e295 87e2 9481 e294 81e2  ................
+00012840: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00012850: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00012860: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00012870: 9481 e294 81e2 9481 e294 81e2 94a9 0a20  ............... 
+00012880: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+00012890: 20e2 9482 2046 6f6f 2020 2020 e294 8220   ... Foo    ... 
+000128a0: 666c 6f61 7433 325b 3136 2c39 5d20 e294  float32[16,9] ..
+000128b0: 8220 666c 6f61 7433 325b 3136 2c32 5d20  . float32[16,2] 
+000128c0: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+000128d0: 2020 2020 2020 2020 20e2 9482 0a20 2020           ....   
+000128e0: 2020 20e2 949c e294 80e2 9480 e294 80e2     .............
+000128f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012900: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00012910: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012930: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012940: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012960: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012970: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012980: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012990: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000129a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000129b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000129c0: 80e2 94a4 0a20 2020 2020 20e2 9482 2044  .....      ... D
+000129d0: 656e 7365 5f30 20e2 9482 2044 656e 7365  ense_0 ... Dense
+000129e0: 2020 e294 8220 666c 6f61 7433 325b 3136    ... float32[16
+000129f0: 2c39 5d20 e294 8220 666c 6f61 7433 325b  ,9] ... float32[
+00012a00: 3136 2c34 5d20 e294 8220 6269 6173 3a20  16,4] ... bias: 
+00012a10: 666c 6f61 7433 325b 345d 2020 2020 20e2  float32[4]     .
+00012a20: 9482 0a20 2020 2020 20e2 9482 2020 2020  ...      ...    
+00012a30: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+00012a40: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+00012a50: 2020 e294 8220 2020 2020 2020 2020 2020    ...           
+00012a60: 2020 2020 e294 8220 6b65 726e 656c 3a20      ... kernel: 
+00012a70: 666c 6f61 7433 325b 392c 345d 20e2 9482  float32[9,4] ...
+00012a80: 0a20 2020 2020 20e2 9482 2020 2020 2020  .      ...      
+00012a90: 2020 20e2 9482 2020 2020 2020 2020 e294     ...        ..
+00012aa0: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00012ab0: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+00012ac0: 2020 e294 8220 2020 2020 2020 2020 2020    ...           
+00012ad0: 2020 2020 2020 2020 2020 20e2 9482 0a20             .... 
+00012ae0: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+00012af0: 20e2 9482 2020 2020 2020 2020 e294 8220   ...        ... 
+00012b00: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+00012b10: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00012b20: e294 8220 3430 2028 3136 3020 4229 2020  ... 40 (160 B)  
+00012b30: 2020 2020 2020 2020 20e2 9482 0a20 2020           ....   
+00012b40: 2020 20e2 949c e294 80e2 9480 e294 80e2     .............
+00012b50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012b60: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00012b70: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012b80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012b90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012ba0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012bb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012bc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012bd0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012be0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012bf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012c00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012c10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012c20: 80e2 94a4 0a20 2020 2020 20e2 9482 2044  .....      ... D
+00012c30: 656e 7365 5f31 20e2 9482 2044 656e 7365  ense_1 ... Dense
+00012c40: 2020 e294 8220 666c 6f61 7433 325b 3136    ... float32[16
+00012c50: 2c34 5d20 e294 8220 666c 6f61 7433 325b  ,4] ... float32[
+00012c60: 3136 2c32 5d20 e294 8220 6269 6173 3a20  16,2] ... bias: 
+00012c70: 666c 6f61 7433 325b 325d 2020 2020 20e2  float32[2]     .
+00012c80: 9482 0a20 2020 2020 20e2 9482 2020 2020  ...      ...    
+00012c90: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+00012ca0: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+00012cb0: 2020 e294 8220 2020 2020 2020 2020 2020    ...           
+00012cc0: 2020 2020 e294 8220 6b65 726e 656c 3a20      ... kernel: 
+00012cd0: 666c 6f61 7433 325b 342c 325d 20e2 9482  float32[4,2] ...
+00012ce0: 0a20 2020 2020 20e2 9482 2020 2020 2020  .      ...      
+00012cf0: 2020 20e2 9482 2020 2020 2020 2020 e294     ...        ..
+00012d00: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00012d10: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+00012d20: 2020 e294 8220 2020 2020 2020 2020 2020    ...           
+00012d30: 2020 2020 2020 2020 2020 20e2 9482 0a20             .... 
+00012d40: 2020 2020 20e2 9482 2020 2020 2020 2020       ...        
+00012d50: 20e2 9482 2020 2020 2020 2020 e294 8220   ...        ... 
+00012d60: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+00012d70: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00012d80: e294 8220 3130 2028 3430 2042 2920 2020  ... 10 (40 B)   
+00012d90: 2020 2020 2020 2020 20e2 9482 0a20 2020           ....   
+00012da0: 2020 20e2 949c e294 80e2 9480 e294 80e2     .............
+00012db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012dc0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00012dd0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012df0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012e00: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012e10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012e20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012e30: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00012e40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012e60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012e70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012e80: 80e2 94a4 0a20 2020 2020 20e2 9482 2020  .....      ...  
+00012e90: 2020 2020 2020 20e2 9482 2020 2020 2020         ...      
+00012ea0: 2020 e294 8220 2020 2020 2020 2020 2020    ...           
+00012eb0: 2020 2020 e294 8220 2020 2020 2020 2020      ...         
+00012ec0: 546f 7461 6c20 e294 8220 3530 2028 3230  Total ... 50 (20
+00012ed0: 3020 4229 2020 2020 2020 2020 2020 20e2  0 B)           .
+00012ee0: 9482 0a20 2020 2020 20e2 9494 e294 80e2  ...      .......
+00012ef0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012f00: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+00012f10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012f20: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00012f30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012f40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012f50: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00012f60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012f70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012f80: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00012f90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00012fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00012fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00012fc0: 80e2 9480 e294 80e2 9498 0a0a 2020 2020  ............    
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 2020 2020 2020 2020 546f 7461 6c20 5061          Total Pa
+00012ff0: 7261 6d65 7465 7273 3a20 3530 2028 3230  rameters: 50 (20
+00013000: 3020 4229 0a0a 2020 2020 2a2a 4e6f 7465  0 B)..    **Note
+00013010: 2a2a 3a20 726f 7773 206f 7264 6572 2069  **: rows order i
+00013020: 6e20 7468 6520 7461 626c 6520 646f 6573  n the table does
+00013030: 206e 6f74 2072 6570 7265 7365 6e74 2065   not represent e
+00013040: 7865 6375 7469 6f6e 206f 7264 6572 2c0a  xecution order,.
+00013050: 2020 2020 696e 7374 6561 6420 6974 2061      instead it a
+00013060: 6c69 676e 7320 7769 7468 2074 6865 206f  ligns with the o
+00013070: 7264 6572 206f 6620 6b65 7973 2069 6e20  rder of keys in 
+00013080: 6076 6172 6961 626c 6573 6020 7768 6963  `variables` whic
+00013090: 6820 6172 6520 736f 7274 6564 0a20 2020  h are sorted.   
+000130a0: 2061 6c70 6861 6265 7469 6361 6c6c 792e   alphabetically.
+000130b0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000130c0: 2020 726e 6773 3a20 5468 6520 726e 6773    rngs: The rngs
+000130d0: 2066 6f72 2074 6865 2076 6172 6961 626c   for the variabl
+000130e0: 6520 636f 6c6c 6563 7469 6f6e 7320 6173  e collections as
+000130f0: 2070 6173 7365 6420 746f 2060 4d6f 6475   passed to `Modu
+00013100: 6c65 2e69 6e69 7460 2e0a 2020 2020 2020  le.init`..      
+00013110: 2a61 7267 733a 2054 6865 2061 7267 756d  *args: The argum
+00013120: 656e 7473 2074 6f20 7468 6520 666f 7277  ents to the forw
+00013130: 6172 6420 636f 6d70 7574 6174 696f 6e2e  ard computation.
+00013140: 0a20 2020 2020 2064 6570 7468 3a20 636f  .      depth: co
+00013150: 6e74 726f 6c73 2068 6f77 206d 616e 7920  ntrols how many 
+00013160: 7375 626d 6f64 756c 6520 6465 6570 2074  submodule deep t
+00013170: 6865 2073 756d 6d61 7279 2063 616e 2067  he summary can g
+00013180: 6f2e 2042 7920 6465 6661 756c 7420 6974  o. By default it
+00013190: 730a 2020 2020 2020 2020 604e 6f6e 6560  s.        `None`
+000131a0: 2077 6869 6368 206d 6561 6e73 206e 6f20   which means no 
+000131b0: 6c69 6d69 742e 2049 6620 6120 7375 626d  limit. If a subm
+000131c0: 6f64 756c 6520 6973 206e 6f74 2073 686f  odule is not sho
+000131d0: 776e 2062 6563 6175 7365 206f 6620 7468  wn because of th
+000131e0: 650a 2020 2020 2020 2020 6465 7074 6820  e.        depth 
+000131f0: 6c69 6d69 742c 2069 7473 2070 6172 616d  limit, its param
+00013200: 6574 6572 2063 6f75 6e74 2061 6e64 2062  eter count and b
+00013210: 7974 6573 2077 696c 6c20 6265 2061 6464  ytes will be add
+00013220: 6564 2074 6f20 7468 6520 726f 7720 6f66  ed to the row of
+00013230: 2069 7473 0a20 2020 2020 2020 2066 6972   its.        fir
+00013240: 7374 2073 686f 776e 2061 6e63 6573 746f  st shown ancesto
+00013250: 7220 7375 6368 2074 6861 7420 7468 6520  r such that the 
+00013260: 7375 6d20 6f66 2061 6c6c 2072 6f77 7320  sum of all rows 
+00013270: 616c 7761 7973 2061 6464 7320 7570 2074  always adds up t
+00013280: 6f20 7468 650a 2020 2020 2020 2020 746f  o the.        to
+00013290: 7461 6c20 6e75 6d62 6572 206f 6620 7061  tal number of pa
+000132a0: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
+000132b0: 4d6f 6475 6c65 2e0a 2020 2020 2020 7368  Module..      sh
+000132c0: 6f77 5f72 6570 6561 7465 643a 2049 6620  ow_repeated: If 
+000132d0: 6054 7275 6560 2c20 7265 7065 6174 6564  `True`, repeated
+000132e0: 2063 616c 6c73 2074 6f20 7468 6520 7361   calls to the sa
+000132f0: 6d65 206d 6f64 756c 6520 7769 6c6c 2062  me module will b
+00013300: 6520 7368 6f77 6e0a 2020 2020 2020 2020  e shown.        
+00013310: 696e 2074 6865 2074 6162 6c65 2c20 6f74  in the table, ot
+00013320: 6865 7277 6973 6520 6f6e 6c79 2074 6865  herwise only the
+00013330: 2066 6972 7374 2063 616c 6c20 7769 6c6c   first call will
+00013340: 2062 6520 7368 6f77 6e2e 2044 6566 6175   be shown. Defau
+00013350: 6c74 2069 730a 2020 2020 2020 2020 6046  lt is.        `F
+00013360: 616c 7365 602e 0a20 2020 2020 206d 7574  alse`..      mut
+00013370: 6162 6c65 3a20 4361 6e20 6265 2062 6f6f  able: Can be boo
+00013380: 6c2c 2073 7472 2c20 6f72 206c 6973 742e  l, str, or list.
+00013390: 2053 7065 6369 6669 6573 2077 6869 6368   Specifies which
+000133a0: 2063 6f6c 6c65 6374 696f 6e73 2073 686f   collections sho
+000133b0: 756c 6420 6265 0a20 2020 2020 2020 2074  uld be.        t
+000133c0: 7265 6174 6564 2061 7320 6d75 7461 626c  reated as mutabl
+000133d0: 653a 2060 6062 6f6f 6c60 603a 2061 6c6c  e: ``bool``: all
+000133e0: 2f6e 6f20 636f 6c6c 6563 7469 6f6e 7320  /no collections 
+000133f0: 6172 6520 6d75 7461 626c 652e 2060 6073  are mutable. ``s
+00013400: 7472 6060 3a20 5468 650a 2020 2020 2020  tr``: The.      
+00013410: 2020 6e61 6d65 206f 6620 6120 7369 6e67    name of a sing
+00013420: 6c65 206d 7574 6162 6c65 2063 6f6c 6c65  le mutable colle
+00013430: 6374 696f 6e2e 2060 606c 6973 7460 603a  ction. ``list``:
+00013440: 2041 206c 6973 7420 6f66 206e 616d 6573   A list of names
+00013450: 206f 6620 6d75 7461 626c 650a 2020 2020   of mutable.    
+00013460: 2020 2020 636f 6c6c 6563 7469 6f6e 732e      collections.
+00013470: 2042 7920 6465 6661 756c 7420 616c 6c20   By default all 
+00013480: 636f 6c6c 6563 7469 6f6e 7320 6578 6365  collections exce
+00013490: 7074 2027 696e 7465 726d 6564 6961 7465  pt 'intermediate
+000134a0: 7327 2061 7265 0a20 2020 2020 2020 206d  s' are.        m
+000134b0: 7574 6162 6c65 2e0a 2020 2020 2020 636f  utable..      co
+000134c0: 6e73 6f6c 655f 6b77 6172 6773 3a20 416e  nsole_kwargs: An
+000134d0: 206f 7074 696f 6e61 6c20 6469 6374 696f   optional dictio
+000134e0: 6e61 7279 2077 6974 6820 6164 6469 7469  nary with additi
+000134f0: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
+00013500: 756d 656e 7473 2074 6861 740a 2020 2020  uments that.    
+00013510: 2020 2020 6172 6520 7061 7373 6564 2074      are passed t
+00013520: 6f20 6072 6963 682e 636f 6e73 6f6c 652e  o `rich.console.
+00013530: 436f 6e73 6f6c 6560 2077 6865 6e20 7265  Console` when re
+00013540: 6e64 6572 696e 6720 7468 6520 7461 626c  ndering the tabl
+00013550: 652e 2044 6566 6175 6c74 2061 7267 756d  e. Default argum
+00013560: 656e 7473 0a20 2020 2020 2020 2061 7265  ents.        are
+00013570: 2060 7b27 666f 7263 655f 7465 726d 696e   `{'force_termin
+00013580: 616c 273a 2054 7275 652c 2027 666f 7263  al': True, 'forc
+00013590: 655f 6a75 7079 7465 7227 3a20 4661 6c73  e_jupyter': Fals
+000135a0: 657d 602e 0a20 2020 2020 2074 6162 6c65  e}`..      table
+000135b0: 5f6b 7761 7267 733a 2041 6e20 6f70 7469  _kwargs: An opti
+000135c0: 6f6e 616c 2064 6963 7469 6f6e 6172 7920  onal dictionary 
+000135d0: 7769 7468 2061 6464 6974 696f 6e61 6c20  with additional 
+000135e0: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+000135f0: 7320 7468 6174 0a20 2020 2020 2020 2061  s that.        a
+00013600: 7265 2070 6173 7365 6420 746f 2060 7269  re passed to `ri
+00013610: 6368 2e74 6162 6c65 2e54 6162 6c65 6020  ch.table.Table` 
+00013620: 636f 6e73 7472 7563 746f 722e 0a20 2020  constructor..   
+00013630: 2020 2063 6f6c 756d 6e5f 6b77 6172 6773     column_kwargs
+00013640: 3a20 416e 206f 7074 696f 6e61 6c20 6469  : An optional di
+00013650: 6374 696f 6e61 7279 2077 6974 6820 6164  ctionary with ad
+00013660: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
+00013670: 2061 7267 756d 656e 7473 2074 6861 740a   arguments that.
+00013680: 2020 2020 2020 2020 6172 6520 7061 7373          are pass
+00013690: 6564 2074 6f20 6072 6963 682e 7461 626c  ed to `rich.tabl
+000136a0: 652e 5461 626c 652e 6164 645f 636f 6c75  e.Table.add_colu
+000136b0: 6d6e 6020 7768 656e 2061 6464 696e 6720  mn` when adding 
+000136c0: 636f 6c75 6d6e 7320 746f 2074 6865 2074  columns to the t
+000136d0: 6162 6c65 2e0a 2020 2020 2020 2a2a 6b77  able..      **kw
+000136e0: 6172 6773 3a20 6b65 7977 6f72 6420 6172  args: keyword ar
+000136f0: 6775 6d65 6e74 7320 746f 2070 6173 7320  guments to pass 
+00013700: 746f 2074 6865 2066 6f72 7761 7264 2063  to the forward c
+00013710: 6f6d 7075 7461 7469 6f6e 2e0a 0a20 2020  omputation...   
+00013720: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00013730: 4120 7374 7269 6e67 2073 756d 6d61 7269  A string summari
+00013740: 7a69 6e67 2074 6865 204d 6f64 756c 652e  zing the Module.
+00013750: 0a20 2020 2022 2222 0a20 2020 2066 726f  .    """.    fro
+00013760: 6d20 666c 6178 2e6c 696e 656e 2069 6d70  m flax.linen imp
+00013770: 6f72 7420 7375 6d6d 6172 790a 0a20 2020  ort summary..   
+00013780: 2074 6162 756c 6174 655f 666e 203d 2073   tabulate_fn = s
+00013790: 756d 6d61 7279 2e74 6162 756c 6174 6528  ummary.tabulate(
+000137a0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000137b0: 2020 2020 2020 2072 6e67 732c 0a20 2020         rngs,.   
+000137c0: 2020 2020 2064 6570 7468 3d64 6570 7468       depth=depth
+000137d0: 2c0a 2020 2020 2020 2020 7368 6f77 5f72  ,.        show_r
+000137e0: 6570 6561 7465 643d 7368 6f77 5f72 6570  epeated=show_rep
+000137f0: 6561 7465 642c 0a20 2020 2020 2020 206d  eated,.        m
+00013800: 7574 6162 6c65 3d6d 7574 6162 6c65 2c0a  utable=mutable,.
+00013810: 2020 2020 2020 2020 636f 6e73 6f6c 655f          console_
+00013820: 6b77 6172 6773 3d63 6f6e 736f 6c65 5f6b  kwargs=console_k
+00013830: 7761 7267 732c 0a20 2020 2020 2020 2074  wargs,.        t
+00013840: 6162 6c65 5f6b 7761 7267 733d 7461 626c  able_kwargs=tabl
+00013850: 655f 6b77 6172 6773 2c0a 2020 2020 2020  e_kwargs,.      
+00013860: 2020 636f 6c75 6d6e 5f6b 7761 7267 733d    column_kwargs=
+00013870: 636f 6c75 6d6e 5f6b 7761 7267 732c 0a20  column_kwargs,. 
+00013880: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
+00013890: 7461 6275 6c61 7465 5f66 6e28 2a61 7267  tabulate_fn(*arg
+000138a0: 732c 202a 2a6b 7761 7267 7329 0a0a 0a5f  s, **kwargs)..._
+000138b0: 5061 7265 6e74 5479 7065 203d 2055 6e69  ParentType = Uni
+000138c0: 6f6e 5b54 7970 655b 4d6f 6475 6c65 5d2c  on[Type[Module],
+000138d0: 2054 7970 655b 5363 6f70 655d 2c20 5479   Type[Scope], Ty
+000138e0: 7065 5b5f 5365 6e74 696e 656c 5d2c 204e  pe[_Sentinel], N
+000138f0: 6f6e 655d 0a0a 0a64 6566 206d 6572 6765  one]...def merge
+00013900: 5f70 6172 616d 286e 616d 653a 2073 7472  _param(name: str
+00013910: 2c20 613a 204f 7074 696f 6e61 6c5b 545d  , a: Optional[T]
+00013920: 2c20 623a 204f 7074 696f 6e61 6c5b 545d  , b: Optional[T]
+00013930: 2920 2d3e 2054 3a0a 2020 2222 224d 6572  ) -> T:.  """Mer
+00013940: 6765 7320 636f 6e73 7472 7563 7469 6f6e  ges construction
+00013950: 2d20 616e 6420 6361 6c6c 2d74 696d 6520  - and call-time 
+00013960: 6172 6775 6d65 6e74 2e0a 0a20 2054 6869  argument...  Thi
+00013970: 7320 6973 2061 2075 7469 6c69 7479 2066  s is a utility f
+00013980: 6f72 2073 7570 706f 7274 696e 6720 6120  or supporting a 
+00013990: 7061 7474 6572 6e20 7768 6572 6520 6120  pattern where a 
+000139a0: 4d6f 6475 6c65 2068 7970 6572 7061 7261  Module hyperpara
+000139b0: 6d65 7465 720a 2020 6361 6e20 6265 2070  meter.  can be p
+000139c0: 6173 7365 6420 6569 7468 6572 2074 6f20  assed either to 
+000139d0: 6060 5f5f 696e 6974 5f5f 6060 206f 7220  ``__init__`` or 
+000139e0: 6060 5f5f 6361 6c6c 5f5f 6060 2c20 616e  ``__call__``, an
+000139f0: 6420 7468 6520 7661 6c75 6520 7468 6174  d the value that
+00013a00: 2069 730a 2020 6e6f 7420 604e 6f6e 6560   is.  not `None`
+00013a10: 2077 696c 6c20 6265 2075 7365 642e 0a0a   will be used...
+00013a20: 2020 4578 616d 706c 653a 3a0a 0a20 2020    Example::..   
+00013a30: 2063 6c61 7373 2046 6f6f 286e 6e2e 4d6f   class Foo(nn.Mo
+00013a40: 6475 6c65 293a 0a20 2020 2020 2074 7261  dule):.      tra
+00013a50: 696e 3a20 4f70 7469 6f6e 616c 5b62 6f6f  in: Optional[boo
+00013a60: 6c5d 203d 204e 6f6e 650a 0a20 2020 2020  l] = None..     
+00013a70: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+00013a80: 6c66 2c20 7472 6169 6e3a 204f 7074 696f  lf, train: Optio
+00013a90: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00013aa0: 293a 0a20 2020 2020 2020 2074 7261 696e  ):.        train
+00013ab0: 203d 206e 6e2e 6d65 7267 655f 7061 7261   = nn.merge_para
+00013ac0: 6d28 2774 7261 696e 272c 2073 656c 662e  m('train', self.
+00013ad0: 7472 6169 6e2c 2074 7261 696e 290a 0a20  train, train).. 
+00013ae0: 2041 6e20 6572 726f 7220 6973 2074 6872   An error is thr
+00013af0: 6f77 6e20 7768 656e 2062 6f74 6820 6172  own when both ar
+00013b00: 6775 6d65 6e74 7320 6172 6520 604e 6f6e  guments are `Non
+00013b10: 6560 206f 7220 626f 7468 2076 616c 7565  e` or both value
+00013b20: 7320 6172 6520 6e6f 740a 2020 604e 6f6e  s are not.  `Non
+00013b30: 6560 2e0a 0a20 2041 7267 733a 0a20 2020  e`...  Args:.   
+00013b40: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
+00013b50: 6f66 2074 6865 2070 6172 616d 6574 6572  of the parameter
+00013b60: 2e20 5573 6564 2066 6f72 2065 7272 6f72  . Used for error
+00013b70: 206d 6573 7361 6765 732e 0a20 2020 2061   messages..    a
+00013b80: 3a20 6f70 7469 6f6e 2061 0a20 2020 2062  : option a.    b
+00013b90: 3a20 6f70 7469 6f6e 2062 0a20 2052 6574  : option b.  Ret
+00013ba0: 7572 6e73 3a0a 2020 2020 6120 6f72 2062  urns:.    a or b
+00013bb0: 2077 6869 6368 6576 6572 2069 7320 6e6f   whichever is no
+00013bc0: 7420 604e 6f6e 6560 2e0a 0a20 2022 2222  t `None`...  """
+00013bd0: 0a20 2069 6620 6120 6973 204e 6f6e 6520  .  if a is None 
+00013be0: 616e 6420 6220 6973 204e 6f6e 653a 0a20  and b is None:. 
+00013bf0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00013c00: 726f 7228 0a20 2020 2020 2020 2066 2750  ror(.        f'P
+00013c10: 6172 616d 6574 6572 2022 7b6e 616d 657d  arameter "{name}
+00013c20: 2220 6d75 7374 2062 6520 7061 7373 6564  " must be passed
+00013c30: 2074 6f20 7468 6520 636f 6e73 7472 7563   to the construc
+00013c40: 746f 7220 6f72 2061 7420 6361 6c6c 2074  tor or at call t
+00013c50: 696d 652e 270a 2020 2020 290a 2020 6966  ime.'.    ).  if
+00013c60: 2061 2069 7320 6e6f 7420 4e6f 6e65 2061   a is not None a
+00013c70: 6e64 2062 2069 7320 6e6f 7420 4e6f 6e65  nd b is not None
+00013c80: 3a0a 2020 2020 7261 6973 6520 5661 6c75  :.    raise Valu
+00013c90: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00013ca0: 6627 5061 7261 6d65 7465 7220 227b 6e61  f'Parameter "{na
+00013cb0: 6d65 7d22 2077 6173 2070 6173 7365 6420  me}" was passed 
+00013cc0: 746f 2074 6865 2063 6f6e 7374 7275 6374  to the construct
+00013cd0: 6f72 2061 6e64 2061 7420 6361 6c6c 2074  or and at call t
+00013ce0: 696d 652e 270a 2020 2020 2020 2020 2720  ime.'.        ' 
+00013cf0: 5368 6f75 6c64 2062 6520 7061 7373 6564  Should be passed
+00013d00: 206a 7573 7420 6f6e 6365 2e27 0a20 2020   just once.'.   
+00013d10: 2029 0a20 2069 6620 6120 6973 204e 6f6e   ).  if a is Non
+00013d20: 653a 0a20 2020 2061 7373 6572 7420 6220  e:.    assert b 
+00013d30: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00013d40: 7265 7475 726e 2062 0a20 2072 6574 7572  return b.  retur
+00013d50: 6e20 610a 0a0a 4074 7261 6365 6261 636b  n a...@traceback
+00013d60: 5f75 7469 6c2e 6170 695f 626f 756e 6461  _util.api_bounda
+00013d70: 7279 0a64 6566 2061 7070 6c79 280a 2020  ry.def apply(.  
+00013d80: 2020 666e 3a20 4361 6c6c 6162 6c65 5b2e    fn: Callable[.
+00013d90: 2e2e 2c20 416e 795d 2c0a 2020 2020 6d6f  .., Any],.    mo
+00013da0: 6475 6c65 3a20 4d6f 6475 6c65 2c0a 2020  dule: Module,.  
+00013db0: 2020 6d75 7461 626c 653a 2043 6f6c 6c65    mutable: Colle
+00013dc0: 6374 696f 6e46 696c 7465 7220 3d20 4661  ctionFilter = Fa
+00013dd0: 6c73 652c 0a20 2020 2063 6170 7475 7265  lse,.    capture
+00013de0: 5f69 6e74 6572 6d65 6469 6174 6573 3a20  _intermediates: 
+00013df0: 556e 696f 6e5b 626f 6f6c 2c20 4361 6c6c  Union[bool, Call
+00013e00: 6162 6c65 5b5b 4d6f 6475 6c65 2c20 7374  able[[Module, st
+00013e10: 725d 2c20 626f 6f6c 5d5d 203d 2046 616c  r], bool]] = Fal
+00013e20: 7365 2c0a 2920 2d3e 2043 616c 6c61 626c  se,.) -> Callabl
+00013e30: 655b 2e2e 2e2c 2041 6e79 5d3a 0a20 2022  e[..., Any]:.  "
+00013e40: 2222 4372 6561 7465 7320 616e 2061 7070  ""Creates an app
+00013e50: 6c79 2066 756e 6374 696f 6e20 746f 2063  ly function to c
+00013e60: 616c 6c20 6060 666e 6060 2077 6974 6820  all ``fn`` with 
+00013e70: 6120 626f 756e 6420 6d6f 6475 6c65 2e0a  a bound module..
+00013e80: 0a20 2055 6e6c 696b 6520 6060 4d6f 6475  .  Unlike ``Modu
+00013e90: 6c65 2e61 7070 6c79 6060 2074 6869 7320  le.apply`` this 
+00013ea0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
+00013eb0: 2061 206e 6577 2066 756e 6374 696f 6e20   a new function 
+00013ec0: 7769 7468 2074 6865 2073 6967 6e61 7475  with the signatu
+00013ed0: 7265 0a20 2060 6028 7661 7269 6162 6c65  re.  ``(variable
+00013ee0: 732c 202a 6172 6773 2c20 726e 6773 3d4e  s, *args, rngs=N
+00013ef0: 6f6e 652c 202a 2a6b 7761 7267 7329 202d  one, **kwargs) -
+00013f00: 3e20 5460 6020 7768 6572 6520 6054 6020  > T`` where `T` 
+00013f10: 6973 2074 6865 2072 6574 7572 6e20 7479  is the return ty
+00013f20: 7065 0a20 206f 6620 6060 666e 6060 2e20  pe.  of ``fn``. 
+00013f30: 4966 2060 606d 7574 6162 6c65 6060 2069  If ``mutable`` i
+00013f40: 7320 6e6f 7420 6060 4661 6c73 6560 6020  s not ``False`` 
+00013f50: 7468 6520 7265 7475 726e 2074 7970 6520  the return type 
+00013f60: 6973 2061 2074 7570 6c65 2077 6865 7265  is a tuple where
+00013f70: 2074 6865 0a20 2073 6563 6f6e 6420 6974   the.  second it
+00013f80: 656d 2069 7320 6120 6060 4672 6f7a 656e  em is a ``Frozen
+00013f90: 4469 6374 6060 2077 6974 6820 7468 6520  Dict`` with the 
+00013fa0: 6d75 7461 7465 6420 7661 7269 6162 6c65  mutated variable
+00013fb0: 732e 0a0a 2020 5468 6520 6170 706c 7920  s...  The apply 
+00013fc0: 6675 6e63 7469 6f6e 2074 6861 7420 6973  function that is
+00013fd0: 2072 6574 7572 6e65 6420 6361 6e20 6265   returned can be
+00013fe0: 2064 6972 6563 746c 7920 636f 6d70 6f73   directly compos
+00013ff0: 6564 2077 6974 680a 2020 4a41 5820 7472  ed with.  JAX tr
+00014000: 616e 7366 6f72 6d61 7469 6f6e 7320 6c69  ansformations li
+00014010: 6b65 2060 606a 6178 2e6a 6974 6060 3a3a  ke ``jax.jit``::
+00014020: 0a0a 2020 2020 6465 6620 6628 666f 6f2c  ..    def f(foo,
+00014030: 2078 293a 0a20 2020 2020 207a 203d 2066   x):.      z = f
+00014040: 6f6f 2e65 6e63 6f64 6528 7829 0a20 2020  oo.encode(x).   
+00014050: 2020 2079 203d 2066 6f6f 2e64 6563 6f64     y = foo.decod
+00014060: 6528 7a29 0a20 2020 2020 2023 202e 2e2e  e(z).      # ...
+00014070: 0a20 2020 2020 2072 6574 7572 6e20 790a  .      return y.
+00014080: 0a20 2020 2066 6f6f 203d 2046 6f6f 2829  .    foo = Foo()
+00014090: 0a20 2020 2066 5f6a 6974 7465 6420 3d20  .    f_jitted = 
+000140a0: 6a61 782e 6a69 7428 6e6e 2e61 7070 6c79  jax.jit(nn.apply
+000140b0: 2866 2c20 666f 6f29 290a 2020 2020 665f  (f, foo)).    f_
+000140c0: 6a69 7474 6564 2876 6172 6961 626c 6573  jitted(variables
+000140d0: 2c20 7829 0a0a 2020 4172 6773 3a0a 2020  , x)..  Args:.  
+000140e0: 2020 666e 3a20 5468 6520 6675 6e63 7469    fn: The functi
+000140f0: 6f6e 2074 6861 7420 7368 6f75 6c64 2062  on that should b
+00014100: 6520 6170 706c 6965 642e 2054 6865 2066  e applied. The f
+00014110: 6972 7374 2061 7267 756d 656e 7420 7061  irst argument pa
+00014120: 7373 6564 2077 696c 6c0a 2020 2020 2020  ssed will.      
+00014130: 6265 2061 6e20 6d6f 6475 6c65 2069 6e73  be an module ins
+00014140: 7461 6e63 6520 6f66 2074 6865 2060 606d  tance of the ``m
+00014150: 6f64 756c 6560 6020 7769 7468 2076 6172  odule`` with var
+00014160: 6961 626c 6573 2061 6e64 2052 4e47 7320  iables and RNGs 
+00014170: 626f 756e 640a 2020 2020 2020 746f 2069  bound.      to i
+00014180: 742e 0a20 2020 206d 6f64 756c 653a 2054  t..    module: T
+00014190: 6865 2060 604d 6f64 756c 6560 6020 7468  he ``Module`` th
+000141a0: 6174 2077 696c 6c20 6265 2075 7365 6420  at will be used 
+000141b0: 746f 2062 696e 6420 7661 7269 6162 6c65  to bind variable
+000141c0: 7320 616e 6420 524e 4773 2074 6f2e 0a20  s and RNGs to.. 
+000141d0: 2020 2020 2054 6865 2060 604d 6f64 756c       The ``Modul
+000141e0: 6560 6020 7061 7373 6564 2061 7320 7468  e`` passed as th
+000141f0: 6520 6669 7273 7420 6172 6775 6d65 6e74  e first argument
+00014200: 2074 6f20 6060 666e 6060 2077 696c 6c20   to ``fn`` will 
+00014210: 6265 2061 2063 6c6f 6e65 0a20 2020 2020  be a clone.     
+00014220: 206f 6620 6d6f 6475 6c65 2e0a 2020 2020   of module..    
+00014230: 6d75 7461 626c 653a 2043 616e 2062 6520  mutable: Can be 
+00014240: 626f 6f6c 2c20 7374 722c 206f 7220 6c69  bool, str, or li
+00014250: 7374 2e20 5370 6563 6966 6965 7320 7768  st. Specifies wh
+00014260: 6963 6820 636f 6c6c 6563 7469 6f6e 7320  ich collections 
+00014270: 7368 6f75 6c64 2062 650a 2020 2020 2020  should be.      
+00014280: 7472 6561 7465 6420 6173 206d 7574 6162  treated as mutab
+00014290: 6c65 3a20 6060 626f 6f6c 6060 3a20 616c  le: ``bool``: al
+000142a0: 6c2f 6e6f 2063 6f6c 6c65 6374 696f 6e73  l/no collections
+000142b0: 2061 7265 206d 7574 6162 6c65 2e0a 2020   are mutable..  
+000142c0: 2020 2020 6060 7374 7260 603a 2054 6865      ``str``: The
+000142d0: 206e 616d 6520 6f66 2061 2073 696e 676c   name of a singl
+000142e0: 6520 6d75 7461 626c 6520 636f 6c6c 6563  e mutable collec
+000142f0: 7469 6f6e 2e20 6060 6c69 7374 6060 3a20  tion. ``list``: 
+00014300: 410a 2020 2020 2020 6c69 7374 206f 6620  A.      list of 
+00014310: 6e61 6d65 7320 6f66 206d 7574 6162 6c65  names of mutable
+00014320: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
+00014330: 2020 6361 7074 7572 655f 696e 7465 726d    capture_interm
+00014340: 6564 6961 7465 733a 2049 6620 6054 7275  ediates: If `Tru
+00014350: 6560 2c20 6361 7074 7572 6573 2069 6e74  e`, captures int
+00014360: 6572 6d65 6469 6174 6520 7265 7475 726e  ermediate return
+00014370: 2076 616c 7565 730a 2020 2020 2020 6f66   values.      of
+00014380: 2061 6c6c 204d 6f64 756c 6573 2069 6e73   all Modules ins
+00014390: 6964 6520 7468 6520 2269 6e74 6572 6d65  ide the "interme
+000143a0: 6469 6174 6573 2220 636f 6c6c 6563 7469  diates" collecti
+000143b0: 6f6e 2e20 4279 2064 6566 6175 6c74 206f  on. By default o
+000143c0: 6e6c 790a 2020 2020 2020 7468 6520 7265  nly.      the re
+000143d0: 7475 726e 2076 616c 7565 7320 6f66 2061  turn values of a
+000143e0: 6c6c 2060 5f5f 6361 6c6c 5f5f 6020 6d65  ll `__call__` me
+000143f0: 7468 6f64 7320 6172 6520 7374 6f72 6564  thods are stored
+00014400: 2e20 4120 6675 6e63 7469 6f6e 2063 616e  . A function can
+00014410: 0a20 2020 2020 2062 6520 7061 7373 6564  .      be passed
+00014420: 2074 6f20 6368 616e 6765 2074 6865 2066   to change the f
+00014430: 696c 7465 7220 6265 6861 7669 6f72 2e20  ilter behavior. 
+00014440: 5468 6520 6669 6c74 6572 2066 756e 6374  The filter funct
+00014450: 696f 6e20 7461 6b65 730a 2020 2020 2020  ion takes.      
+00014460: 7468 6520 4d6f 6475 6c65 2069 6e73 7461  the Module insta
+00014470: 6e63 6520 616e 6420 6d65 7468 6f64 206e  nce and method n
+00014480: 616d 6520 616e 6420 7265 7475 726e 7320  ame and returns 
+00014490: 6120 626f 6f6c 2069 6e64 6963 6174 696e  a bool indicatin
+000144a0: 670a 2020 2020 2020 7768 6574 6865 7220  g.      whether 
+000144b0: 7468 6520 6f75 7470 7574 206f 6620 7468  the output of th
+000144c0: 6174 206d 6574 686f 6420 696e 766f 6361  at method invoca
+000144d0: 7469 6f6e 2073 686f 756c 6420 6265 2073  tion should be s
+000144e0: 746f 7265 642e 0a20 2052 6574 7572 6e73  tored..  Returns
+000144f0: 3a0a 2020 2020 5468 6520 6170 706c 7920  :.    The apply 
+00014500: 6675 6e63 7469 6f6e 2077 7261 7070 696e  function wrappin
+00014510: 6720 6060 666e 6060 2e0a 2020 2222 220a  g ``fn``..  """.
+00014520: 0a20 2040 6675 6e63 746f 6f6c 732e 7772  .  @functools.wr
+00014530: 6170 7328 666e 290a 2020 6465 6620 7363  aps(fn).  def sc
+00014540: 6f70 655f 666e 2873 636f 7065 2c20 2a61  ope_fn(scope, *a
+00014550: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00014560: 2020 2020 5f63 6f6e 7465 7874 2e63 6170      _context.cap
+00014570: 7475 7265 5f73 7461 636b 2e61 7070 656e  ture_stack.appen
+00014580: 6428 6361 7074 7572 655f 696e 7465 726d  d(capture_interm
+00014590: 6564 6961 7465 7329 0a20 2020 2074 7279  ediates).    try
+000145a0: 3a0a 2020 2020 2020 7265 7475 726e 2066  :.      return f
+000145b0: 6e28 6d6f 6475 6c65 2e63 6c6f 6e65 2870  n(module.clone(p
+000145c0: 6172 656e 743d 7363 6f70 652c 205f 6465  arent=scope, _de
+000145d0: 6570 5f63 6c6f 6e65 3d54 7275 6529 2c20  ep_clone=True), 
+000145e0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+000145f0: 0a20 2020 2066 696e 616c 6c79 3a0a 2020  .    finally:.  
+00014600: 2020 2020 5f63 6f6e 7465 7874 2e63 6170      _context.cap
+00014610: 7475 7265 5f73 7461 636b 2e70 6f70 2829  ture_stack.pop()
+00014620: 0a0a 2020 6966 2063 6170 7475 7265 5f69  ..  if capture_i
+00014630: 6e74 6572 6d65 6469 6174 6573 2069 7320  ntermediates is 
+00014640: 5472 7565 3a20 2023 2070 796c 696e 743a  True:  # pylint:
+00014650: 2064 6973 6162 6c65 3d67 2d62 6f6f 6c2d   disable=g-bool-
+00014660: 6964 2d63 6f6d 7061 7269 736f 6e0a 2020  id-comparison.  
+00014670: 2020 6361 7074 7572 655f 696e 7465 726d    capture_interm
+00014680: 6564 6961 7465 7320 3d20 6361 7074 7572  ediates = captur
+00014690: 655f 6361 6c6c 5f69 6e74 6572 6d65 6469  e_call_intermedi
+000146a0: 6174 6573 0a20 2069 6620 6361 7074 7572  ates.  if captur
+000146b0: 655f 696e 7465 726d 6564 6961 7465 733a  e_intermediates:
+000146c0: 0a20 2020 206d 7574 6162 6c65 203d 2075  .    mutable = u
+000146d0: 6e69 6f6e 5f66 696c 7465 7273 286d 7574  nion_filters(mut
+000146e0: 6162 6c65 2c20 2769 6e74 6572 6d65 6469  able, 'intermedi
+000146f0: 6174 6573 2729 0a20 2072 6574 7572 6e20  ates').  return 
+00014700: 636f 7265 2e61 7070 6c79 2873 636f 7065  core.apply(scope
+00014710: 5f66 6e2c 206d 7574 6162 6c65 3d6d 7574  _fn, mutable=mut
+00014720: 6162 6c65 290a 0a0a 4074 7261 6365 6261  able)...@traceba
+00014730: 636b 5f75 7469 6c2e 6170 695f 626f 756e  ck_util.api_boun
+00014740: 6461 7279 0a64 6566 2069 6e69 745f 7769  dary.def init_wi
+00014750: 7468 5f6f 7574 7075 7428 0a20 2020 2066  th_output(.    f
+00014760: 6e3a 2043 616c 6c61 626c 655b 2e2e 2e2c  n: Callable[...,
+00014770: 2041 6e79 5d2c 0a20 2020 206d 6f64 756c   Any],.    modul
+00014780: 653a 204d 6f64 756c 652c 0a20 2020 206d  e: Module,.    m
+00014790: 7574 6162 6c65 3a20 436f 6c6c 6563 7469  utable: Collecti
+000147a0: 6f6e 4669 6c74 6572 203d 2044 656e 794c  onFilter = DenyL
+000147b0: 6973 7428 2769 6e74 6572 6d65 6469 6174  ist('intermediat
+000147c0: 6573 2729 2c0a 2020 2020 6361 7074 7572  es'),.    captur
+000147d0: 655f 696e 7465 726d 6564 6961 7465 733a  e_intermediates:
+000147e0: 2055 6e69 6f6e 5b62 6f6f 6c2c 2043 616c   Union[bool, Cal
+000147f0: 6c61 626c 655b 5b4d 6f64 756c 652c 2073  lable[[Module, s
+00014800: 7472 5d2c 2062 6f6f 6c5d 5d20 3d20 4661  tr], bool]] = Fa
+00014810: 6c73 652c 0a29 202d 3e20 4361 6c6c 6162  lse,.) -> Callab
+00014820: 6c65 5b2e 2e2e 2c20 5475 706c 655b 416e  le[..., Tuple[An
+00014830: 792c 2055 6e69 6f6e 5b46 726f 7a65 6e56  y, Union[FrozenV
+00014840: 6172 6961 626c 6544 6963 742c 2044 6963  ariableDict, Dic
+00014850: 745b 7374 722c 2041 6e79 5d5d 5d5d 3a0a  t[str, Any]]]]:.
+00014860: 2020 2222 2243 7265 6174 6573 2061 6e20    """Creates an 
+00014870: 696e 6974 2066 756e 6374 696f 6e20 746f  init function to
+00014880: 2063 616c 6c20 6060 666e 6060 2077 6974   call ``fn`` wit
+00014890: 6820 6120 626f 756e 6420 6d6f 6475 6c65  h a bound module
+000148a0: 2074 6861 7420 616c 736f 2072 6574 7572   that also retur
+000148b0: 6e73 2074 6865 2066 756e 6374 696f 6e20  ns the function 
+000148c0: 6f75 7470 7574 732e 0a0a 2020 556e 6c69  outputs...  Unli
+000148d0: 6b65 2060 604d 6f64 756c 652e 696e 6974  ke ``Module.init
+000148e0: 5f77 6974 685f 6f75 7470 7574 6060 2074  _with_output`` t
+000148f0: 6869 7320 6675 6e63 7469 6f6e 2072 6574  his function ret
+00014900: 7572 6e73 2061 206e 6577 2066 756e 6374  urns a new funct
+00014910: 696f 6e20 7769 7468 2074 6865 2073 6967  ion with the sig
+00014920: 6e61 7475 7265 0a20 2060 6028 726e 6773  nature.  ``(rngs
+00014930: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00014940: 7329 202d 3e20 2854 2c20 7661 7269 6162  s) -> (T, variab
+00014950: 6c65 7329 6060 2077 6865 7265 2060 5460  les)`` where `T`
+00014960: 2069 7320 7468 6520 7265 7475 726e 2074   is the return t
+00014970: 7970 6520 6f66 2060 6066 6e60 602e 0a20  ype of ``fn``.. 
+00014980: 2054 6865 2072 6e67 7320 6361 6e20 6265   The rngs can be
+00014990: 2061 2064 6963 7420 6f66 2050 524e 474b   a dict of PRNGK
+000149a0: 6579 7320 6f72 2061 2073 696e 676c 6520  eys or a single 
+000149b0: 6060 6050 524e 474b 6579 6060 2077 6869  ```PRNGKey`` whi
+000149c0: 6368 2069 730a 2020 6571 7569 7661 6c65  ch is.  equivale
+000149d0: 6e74 2074 6f20 7061 7373 696e 6720 6120  nt to passing a 
+000149e0: 6469 6374 2077 6974 6820 6f6e 6520 5052  dict with one PR
+000149f0: 4e47 4b65 7920 7769 7468 2074 6865 206e  NGKey with the n
+00014a00: 616d 6520 2270 6172 616d 7322 2e0a 0a20  ame "params"... 
+00014a10: 2054 6865 2069 6e69 7420 6675 6e63 7469   The init functi
+00014a20: 6f6e 2074 6861 7420 6973 2072 6574 7572  on that is retur
+00014a30: 6e65 6420 6361 6e20 6265 2064 6972 6563  ned can be direc
+00014a40: 746c 7920 636f 6d70 6f73 6564 2077 6974  tly composed wit
+00014a50: 680a 2020 4a41 5820 7472 616e 7366 6f72  h.  JAX transfor
+00014a60: 6d61 7469 6f6e 7320 6c69 6b65 2060 606a  mations like ``j
+00014a70: 6178 2e6a 6974 6060 3a3a 0a0a 2020 2020  ax.jit``::..    
+00014a80: 6465 6620 6628 666f 6f2c 2078 293a 0a20  def f(foo, x):. 
+00014a90: 2020 2020 207a 203d 2066 6f6f 2e65 6e63       z = foo.enc
+00014aa0: 6f64 6528 7829 0a20 2020 2020 2079 203d  ode(x).      y =
+00014ab0: 2066 6f6f 2e64 6563 6f64 6528 7a29 0a20   foo.decode(z). 
+00014ac0: 2020 2020 2023 202e 2e2e 0a20 2020 2020       # ....     
+00014ad0: 2072 6574 7572 6e20 790a 0a20 2020 2066   return y..    f
+00014ae0: 6f6f 203d 2046 6f6f 2829 0a20 2020 2066  oo = Foo().    f
+00014af0: 5f6a 6974 7465 6420 3d20 6a61 782e 6a69  _jitted = jax.ji
+00014b00: 7428 6e6e 2e69 6e69 745f 7769 7468 5f6f  t(nn.init_with_o
+00014b10: 7574 7075 7428 662c 2066 6f6f 2929 0a20  utput(f, foo)). 
+00014b20: 2020 2079 2c20 7661 7269 6162 6c65 7320     y, variables 
+00014b30: 3d20 665f 6a69 7474 6564 2872 6e67 2c20  = f_jitted(rng, 
+00014b40: 7829 0a0a 2020 4172 6773 3a0a 2020 2020  x)..  Args:.    
+00014b50: 666e 3a20 5468 6520 6675 6e63 7469 6f6e  fn: The function
+00014b60: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
+00014b70: 6170 706c 6965 642e 2054 6865 2066 6972  applied. The fir
+00014b80: 7374 2061 7267 756d 656e 7420 7061 7373  st argument pass
+00014b90: 6564 2077 696c 6c0a 2020 2020 2020 6265  ed will.      be
+00014ba0: 2061 6e20 6d6f 6475 6c65 2069 6e73 7461   an module insta
+00014bb0: 6e63 6520 6f66 2074 6865 2060 606d 6f64  nce of the ``mod
+00014bc0: 756c 6560 6020 7769 7468 2076 6172 6961  ule`` with varia
+00014bd0: 626c 6573 2061 6e64 2052 4e47 7320 626f  bles and RNGs bo
+00014be0: 756e 640a 2020 2020 2020 746f 2069 742e  und.      to it.
+00014bf0: 0a20 2020 206d 6f64 756c 653a 2054 6865  .    module: The
+00014c00: 2060 604d 6f64 756c 6560 6020 7468 6174   ``Module`` that
+00014c10: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
+00014c20: 2062 696e 6420 7661 7269 6162 6c65 7320   bind variables 
+00014c30: 616e 6420 524e 4773 2074 6f2e 0a20 2020  and RNGs to..   
+00014c40: 2020 2054 6865 2060 604d 6f64 756c 6560     The ``Module`
+00014c50: 6020 7061 7373 6564 2061 7320 7468 6520  ` passed as the 
+00014c60: 6669 7273 7420 6172 6775 6d65 6e74 2074  first argument t
+00014c70: 6f20 6060 666e 6060 2077 696c 6c20 6265  o ``fn`` will be
+00014c80: 2061 2063 6c6f 6e65 0a20 2020 2020 206f   a clone.      o
+00014c90: 6620 6d6f 6475 6c65 2e0a 2020 2020 6d75  f module..    mu
+00014ca0: 7461 626c 653a 2043 616e 2062 6520 626f  table: Can be bo
+00014cb0: 6f6c 2c20 7374 722c 206f 7220 6c69 7374  ol, str, or list
+00014cc0: 2e20 5370 6563 6966 6965 7320 7768 6963  . Specifies whic
+00014cd0: 6820 636f 6c6c 6563 7469 6f6e 7320 7368  h collections sh
+00014ce0: 6f75 6c64 2062 650a 2020 2020 2020 7472  ould be.      tr
+00014cf0: 6561 7465 6420 6173 206d 7574 6162 6c65  eated as mutable
+00014d00: 3a20 6060 626f 6f6c 6060 3a20 616c 6c2f  : ``bool``: all/
+00014d10: 6e6f 2063 6f6c 6c65 6374 696f 6e73 2061  no collections a
+00014d20: 7265 206d 7574 6162 6c65 2e0a 2020 2020  re mutable..    
+00014d30: 2020 6060 7374 7260 603a 2054 6865 206e    ``str``: The n
+00014d40: 616d 6520 6f66 2061 2073 696e 676c 6520  ame of a single 
+00014d50: 6d75 7461 626c 6520 636f 6c6c 6563 7469  mutable collecti
+00014d60: 6f6e 2e20 6060 6c69 7374 6060 3a20 410a  on. ``list``: A.
+00014d70: 2020 2020 2020 6c69 7374 206f 6620 6e61        list of na
+00014d80: 6d65 7320 6f66 206d 7574 6162 6c65 2063  mes of mutable c
+00014d90: 6f6c 6c65 6374 696f 6e73 2e20 4279 2064  ollections. By d
+00014da0: 6566 6175 6c74 2061 6c6c 2063 6f6c 6c65  efault all colle
+00014db0: 6374 696f 6e73 0a20 2020 2020 2065 7863  ctions.      exc
+00014dc0: 6570 7420 2269 6e74 6572 6d65 6469 6174  ept "intermediat
+00014dd0: 6573 2220 6172 6520 6d75 7461 626c 652e  es" are mutable.
+00014de0: 0a20 2020 2063 6170 7475 7265 5f69 6e74  .    capture_int
+00014df0: 6572 6d65 6469 6174 6573 3a20 4966 2060  ermediates: If `
+00014e00: 5472 7565 602c 2063 6170 7475 7265 7320  True`, captures 
+00014e10: 696e 7465 726d 6564 6961 7465 2072 6574  intermediate ret
+00014e20: 7572 6e20 7661 6c75 6573 0a20 2020 2020  urn values.     
+00014e30: 206f 6620 616c 6c20 4d6f 6475 6c65 7320   of all Modules 
+00014e40: 696e 7369 6465 2074 6865 2022 696e 7465  inside the "inte
+00014e50: 726d 6564 6961 7465 7322 2063 6f6c 6c65  rmediates" colle
+00014e60: 6374 696f 6e2e 2042 7920 6465 6661 756c  ction. By defaul
+00014e70: 7420 6f6e 6c79 0a20 2020 2020 2074 6865  t only.      the
+00014e80: 2072 6574 7572 6e20 7661 6c75 6573 206f   return values o
+00014e90: 6620 616c 6c20 605f 5f63 616c 6c5f 5f60  f all `__call__`
+00014ea0: 206d 6574 686f 6473 2061 7265 2073 746f   methods are sto
+00014eb0: 7265 642e 2041 2066 756e 6374 696f 6e20  red. A function 
+00014ec0: 6361 6e0a 2020 2020 2020 6265 2070 6173  can.      be pas
+00014ed0: 7365 6420 746f 2063 6861 6e67 6520 7468  sed to change th
+00014ee0: 6520 6669 6c74 6572 2062 6568 6176 696f  e filter behavio
+00014ef0: 722e 2054 6865 2066 696c 7465 7220 6675  r. The filter fu
+00014f00: 6e63 7469 6f6e 2074 616b 6573 0a20 2020  nction takes.   
+00014f10: 2020 2074 6865 204d 6f64 756c 6520 696e     the Module in
+00014f20: 7374 616e 6365 2061 6e64 206d 6574 686f  stance and metho
+00014f30: 6420 6e61 6d65 2061 6e64 2072 6574 7572  d name and retur
+00014f40: 6e73 2061 2062 6f6f 6c20 696e 6469 6361  ns a bool indica
+00014f50: 7469 6e67 0a20 2020 2020 2077 6865 7468  ting.      wheth
+00014f60: 6572 2074 6865 206f 7574 7075 7420 6f66  er the output of
+00014f70: 2074 6861 7420 6d65 7468 6f64 2069 6e76   that method inv
+00014f80: 6f63 6174 696f 6e20 7368 6f75 6c64 2062  ocation should b
+00014f90: 6520 7374 6f72 6564 2e0a 2020 5265 7475  e stored..  Retu
+00014fa0: 726e 733a 0a20 2020 2054 6865 2069 6e69  rns:.    The ini
+00014fb0: 7420 6675 6e63 7469 6f6e 2077 7261 7070  t function wrapp
+00014fc0: 696e 6720 6060 666e 6060 2e0a 2020 2222  ing ``fn``..  ""
+00014fd0: 220a 0a20 2040 6675 6e63 746f 6f6c 732e  "..  @functools.
+00014fe0: 7772 6170 7328 666e 290a 2020 6465 6620  wraps(fn).  def 
+00014ff0: 7363 6f70 655f 666e 2873 636f 7065 2c20  scope_fn(scope, 
+00015000: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00015010: 3a0a 2020 2020 5f63 6f6e 7465 7874 2e63  :.    _context.c
+00015020: 6170 7475 7265 5f73 7461 636b 2e61 7070  apture_stack.app
+00015030: 656e 6428 6361 7074 7572 655f 696e 7465  end(capture_inte
+00015040: 726d 6564 6961 7465 7329 0a20 2020 2074  rmediates).    t
+00015050: 7279 3a0a 2020 2020 2020 7265 7475 726e  ry:.      return
+00015060: 2066 6e28 6d6f 6475 6c65 2e63 6c6f 6e65   fn(module.clone
+00015070: 2870 6172 656e 743d 7363 6f70 652c 205f  (parent=scope, _
+00015080: 6465 6570 5f63 6c6f 6e65 3d54 7275 6529  deep_clone=True)
+00015090: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+000150a0: 7329 0a20 2020 2066 696e 616c 6c79 3a0a  s).    finally:.
+000150b0: 2020 2020 2020 5f63 6f6e 7465 7874 2e63        _context.c
+000150c0: 6170 7475 7265 5f73 7461 636b 2e70 6f70  apture_stack.pop
+000150d0: 2829 0a0a 2020 6966 2063 6170 7475 7265  ()..  if capture
+000150e0: 5f69 6e74 6572 6d65 6469 6174 6573 2069  _intermediates i
+000150f0: 7320 5472 7565 3a20 2023 2070 796c 696e  s True:  # pylin
+00015100: 743a 2064 6973 6162 6c65 3d67 2d62 6f6f  t: disable=g-boo
+00015110: 6c2d 6964 2d63 6f6d 7061 7269 736f 6e0a  l-id-comparison.
+00015120: 2020 2020 6361 7074 7572 655f 696e 7465      capture_inte
+00015130: 726d 6564 6961 7465 7320 3d20 6361 7074  rmediates = capt
+00015140: 7572 655f 6361 6c6c 5f69 6e74 6572 6d65  ure_call_interme
+00015150: 6469 6174 6573 0a20 2069 6620 6361 7074  diates.  if capt
+00015160: 7572 655f 696e 7465 726d 6564 6961 7465  ure_intermediate
+00015170: 733a 0a20 2020 206d 7574 6162 6c65 203d  s:.    mutable =
+00015180: 2075 6e69 6f6e 5f66 696c 7465 7273 286d   union_filters(m
+00015190: 7574 6162 6c65 2c20 2769 6e74 6572 6d65  utable, 'interme
+000151a0: 6469 6174 6573 2729 0a20 2072 6574 7572  diates').  retur
+000151b0: 6e20 636f 7265 2e69 6e69 7428 7363 6f70  n core.init(scop
+000151c0: 655f 666e 2c20 6d75 7461 626c 653d 6d75  e_fn, mutable=mu
+000151d0: 7461 626c 6529 0a0a 0a40 7472 6163 6562  table)...@traceb
+000151e0: 6163 6b5f 7574 696c 2e61 7069 5f62 6f75  ack_util.api_bou
+000151f0: 6e64 6172 790a 6465 6620 696e 6974 280a  ndary.def init(.
+00015200: 2020 2020 666e 3a20 4361 6c6c 6162 6c65      fn: Callable
+00015210: 5b2e 2e2e 2c20 416e 795d 2c0a 2020 2020  [..., Any],.    
+00015220: 6d6f 6475 6c65 3a20 4d6f 6475 6c65 2c0a  module: Module,.
+00015230: 2020 2020 6d75 7461 626c 653a 2043 6f6c      mutable: Col
+00015240: 6c65 6374 696f 6e46 696c 7465 7220 3d20  lectionFilter = 
+00015250: 4465 6e79 4c69 7374 2827 696e 7465 726d  DenyList('interm
+00015260: 6564 6961 7465 7327 292c 0a20 2020 2063  ediates'),.    c
+00015270: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
+00015280: 6174 6573 3a20 556e 696f 6e5b 626f 6f6c  ates: Union[bool
+00015290: 2c20 4361 6c6c 6162 6c65 5b5b 4d6f 6475  , Callable[[Modu
+000152a0: 6c65 2c20 7374 725d 2c20 626f 6f6c 5d5d  le, str], bool]]
+000152b0: 203d 2046 616c 7365 2c0a 2920 2d3e 2043   = False,.) -> C
+000152c0: 616c 6c61 626c 655b 2e2e 2e2c 2055 6e69  allable[..., Uni
+000152d0: 6f6e 5b46 726f 7a65 6e56 6172 6961 626c  on[FrozenVariabl
+000152e0: 6544 6963 742c 2044 6963 745b 7374 722c  eDict, Dict[str,
+000152f0: 2041 6e79 5d5d 5d3a 0a20 2022 2222 4372   Any]]]:.  """Cr
+00015300: 6561 7465 7320 616e 2069 6e69 7420 6675  eates an init fu
+00015310: 6e63 7469 6f6e 2074 6f20 6361 6c6c 2060  nction to call `
+00015320: 6066 6e60 6020 7769 7468 2061 2062 6f75  `fn`` with a bou
+00015330: 6e64 206d 6f64 756c 652e 0a0a 2020 556e  nd module...  Un
+00015340: 6c69 6b65 2060 604d 6f64 756c 652e 696e  like ``Module.in
+00015350: 6974 6060 2074 6869 7320 6675 6e63 7469  it`` this functi
+00015360: 6f6e 2072 6574 7572 6e73 2061 206e 6577  on returns a new
+00015370: 2066 756e 6374 696f 6e20 7769 7468 2074   function with t
+00015380: 6865 2073 6967 6e61 7475 7265 0a20 2060  he signature.  `
+00015390: 6028 726e 6773 2c20 2a61 7267 732c 202a  `(rngs, *args, *
+000153a0: 2a6b 7761 7267 7329 202d 3e20 7661 7269  *kwargs) -> vari
+000153b0: 6162 6c65 7360 602e 0a20 2054 6865 2072  ables``..  The r
+000153c0: 6e67 7320 6361 6e20 6265 2061 2064 6963  ngs can be a dic
+000153d0: 7420 6f66 2050 524e 474b 6579 7320 6f72  t of PRNGKeys or
+000153e0: 2061 2073 696e 676c 6520 6060 6050 524e   a single ```PRN
+000153f0: 474b 6579 6060 2077 6869 6368 2069 730a  GKey`` which is.
+00015400: 2020 6571 7569 7661 6c65 6e74 2074 6f20    equivalent to 
+00015410: 7061 7373 696e 6720 6120 6469 6374 2077  passing a dict w
+00015420: 6974 6820 6f6e 6520 5052 4e47 4b65 7920  ith one PRNGKey 
+00015430: 7769 7468 2074 6865 206e 616d 6520 2270  with the name "p
+00015440: 6172 616d 7322 2e0a 0a20 2054 6865 2069  arams"...  The i
+00015450: 6e69 7420 6675 6e63 7469 6f6e 2074 6861  nit function tha
+00015460: 7420 6973 2072 6574 7572 6e65 6420 6361  t is returned ca
+00015470: 6e20 6265 2064 6972 6563 746c 7920 636f  n be directly co
+00015480: 6d70 6f73 6564 2077 6974 680a 2020 4a41  mposed with.  JA
+00015490: 5820 7472 616e 7366 6f72 6d61 7469 6f6e  X transformation
+000154a0: 7320 6c69 6b65 2060 606a 6178 2e6a 6974  s like ``jax.jit
+000154b0: 6060 3a3a 0a0a 2020 2020 6465 6620 6628  ``::..    def f(
+000154c0: 666f 6f2c 2078 293a 0a20 2020 2020 207a  foo, x):.      z
+000154d0: 203d 2066 6f6f 2e65 6e63 6f64 6528 7829   = foo.encode(x)
+000154e0: 0a20 2020 2020 2079 203d 2066 6f6f 2e64  .      y = foo.d
+000154f0: 6563 6f64 6528 7a29 0a20 2020 2020 2023  ecode(z).      #
+00015500: 202e 2e2e 0a20 2020 2020 2072 6574 7572   ....      retur
+00015510: 6e20 790a 0a20 2020 2066 6f6f 203d 2046  n y..    foo = F
+00015520: 6f6f 2829 0a20 2020 2066 5f6a 6974 7465  oo().    f_jitte
+00015530: 6420 3d20 6a61 782e 6a69 7428 6e6e 2e69  d = jax.jit(nn.i
+00015540: 6e69 7428 662c 2066 6f6f 2929 0a20 2020  nit(f, foo)).   
+00015550: 2076 6172 6961 626c 6573 203d 2066 5f6a   variables = f_j
+00015560: 6974 7465 6428 726e 672c 2078 290a 0a20  itted(rng, x).. 
+00015570: 2041 7267 733a 0a20 2020 2066 6e3a 2054   Args:.    fn: T
+00015580: 6865 2066 756e 6374 696f 6e20 7468 6174  he function that
+00015590: 2073 686f 756c 6420 6265 2061 7070 6c69   should be appli
+000155a0: 6564 2e20 5468 6520 6669 7273 7420 6172  ed. The first ar
+000155b0: 6775 6d65 6e74 2070 6173 7365 6420 7769  gument passed wi
+000155c0: 6c6c 0a20 2020 2020 2062 6520 616e 206d  ll.      be an m
+000155d0: 6f64 756c 6520 696e 7374 616e 6365 206f  odule instance o
+000155e0: 6620 7468 6520 6060 6d6f 6475 6c65 6060  f the ``module``
+000155f0: 2077 6974 6820 7661 7269 6162 6c65 7320   with variables 
+00015600: 616e 6420 524e 4773 2062 6f75 6e64 0a20  and RNGs bound. 
+00015610: 2020 2020 2074 6f20 6974 2e0a 2020 2020       to it..    
+00015620: 6d6f 6475 6c65 3a20 5468 6520 6060 4d6f  module: The ``Mo
+00015630: 6475 6c65 6060 2074 6861 7420 7769 6c6c  dule`` that will
+00015640: 2062 6520 7573 6564 2074 6f20 6269 6e64   be used to bind
+00015650: 2076 6172 6961 626c 6573 2061 6e64 2052   variables and R
+00015660: 4e47 7320 746f 2e0a 2020 2020 2020 5468  NGs to..      Th
+00015670: 6520 6060 4d6f 6475 6c65 6060 2070 6173  e ``Module`` pas
+00015680: 7365 6420 6173 2074 6865 2066 6972 7374  sed as the first
+00015690: 2061 7267 756d 656e 7420 746f 2060 6066   argument to ``f
+000156a0: 6e60 6020 7769 6c6c 2062 6520 6120 636c  n`` will be a cl
+000156b0: 6f6e 650a 2020 2020 2020 6f66 206d 6f64  one.      of mod
+000156c0: 756c 652e 0a20 2020 206d 7574 6162 6c65  ule..    mutable
+000156d0: 3a20 4361 6e20 6265 2062 6f6f 6c2c 2073  : Can be bool, s
+000156e0: 7472 2c20 6f72 206c 6973 742e 2053 7065  tr, or list. Spe
+000156f0: 6369 6669 6573 2077 6869 6368 2063 6f6c  cifies which col
+00015700: 6c65 6374 696f 6e73 2073 686f 756c 6420  lections should 
+00015710: 6265 0a20 2020 2020 2074 7265 6174 6564  be.      treated
+00015720: 2061 7320 6d75 7461 626c 653a 2060 6062   as mutable: ``b
+00015730: 6f6f 6c60 603a 2061 6c6c 2f6e 6f20 636f  ool``: all/no co
+00015740: 6c6c 6563 7469 6f6e 7320 6172 6520 6d75  llections are mu
+00015750: 7461 626c 652e 0a20 2020 2020 2060 6073  table..      ``s
+00015760: 7472 6060 3a20 5468 6520 6e61 6d65 206f  tr``: The name o
+00015770: 6620 6120 7369 6e67 6c65 206d 7574 6162  f a single mutab
+00015780: 6c65 2063 6f6c 6c65 6374 696f 6e2e 2060  le collection. `
+00015790: 606c 6973 7460 603a 2041 0a20 2020 2020  `list``: A.     
+000157a0: 206c 6973 7420 6f66 206e 616d 6573 206f   list of names o
+000157b0: 6620 6d75 7461 626c 6520 636f 6c6c 6563  f mutable collec
+000157c0: 7469 6f6e 732e 2042 7920 6465 6661 756c  tions. By defaul
+000157d0: 7420 616c 6c20 636f 6c6c 6563 7469 6f6e  t all collection
+000157e0: 730a 2020 2020 2020 6578 6365 7074 2022  s.      except "
+000157f0: 696e 7465 726d 6564 6961 7465 7322 2061  intermediates" a
+00015800: 7265 206d 7574 6162 6c65 2e0a 2020 2020  re mutable..    
+00015810: 6361 7074 7572 655f 696e 7465 726d 6564  capture_intermed
+00015820: 6961 7465 733a 2049 6620 6054 7275 6560  iates: If `True`
+00015830: 2c20 6361 7074 7572 6573 2069 6e74 6572  , captures inter
+00015840: 6d65 6469 6174 6520 7265 7475 726e 2076  mediate return v
+00015850: 616c 7565 730a 2020 2020 2020 6f66 2061  alues.      of a
+00015860: 6c6c 204d 6f64 756c 6573 2069 6e73 6964  ll Modules insid
+00015870: 6520 7468 6520 2269 6e74 6572 6d65 6469  e the "intermedi
+00015880: 6174 6573 2220 636f 6c6c 6563 7469 6f6e  ates" collection
+00015890: 2e20 4279 2064 6566 6175 6c74 206f 6e6c  . By default onl
+000158a0: 790a 2020 2020 2020 7468 6520 7265 7475  y.      the retu
+000158b0: 726e 2076 616c 7565 7320 6f66 2061 6c6c  rn values of all
+000158c0: 2060 5f5f 6361 6c6c 5f5f 6020 6d65 7468   `__call__` meth
+000158d0: 6f64 7320 6172 6520 7374 6f72 6564 2e20  ods are stored. 
+000158e0: 4120 6675 6e63 7469 6f6e 2063 616e 0a20  A function can. 
+000158f0: 2020 2020 2062 6520 7061 7373 6564 2074       be passed t
+00015900: 6f20 6368 616e 6765 2074 6865 2066 696c  o change the fil
+00015910: 7465 7220 6265 6861 7669 6f72 2e20 5468  ter behavior. Th
+00015920: 6520 6669 6c74 6572 2066 756e 6374 696f  e filter functio
+00015930: 6e20 7461 6b65 730a 2020 2020 2020 7468  n takes.      th
+00015940: 6520 4d6f 6475 6c65 2069 6e73 7461 6e63  e Module instanc
+00015950: 6520 616e 6420 6d65 7468 6f64 206e 616d  e and method nam
+00015960: 6520 616e 6420 7265 7475 726e 7320 6120  e and returns a 
+00015970: 626f 6f6c 2069 6e64 6963 6174 696e 670a  bool indicating.
+00015980: 2020 2020 2020 7768 6574 6865 7220 7468        whether th
+00015990: 6520 6f75 7470 7574 206f 6620 7468 6174  e output of that
+000159a0: 206d 6574 686f 6420 696e 766f 6361 7469   method invocati
+000159b0: 6f6e 2073 686f 756c 6420 6265 2073 746f  on should be sto
+000159c0: 7265 642e 0a20 2052 6574 7572 6e73 3a0a  red..  Returns:.
+000159d0: 2020 2020 5468 6520 696e 6974 2066 756e      The init fun
+000159e0: 6374 696f 6e20 7772 6170 7069 6e67 2060  ction wrapping `
+000159f0: 6066 6e60 602e 0a20 2022 2222 0a20 2069  `fn``..  """.  i
+00015a00: 6e69 745f 666e 203d 2069 6e69 745f 7769  nit_fn = init_wi
+00015a10: 7468 5f6f 7574 7075 7428 666e 2c20 6d6f  th_output(fn, mo
+00015a20: 6475 6c65 2c20 6d75 7461 626c 652c 2063  dule, mutable, c
+00015a30: 6170 7475 7265 5f69 6e74 6572 6d65 6469  apture_intermedi
+00015a40: 6174 6573 290a 0a20 2040 6675 6e63 746f  ates)..  @functo
+00015a50: 6f6c 732e 7772 6170 7328 696e 6974 5f66  ols.wraps(init_f
+00015a60: 6e29 0a20 2064 6566 2069 6e69 745f 7772  n).  def init_wr
+00015a70: 6170 7065 7228 2a61 7267 732c 202a 2a6b  apper(*args, **k
+00015a80: 7761 7267 7329 3a0a 2020 2020 7265 7475  wargs):.    retu
+00015a90: 726e 2069 6e69 745f 666e 282a 6172 6773  rn init_fn(*args
+00015aa0: 2c20 2a2a 6b77 6172 6773 295b 315d 0a0a  , **kwargs)[1]..
+00015ab0: 2020 7265 7475 726e 2069 6e69 745f 7772    return init_wr
+00015ac0: 6170 7065 720a                           apper.
```

### Comparing `flax-0.7.1/flax/linen/normalization.py` & `flax-0.7.2/flax/linen/normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,28 +225,31 @@
     axis_name: the axis name used to combine batch statistics from multiple
       devices. See `jax.pmap` for a description of axis names (default: None).
     axis_index_groups: groups of axis indices within that named axis
       representing subsets of devices to reduce over (default: None). For
       example, `[[0, 1], [2, 3]]` would independently batch-normalize over
       the examples on the first two and last two devices. See `jax.lax.psum`
       for more details.
+    use_fast_variance: If true, use a faster, but less numerically stable,
+      calculation for the variance.
   """
 
   use_running_average: Optional[bool] = None
   axis: int = -1
   momentum: float = 0.99
   epsilon: float = 1e-5
   dtype: Optional[Dtype] = None
   param_dtype: Dtype = jnp.float32
   use_bias: bool = True
   use_scale: bool = True
   bias_init: Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros
   scale_init: Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones
   axis_name: Optional[str] = None
   axis_index_groups: Any = None
+  use_fast_variance: bool = True
 
   @compact
   def __call__(self, x, use_running_average: Optional[bool] = None):
     """Normalizes the input using batch statistics.
 
     NOTE:
     During initialization (when `self.is_initializing()` is `True`) the running
@@ -286,14 +289,15 @@
     else:
       mean, var = _compute_stats(
           x,
           reduction_axes,
           dtype=self.dtype,
           axis_name=self.axis_name if not self.is_initializing() else None,
           axis_index_groups=self.axis_index_groups,
+          use_fast_variance=self.use_fast_variance,
       )
 
       if not self.is_initializing():
         ra_mean.value = (
             self.momentum * ra_mean.value + (1 - self.momentum) * mean
         )
         ra_var.value = self.momentum * ra_var.value + (1 - self.momentum) * var
@@ -511,27 +515,30 @@
       This is only needed if the model is subdivided across devices, i.e. the
       array being normalized is sharded across devices within a pmap.
     axis_index_groups: groups of axis indices within that named axis
       representing subsets of devices to reduce over (default: None). For
       example, `[[0, 1], [2, 3]]` would independently batch-normalize over the
       examples on the first two and last two devices. See `jax.lax.psum` for
       more details.
+    use_fast_variance: If true, use a faster, but less numerically stable,
+      calculation for the variance.
   """
 
   num_groups: Optional[int] = 32
   group_size: Optional[int] = None
   epsilon: float = 1e-6
   dtype: Optional[Dtype] = None
   param_dtype: Dtype = jnp.float32
   use_bias: bool = True
   use_scale: bool = True
   bias_init: Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros
   scale_init: Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones
   axis_name: Optional[str] = None
   axis_index_groups: Any = None
+  use_fast_variance: bool = True
 
   @compact
   def __call__(self, x):
     """Applies group normalization to the input (arxiv.org/abs/1803.08494).
 
     Args:
       x: the input of shape N...C, where N is a batch dimension and C is a
@@ -577,14 +584,15 @@
 
     mean, var = _compute_stats(
         x.reshape(group_shape),
         reduction_axes,
         self.dtype,
         self.axis_name,
         self.axis_index_groups,
+        use_fast_variance=self.use_fast_variance,
     )
     mean = jnp.repeat(mean, group_size, axis=-1)
     var = jnp.repeat(var, group_size, axis=-1)
 
     return _normalize(
         self,
         x,
```

### Comparing `flax-0.7.1/flax/linen/partitioning.py` & `flax-0.7.2/flax/linen/partitioning.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/pooling.py` & `flax-0.7.2/flax/linen/pooling.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/recurrent.py` & `flax-0.7.2/flax/linen/recurrent.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/spmd.py` & `flax-0.7.2/flax/linen/spmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 import dataclasses
 import enum
 import functools
 import threading
 from typing import Any, Callable, List, Optional, Sequence, Tuple, Union
 
 import jax
-from jax.experimental import maps, pjit
+from jax import lax
+from jax.experimental import maps
 from flax import struct
 
 from flax.core import meta
 from flax.core.lift import In as ScanIn  # pylint: disable=unused-import
 from flax.core.lift import Out as ScanOut  # pylint: disable=unused-import
 
 # Real types and dummy aliases for documentation
@@ -221,24 +222,24 @@
 
 
 def _with_sharding_constraint(
     x: Array,
     axis_resources: Optional[jax.sharding.PartitionSpec],
     mesh: Optional[jax.sharding.Mesh] = None,
 ):
-  """Wrapper for pjit with_sharding_constraint, no-op on cpu or outside pjit."""
+  """Wrapper for lax.with_sharding_constraint, no-op on cpu or outside pjit."""
   if jax.devices()[0].platform == 'cpu' or (
       not _global_mesh_defined() and mesh is None
   ):
     return x
   else:
     if mesh is not None and axis_resources is not None:
       sharding = jax.sharding.NamedSharding(mesh, axis_resources)
-      return pjit.with_sharding_constraint(x, sharding)
-    return pjit.with_sharding_constraint(x, axis_resources)
+      return lax.with_sharding_constraint(x, sharding)
+    return lax.with_sharding_constraint(x, axis_resources)
 
 
 def _with_sharding_constraint_one_fallback(
     axis_resources: LogicalPartitionSpec,
     x: Array,
     fallback: RulesFallback = RulesFallback.AXIS_IS_UNSHARDED,
     rules: Optional[LogicalRules] = None,
```

### Comparing `flax-0.7.1/flax/linen/stochastic.py` & `flax-0.7.2/flax/linen/stochastic.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/summary.py` & `flax-0.7.2/flax/linen/summary.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/linen/transforms.py` & `flax-0.7.2/flax/linen/transforms.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/metrics/__init__.py` & `flax-0.7.2/flax/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/metrics/tensorboard.py` & `flax-0.7.2/flax/metrics/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/serialization.py` & `flax-0.7.2/flax/serialization.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/struct.py` & `flax-0.7.2/flax/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 _T = TypeVar('_T')
 
 
 def field(pytree_node=True, **kwargs):
   return dataclasses.field(metadata={'pytree_node': pytree_node}, **kwargs)
 
 
-@dataclass_transform(field_descriptors=(field,))  # type: ignore[literal-required]
+@dataclass_transform(field_specifiers=(field,))  # type: ignore[literal-required]
 def dataclass(clz: _T) -> _T:
   """Create a class which can be passed to functional transformations.
 
   NOTE: Inherit from ``PyTreeNode`` instead to avoid type checking issues when
   using PyType.
 
   Jax transformations such as `jax.jit` and `jax.grad` require objects that are
@@ -177,15 +177,15 @@
 
   return data_clz  # type: ignore
 
 
 TNode = TypeVar('TNode', bound='PyTreeNode')
 
 
-@dataclass_transform(field_descriptors=(field,))  # type: ignore[literal-required]
+@dataclass_transform(field_specifiers=(field,))  # type: ignore[literal-required]
 class PyTreeNode:
   """Base class for dataclasses that should act like a JAX pytree node.
 
   See ``flax.struct.dataclass`` for the ``jax.tree_util`` behavior.
   This base class additionally avoids type checking errors when using PyType.
 
   Example::
```

### Comparing `flax-0.7.1/flax/testing/__init__.py` & `flax-0.7.2/flax/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/testing/benchmark.py` & `flax-0.7.2/flax/testing/benchmark.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/traceback_util.py` & `flax-0.7.2/flax/traceback_util.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/__init__.py` & `flax-0.7.2/flax/training/__init__.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/checkpoints.py` & `flax-0.7.2/flax/training/checkpoints.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/common_utils.py` & `flax-0.7.2/flax/training/common_utils.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/dynamic_scale.py` & `flax-0.7.2/flax/training/dynamic_scale.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/early_stopping.py` & `flax-0.7.2/flax/training/early_stopping.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/lr_schedule.py` & `flax-0.7.2/flax/training/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/orbax_utils.py` & `flax-0.7.2/flax/training/orbax_utils.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/prefetch_iterator.py` & `flax-0.7.2/flax/training/prefetch_iterator.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/training/train_state.py` & `flax-0.7.2/flax/training/train_state.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/traverse_util.py` & `flax-0.7.2/flax/traverse_util.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/flax/version.py` & `flax-0.7.2/flax/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current Flax version at head on Github."""
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

### Comparing `flax-0.7.1/flax.egg-info/PKG-INFO` & `flax-0.7.2/flax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flax
-Version: 0.7.1
+Version: 0.7.2
 Summary: Flax: A neural network library for JAX designed for flexibility
 Author-email: Flax team <flax-dev@google.com>
 Project-URL: homepage, https://github.com/google/flax
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -211,15 +211,15 @@
 To cite this repository:
 
 ```
 @software{flax2020github,
   author = {Jonathan Heek and Anselm Levskaya and Avital Oliver and Marvin Ritter and Bertrand Rondepierre and Andreas Steiner and Marc van {Z}ee},
   title = {{F}lax: A neural network library and ecosystem for {JAX}},
   url = {http://github.com/google/flax},
-  version = {0.7.1},
+  version = {0.7.2},
   year = {2023},
 }
 ```
 
 In the above bibtex entry, names are in alphabetical order, the version number
 is intended to be that from [flax/version.py](https://github.com/google/flax/blob/main/flax/version.py), and the year corresponds to the project's open-source release.
```

### Comparing `flax-0.7.1/flax.egg-info/SOURCES.txt` & `flax-0.7.2/flax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/images/flax_logo.png` & `flax-0.7.2/images/flax_logo.png`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/images/flax_logo.svg` & `flax-0.7.2/images/flax_logo.svg`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/images/flax_logo_250px.png` & `flax-0.7.2/images/flax_logo_250px.png`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/images/flax_logo_500px.png` & `flax-0.7.2/images/flax_logo_500px.png`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/pylintrc` & `flax-0.7.2/pylintrc`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/pyproject.toml` & `flax-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/checkpoints_test.py` & `flax-0.7.2/tests/checkpoints_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/colab_tpu_jax_version.ipynb` & `flax-0.7.2/tests/colab_tpu_jax_version.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/core_frozen_dict_test.py` & `flax-0.7.2/tests/core/core_frozen_dict_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,26 @@
     self.assertTrue(
         new_x == actual_new_x and isinstance(new_x, type(actual_new_x))
     )
 
   @parameterized.parameters(
       {
           'x': {'a': 1, 'b': {'c': 2}},
+      },
+      {
+          'x': FrozenDict({'a': 1, 'b': {'c': 2}}),
+      },
+  )
+  def test_utility_copy_singlearg(self, x):
+    new_x = copy(x)
+    self.assertTrue(new_x == x and isinstance(new_x, type(x)))
+
+  @parameterized.parameters(
+      {
+          'x': {'a': 1, 'b': {'c': 2}},
           'pretty_str': '{\n    a: 1,\n    b: {\n        c: 2,\n    },\n}',
       },
       {
           'x': FrozenDict({'a': 1, 'b': {'c': 2}}),
           'pretty_str': (
               'FrozenDict({\n    a: 1,\n    b: {\n        c: 2,\n    },\n})'
           ),
```

### Comparing `flax-0.7.1/tests/core/core_lift_test.py` & `flax-0.7.2/tests/core/core_lift_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/core_meta_test.py` & `flax-0.7.2/tests/core/core_meta_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/core_scope_test.py` & `flax-0.7.2/tests/core/core_scope_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_attention_test.py` & `flax-0.7.2/tests/core/design/core_attention_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_auto_encoder_test.py` & `flax-0.7.2/tests/core/design/core_auto_encoder_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_big_resnets_test.py` & `flax-0.7.2/tests/core/design/core_big_resnets_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_custom_vjp_test.py` & `flax-0.7.2/tests/core/design/core_custom_vjp_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_dense_test.py` & `flax-0.7.2/tests/core/design/core_dense_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_flow_test.py` & `flax-0.7.2/tests/core/design/core_flow_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_resnet_test.py` & `flax-0.7.2/tests/core/design/core_resnet_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_scan_test.py` & `flax-0.7.2/tests/core/design/core_scan_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_tied_autoencoder_test.py` & `flax-0.7.2/tests/core/design/core_tied_autoencoder_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_vmap_test.py` & `flax-0.7.2/tests/core/design/core_vmap_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/core/design/core_weight_std_test.py` & `flax-0.7.2/tests/core/design/core_weight_std_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/download_dataset_metadata.sh` & `flax-0.7.2/tests/download_dataset_metadata.sh`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/early_stopping_test.py` & `flax-0.7.2/tests/early_stopping_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/import_test.ipynb` & `flax-0.7.2/tests/import_test.ipynb`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/io_test.py` & `flax-0.7.2/tests/io_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/jax_utils_test.py` & `flax-0.7.2/tests/jax_utils_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/initializers_test.py` & `flax-0.7.2/tests/linen/initializers_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/kw_only_dataclasses_test.py` & `flax-0.7.2/tests/linen/kw_only_dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_activation_test.py` & `flax-0.7.2/tests/linen/linen_activation_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_attention_test.py` & `flax-0.7.2/tests/linen/linen_attention_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_combinators_test.py` & `flax-0.7.2/tests/linen/linen_combinators_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_dtypes_test.py` & `flax-0.7.2/tests/linen/linen_dtypes_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_linear_test.py` & `flax-0.7.2/tests/linen/linen_linear_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_meta_test.py` & `flax-0.7.2/tests/linen/linen_meta_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_module_test.py` & `flax-0.7.2/tests/linen/linen_module_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_recurrent_test.py` & `flax-0.7.2/tests/linen/linen_recurrent_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_test.py` & `flax-0.7.2/tests/linen/linen_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/linen_transforms_test.py` & `flax-0.7.2/tests/linen/linen_transforms_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/partitioning_test.py` & `flax-0.7.2/tests/linen/partitioning_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/summary_test.py` & `flax-0.7.2/tests/linen/summary_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/linen/toplevel_test.py` & `flax-0.7.2/tests/linen/toplevel_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/run_all_tests.sh` & `flax-0.7.2/tests/run_all_tests.sh`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/serialization_test.py` & `flax-0.7.2/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/struct_test.py` & `flax-0.7.2/tests/struct_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/tensorboard_test.py` & `flax-0.7.2/tests/tensorboard_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/traceback_util_test.py` & `flax-0.7.2/tests/traceback_util_test.py`

 * *Files identical despite different names*

### Comparing `flax-0.7.1/tests/traverse_util_test.py` & `flax-0.7.2/tests/traverse_util_test.py`

 * *Files identical despite different names*


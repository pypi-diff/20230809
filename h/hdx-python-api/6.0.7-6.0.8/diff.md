# Comparing `tmp/hdx_python_api-6.0.7.tar.gz` & `tmp/hdx_python_api-6.0.8.tar.gz`

## Comparing `hdx_python_api-6.0.7.tar` & `hdx_python_api-6.0.8.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    44094 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/documentation/main.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/_version.py
--rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/configuration.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/hdx_base_configuration.yaml
--rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/locations.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/__init__.py
--rwxr-xr-x   0        0        0   112338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/dataset.py
--rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0        0        0     6883 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/date_helper.py
--rwxr-xr-x   0        0        0     3830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/hdxobject.py
--rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/indicator_resource_view_template.yaml
--rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/organization.py
--rwxr-xr-x   0        0        0    27610 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/resource.py
--rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/resource_view.py
--rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/showcase.py
--rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/user.py
--rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/vocabulary.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/simple.py
--rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/Tag_Mapping_ChainRuleError.csv
--rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/dataset_search_results.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/empty.csv
--rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/organization_show_results.yaml
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/resource_formats.json
--rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/showcase_all_search_results.yaml
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/test_data.zip
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_base_config.yaml
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_email_configuration.yaml
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_organization_static.yaml
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_static.yaml
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_view_static.yaml
--rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_showcase_static.yaml
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_user_static.yaml
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_vocabulary_static.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/test_data_no_years.csv
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources.yaml
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources_new.yaml
--rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/api/test_locations.py
--rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/__init__.py
--rwxr-xr-x   0        0        0    49390 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_organization.py
--rwxr-xr-x   0        0        0    47292 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_resource.py
--rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_showcase.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_user.py
--rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_vocabulary.py
--rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/test_simple.py
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/my_code.py
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/my_resource.csv
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/my_resource.xlsx
--rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/run.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/LICENSE
--rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/README.md
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/pyproject.toml
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     5102 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    44094 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/documentation/main.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/api/locations.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   112338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     6883 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    27610 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49390 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    47292 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/workingexample/run.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/LICENSE
+-rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/README.md
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.8/PKG-INFO
```

### Comparing `hdx_python_api-6.0.7/CONTRIBUTING.md` & `hdx_python_api-6.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/requirements.txt` & `hdx_python_api-6.0.8/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
+annotated-types==0.5.0
+    # via pydantic
 attrs==23.1.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-chardet==5.1.0
+chardet==5.2.0
     # via frictionless
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 ckanapi==4.7
     # via hdx-python-api (pyproject.toml)
-click==8.1.3
+click==8.1.6
     # via typer
 colorama==0.4.6
     # via typer
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.1
+cryptography==41.0.3
     # via pyopenssl
 decorator==5.1.1
     # via
     #   jsonpath-ng
     #   validators
 defopt==6.4.0
     # via hdx-python-api (pyproject.toml)
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-dnspython==2.3.0
+dnspython==2.4.1
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
 docutils==0.20.1
     # via defopt
 email-validator==2.0.0.post2
     # via hdx-python-api (pyproject.toml)
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
-frictionless==5.13.1
+frictionless==5.15.10
     # via hdx-python-utilities
-hdx-python-country==3.5.1
+hdx-python-country==3.5.2
     # via hdx-python-api (pyproject.toml)
-hdx-python-utilities==3.6.1
+hdx-python-utilities==3.6.2
     # via hdx-python-country
-humanize==4.6.0
+humanize==4.7.0
     # via frictionless
-identify==2.5.24
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   email-validator
     #   requests
-ijson==3.2.2
+ijson==3.2.3
     # via hdx-python-utilities
-inflect==6.0.4
+inflect==7.0.0
     # via quantulum3
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.2
     # via frictionless
@@ -79,15 +81,15 @@
     # via hdx-python-utilities
 jsonpath-ng==1.5.3
     # via libhxl
 jsonschema==4.17.3
     # via
     #   frictionless
     #   tableschema-to-template
-libhxl==5.0.1
+libhxl==5.0.2
     # via hdx-python-country
 loguru==0.7.0
     # via hdx-python-utilities
 makefun==1.15.1
     # via hdx-python-api (pyproject.toml)
 markdown-it-py==3.0.0
     # via rich
@@ -105,15 +107,15 @@
     # via quantulum3
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==23.1
     # via pytest
 petl==1.7.12
     # via frictionless
-platformdirs==3.8.0
+platformdirs==3.10.0
     # via virtualenv
 pluggy==1.2.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
@@ -123,19 +125,21 @@
     # via hdx-python-api (pyproject.toml)
 pyasn1==0.5.0
     # via
     #   hdx-python-api (pyproject.toml)
     #   ndg-httpsclient
 pycparser==2.21
     # via cffi
-pydantic==1.10.9
+pydantic==2.1.1
     # via
     #   frictionless
     #   inflect
-pygments==2.15.1
+pydantic-core==2.4.0
+    # via pydantic
+pygments==2.16.1
     # via rich
 pyopenssl==23.2.0
     # via
     #   hdx-python-api (pyproject.toml)
     #   ndg-httpsclient
 pyphonetics==0.5.3
     # via hdx-python-country
@@ -155,15 +159,15 @@
     #   libhxl
 python-io-wrapper==0.3.1
     # via libhxl
 python-slugify==8.0.1
     # via
     #   ckanapi
     #   frictionless
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 quantulum3==0.9.0
     # via hdx-python-api (pyproject.toml)
 ratelimit==2.2.1
@@ -174,15 +178,15 @@
     #   frictionless
     #   libhxl
     #   requests-file
 requests-file==1.5.1
     # via hdx-python-utilities
 rfc3986==2.0.0
     # via frictionless
-rich==13.4.2
+rich==13.5.2
     # via typer
 ruamel-yaml==0.17.32
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 shellingham==1.5.0.post1
     # via typer
@@ -207,32 +211,34 @@
     # via hdx-python-utilities
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
 typer[all]==0.9.0
     # via frictionless
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   frictionless
+    #   inflect
     #   pydantic
+    #   pydantic-core
     #   typer
 unidecode==1.3.6
     # via
     #   libhxl
     #   pyphonetics
-urllib3==2.0.3
+urllib3==2.0.4
     # via
     #   libhxl
     #   requests
 validators==0.20.0
     # via frictionless
-virtualenv==20.23.1
+virtualenv==20.24.2
     # via pre-commit
-wheel==0.40.0
+wheel==0.41.1
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
 xlsxwriter==3.1.2
     # via tableschema-to-template
```

### Comparing `hdx_python_api-6.0.7/.config/pre-commit-config.yaml` & `hdx_python_api-6.0.8/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/.github/workflows/publish.yaml` & `hdx_python_api-6.0.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/.github/workflows/run-python-tests.yaml` & `hdx_python_api-6.0.8/.github/workflows/run-python-tests.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 name: Run tests
 
 on:
   workflow_dispatch: # add run button in github
   push:
     branches-ignore:
       - gh-pages
+      - 'dependabot/**'
   pull_request:
     branches-ignore:
       - gh-pages
 
 jobs:
   build:
     runs-on: ubuntu-latest
```

### Comparing `hdx_python_api-6.0.7/documentation/main.md` & `hdx_python_api-6.0.8/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/documentation/pydoc-markdown.yaml` & `hdx_python_api-6.0.8/documentation/pydoc-markdown.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - hdx.data
       - hdx.facades
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python API
-    theme: readthedocs
+    theme: mkdocs
     repo_url: "https://github.com/OCHA-DAP/hdx-python-api"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-api
   pages:
     - title: Home
```

### Comparing `hdx_python_api-6.0.7/src/hdx/api/configuration.py` & `hdx_python_api-6.0.8/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/api/hdx_base_configuration.yaml` & `hdx_python_api-6.0.8/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/api/locations.py` & `hdx_python_api-6.0.8/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/dataset.py` & `hdx_python_api-6.0.8/src/hdx/data/dataset.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.0.8/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/date_helper.py` & `hdx_python_api-6.0.8/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.0.8/src/hdx/data/filestore_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/hdxobject.py` & `hdx_python_api-6.0.8/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/indicator_resource_view_template.yaml` & `hdx_python_api-6.0.8/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/organization.py` & `hdx_python_api-6.0.8/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/resource.py` & `hdx_python_api-6.0.8/src/hdx/data/resource.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.0.8/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/resource_view.py` & `hdx_python_api-6.0.8/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/showcase.py` & `hdx_python_api-6.0.8/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/user.py` & `hdx_python_api-6.0.8/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/data/vocabulary.py` & `hdx_python_api-6.0.8/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.0.8/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.0.8/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/src/hdx/facades/simple.py` & `hdx_python_api-6.0.8/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.0.8/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.0.8/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/dataset_search_results.yaml` & `hdx_python_api-6.0.8/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/organization_show_results.yaml` & `hdx_python_api-6.0.8/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/resource_formats.json` & `hdx_python_api-6.0.8/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/showcase_all_search_results.yaml` & `hdx_python_api-6.0.8/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/test_data.csv` & `hdx_python_api-6.0.8/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/test_data.zip` & `hdx_python_api-6.0.8/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.0.8/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.yaml` & `hdx_python_api-6.0.8/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.0.8/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_view_static.yaml` & `hdx_python_api-6.0.8/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.0.8/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.0.8/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.8/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.0.8/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.8/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.0.8/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources.yaml` & `hdx_python_api-6.0.8/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources_new.yaml` & `hdx_python_api-6.0.8/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/conftest.py` & `hdx_python_api-6.0.8/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.0.8/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/api/test_locations.py` & `hdx_python_api-6.0.8/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/__init__.py` & `hdx_python_api-6.0.8/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_dataset_core.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_dataset_noncore.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_organization.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_resource.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_resource.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_update_dataset_resources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_user.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.0.8/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/facades/__init__.py` & `hdx_python_api-6.0.8/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.0.8/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.0.8/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.0.8/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/workingexample/my_resource.xlsx` & `hdx_python_api-6.0.8/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/.gitignore` & `hdx_python_api-6.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/LICENSE` & `hdx_python_api-6.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/README.md` & `hdx_python_api-6.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.7/pyproject.toml` & `hdx_python_api-6.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ]
 requires-python = ">=3.8"
 
 dependencies = [
     "ckanapi >= 4.7",
     "defopt >= 6.4.0",
     "email_validator",
-    "hdx-python-country>= 3.5.1",
+    "hdx-python-country>= 3.5.2",
     "makefun",
     "ndg-httpsclient",
     "pyasn1",
     "pyOpenSSL",
     "quantulum3",
 ]
 dynamic = ["version"]
```

### Comparing `hdx_python_api-6.0.7/PKG-INFO` & `hdx_python_api-6.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.7
+Version: 6.0.8
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: ckanapi>=4.7
 Requires-Dist: defopt>=6.4.0
 Requires-Dist: email-validator
-Requires-Dist: hdx-python-country>=3.5.1
+Requires-Dist: hdx-python-country>=3.5.2
 Requires-Dist: makefun
 Requires-Dist: ndg-httpsclient
 Requires-Dist: pyasn1
 Requires-Dist: pyopenssl
 Requires-Dist: quantulum3
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
```


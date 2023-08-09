# Comparing `tmp/asf_search-6.6.1.tar.gz` & `tmp/asf_search-6.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asf_search-6.6.1.tar", last modified: Wed Jul 26 17:32:21 2023, max compression
+gzip compressed data, was "asf_search-6.6.2.tar", last modified: Wed Aug  9 00:29:54 2023, max compression
```

## Comparing `asf_search-6.6.1.tar` & `asf_search-6.6.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.067240 asf_search-6.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 17:32:09.000000 asf_search-6.6.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.019239 asf_search-6.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.023239 asf_search-6.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.023239 asf_search-6.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-26 17:32:09.000000 asf_search-6.6.1/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-26 17:32:09.000000 asf_search-6.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-07-26 17:32:09.000000 asf_search-6.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-26 17:32:09.000000 asf_search-6.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-26 17:32:21.067240 asf_search-6.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-26 17:32:09.000000 asf_search-6.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.027239 asf_search-6.6.1/asf_search/
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.031239 asf_search-6.6.1/asf_search/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/ASFSearchOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/validator_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchOptions/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.031239 asf_search-6.6.1/asf_search/CMR/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/MissionList.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/field_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/subquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/CMR/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.035239 asf_search-6.6.1/asf_search/WKT/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/WKT/RepairEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/WKT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/WKT/validate_wkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.035239 asf_search-6.6.1/asf_search/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/baseline/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/baseline/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.039240 asf_search-6.6.1/asf_search/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/BEAMMODE.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/FLIGHT_DIRECTION.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/INSTRUMENT.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/INTERNAL.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/PLATFORM.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/POLARIZATION.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/PRODUCT_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.039240 asf_search-6.6.1/asf_search/download/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/download/file_download_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.043240 asf_search-6.6.1/asf_search/export/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/export_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/jsonlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/jsonlite2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/export/metalink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.043240 asf_search-6.6.1/asf_search/health/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/health/health.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/asf_search/search/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/baseline_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/geo_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/granule_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/product_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/search_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-26 17:32:09.000000 asf_search-6.6.1/asf_search/search/search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.027239 asf_search-6.6.1/asf_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-26 17:32:21.000000 asf_search-6.6.1/asf_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 17:32:20.000000 asf_search-6.6.1/asf_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/0-Intro.md
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/1-Basic_Overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/2-Geographic_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/3-Granule_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/4-Baseline_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/5-Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/6-Outro.md
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-26 17:32:09.000000 asf_search-6.6.1/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 17:32:09.000000 asf_search-6.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:32:21.067240 asf_search-6.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-26 17:32:09.000000 asf_search-6.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/tests/ASFProduct/
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFProduct/test_ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.047240 asf_search-6.6.1/tests/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFSearchOptions/test_ASFSearchOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/ASFSearchResults/
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFSearchResults/test_ASFSearchResults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/ASFSession/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/ASFSession/test_ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/BaselineSearch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/BaselineSearch/Stack/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/BaselineSearch/Stack/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/BaselineSearch/test_baseline_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/CMR/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/CMR/test_MissionList.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/Search/
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/Search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/Search/test_search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/Serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/Serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/WKT/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/WKT/test_validate_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.051240 asf_search-6.6.1/tests/download/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/download/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/pytest-managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.055240 asf_search-6.6.1/tests/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:32:21.067240 asf_search-6.6.1/tests/yml_tests/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Alos_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_L1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (123)    48181 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    46473 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.kml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
--rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53132 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)   376802 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
--rw-r--r--   0 runner    (1001) docker     (123)    38828 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/S1_baseline_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/S1_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25903 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/SMAP_response.yml
--rw-r--r--   0 runner    (1001) docker     (123)   600436 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFProduct.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFSearchOptions.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFSearchResults.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_ASFSession.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_baseline_search.yml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_campaigns.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_download.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_known_bugs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_notebooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_search.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_search_generator.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_serialization.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_stack.yml
--rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-07-26 17:32:09.000000 asf_search-6.6.1/tests/yml_tests/test_validate_wkt.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.787320 asf_search-6.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-09 00:29:38.000000 asf_search-6.6.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.767321 asf_search-6.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.767321 asf_search-6.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.767321 asf_search-6.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-09 00:29:38.000000 asf_search-6.6.2/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-09 00:29:38.000000 asf_search-6.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21457 2023-08-09 00:29:38.000000 asf_search-6.6.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-09 00:29:38.000000 asf_search-6.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-09 00:29:54.787320 asf_search-6.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-09 00:29:38.000000 asf_search-6.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.767321 asf_search-6.6.2/asf_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSearchOptions/ASFSearchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSearchOptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSearchOptions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSearchOptions/validator_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSearchOptions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/CMR/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/CMR/MissionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/CMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/CMR/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/CMR/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/CMR/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/WKT/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/WKT/RepairEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/WKT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/WKT/validate_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/baseline/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/baseline/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/BEAMMODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/FLIGHT_DIRECTION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/INSTRUMENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/INTERNAL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/PLATFORM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/POLARIZATION.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/PRODUCT_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/download/file_download_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.771321 asf_search-6.6.2/asf_search/export/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/export_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/jsonlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/jsonlite2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/export/metalink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/asf_search/health/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/health/health.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/asf_search/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/baseline_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/geo_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/granule_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/product_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/search_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-08-09 00:29:38.000000 asf_search-6.6.2/asf_search/search/search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.767321 asf_search-6.6.2/asf_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-09 00:29:54.000000 asf_search-6.6.2/asf_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-09 00:29:54.000000 asf_search-6.6.2/asf_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:29:54.000000 asf_search-6.6.2/asf_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-09 00:29:54.000000 asf_search-6.6.2/asf_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-09 00:29:54.000000 asf_search-6.6.2/asf_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/0-Intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/1-Basic_Overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/2-Geographic_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/3-Granule_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/4-Baseline_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/5-Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/6-Outro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-09 00:29:38.000000 asf_search-6.6.2/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-09 00:29:38.000000 asf_search-6.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:29:54.787320 asf_search-6.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-09 00:29:38.000000 asf_search-6.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/ASFProduct/
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/ASFProduct/test_ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/ASFSearchOptions/test_ASFSearchOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/ASFSearchResults/
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/ASFSearchResults/test_ASFSearchResults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/ASFSession/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/ASFSession/test_ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/BaselineSearch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/BaselineSearch/Stack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/BaselineSearch/Stack/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/BaselineSearch/test_baseline_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/CMR/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/CMR/test_MissionList.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/Search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/Search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/Search/test_search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/Serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.775321 asf_search-6.6.2/tests/WKT/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/WKT/test_validate_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.779321 asf_search-6.6.2/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/download/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/pytest-managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.779321 asf_search-6.6.2/tests/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:29:54.787320 asf_search-6.6.2/tests/yml_tests/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Alos_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Alos_response_maxResults3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_L1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    48181 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    46473 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.kml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.metalink
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    52821 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53132 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   376802 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    38828 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/S1_baseline_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/S1_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/SLC_BURST.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25903 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/SLC_BURST_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/SMAP_response.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   600436 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_ASFProduct.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_ASFSearchOptions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_ASFSearchResults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_ASFSession.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_baseline_search.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_campaigns.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_download.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_known_bugs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_search.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_search_generator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_serialization.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-08-09 00:29:38.000000 asf_search-6.6.2/tests/yml_tests/test_validate_wkt.yml
```

### Comparing `asf_search-6.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `asf_search-6.6.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/.github/ISSUE_TEMPLATE/feature_request.md` & `asf_search-6.6.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/.github/workflows/prod-request-merged.yml` & `asf_search-6.6.2/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/.github/workflows/pypi-publish.yml` & `asf_search-6.6.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/.github/workflows/run-pytest.yml` & `asf_search-6.6.2/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/.gitignore` & `asf_search-6.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/CHANGELOG.md` & `asf_search-6.6.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 - 
 
 ### Removed:
 -
 
 -->
 ------
+## [v6.6.2](https://github.com/asfadmin/Discovery-asf_search/compare/v6.6.1...v6.6.2)
+### Added
+- Adds new `CMRIncompleteError` exception, raised by search methods when CMR returns an incomplete page
+### Fixed
+- Fixes bug in `search_generator()` causing results to sometimes wrongly be marked as incomplete
+### Changed
+- `stack_from_id()` now raises if results are incomplete, before checking if reference was found
+
+------
 ## [v6.6.1](https://github.com/asfadmin/Discovery-asf_search/compare/v6.6.0...v6.6.1)
 ### Added
 - Adds automated release notes
 ### Fixed
 - `filename` can be used again with `ASFProduct.Download()` method (ignored if multiple files are to be downloaded)
 
 ------
```

### Comparing `asf_search-6.6.1/LICENSE` & `asf_search-6.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/PKG-INFO` & `asf_search-6.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 6.6.1
+Version: 6.6.2
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `asf_search-6.6.1/README.md` & `asf_search-6.6.2/README.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/ASFProduct.py` & `asf_search-6.6.2/asf_search/ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/ASFSearchOptions/ASFSearchOptions.py` & `asf_search-6.6.2/asf_search/ASFSearchOptions/ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/ASFSearchOptions/validator_map.py` & `asf_search-6.6.2/asf_search/ASFSearchOptions/validator_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/ASFSearchOptions/validators.py` & `asf_search-6.6.2/asf_search/ASFSearchOptions/validators.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/ASFSearchResults.py` & `asf_search-6.6.2/asf_search/ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/ASFSession.py` & `asf_search-6.6.2/asf_search/ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/CMR/MissionList.py` & `asf_search-6.6.2/asf_search/CMR/MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/CMR/field_map.py` & `asf_search-6.6.2/asf_search/CMR/field_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/CMR/subquery.py` & `asf_search-6.6.2/asf_search/CMR/subquery.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/CMR/translate.py` & `asf_search-6.6.2/asf_search/CMR/translate.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/WKT/validate_wkt.py` & `asf_search-6.6.2/asf_search/WKT/validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/__init__.py` & `asf_search-6.6.2/asf_search/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/baseline/calc.py` & `asf_search-6.6.2/asf_search/baseline/calc.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/baseline/stack.py` & `asf_search-6.6.2/asf_search/baseline/stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/constants/BEAMMODE.py` & `asf_search-6.6.2/asf_search/constants/BEAMMODE.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/constants/INTERNAL.py` & `asf_search-6.6.2/asf_search/constants/INTERNAL.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/constants/PRODUCT_TYPE.py` & `asf_search-6.6.2/asf_search/constants/PRODUCT_TYPE.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/download/download.py` & `asf_search-6.6.2/asf_search/download/download.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/exceptions.py` & `asf_search-6.6.2/asf_search/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,7 +33,10 @@
     """Raise when wkt related errors occur"""
 
 class CMRError(Exception):
     """Base CMR Exception"""
 
 class CMRConceptIDError(CMRError):
     """Raise when CMR encounters a concept-id error"""
+
+class CMRIncompleteError(CMRError):
+    """Raise when CMR returns an incomplete page of results"""
```

### Comparing `asf_search-6.6.1/asf_search/export/csv.py` & `asf_search-6.6.2/asf_search/export/csv.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/export/export_translators.py` & `asf_search-6.6.2/asf_search/export/export_translators.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/export/geojson.py` & `asf_search-6.6.2/asf_search/export/geojson.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/export/jsonlite.py` & `asf_search-6.6.2/asf_search/export/jsonlite.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/export/jsonlite2.py` & `asf_search-6.6.2/asf_search/export/jsonlite2.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/export/kml.py` & `asf_search-6.6.2/asf_search/export/kml.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/export/metalink.py` & `asf_search-6.6.2/asf_search/export/metalink.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/health/health.py` & `asf_search-6.6.2/asf_search/health/health.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/baseline_search.py` & `asf_search-6.6.2/asf_search/search/baseline_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     stack, warnings = get_baseline_from_stack(reference=reference, stack=stack)
     stack.searchComplete = is_complete # preserve final outcome of earlier search()
 
     stack.sort(key=lambda product: product.properties['temporalBaseline'])
 
     return stack
 
+
 def stack_from_id(
         reference_id: str,
         opts: ASFSearchOptions = None
 ) -> ASFSearchResults:
     """
     Finds a baseline stack from a reference product ID
 
@@ -56,16 +57,19 @@
     :param opts: An ASFSearchOptions object describing the search parameters to be used. Search parameters specified outside this object will override in event of a conflict.
 
     :return: ASFSearchResults(list) of search results
     """
 
     opts = (ASFSearchOptions() if opts is None else copy(opts))
 
-    reference_results = product_search(product_list=reference_id, opts=opts)
 
+    reference_results = product_search(product_list=reference_id, opts=opts)
+    
+    reference_results.raise_if_incomplete()
+    
     if len(reference_results) <= 0:
         raise ASFSearchError(f'Reference product not found: {reference_id}')
     reference = reference_results[0]
 
     return stack_from_product(reference, opts=opts)
```

### Comparing `asf_search-6.6.1/asf_search/search/campaigns.py` & `asf_search-6.6.2/asf_search/search/campaigns.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/error_reporting.py` & `asf_search-6.6.2/asf_search/search/error_reporting.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/geo_search.py` & `asf_search-6.6.2/asf_search/search/geo_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/granule_search.py` & `asf_search-6.6.2/asf_search/search/granule_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/product_search.py` & `asf_search-6.6.2/asf_search/search/product_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/search.py` & `asf_search-6.6.2/asf_search/search/search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/asf_search/search/search_count.py` & `asf_search-6.6.2/asf_search/search/search_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 
     count = 0
     for query in build_subqueries(opts):
         translated_opts = translate_opts(query)
         idx = translated_opts.index(('page_size', INTERNAL.CMR_PAGE_SIZE))
         translated_opts[idx] = ('page_size', 0)
         
-        response = get_page(session=opts.session, url=url, translated_opts=translated_opts, search_opts=query)
+        response = get_page(session=opts.session, url=url, translated_opts=translated_opts)
         count += response.json()['hits']
     return count
```

### Comparing `asf_search-6.6.1/asf_search/search/search_generator.py` & `asf_search-6.6.2/asf_search/search/search_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from typing import Generator, Union, Iterable, Tuple
 from copy import copy
 from requests.exceptions import HTTPError
 from requests import ReadTimeout, Response
-from tenacity import retry, retry_if_exception_type, stop_after_delay, wait_exponential
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_exponential, wait_fixed
 import datetime
 import dateparser
 import warnings
 
 from asf_search import __version__
 
 from asf_search.ASFSearchResults import ASFSearchResults
 from asf_search.ASFSearchOptions import ASFSearchOptions
 from asf_search.CMR import build_subqueries, translate_opts
 from asf_search.ASFSession import ASFSession
 from asf_search.ASFProduct import ASFProduct
-from asf_search.exceptions import ASFSearch4xxError, ASFSearch5xxError, ASFSearchError
+from asf_search.exceptions import ASFSearch4xxError, ASFSearch5xxError, ASFSearchError, CMRIncompleteError
 from asf_search.constants import INTERNAL
 from asf_search.WKT.validate_wkt import validate_wkt
 from asf_search.search.error_reporting import report_search_error
 
 
 def search_generator(        
         absoluteOrbit: Union[int, Tuple[int, int], Iterable[Union[int, Tuple[int, int]]]] = None,
@@ -74,86 +74,83 @@
     if maxResults is not None and \
         (getattr(opts, 'granule_list', False) or getattr(opts, 'product_list', False)):
             raise ValueError("Cannot use maxResults along with product_list/granule_list.")
 
     preprocess_opts(opts)
 
     url = '/'.join(s.strip('/') for s in [f'https://{opts.host}', f'{INTERNAL.CMR_GRANULE_PATH}'])
-    count = 0
+    total = 0
     
-    for query in build_subqueries(opts):
+    queries = build_subqueries(opts)
+    for query in queries:
         translated_opts = translate_opts(query)
-        try:
-            response = get_page(session=opts.session, url=url, translated_opts=translated_opts, search_opts=query)
-        except ASFSearchError as e:
-            message = str(e)
-            logging.error(message)
-            report_search_error(query, message)
-            opts.session.headers.pop('CMR-Search-After', None)
-            return
-
-        hits = [ASFProduct(f, session=query.session) for f in response.json()['items']]
-
-        if 'CMR-Search-After' in response.headers:
-            opts.session.headers.update({'CMR-Search-After': response.headers['CMR-Search-After']})
-
-        if maxResults != None:
-            last_page = ASFSearchResults(hits[:min(maxResults - count, len(hits))], opts=opts)
-            count += len(last_page)
-            
-            if count == maxResults:
-                last_page.searchComplete = True
-                yield last_page
-                return
-            else:
-                yield last_page
-        else:
-            count += len(hits)
-            yield ASFSearchResults(hits, opts=opts)
-
-        while('CMR-Search-After' in response.headers):
-            opts.session.headers.update({'CMR-Search-After': response.headers['CMR-Search-After']})
-
+        cmr_search_after_header = ""
+        subquery_count = 0
+        
+        while(cmr_search_after_header is not None):
             try:
-                response = get_page(session=opts.session, url=url, translated_opts=translated_opts, search_opts=query)
-            except ASFSearchError as e:
+                items, subquery_max_results, cmr_search_after_header = query_cmr(opts.session, url, translated_opts, subquery_count)
+            except (ASFSearchError, CMRIncompleteError) as e:
                 message = str(e)
                 logging.error(message)
                 report_search_error(query, message)
                 opts.session.headers.pop('CMR-Search-After', None)
                 return
+            
+            opts.session.headers.update({'CMR-Search-After': cmr_search_after_header})
+            last_page = process_page(items, maxResults, subquery_max_results, total, subquery_count, opts)
+            subquery_count += len(last_page)
+            total += len(last_page)
+            last_page.searchComplete = subquery_count == subquery_max_results or total == maxResults
+            yield last_page
+            
+            if last_page.searchComplete:
+                if total == maxResults: # the user has as many results as they wanted
+                    opts.session.headers.pop('CMR-Search-After', None)
+                    return
+                else: # or we've gotten all possible results for this subquery
+                    cmr_search_after_header = None
+        
+        opts.session.headers.pop('CMR-Search-After', None)
 
-            hits = [ASFProduct(f, session=query.session) for f in response.json()['items']]
 
-            if len(hits):
-                if maxResults != None:
-                    last_page = ASFSearchResults(hits[:min(maxResults - count, len(hits))], opts=opts)
-                    count += len(last_page)
-                    # results.extend(hits[:min(maxResults - len(results), len(hits))])
-                    if count == maxResults:
-                        last_page.searchComplete = True
-                        yield last_page
-                        return
-                    else:
-                        yield last_page
-                else:
-                    count += len(hits)
-                    yield ASFSearchResults(hits, opts=opts)
+@retry(reraise=True,
+       retry=retry_if_exception_type(CMRIncompleteError),
+       wait=wait_fixed(2),
+       stop=stop_after_attempt(3),
+    )
+def query_cmr(session: ASFSession, url: str, translated_opts: dict, sub_query_count: int):
+    response = get_page(session=session, url=url, translated_opts=translated_opts)
 
-        opts.session.headers.pop('CMR-Search-After', None)
+    items = [ASFProduct(f, session=session) for f in response.json()['items']]
+    hits: int = response.json()['hits'] # total count of products given search opts
+
+    # sometimes CMR returns results with the wrong page size
+    if len(items) != INTERNAL.CMR_PAGE_SIZE and len(items) + sub_query_count < hits:
+        raise CMRIncompleteError(f"CMR returned page of incomplete results. Expected {min(INTERNAL.CMR_PAGE_SIZE, hits - sub_query_count)} results, got {len(items)}")
+
+    return items, hits, response.headers.get('CMR-Search-After', None)
+    
+
+def process_page(items: list[ASFProduct], max_results: int, subquery_max_results: int, total: int, subquery_count: int, opts: ASFSearchOptions):
+    if max_results is None:
+        last_page = ASFSearchResults(items[:min(subquery_max_results - subquery_count, len(items))], opts=opts)
+    else:
+        last_page = ASFSearchResults(items[:min(max_results - total, len(items))], opts=opts)
+    return last_page
 
 
 @retry(reraise=True,
-       retry=retry_if_exception_type((TimeoutError, ASFSearch5xxError)),
-       wait=wait_exponential(multiplier=1, min=4, max=10),
-       stop=stop_after_delay(340),
+       retry=retry_if_exception_type(ASFSearch5xxError),
+       wait=wait_exponential(multiplier=1, min=3, max=10),  # Wait 2^x * 1 starting with 3 seconds, max 10 seconds between retries
+       stop=stop_after_attempt(3),
     )
-def get_page(session: ASFSession, url: str, translated_opts: list, search_opts: ASFSearchOptions) -> Response:
+def get_page(session: ASFSession, url: str, translated_opts: list) -> Response:
     try:
-        response = session.post(url=url, data=translated_opts, timeout=170)
+        response = session.post(url=url, data=translated_opts, timeout=30)
         response.raise_for_status()
     except HTTPError as exc:
         error_message = f'HTTP {response.status_code}: {response.json()["errors"]}'
         if 400 <= response.status_code <= 499:
             raise ASFSearch4xxError(error_message) from exc
         if 500 <= response.status_code <= 599:
             raise ASFSearch5xxError(error_message) from exc
```

### Comparing `asf_search-6.6.1/asf_search.egg-info/PKG-INFO` & `asf_search-6.6.2/asf_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf-search
-Version: 6.6.1
+Version: 6.6.2
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `asf_search-6.6.1/asf_search.egg-info/SOURCES.txt` & `asf_search-6.6.2/asf_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/0-Intro.md` & `asf_search-6.6.2/examples/0-Intro.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/1-Basic_Overview.ipynb` & `asf_search-6.6.2/examples/1-Basic_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/2-Geographic_Search.ipynb` & `asf_search-6.6.2/examples/2-Geographic_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/3-Granule_Search.ipynb` & `asf_search-6.6.2/examples/3-Granule_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/4-Baseline_Search.ipynb` & `asf_search-6.6.2/examples/4-Baseline_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/5-Download.ipynb` & `asf_search-6.6.2/examples/5-Download.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/6-Outro.md` & `asf_search-6.6.2/examples/6-Outro.md`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/examples/hello_world.py` & `asf_search-6.6.2/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/setup.py` & `asf_search-6.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/ASFProduct/test_ASFProduct.py` & `asf_search-6.6.2/tests/ASFProduct/test_ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/ASFSearchOptions/test_ASFSearchOptions.py` & `asf_search-6.6.2/tests/ASFSearchOptions/test_ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/ASFSearchResults/test_ASFSearchResults.py` & `asf_search-6.6.2/tests/ASFSearchResults/test_ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/ASFSession/test_ASFSession.py` & `asf_search-6.6.2/tests/ASFSession/test_ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/BaselineSearch/Stack/test_stack.py` & `asf_search-6.6.2/tests/BaselineSearch/Stack/test_stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/BaselineSearch/test_baseline_search.py` & `asf_search-6.6.2/tests/BaselineSearch/test_baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/CMR/test_MissionList.py` & `asf_search-6.6.2/tests/CMR/test_MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/Search/test_search.py` & `asf_search-6.6.2/tests/Search/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         assert(feature.geojson()['geometry'] == search_resp[idx]['geometry'])
         for key, item in feature.geojson()['properties'].items():
             assert(item == search_resp[idx]['properties'][key])
 
 def run_test_search(search_parameters, answer):
     with requests_mock.Mocker() as m:
-        m.post(f"https://{INTERNAL.CMR_HOST}{INTERNAL.CMR_GRANULE_PATH}", json={'items': answer})
+        m.post(f"https://{INTERNAL.CMR_HOST}{INTERNAL.CMR_GRANULE_PATH}", json={'items': answer, 'hits': len(answer)})
         response = search(**search_parameters)
 
         if search_parameters.get("maxResults", False):
             assert(len(response) == search_parameters["maxResults"])
 
         assert(len(response) == len(answer))
         # assert(response.geojson()["features"] == answer)
```

### Comparing `asf_search-6.6.1/tests/Search/test_search_generator.py` & `asf_search-6.6.2/tests/Search/test_search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/Serialization/test_serialization.py` & `asf_search-6.6.2/tests/Serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/WKT/test_validate_wkt.py` & `asf_search-6.6.2/tests/WKT/test_validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/download/test_download.py` & `asf_search-6.6.2/tests/download/test_download.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/pytest-config.yml` & `asf_search-6.6.2/tests/pytest-config.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/pytest-managers.py` & `asf_search-6.6.2/tests/pytest-managers.py`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Alos_response.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Alos_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Alos_response_maxResults3.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Alos_response_missing_baseline.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_L1.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_L1.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.csv` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.csv`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.kml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.kml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.metalink`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_ers_reference.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Fairbanks_ers_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/S1_baseline_stack.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/S1_baseline_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/S1_response.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/S1_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/SLC_BURST.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/SLC_BURST_stack.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/SLC_BURST_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/SMAP_response.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/SMAP_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/ShorelineMask26.shp` & `asf_search-6.6.2/tests/yml_tests/Resources/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml` & `asf_search-6.6.2/tests/yml_tests/Resources/Shovel_Creek_many_points.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_ASFProduct.yml` & `asf_search-6.6.2/tests/yml_tests/test_ASFProduct.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_ASFSearchOptions.yml` & `asf_search-6.6.2/tests/yml_tests/test_ASFSearchOptions.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_ASFSearchResults.yml` & `asf_search-6.6.2/tests/yml_tests/test_ASFSearchResults.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_ASFSession.yml` & `asf_search-6.6.2/tests/yml_tests/test_ASFSession.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_baseline_search.yml` & `asf_search-6.6.2/tests/yml_tests/test_baseline_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_download.yml` & `asf_search-6.6.2/tests/yml_tests/test_download.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_search.yml` & `asf_search-6.6.2/tests/yml_tests/test_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_serialization.yml` & `asf_search-6.6.2/tests/yml_tests/test_serialization.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_stack.yml` & `asf_search-6.6.2/tests/yml_tests/test_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-6.6.1/tests/yml_tests/test_validate_wkt.yml` & `asf_search-6.6.2/tests/yml_tests/test_validate_wkt.yml`

 * *Files identical despite different names*


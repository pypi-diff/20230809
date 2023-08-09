# Comparing `tmp/hdx_python_scraper-2.1.7.tar.gz` & `tmp/hdx_python_scraper-2.1.8.tar.gz`

## Comparing `hdx_python_scraper-2.1.7.tar` & `hdx_python_scraper-2.1.8.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     5635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    62577 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/documentation/main.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/_version.py
--rw-r--r--   0        0        0    14130 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/base_scraper.py
--rw-r--r--   0        0        0    46946 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/__init__.py
--rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/aggregator.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/resource_downloader.py
--rwxr-xr-x   0        0        0    14635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/rowparser.py
--rw-r--r--   0        0        0    20217 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/scraper.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/timeseries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/__init__.py
--rwxr-xr-x   0        0        0     2566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/base.py
--rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/excelfile.py
--rwxr-xr-x   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/googlesheets.py
--rwxr-xr-x   0        0        0     9498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/json.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/__init__.py
--rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/fallbacks.py
--rw-r--r--   0        0        0    16403 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/reader.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/region_lookup.py
--rw-r--r--   0        0        0    11204 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/sources.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/writer.py
--rwxr-xr-x   0        0        0    63512 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/config/project_configuration.yaml
--rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/additional-json.json
--rw-r--r--   0        0        0    57147 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv
--rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cbpf-allocations-and-contributions.json
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cbpf2-allocations-and-contributions.json
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf-covid-19-allocations.json
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf2-covid-19-allocations.json
--rw-r--r--   0        0        0  8415576 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv
--rw-r--r--   0        0        0  8415576 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
--rw-r--r--   0        0        0   201089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/covidtests_data-owid-covid-data.xlsx
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-nutrition.csv
--rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/education_closures_download-covid-impact-education.csv
--rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-drought-related-key-figures.json
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/fallbacks.json
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/global-school-closures-covid19.json
--rw-r--r--   0        0        0    78566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idmc-internally-displaced-persons-idps.json
--rw-r--r--   0        0        0    51259 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idps_download-displacement-data.csv
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
--rw-r--r--   0        0        0  1371019 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/kenya-drought-related-key-figures.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/population.json
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx
--rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/sadd-countries-to-include.csv
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv
--rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/sahel-humanitarian-needs-overview.json
--rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-acute-food-insecurity-country-data.json
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-drought-related-key-figures.json
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-internally-displaced-persons-idps.json
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json
--rwxr-xr-x   0        0        0     5328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_output.xlsx
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_scraper_all.json
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_scraper_other.json
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/test_scraper_population.json
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/total-covid-19-tests-performed-by-country.json
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ukraine-border-crossings.json
--rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/ukraine-who-does-what-where-3w.json
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/unocha-office-locations.json
--rwxr-xr-x   0        0        0    21332 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/who_national2_who-covid-19-global-data.csv
--rwxr-xr-x   0        0        0    21332 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/who_national_who-covid-19-global-data.csv
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/whowhatwhere_afg_3w_data.csv
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/fixtures/whowhatwhere_notags_3w_data.csv
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/__init__.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/affected_targeted_reached.py
--rwxr-xr-x   0        0        0     4631 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/conftest.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/education_closures.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/education_enrolment.py
--rwxr-xr-x   0        0        0     7256 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_output.py
--rwxr-xr-x   0        0        0     8566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_readers.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_regionlookup.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_runner_get_results.py
--rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_aggregation.py
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_appenddata.py
--rw-r--r--   0        0        0    34104 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_custom.py
--rwxr-xr-x   0        0        0    25502 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_global.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_multipleurls.py
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_national.py
--rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_resource_downloaders.py
--rw-r--r--   0        0        0    17601 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_subnational.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_timeseries.py
--rw-r--r--   0        0        0     8096 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_sources.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/test_utils.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/tests/hdx/scraper/unhcr_myanmar_idps.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/LICENSE
--rwxr-xr-x   0        0        0     1711 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/README.md
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     5760 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    62577 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/documentation/main.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/_version.py
+-rw-r--r--   0        0        0    14130 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/base_scraper.py
+-rw-r--r--   0        0        0    46946 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/__init__.py
+-rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/aggregator.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/resource_downloader.py
+-rwxr-xr-x   0        0        0    14635 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/rowparser.py
+-rw-r--r--   0        0        0    20217 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/scraper.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/timeseries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/__init__.py
+-rwxr-xr-x   0        0        0     2566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/base.py
+-rwxr-xr-x   0        0        0     2197 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/excelfile.py
+-rwxr-xr-x   0        0        0     3087 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/googlesheets.py
+-rwxr-xr-x   0        0        0     9498 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/json.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/__init__.py
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/fallbacks.py
+-rw-r--r--   0        0        0    16403 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/reader.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/region_lookup.py
+-rw-r--r--   0        0        0    11204 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/sources.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/writer.py
+-rwxr-xr-x   0        0        0    63512 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/additional-json.json
+-rw-r--r--   0        0        0    57147 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/cbpf-allocations-and-contributions.json
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/cbpf2-allocations-and-contributions.json
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/cerf-covid-19-allocations.json
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/cerf2-covid-19-allocations.json
+-rw-r--r--   0        0        0  8415576 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0        0        0  8415576 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv
+-rw-r--r--   0        0        0   201089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/covidtests_data-owid-covid-data.xlsx
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/download-hno-2017-sahel-nutrition.csv
+-rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/education_closures_download-covid-impact-education.csv
+-rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ethiopia-drought-related-key-figures.json
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/fallbacks.json
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/global-school-closures-covid19.json
+-rw-r--r--   0        0        0    78566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/idmc-internally-displaced-persons-idps.json
+-rw-r--r--   0        0        0    51259 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/idps_download-displacement-data.csv
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json
+-rw-r--r--   0        0        0  1371019 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/kenya-drought-related-key-figures.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0   985584 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/population.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx
+-rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/sadd-countries-to-include.csv
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/sahel-humanitarian-needs-overview.json
+-rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/somalia-acute-food-insecurity-country-data.json
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/somalia-drought-related-key-figures.json
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/somalia-internally-displaced-persons-idps.json
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json
+-rwxr-xr-x   0        0        0     5328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/test_output.xlsx
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/test_scraper_all.json
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/test_scraper_other.json
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/test_scraper_population.json
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/total-covid-19-tests-performed-by-country.json
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ukraine-border-crossings.json
+-rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/ukraine-who-does-what-where-3w.json
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/unocha-office-locations.json
+-rwxr-xr-x   0        0        0    21332 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/who_national2_who-covid-19-global-data.csv
+-rwxr-xr-x   0        0        0    21332 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/who_national_who-covid-19-global-data.csv
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/whowhatwhere_afg_3w_data.csv
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/fixtures/whowhatwhere_notags_3w_data.csv
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/__init__.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/affected_targeted_reached.py
+-rwxr-xr-x   0        0        0     4631 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/conftest.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/education_closures.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/education_enrolment.py
+-rwxr-xr-x   0        0        0     7256 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_output.py
+-rwxr-xr-x   0        0        0     8566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_readers.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_regionlookup.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_runner_get_results.py
+-rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_aggregation.py
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_appenddata.py
+-rw-r--r--   0        0        0    34104 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_custom.py
+-rwxr-xr-x   0        0        0    25502 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_global.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_multipleurls.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_national.py
+-rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_regionaltoplevel.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_resource_downloaders.py
+-rw-r--r--   0        0        0    17601 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_subnational.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_timeseries.py
+-rw-r--r--   0        0        0     8096 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_sources.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/test_utils.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/tests/hdx/scraper/unhcr_myanmar_idps.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/LICENSE
+-rwxr-xr-x   0        0        0     1711 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/README.md
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 hdx_python_scraper-2.1.8/PKG-INFO
```

### Comparing `hdx_python_scraper-2.1.7/CONTRIBUTING.md` & `hdx_python_scraper-2.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/requirements.txt` & `hdx_python_scraper-2.1.8/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,91 @@
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
 cachetools==5.3.1
     # via google-auth
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
     # via hdx-python-api
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
     # via hdx-python-api
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
     # via hdx-python-api
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
-frictionless==5.13.1
+frictionless==5.15.10
     # via hdx-python-utilities
-google-auth==2.21.0
+google-auth==2.22.0
     # via
     #   google-auth-oauthlib
     #   gspread
 google-auth-oauthlib==1.0.0
     # via gspread
-gspread==5.9.0
+gspread==5.10.0
     # via hdx-python-scraper (pyproject.toml)
-hdx-python-api==6.0.4
+hdx-python-api==6.0.8
     # via hdx-python-scraper (pyproject.toml)
-hdx-python-country==3.5.1
+hdx-python-country==3.5.2
     # via hdx-python-api
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
@@ -91,15 +93,15 @@
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
     # via hdx-python-api
 markdown-it-py==3.0.0
     # via rich
@@ -111,27 +113,27 @@
     # via markdown-it-py
 ndg-httpsclient==0.5.1
     # via hdx-python-api
 nodeenv==1.8.0
     # via pre-commit
 num2words==0.5.12
     # via quantulum3
-numpy==1.25.0
+numpy==1.25.2
     # via pandas
 oauthlib==3.2.2
     # via requests-oauthlib
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==23.1
     # via pytest
-pandas==2.0.2
+pandas==2.0.3
     # via hdx-python-scraper (pyproject.toml)
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
@@ -145,19 +147,21 @@
     #   ndg-httpsclient
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.3.0
     # via google-auth
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
     #   hdx-python-api
     #   ndg-httpsclient
 pyphonetics==0.5.3
     # via hdx-python-country
@@ -180,39 +184,39 @@
     # via libhxl
 python-slugify==8.0.1
     # via
     #   ckanapi
     #   frictionless
 pytz==2023.3
     # via pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 quantulum3==0.9.0
     # via hdx-python-api
 ratelimit==2.2.1
     # via hdx-python-utilities
-regex==2023.6.3
+regex==2023.8.8
     # via hdx-python-scraper (pyproject.toml)
 requests==2.31.0
     # via
     #   ckanapi
     #   frictionless
     #   libhxl
     #   requests-file
     #   requests-oauthlib
 requests-file==1.5.1
     # via hdx-python-utilities
 requests-oauthlib==1.3.1
     # via google-auth-oauthlib
 rfc3986==2.0.0
     # via frictionless
-rich==13.4.2
+rich==13.5.2
     # via typer
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.17.32
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
@@ -240,35 +244,37 @@
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
 tzdata==2023.3
     # via pandas
 unidecode==1.3.6
     # via
     #   libhxl
     #   pyphonetics
 urllib3==1.26.16
     # via
     #   google-auth
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

### Comparing `hdx_python_scraper-2.1.7/.config/pre-commit-config.yaml` & `hdx_python_scraper-2.1.8/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/.github/workflows/publish.yaml` & `hdx_python_scraper-2.1.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/.github/workflows/run-python-tests.yaml` & `hdx_python_scraper-2.1.8/.github/workflows/run-python-tests.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # This workflow will install Python dependencies, lint and run tests
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Run tests
 
 on:
+  workflow_dispatch: # add run button in github
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

### Comparing `hdx_python_scraper-2.1.7/documentation/main.md` & `hdx_python_scraper-2.1.8/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/documentation/pydoc-markdown.yaml` & `hdx_python_scraper-2.1.8/documentation/pydoc-markdown.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.scraper
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Scraper
-    theme: readthedocs
+    theme: mkdocs
     repo_url: "https://github.com/OCHA-DAP/hdx-python-scraper"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-scraper
   pages:
     - title: Home
```

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/base_scraper.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/base_scraper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/runner.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/runner.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/aggregator.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/aggregator.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/resource_downloader.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/rowparser.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/rowparser.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/scraper.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/scraper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/configurable/timeseries.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/configurable/timeseries.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/base.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/base.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/excelfile.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/excelfile.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/googlesheets.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/googlesheets.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/outputs/json.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/outputs/json.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/__init__.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/fallbacks.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/fallbacks.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/reader.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/reader.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/region_lookup.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/region_lookup.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/sources.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/sources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/src/hdx/scraper/utilities/writer.py` & `hdx_python_scraper-2.1.8/src/hdx/scraper/utilities/writer.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/config/project_configuration.yaml` & `hdx_python_scraper-2.1.8/tests/config/project_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/access_2pacx-1vrszjzuyvt9i-mkrq2hbxrul2lx2vihkthqm-lae8nyhqty70zqtcufs3pxbhzgat1l2bkoa4-daoap-pub-gid-574237756-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/affected_targeted_reached_affected_targeted_reached_eth_ethiopia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/affected_targeted_reached_affected_targeted_reached_ken_kenya_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/affected_targeted_reached_affected_targeted_reached_som_somalia_drought_affected_targeted_reached_by_cluster.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/altworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/cbpf-allocations-and-contributions.json` & `hdx_python_scraper-2.1.8/tests/fixtures/cbpf-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/cbpf2-allocations-and-contributions.json` & `hdx_python_scraper-2.1.8/tests/fixtures/cbpf2-allocations-and-contributions.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/cerf-covid-19-allocations.json` & `hdx_python_scraper-2.1.8/tests/fixtures/cerf-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/cerf2-covid-19-allocations.json` & `hdx_python_scraper-2.1.8/tests/fixtures/cerf2-covid-19-allocations.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/cerf2_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/cerf_global_download-full-pfmb-allocations.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/covax_2pacx-1vtvzu79pptfaa2syevoqfyrrjy63djwitqu0ffbxiqczoun9k9timwmrvfgg1rbsnlmgyugzseiaye2-pub-gid-992438980-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/covidtests_data-owid-covid-data.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/covidtests_data-owid-covid-data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-nutrition.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/download-hno-2017-sahel-nutrition.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/download-hno-2017-sahel-people-in-need.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/education_enrolment_download-countries-enrollment-data-uis-feb-22.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-drought-related-key-figures.json` & `hdx_python_scraper-2.1.8/tests/fixtures/ethiopia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.1.8/tests/fixtures/ethiopia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/fallbacks.json` & `hdx_python_scraper-2.1.8/tests/fixtures/fallbacks.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/gam_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/gam_other_download-unicef-who-wb-global-expanded-databases-severe-wasting.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/global-school-closures-covid19.json` & `hdx_python_scraper-2.1.8/tests/fixtures/global-school-closures-covid19.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/hdx_resource_downloader_xlsx_ukr_border_crossings_090622.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/idmc-internally-displaced-persons-idps.json` & `hdx_python_scraper-2.1.8/tests/fixtures/idmc-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/idps_download-displacement-data.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/idps_download-displacement-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json` & `hdx_python_scraper-2.1.8/tests/fixtures/idps_override_population-widget-id-264111-geo-id-693-population-group-54074999.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/idps_somalia_download-som-unhcr-prmn-displacement-dataset.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/ipc_somalia_download-som-food-insecurity-oct-dec2022-projection.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/kenya-drought-related-key-figures.json` & `hdx_python_scraper-2.1.8/tests/fixtures/kenya-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.1.8/tests/fixtures/kenya-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/key_figures_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/key_figures_eth_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-2015311116-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/key_figures_ken_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-1275038715-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/key_figures_som_2pacx-1vrppqx8jtkkkrckmzfncmmtfecvcpkbp9pdhs1sqtuyacmbsx8tlaxpgblfce-lcehukregguxja-4s-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/ourworldindata_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/ourworldindata_other_data-tagger-match-all-on-tagger-01-header-location-tagger-01-tag.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/population.json` & `hdx_python_scraper-2.1.8/tests/fixtures/population.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx_python_scraper-2.1.8/tests/fixtures/population_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls` & `hdx_python_scraper-2.1.8/tests/fixtures/population_other_indicator-sp-pop-downloadformat-excel-dataformat-list-totl.xls`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/regions_download-tbl-regcov-2020-ocha.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/sadd_covid-data-dataset-fullvars-extype-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/sahel-humanitarian-needs-overview.json` & `hdx_python_scraper-2.1.8/tests/fixtures/sahel-humanitarian-needs-overview.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/somalia-acute-food-insecurity-country-data.json` & `hdx_python_scraper-2.1.8/tests/fixtures/somalia-acute-food-insecurity-country-data.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/somalia-drought-related-key-figures.json` & `hdx_python_scraper-2.1.8/tests/fixtures/somalia-drought-related-key-figures.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/somalia-internally-displaced-persons-idps.json` & `hdx_python_scraper-2.1.8/tests/fixtures/somalia-internally-displaced-persons-idps.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json` & `hdx_python_scraper-2.1.8/tests/fixtures/somalia-pin-targeted-reached-by-location-and-cluster.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/test_output.xlsx` & `hdx_python_scraper-2.1.8/tests/fixtures/test_output.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/timeseries_casualties_2pacx-1vqidedbzz0ehrc0b4fswip14r7mdtu1mpmwakuxupelsah2awcurkgalfduhjvyjul8vzzat3r1b5qg-pub-gid-0-single-true-output-csv.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/total-covid-19-tests-performed-by-country.json` & `hdx_python_scraper-2.1.8/tests/fixtures/total-covid-19-tests-performed-by-country.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ukraine-border-crossings.json` & `hdx_python_scraper-2.1.8/tests/fixtures/ukraine-border-crossings.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/ukraine-who-does-what-where-3w.json` & `hdx_python_scraper-2.1.8/tests/fixtures/ukraine-who-does-what-where-3w.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/unocha-office-locations.json` & `hdx_python_scraper-2.1.8/tests/fixtures/unocha-office-locations.json`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/who_national2_who-covid-19-global-data.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/who_national2_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/who_national_who-covid-19-global-data.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/who_national_who-covid-19-global-data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/fixtures/whowhatwhere_afg_3w_data.csv` & `hdx_python_scraper-2.1.8/tests/fixtures/whowhatwhere_afg_3w_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/__init__.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/affected_targeted_reached.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/affected_targeted_reached.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/conftest.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/education_closures.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/education_closures.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/education_enrolment.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/education_enrolment.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_output.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_output.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_readers.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_readers.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_regionlookup.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_regionlookup.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_runner_get_results.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_runner_get_results.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_aggregation.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_aggregation.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_appenddata.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_appenddata.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_custom.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_custom.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_global.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_global.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_multipleurls.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_multipleurls.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_national.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_national.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_regionaltoplevel.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_regionaltoplevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_resource_downloaders.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_resource_downloaders.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_subnational.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_subnational.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_scrapers_timeseries.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_scrapers_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/test_sources.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/test_sources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/tests/hdx/scraper/unhcr_myanmar_idps.py` & `hdx_python_scraper-2.1.8/tests/hdx/scraper/unhcr_myanmar_idps.py`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/.gitignore` & `hdx_python_scraper-2.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/LICENSE` & `hdx_python_scraper-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/README.md` & `hdx_python_scraper-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_scraper-2.1.7/pyproject.toml` & `hdx_python_scraper-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,29 +30,29 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "hdx-python-api >= 6.0.4",
+    "hdx-python-api >= 6.0.8",
     "gspread",
     "regex",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/OCHA-DAP/hdx-python-scraper"
 
 [project.optional-dependencies]
-pandas = ["pandas>=2.0.2"]
+pandas = ["pandas>=2.0.3"]
 test = ["pytest", "pytest-cov"]
 dev = ["pre-commit"]
 
 
 #########
 # Hatch #
 #########
```

### Comparing `hdx_python_scraper-2.1.7/PKG-INFO` & `hdx_python_scraper-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-scraper
-Version: 2.1.7
+Version: 2.1.8
 Summary: HDX Python scraper utilities to assemble data from multiple sources
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-scraper
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,data assembly,data transformation,scrapers,tabular data
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,20 +22,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: gspread
-Requires-Dist: hdx-python-api>=6.0.4
+Requires-Dist: hdx-python-api>=6.0.8
 Requires-Dist: regex
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: pandas
-Requires-Dist: pandas>=2.0.2; extra == 'pandas'
+Requires-Dist: pandas>=2.0.3; extra == 'pandas'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-scraper/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-scraper/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-scraper?branch=main)
```


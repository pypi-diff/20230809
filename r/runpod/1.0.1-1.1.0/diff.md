# Comparing `tmp/runpod-1.0.1.tar.gz` & `tmp/runpod-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpod-1.0.1.tar", last modified: Mon Aug  7 03:35:50 2023, max compression
+gzip compressed data, was "runpod-1.1.0.tar", last modified: Tue Aug  8 23:26:08 2023, max compression
```

## Comparing `runpod-1.0.1.tar` & `runpod-1.1.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.169640 runpod-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.149639 runpod-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.149639 runpod-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.149639 runpod-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/workflows/CD-publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/workflows/CD-test_publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/workflows/CI-codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/workflows/CI-pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-07 03:35:28.000000 runpod-1.0.1/.github/workflows/CI-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-07 03:35:28.000000 runpod-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-07 03:35:28.000000 runpod-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-07 03:35:28.000000 runpod-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-07 03:35:50.169640 runpod-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-07 03:35:28.000000 runpod-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-07 03:35:28.000000 runpod-1.0.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.141640 runpod-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.149639 runpod-1.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/api/quries.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.149639 runpod-1.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/images/env_var_location.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.153640 runpod-1.0.1/docs/serverless/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.153640 runpod-1.0.1/docs/serverless/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/functions/error_handling.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/functions/logging.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/local_testing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.153640 runpod-1.0.1/docs/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/utils/rp_cleanup.md
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/utils/rp_debugger.md
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/utils/rp_download.md
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/utils/rp_upload.md
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/utils/rp_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/worker.md
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-07 03:35:28.000000 runpod-1.0.1/docs/serverless/worker_realtime.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.153640 runpod-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-07 03:35:28.000000 runpod-1.0.1/examples/call_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-07 03:35:28.000000 runpod-1.0.1/examples/call_endpoint_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-07 03:35:28.000000 runpod-1.0.1/examples/graphql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 03:35:28.000000 runpod-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 03:35:28.000000 runpod-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.153640 runpod-1.0.1/runpod/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.157640 runpod-1.0.1/runpod/api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/ctl_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.157640 runpod-1.0.1/runpod/api_wrapper/mutations/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/mutations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.157640 runpod-1.0.1/runpod/api_wrapper/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/api_wrapper/queries/gpus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.161640 runpod-1.0.1/runpod/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.161640 runpod-1.0.1/runpod/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.161640 runpod-1.0.1/runpod/endpoint/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/endpoint/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/endpoint/asyncio/asyncio_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/endpoint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.161640 runpod-1.0.1/runpod/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/runpod/serverless/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/rp_tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/modules/worker_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/runpod/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/rp_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/rp_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/rp_debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/rp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/rp_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/utils/rp_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-07 03:35:28.000000 runpod-1.0.1/runpod/serverless/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.157640 runpod-1.0.1/runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-07 03:35:50.000000 runpod-1.0.1/runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-07 03:35:50.000000 runpod-1.0.1/runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:35:50.000000 runpod-1.0.1/runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 03:35:50.000000 runpod-1.0.1/runpod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-07 03:35:50.000000 runpod-1.0.1/runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 03:35:50.000000 runpod-1.0.1/runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-07 03:35:50.169640 runpod-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-07 03:35:28.000000 runpod-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/tests/test_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_api_wrapper/test_ctl_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_api_wrapper/test_mutations_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_cli/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/tests/test_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_endpoint/test_asyncio_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_endpoint/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.165640 runpod-1.0.1/tests/test_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.169640 runpod-1.0.1/tests/test_serverless/test_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_modules/test_tips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:35:50.169640 runpod-1.0.1/tests/test_serverless/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/test_debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_utils/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_serverless/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/test_whatever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 03:35:28.000000 runpod-1.0.1/tests/whatever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.552548 runpod-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/workflows/CD-publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/workflows/CD-test_publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/workflows/CI-codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/workflows/CI-pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-08 23:25:40.000000 runpod-1.1.0/.github/workflows/CI-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-08 23:25:40.000000 runpod-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-08 23:25:40.000000 runpod-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-08 23:25:40.000000 runpod-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-08 23:26:08.552548 runpod-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-08 23:25:40.000000 runpod-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 23:25:40.000000 runpod-1.1.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.528547 runpod-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/api/quries.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/images/env_var_location.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/docs/serverless/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/docs/serverless/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/functions/error_handling.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/functions/logging.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/local_testing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.536547 runpod-1.1.0/docs/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/utils/rp_cleanup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/utils/rp_debugger.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/utils/rp_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/utils/rp_upload.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/utils/rp_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/worker.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 23:25:40.000000 runpod-1.1.0/docs/serverless/worker_realtime.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 23:25:40.000000 runpod-1.1.0/examples/call_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-08 23:25:40.000000 runpod-1.1.0/examples/call_endpoint_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 23:25:40.000000 runpod-1.1.0/examples/graphql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 23:25:40.000000 runpod-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 23:25:40.000000 runpod-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod/api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod/api_wrapper/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/mutations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod/api_wrapper/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/api_wrapper/queries/gpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.544547 runpod-1.1.0/runpod/endpoint/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/endpoint/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/endpoint/asyncio/asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/endpoint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.544547 runpod-1.1.0/runpod/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.544547 runpod-1.1.0/runpod/serverless/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/rp_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/modules/worker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.548547 runpod-1.1.0/runpod/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/rp_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/rp_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/rp_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/rp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/rp_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/utils/rp_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-08 23:25:40.000000 runpod-1.1.0/runpod/serverless/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.540547 runpod-1.1.0/runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-08 23:26:08.000000 runpod-1.1.0/runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-08 23:26:08.000000 runpod-1.1.0/runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:26:08.000000 runpod-1.1.0/runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 23:26:08.000000 runpod-1.1.0/runpod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 23:26:08.000000 runpod-1.1.0/runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 23:26:08.000000 runpod-1.1.0/runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-08 23:26:08.552548 runpod-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-08 23:25:40.000000 runpod-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.548547 runpod-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.548547 runpod-1.1.0/tests/test_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_api_wrapper/test_ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_api_wrapper/test_mutations_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.548547 runpod-1.1.0/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_cli/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.548547 runpod-1.1.0/tests/test_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_endpoint/test_asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_endpoint/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.548547 runpod-1.1.0/tests/test_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.552548 runpod-1.1.0/tests/test_serverless/test_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_modules/test_tips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:26:08.552548 runpod-1.1.0/tests/test_serverless/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/test_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_utils/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_serverless/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/test_whatever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-08 23:25:40.000000 runpod-1.1.0/tests/whatever.py
```

### Comparing `runpod-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `runpod-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `runpod-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/dependabot.yml` & `runpod-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/workflows/CD-publish_to_pypi.yml` & `runpod-1.1.0/.github/workflows/CD-publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/workflows/CD-test_publish_to_pypi.yml` & `runpod-1.1.0/.github/workflows/CD-test_publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/workflows/CI-codeql.yml` & `runpod-1.1.0/.github/workflows/CI-codeql.yml`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/workflows/CI-pylint.yml` & `runpod-1.1.0/.github/workflows/CI-pylint.yml`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.github/workflows/CI-tests.yml` & `runpod-1.1.0/.github/workflows/CI-tests.yml`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/.gitignore` & `runpod-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/CONTRIBUTING.md` & `runpod-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/LICENSE` & `runpod-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/PKG-INFO` & `runpod-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 1.0.1
+Version: 1.1.0
 Summary: 🐍 | Python library for RunPod API and serverless worker SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
```

### Comparing `runpod-1.0.1/README.md` & `runpod-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/api/quries.md` & `runpod-1.1.0/docs/api/quries.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/images/env_var_location.png` & `runpod-1.1.0/docs/images/env_var_location.png`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/functions/error_handling.md` & `runpod-1.1.0/docs/serverless/functions/error_handling.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/functions/logging.md` & `runpod-1.1.0/docs/serverless/functions/logging.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/local_testing.md` & `runpod-1.1.0/docs/serverless/local_testing.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/utils/rp_debugger.md` & `runpod-1.1.0/docs/serverless/utils/rp_debugger.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/utils/rp_download.md` & `runpod-1.1.0/docs/serverless/utils/rp_download.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/utils/rp_upload.md` & `runpod-1.1.0/docs/serverless/utils/rp_upload.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/utils/rp_validator.md` & `runpod-1.1.0/docs/serverless/utils/rp_validator.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/worker.md` & `runpod-1.1.0/docs/serverless/worker.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/docs/serverless/worker_realtime.md` & `runpod-1.1.0/docs/serverless/worker_realtime.md`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/examples/call_endpoint_asyncio.py` & `runpod-1.1.0/examples/call_endpoint_asyncio.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/examples/graphql_wrapper.py` & `runpod-1.1.0/examples/graphql_wrapper.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/__init__.py` & `runpod-1.1.0/runpod/__init__.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/api_wrapper/ctl_commands.py` & `runpod-1.1.0/runpod/api_wrapper/ctl_commands.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/api_wrapper/graphql.py` & `runpod-1.1.0/runpod/api_wrapper/graphql.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/api_wrapper/mutations/pods.py` & `runpod-1.1.0/runpod/api_wrapper/mutations/pods.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/api_wrapper/queries/gpus.py` & `runpod-1.1.0/runpod/api_wrapper/queries/gpus.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/cli/config.py` & `runpod-1.1.0/runpod/cli/config.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/endpoint/asyncio/asyncio_runner.py` & `runpod-1.1.0/runpod/endpoint/asyncio/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/endpoint/runner.py` & `runpod-1.1.0/runpod/endpoint/runner.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/__init__.py` & `runpod-1.1.0/runpod/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/retry.py` & `runpod-1.1.0/runpod/serverless/modules/retry.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_fastapi.py` & `runpod-1.1.0/runpod/serverless/modules/rp_fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import uvicorn
 from fastapi import FastAPI, APIRouter
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 
 from .rp_job import run_job
 from .worker_state import Jobs
-from .rp_ping import HeartbeatSender
+from .rp_ping import Heartbeat
 
 RUNPOD_ENDPOINT_ID = os.environ.get("RUNPOD_ENDPOINT_ID", None)
 
 DESCRIPTION = """
 This API server is provided as a method of testing and debugging your worker locally.
 Additionally, you can use this to test code that will be making requests to your worker.
 
@@ -25,15 +25,15 @@
 ---
 
 *Note: When running your worker on the RunPod platform, this API server will not be used.*
 """
 
 job_list = Jobs()
 
-heartbeat = HeartbeatSender()
+heartbeat = Heartbeat()
 
 
 # ------------------------------- Input Objects ------------------------------ #
 class Job(BaseModel):
     ''' Represents a job. '''
     id: str
     input: dict | list | str | int | float | bool
```

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_http.py` & `runpod-1.1.0/runpod/serverless/modules/rp_http.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_job.py` & `runpod-1.1.0/runpod/serverless/modules/rp_job.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_local.py` & `runpod-1.1.0/runpod/serverless/modules/rp_local.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_logger.py` & `runpod-1.1.0/runpod/serverless/modules/rp_logger.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_ping.py` & `runpod-1.1.0/runpod/serverless/modules/rp_ping.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-"""Enables heartbeats."""
-# pylint: disable=too-few-public-methods
-
+"""
+This module defines the Heartbeat class.
+The heartbeat is responsible for sending periodic pings to the Runpod server.
+"""
 import os
-import asyncio
+import time
+import threading
 
-import aiohttp
+import requests
 
 from runpod.serverless.modules.rp_logger import RunPodLogger
 from .worker_state import Jobs, WORKER_ID
 
-# --------------------------------- Variables -------------------------------- #
-PING_URL = os.environ.get('RUNPOD_WEBHOOK_PING', "PING_NOT_SET")
-PING_URL = PING_URL.replace('$RUNPOD_POD_ID', WORKER_ID)
-PING_INTERVAL = int(os.environ.get('RUNPOD_PING_INTERVAL', 10000))
-
 log = RunPodLogger()
 jobs = Jobs() # Contains the list of jobs that are currently running.
 
 
-class HeartbeatSender:
+class Heartbeat:
     ''' Sends heartbeats to the Runpod server. '''
 
-    _instance = None
+    PING_URL = os.environ.get('RUNPOD_WEBHOOK_PING', "PING_NOT_SET")
+    PING_URL = PING_URL.replace('$RUNPOD_POD_ID', WORKER_ID)
+    PING_INTERVAL = int(os.environ.get('RUNPOD_PING_INTERVAL', 10000))//1000
+
+    _session = requests.Session()
+    _session.headers.update({"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"})
+
+    def start_ping(self, test=False):
+        '''
+        Sends heartbeat pings to the Runpod server.
+        '''
+        if self.PING_URL in ["PING_NOT_SET", None]:
+            log.error("Ping URL not set, cannot start ping.")
+            return
 
-    def __new__(cls):
-        if HeartbeatSender._instance is None:
-            HeartbeatSender._instance = object.__new__(cls)
-        return HeartbeatSender._instance
+        threading.Thread(target=self.ping_loop, daemon=True, args=(test,)).start()
 
-    async def start_ping(self, test=False):
+    def ping_loop(self, test=False):
         '''
         Sends heartbeat pings to the Runpod server.
         '''
         while True:
             try:
-                while True:
-                    await self._send_ping()
-                    await asyncio.sleep(int(PING_INTERVAL / 1000))
-
-                    if test:
-                        return
-            except (aiohttp.ClientError, asyncio.TimeoutError, asyncio.CancelledError) as err:
+                self._send_ping()
+                time.sleep(self.PING_INTERVAL)
+            except requests.RequestException as err:
                 log.error(f"Ping Error: {err}, attempting to restart ping.")
                 if test:
                     return
 
+            if test:
+                return
 
-    async def _send_ping(self):
+    def _send_ping(self):
         '''
         Sends a heartbeat to the Runpod server.
         '''
-        async with aiohttp.ClientSession(
-            headers={"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"} ) as session:
-            job_ids = jobs.get_job_list()
-
-            ping_params = {
-                'job_id': job_ids,
-            } if job_ids is not None else None
-
-            if PING_URL not in [None, 'PING_NOT_SET']:
-                result = await session.get(
-                    PING_URL,
-                    params=ping_params,
-                    timeout=int(PING_INTERVAL / 1000)
-                )
+        job_ids = jobs.get_job_list()
+        ping_params = {'job_id': job_ids} if job_ids is not None else None
+
+        result = self._session.get(
+            self.PING_URL, params=ping_params,
+            timeout=self.PING_INTERVAL
+        )
 
-                log.debug(f"Heartbeat Sent | URL: {PING_URL} | Status: {result.status}")
+        log.debug(f"Heartbeat Sent | URL: {self.PING_URL} | Status: {result.status_code}")
```

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_scale.py` & `runpod-1.1.0/runpod/serverless/modules/rp_scale.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/rp_tips.py` & `runpod-1.1.0/runpod/serverless/modules/rp_tips.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/modules/worker_state.py` & `runpod-1.1.0/runpod/serverless/modules/worker_state.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/utils/rp_cleanup.py` & `runpod-1.1.0/runpod/serverless/utils/rp_cleanup.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/utils/rp_debugger.py` & `runpod-1.1.0/runpod/serverless/utils/rp_debugger.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/utils/rp_download.py` & `runpod-1.1.0/runpod/serverless/utils/rp_download.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/utils/rp_upload.py` & `runpod-1.1.0/runpod/serverless/utils/rp_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/utils/rp_validator.py` & `runpod-1.1.0/runpod/serverless/utils/rp_validator.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/runpod/serverless/worker.py` & `runpod-1.1.0/runpod/serverless/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from typing import Dict, Any
 
 import aiohttp
 
 from runpod.serverless.modules.rp_logger import RunPodLogger
 from runpod.serverless.modules.rp_scale import JobScaler
 from .modules import rp_local
-from .modules.rp_ping import HeartbeatSender
+from .modules.rp_ping import Heartbeat
 from .modules.rp_job import run_job, run_job_generator
 from .modules.rp_http import send_result, stream_result
 from .modules.worker_state import REF_COUNT_ZERO, Jobs
 from .utils import rp_debugger
 
 log = RunPodLogger()
 job_list = Jobs()
-heartbeat = HeartbeatSender()
+heartbeat = Heartbeat()
 
 _TIMEOUT = aiohttp.ClientTimeout(total=300, connect=2, sock_connect=2)
 
 
 def _get_auth_header() -> Dict[str, str]:
     '''
     Returns the authorization header for the worker HTTP requests.
@@ -58,14 +58,16 @@
             connector=connector, headers=_get_auth_header(), timeout=_TIMEOUT) as session:
 
         job_scaler = JobScaler(
             concurrency_controller=config.get('concurrency_controller', None)
         )
 
         while job_scaler.is_alive():
+            heartbeat.start_ping()
+
             async def process_job(job):
                 if inspect.isgeneratorfunction(config["handler"]) \
                     or inspect.isasyncgenfunction(config["handler"]):
                     job_result = run_job_generator(config["handler"], job)
 
                     log.debug("Handler is a generator, streaming results.")
                     async for job_stream in job_result:
@@ -117,15 +119,12 @@
     """
     if _is_local(config):
         asyncio.run(rp_local.run_local(config))
 
     else:
         try:
             work_loop = asyncio.new_event_loop()
-
-            asyncio.ensure_future(heartbeat.start_ping(), loop=work_loop)
             asyncio.ensure_future(run_worker(config), loop=work_loop)
-
             work_loop.run_forever()
 
         finally:
             work_loop.close()
```

### Comparing `runpod-1.0.1/runpod.egg-info/PKG-INFO` & `runpod-1.1.0/runpod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 1.0.1
+Version: 1.1.0
 Summary: 🐍 | Python library for RunPod API and serverless worker SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
```

### Comparing `runpod-1.0.1/runpod.egg-info/SOURCES.txt` & `runpod-1.1.0/runpod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/setup.cfg` & `runpod-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_api_wrapper/test_ctl_commands.py` & `runpod-1.1.0/tests/test_api_wrapper/test_ctl_commands.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_api_wrapper/test_mutations_pods.py` & `runpod-1.1.0/tests/test_api_wrapper/test_mutations_pods.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_cli/test_config.py` & `runpod-1.1.0/tests/test_cli/test_config.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_endpoint/test_asyncio_runner.py` & `runpod-1.1.0/tests/test_endpoint/test_asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_endpoint/test_runner.py` & `runpod-1.1.0/tests/test_endpoint/test_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_fastapi.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_fastapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.handler.return_value = {"result": "success"}
 
     def test_start_serverless_with_realtime(self):
         '''
         Tests the start_serverless() method with the realtime option.
         '''
         module_location = "runpod.serverless.modules.rp_fastapi"
-        with patch(f"{module_location}.HeartbeatSender.start_ping", Mock()) as mock_ping, \
+        with patch(f"{module_location}.Heartbeat.start_ping", Mock()) as mock_ping, \
             patch(f"{module_location}.FastAPI", Mock()) as mock_fastapi, \
             patch(f"{module_location}.APIRouter", return_value=Mock()) as mock_router, \
             patch(f"{module_location}.uvicorn", Mock()) as mock_uvicorn:
 
 
             rp_fastapi.RUNPOD_REALTIME_PORT = '1111'
             rp_fastapi.RUNPOD_ENDPOINT_ID = 'test_endpoint_id'
@@ -50,15 +50,15 @@
     def test_run(self):
         '''
         Tests the _run() method.
         '''
         loop = asyncio.get_event_loop()
 
         module_location = "runpod.serverless.modules.rp_fastapi"
-        with patch(f"{module_location}.HeartbeatSender.start_ping", Mock()) as mock_ping, \
+        with patch(f"{module_location}.Heartbeat.start_ping", Mock()) as mock_ping, \
             patch(f"{module_location}.FastAPI", Mock()), \
             patch(f"{module_location}.APIRouter", return_value=Mock()), \
             patch(f"{module_location}.uvicorn", Mock()):
 
             job_object = rp_fastapi.Job(
                 id="test_job_id",
                 input={"test_input": "test_input"}
```

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_http.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_http.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_job.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_job.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_local.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_local.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_logger.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_logger.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_ping.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_ping.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 ''' Tests for runpod.serverless.modules.rp_ping '''
 
 import os
 import importlib
 
-from unittest import IsolatedAsyncioTestCase
+import unittest
 from unittest.mock import patch, Mock
 
-import pytest
-import aiohttp
+import requests
 from runpod.serverless.modules import rp_ping
 
 class MockResponse: # pylint: disable=too-few-public-methods
     ''' Mock response for aiohttp '''
-    status = 200
+    status_code = 200
 
-async def mock_get(*args, **kwargs): # pylint: disable=unused-argument
+def mock_get(*args, **kwargs): # pylint: disable=unused-argument
     '''
     Mock get function for aiohttp
     '''
     return MockResponse()
 
-class TestPing(IsolatedAsyncioTestCase):
+class TestPing(unittest.TestCase):
     ''' Tests for rp_ping '''
 
     def test_variables(self):
         '''
         Tests that the variables are set correctly
         '''
         os.environ["RUNPOD_WEBHOOK_PING"] = "PING_NOT_SET"
 
         importlib.reload(rp_ping)
 
-        self.assertEqual(rp_ping.PING_URL, "PING_NOT_SET")
-        self.assertEqual(rp_ping.PING_INTERVAL, 10000)
+        self.assertEqual(rp_ping.Heartbeat.PING_URL, "PING_NOT_SET")
+        self.assertEqual(rp_ping.Heartbeat.PING_INTERVAL, 10)
 
         os.environ["RUNPOD_WEBHOOK_PING"] = "https://test.com/ping"
         os.environ["RUNPOD_PING_INTERVAL"] = "20000"
 
         importlib.reload(rp_ping)
 
-        self.assertEqual(rp_ping.PING_URL, "https://test.com/ping")
-        self.assertEqual(rp_ping.PING_INTERVAL, 20000)
+        self.assertEqual(rp_ping.Heartbeat.PING_URL, "https://test.com/ping")
+        self.assertEqual(rp_ping.Heartbeat.PING_INTERVAL, 20)
 
-    @pytest.mark.asyncio
-    @patch("aiohttp.ClientSession.get", side_effect=mock_get)
-    async def test_start_ping(self, mock_get_return):
+    @patch("requests.Session.get", side_effect=mock_get)
+    def test_start_ping(self, mock_get_return):
         '''
         Tests that the start_ping function works correctly
         '''
         os.environ["RUNPOD_WEBHOOK_PING"] = "https://test.com/ping"
 
         importlib.reload(rp_ping)
-        new_ping = rp_ping.HeartbeatSender()
+        new_ping = rp_ping.Heartbeat()
 
         mock_session = Mock()
         mock_session.headers.update = Mock()
 
         # Success case
-        await new_ping.start_ping(test=True)
+        with patch("threading.Thread.start") as mock_thread_start:
+            new_ping.start_ping(test=True)
+            assert mock_thread_start.call_count == 1
 
-        rp_ping.PING_URL = "https://test.com/ping"
+        rp_ping.Heartbeat.PING_URL = "https://test.com/ping"
+        new_ping.ping_loop(test=True)
 
-        self.assertEqual(rp_ping.PING_URL, "https://test.com/ping")
+        self.assertEqual(rp_ping.Heartbeat.PING_URL, "https://test.com/ping")
 
         # Exception case
-        mock_get_return.side_effect = aiohttp.ClientError("Test Error")
+        mock_get_return.side_effect = requests.RequestException("Test Error")
 
         with patch("runpod.serverless.modules.rp_ping.log.error") as mock_log_error:
-            await new_ping.start_ping(test=True)
+            new_ping.ping_loop(test=True)
             assert mock_log_error.call_count == 1
```

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_retry.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_retry.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_state.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_state.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_modules/test_tips.py` & `runpod-1.1.0/tests/test_serverless/test_modules/test_tips.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_utils/test_cleanup.py` & `runpod-1.1.0/tests/test_serverless/test_utils/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_utils/test_cuda.py` & `runpod-1.1.0/tests/test_serverless/test_utils/test_cuda.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_utils/test_debugger.py` & `runpod-1.1.0/tests/test_serverless/test_utils/test_debugger.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_utils/test_download.py` & `runpod-1.1.0/tests/test_serverless/test_utils/test_download.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_utils/test_upload.py` & `runpod-1.1.0/tests/test_serverless/test_utils/test_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_utils/test_validate.py` & `runpod-1.1.0/tests/test_serverless/test_utils/test_validate.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_serverless/test_worker.py` & `runpod-1.1.0/tests/test_serverless/test_worker.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/test_whatever.py` & `runpod-1.1.0/tests/test_whatever.py`

 * *Files identical despite different names*

### Comparing `runpod-1.0.1/tests/whatever.py` & `runpod-1.1.0/tests/whatever.py`

 * *Files identical despite different names*


# Comparing `tmp/pip-tools-7.2.0.tar.gz` & `tmp/pip-tools-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-tools-7.2.0.tar", last modified: Wed Aug  2 23:42:33 2023, max compression
+gzip compressed data, was "pip-tools-7.3.0.tar", last modified: Tue Aug  8 23:40:17 2023, max compression
```

## Comparing `pip-tools-7.2.0.tar` & `pip-tools-7.3.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.github/workflows/reusable-qa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 23:42:09.000000 pip-tools-7.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    43984 2023-08-02 23:42:09.000000 pip-tools-7.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-02 23:42:09.000000 pip-tools-7.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-02 23:42:09.000000 pip-tools-7.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 23:42:09.000000 pip-tools-7.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-08-02 23:42:33.262357 pip-tools-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-08-02 23:42:09.000000 pip-tools-7.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 23:42:09.000000 pip-tools-7.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.242356 pip-tools-7.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/cli/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/cli/pip-compile.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/cli/pip-sync.md
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 23:42:09.000000 pip-tools-7.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/django.in
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/flask.in
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/hypothesis.in
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/protection.in
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 23:42:09.000000 pip-tools-7.2.0/examples/sentry.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-02 23:42:09.000000 pip-tools-7.2.0/img/pip-tools-overview.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.246356 pip-tools-7.2.0/pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 23:42:33.000000 pip-tools-7.2.0/pip_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/_compat/pip_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/repositories/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.250356 pip-tools-7.2.0/piptools/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22721 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/scripts/compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9713 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/scripts/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-08-02 23:42:09.000000 pip-tools-7.2.0/piptools/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-02 23:42:09.000000 pip-tools-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:42:33.262357 pip-tools-7.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.258357 pip-tools-7.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    95931 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_cli_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_cli_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.258357 pip-tools-7.2.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/fake-editables.json
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/fake-index.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/minimal_wheels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.238356 pip-tools-7.2.0/tests/test_data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_a/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_a/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.238356 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_subdir/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:33.262357 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_unpinned_deps/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_fake_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_minimal_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_repository_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_repository_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_top_level_editable.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-02 23:42:09.000000 pip-tools-7.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.github/workflows/reusable-qa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 23:40:00.000000 pip-tools-7.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    44756 2023-08-08 23:40:00.000000 pip-tools-7.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-08 23:40:00.000000 pip-tools-7.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-08 23:40:00.000000 pip-tools-7.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-08 23:40:00.000000 pip-tools-7.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-08-08 23:40:17.804477 pip-tools-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20897 2023-08-08 23:40:00.000000 pip-tools-7.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 23:40:00.000000 pip-tools-7.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/cli/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/cli/pip-compile.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/cli/pip-sync.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 23:40:00.000000 pip-tools-7.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 23:40:00.000000 pip-tools-7.3.0/examples/django.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 23:40:00.000000 pip-tools-7.3.0/examples/flask.in
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 23:40:00.000000 pip-tools-7.3.0/examples/hypothesis.in
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 23:40:00.000000 pip-tools-7.3.0/examples/protection.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 23:40:00.000000 pip-tools-7.3.0/examples/sentry.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-08 23:40:00.000000 pip-tools-7.3.0/img/pip-tools-overview.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.796477 pip-tools-7.3.0/pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-08-08 23:40:17.000000 pip-tools-7.3.0/pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-08 23:40:17.000000 pip-tools-7.3.0/pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:40:17.000000 pip-tools-7.3.0/pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 23:40:17.000000 pip-tools-7.3.0/pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-08 23:40:17.000000 pip-tools-7.3.0/pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 23:40:17.000000 pip-tools-7.3.0/pip_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.800477 pip-tools-7.3.0/piptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.800477 pip-tools-7.3.0/piptools/_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/_compat/pip_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.800477 pip-tools-7.3.0/piptools/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/repositories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/repositories/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/repositories/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.800477 pip-tools-7.3.0/piptools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23167 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/scripts/compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9783 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/scripts/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-08-08 23:40:00.000000 pip-tools-7.3.0/piptools/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-08 23:40:00.000000 pip-tools-7.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:40:17.804477 pip-tools-7.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97118 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_cli_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_cli_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/fake-editables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/fake-index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/minimal_wheels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.792477 pip-tools-7.3.0/tests/test_data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/packages/fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/packages/fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/packages/small_fake_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/packages/small_fake_a/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.792477 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_subdir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:17.804477 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_unpinned_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_fake_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_minimal_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_repository_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_repository_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_top_level_editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27305 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-08 23:40:00.000000 pip-tools-7.3.0/tox.ini
```

### Comparing `pip-tools-7.2.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pip-tools-7.3.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `pip-tools-7.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--- Describe the changes here. --->
 
 ##### Contributor checklist
 
-- [ ] Provided the tests for the changes.
-- [ ] Assure PR title is short, clear, and good to be included in the user-oriented changelog
+- [ ] Included tests for the changes.
+- [ ] PR title is short, clear, and ready to be included in the user-facing changelog.
 
 ##### Maintainer checklist
 
-- [ ] Assure one of these labels is present: `backwards incompatible`, `feature`, `enhancement`, `deprecation`, `bug`, `dependency`, `docs` or `skip-changelog` as they determine changelog listing.
+- [ ] Verified one of these labels is present: `backwards incompatible`, `feature`, `enhancement`, `deprecation`, `bug`, `dependency`, `docs` or `skip-changelog` as they determine changelog listing.
 - [ ] Assign the PR to an existing or new milestone for the target version (following [Semantic Versioning](https://blog.versioneye.com/2014/01/16/semantic-versioning/)).
```

### Comparing `pip-tools-7.2.0/.github/release-drafter.yml` & `pip-tools-7.3.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/.github/workflows/ci.yml` & `pip-tools-7.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/.github/workflows/release-drafter.yml` & `pip-tools-7.3.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/.github/workflows/release.yml` & `pip-tools-7.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/.github/workflows/reusable-qa.yml` & `pip-tools-7.3.0/.github/workflows/reusable-qa.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/.pre-commit-config.yaml` & `pip-tools-7.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/CHANGELOG.md` & `pip-tools-7.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+## v7.3.0
+
+09 Aug 2023
+
+Features:
+
+- Add `--no-strip-extras` and warn about strip extras by default
+  ([#1954](https://github.com/jazzband/pip-tools/pull/1954)). Thanks @ryanhiebert
+
+Bug Fixes:
+
+- Fix revealed default config in header if requirements in subfolder
+  ([#1904](https://github.com/jazzband/pip-tools/pull/1904)). Thanks @atugushev
+- Direct references show extra requirements in .txt files
+  ([#1582](https://github.com/jazzband/pip-tools/pull/1582)). Thanks @FlorentJeannot
+
+Other Changes:
+
+- Document how to run under `pipx run`
+  ([#1951](https://github.com/jazzband/pip-tools/pull/1951)). Thanks @brettcannon
+- Document that the backtracking resolver is the current default
+  ([#1948](https://github.com/jazzband/pip-tools/pull/1948)). Thanks @jeffwidman
+
 ## v7.2.0
 
 02 Aug 2023
 
 Features:
 
 - Add `-c/--constraint` option to `pip-compile`
```

### Comparing `pip-tools-7.2.0/CODE_OF_CONDUCT.md` & `pip-tools-7.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/CONTRIBUTING.md` & `pip-tools-7.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/LICENSE` & `pip-tools-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/PKG-INFO` & `pip-tools-7.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 7.2.0
+Version: 7.3.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Author-email: Vincent Driessen <me@nvie.com>
 License: BSD
 Project-URL: homepage, https://github.com/jazzband/pip-tools/
 Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jazzband/pip-tools
 Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
@@ -67,17 +67,19 @@
 
 ## Example usage for `pip-compile`
 
 The `pip-compile` command lets you compile a `requirements.txt` file from
 your dependencies, specified in either `pyproject.toml`, `setup.cfg`,
 `setup.py`, or `requirements.in`.
 
-Run it with `pip-compile` or `python -m piptools compile`. If you use
-multiple Python versions, you can also run `py -X.Y -m piptools compile` on
-Windows and `pythonX.Y -m piptools compile` on other systems.
+Run it with `pip-compile` or `python -m piptools compile` (or
+`pipx run --spec pip-tools pip-compile` if `pipx` was installed with the
+appropriate Python version). If you use multiple Python versions, you can also
+run `py -X.Y -m piptools compile` on Windows and `pythonX.Y -m piptools compile`
+on other systems.
 
 `pip-compile` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
 or other environment markers, resolve relative to your project's
 environment.
 
 **Note**: If `pip-compile` finds an existing `requirements.txt` file that
@@ -455,37 +457,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
@@ -592,51 +594,33 @@
   - [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VS Code.
   - [pip-requirements.el](https://github.com/Wilfred/pip-requirements.el) for Emacs.
 
 ### Deprecations
 
 This section lists `pip-tools` features that are currently deprecated.
 
-- In future versions, the `--allow-unsafe` behavior will be enabled by
-  default. Use `--no-allow-unsafe` to keep the old behavior. It is
-  recommended to pass the `--allow-unsafe` now to adapt to the upcoming
-  change.
-- Legacy resolver is deprecated and will be removed in future versions.
-  Use `--resolver=backtracking` instead.
+- In the next major release, the `--allow-unsafe` behavior will be enabled by
+  default (https://github.com/jazzband/pip-tools/issues/989).
+  Use `--no-allow-unsafe` to keep the old behavior. It is recommended
+  to pass `--allow-unsafe` now to adapt to the upcoming change.
+- The legacy resolver is deprecated and will be removed in future versions.
+  The new default is `--resolver=backtracking`.
+- In the next major release, the `--strip-extras` behavior will be enabled by
+  default (https://github.com/jazzband/pip-tools/issues/1613).
+  Use `--no-strip-extras` to keep the old behavior.
 
 ### A Note on Resolvers
 
-You can choose from either the legacy or the backtracking resolver.
-The backtracking resolver is recommended, and will become the default
-with the 7.0 release.
-
-Use it now with the `--resolver=backtracking` option to `pip-compile`.
+You can choose from either default backtracking resolver or the deprecated legacy resolver.
 
 The legacy resolver will occasionally fail to resolve dependencies. The
-backtracking resolver is more robust, but can take longer to run in
-general.
-
-You can continue using the legacy resolver with `--resolver=legacy`.
-
-### Versions and compatibility
+backtracking resolver is more robust, but can take longer to run in general.
 
-The table below summarizes the latest `pip-tools` versions with the required
-`pip` and Python versions. Generally, `pip-tools` supports the same Python
-versions as the required `pip` versions.
-
-| pip-tools      | pip            | Python         |
-| -------------- | -------------- | -------------- |
-| 4.5.\*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
-| 5.0.0 - 5.3.0  | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
-| 5.4.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.8 |
-| 5.5.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.9 |
-| 6.0.0 - 6.3.1  | 20.3 - 21.2.\* | 3.6 - 3.9      |
-| 6.4.0          | 21.2 - 21.3.\* | 3.6 - 3.10     |
-| 6.5.0 - 6.10.0 | 21.2 - 22.3.\* | 3.7 - 3.11     |
-| 6.11.0+        | 22.2+          | 3.7 - 3.11     |
+You can continue using the legacy resolver with `--resolver=legacy` although
+note that it is deprecated and will be removed in a future release.
 
 [jazzband]: https://jazzband.co/
 [jazzband-image]: https://jazzband.co/static/img/badge.svg
 [pypi]: https://pypi.org/project/pip-tools/
 [pypi-image]: https://img.shields.io/pypi/v/pip-tools.svg
 [pyversions]: https://pypi.org/project/pip-tools/
 [pyversions-image]: https://img.shields.io/pypi/pyversions/pip-tools.svg
```

### Comparing `pip-tools-7.2.0/README.md` & `pip-tools-7.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 
 ## Example usage for `pip-compile`
 
 The `pip-compile` command lets you compile a `requirements.txt` file from
 your dependencies, specified in either `pyproject.toml`, `setup.cfg`,
 `setup.py`, or `requirements.in`.
 
-Run it with `pip-compile` or `python -m piptools compile`. If you use
-multiple Python versions, you can also run `py -X.Y -m piptools compile` on
-Windows and `pythonX.Y -m piptools compile` on other systems.
+Run it with `pip-compile` or `python -m piptools compile` (or
+`pipx run --spec pip-tools pip-compile` if `pipx` was installed with the
+appropriate Python version). If you use multiple Python versions, you can also
+run `py -X.Y -m piptools compile` on Windows and `pythonX.Y -m piptools compile`
+on other systems.
 
 `pip-compile` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
 or other environment markers, resolve relative to your project's
 environment.
 
 **Note**: If `pip-compile` finds an existing `requirements.txt` file that
@@ -418,37 +420,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
@@ -555,51 +557,33 @@
   - [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VS Code.
   - [pip-requirements.el](https://github.com/Wilfred/pip-requirements.el) for Emacs.
 
 ### Deprecations
 
 This section lists `pip-tools` features that are currently deprecated.
 
-- In future versions, the `--allow-unsafe` behavior will be enabled by
-  default. Use `--no-allow-unsafe` to keep the old behavior. It is
-  recommended to pass the `--allow-unsafe` now to adapt to the upcoming
-  change.
-- Legacy resolver is deprecated and will be removed in future versions.
-  Use `--resolver=backtracking` instead.
+- In the next major release, the `--allow-unsafe` behavior will be enabled by
+  default (https://github.com/jazzband/pip-tools/issues/989).
+  Use `--no-allow-unsafe` to keep the old behavior. It is recommended
+  to pass `--allow-unsafe` now to adapt to the upcoming change.
+- The legacy resolver is deprecated and will be removed in future versions.
+  The new default is `--resolver=backtracking`.
+- In the next major release, the `--strip-extras` behavior will be enabled by
+  default (https://github.com/jazzband/pip-tools/issues/1613).
+  Use `--no-strip-extras` to keep the old behavior.
 
 ### A Note on Resolvers
 
-You can choose from either the legacy or the backtracking resolver.
-The backtracking resolver is recommended, and will become the default
-with the 7.0 release.
-
-Use it now with the `--resolver=backtracking` option to `pip-compile`.
+You can choose from either default backtracking resolver or the deprecated legacy resolver.
 
 The legacy resolver will occasionally fail to resolve dependencies. The
-backtracking resolver is more robust, but can take longer to run in
-general.
-
-You can continue using the legacy resolver with `--resolver=legacy`.
-
-### Versions and compatibility
+backtracking resolver is more robust, but can take longer to run in general.
 
-The table below summarizes the latest `pip-tools` versions with the required
-`pip` and Python versions. Generally, `pip-tools` supports the same Python
-versions as the required `pip` versions.
-
-| pip-tools      | pip            | Python         |
-| -------------- | -------------- | -------------- |
-| 4.5.\*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
-| 5.0.0 - 5.3.0  | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
-| 5.4.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.8 |
-| 5.5.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.9 |
-| 6.0.0 - 6.3.1  | 20.3 - 21.2.\* | 3.6 - 3.9      |
-| 6.4.0          | 21.2 - 21.3.\* | 3.6 - 3.10     |
-| 6.5.0 - 6.10.0 | 21.2 - 22.3.\* | 3.7 - 3.11     |
-| 6.11.0+        | 22.2+          | 3.7 - 3.11     |
+You can continue using the legacy resolver with `--resolver=legacy` although
+note that it is deprecated and will be removed in a future release.
 
 [jazzband]: https://jazzband.co/
 [jazzband-image]: https://jazzband.co/static/img/badge.svg
 [pypi]: https://pypi.org/project/pip-tools/
 [pypi-image]: https://img.shields.io/pypi/v/pip-tools.svg
 [pyversions]: https://pypi.org/project/pip-tools/
 [pyversions-image]: https://img.shields.io/pypi/pyversions/pip-tools.svg
```

### Comparing `pip-tools-7.2.0/docs/conf.py` & `pip-tools-7.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/img/pip-tools-overview.svg` & `pip-tools-7.3.0/img/pip-tools-overview.svg`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/pip_tools.egg-info/PKG-INFO` & `pip-tools-7.3.0/pip_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 7.2.0
+Version: 7.3.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Author-email: Vincent Driessen <me@nvie.com>
 License: BSD
 Project-URL: homepage, https://github.com/jazzband/pip-tools/
 Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jazzband/pip-tools
 Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
@@ -67,17 +67,19 @@
 
 ## Example usage for `pip-compile`
 
 The `pip-compile` command lets you compile a `requirements.txt` file from
 your dependencies, specified in either `pyproject.toml`, `setup.cfg`,
 `setup.py`, or `requirements.in`.
 
-Run it with `pip-compile` or `python -m piptools compile`. If you use
-multiple Python versions, you can also run `py -X.Y -m piptools compile` on
-Windows and `pythonX.Y -m piptools compile` on other systems.
+Run it with `pip-compile` or `python -m piptools compile` (or
+`pipx run --spec pip-tools pip-compile` if `pipx` was installed with the
+appropriate Python version). If you use multiple Python versions, you can also
+run `py -X.Y -m piptools compile` on Windows and `pythonX.Y -m piptools compile`
+on other systems.
 
 `pip-compile` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
 or other environment markers, resolve relative to your project's
 environment.
 
 **Note**: If `pip-compile` finds an existing `requirements.txt` file that
@@ -455,37 +457,37 @@
 You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
 See [pre-commit docs](https://pre-commit.com/) for instructions.
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
 ```
 
 You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
         files: ^requirements/production\.(in|txt)$
         args: [--index-url=https://example.com, requirements/production.in]
 ```
 
 If you have multiple requirement files make sure you create a hook for each file.
 
 ```yaml
 repos:
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.2.0
+    rev: 7.3.0
     hooks:
       - id: pip-compile
         name: pip-compile setup.py
         files: ^(setup\.py|requirements\.txt)$
       - id: pip-compile
         name: pip-compile requirements-dev.in
         args: [requirements-dev.in]
@@ -592,51 +594,33 @@
   - [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VS Code.
   - [pip-requirements.el](https://github.com/Wilfred/pip-requirements.el) for Emacs.
 
 ### Deprecations
 
 This section lists `pip-tools` features that are currently deprecated.
 
-- In future versions, the `--allow-unsafe` behavior will be enabled by
-  default. Use `--no-allow-unsafe` to keep the old behavior. It is
-  recommended to pass the `--allow-unsafe` now to adapt to the upcoming
-  change.
-- Legacy resolver is deprecated and will be removed in future versions.
-  Use `--resolver=backtracking` instead.
+- In the next major release, the `--allow-unsafe` behavior will be enabled by
+  default (https://github.com/jazzband/pip-tools/issues/989).
+  Use `--no-allow-unsafe` to keep the old behavior. It is recommended
+  to pass `--allow-unsafe` now to adapt to the upcoming change.
+- The legacy resolver is deprecated and will be removed in future versions.
+  The new default is `--resolver=backtracking`.
+- In the next major release, the `--strip-extras` behavior will be enabled by
+  default (https://github.com/jazzband/pip-tools/issues/1613).
+  Use `--no-strip-extras` to keep the old behavior.
 
 ### A Note on Resolvers
 
-You can choose from either the legacy or the backtracking resolver.
-The backtracking resolver is recommended, and will become the default
-with the 7.0 release.
-
-Use it now with the `--resolver=backtracking` option to `pip-compile`.
+You can choose from either default backtracking resolver or the deprecated legacy resolver.
 
 The legacy resolver will occasionally fail to resolve dependencies. The
-backtracking resolver is more robust, but can take longer to run in
-general.
-
-You can continue using the legacy resolver with `--resolver=legacy`.
-
-### Versions and compatibility
+backtracking resolver is more robust, but can take longer to run in general.
 
-The table below summarizes the latest `pip-tools` versions with the required
-`pip` and Python versions. Generally, `pip-tools` supports the same Python
-versions as the required `pip` versions.
-
-| pip-tools      | pip            | Python         |
-| -------------- | -------------- | -------------- |
-| 4.5.\*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
-| 5.0.0 - 5.3.0  | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
-| 5.4.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.8 |
-| 5.5.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.9 |
-| 6.0.0 - 6.3.1  | 20.3 - 21.2.\* | 3.6 - 3.9      |
-| 6.4.0          | 21.2 - 21.3.\* | 3.6 - 3.10     |
-| 6.5.0 - 6.10.0 | 21.2 - 22.3.\* | 3.7 - 3.11     |
-| 6.11.0+        | 22.2+          | 3.7 - 3.11     |
+You can continue using the legacy resolver with `--resolver=legacy` although
+note that it is deprecated and will be removed in a future release.
 
 [jazzband]: https://jazzband.co/
 [jazzband-image]: https://jazzband.co/static/img/badge.svg
 [pypi]: https://pypi.org/project/pip-tools/
 [pypi-image]: https://img.shields.io/pypi/v/pip-tools.svg
 [pyversions]: https://pypi.org/project/pip-tools/
 [pyversions-image]: https://img.shields.io/pypi/pyversions/pip-tools.svg
```

### Comparing `pip-tools-7.2.0/pip_tools.egg-info/SOURCES.txt` & `pip-tools-7.3.0/pip_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/_compat/pip_compat.py` & `pip-tools-7.3.0/piptools/_compat/pip_compat.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/cache.py` & `pip-tools-7.3.0/piptools/cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/exceptions.py` & `pip-tools-7.3.0/piptools/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/logging.py` & `pip-tools-7.3.0/piptools/logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/repositories/base.py` & `pip-tools-7.3.0/piptools/repositories/base.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/repositories/local.py` & `pip-tools-7.3.0/piptools/repositories/local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/repositories/pypi.py` & `pip-tools-7.3.0/piptools/repositories/pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/resolver.py` & `pip-tools-7.3.0/piptools/resolver.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/scripts/compile.py` & `pip-tools-7.3.0/piptools/scripts/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pip._internal.req import InstallRequirement
 from pip._internal.req.constructors import install_req_from_line
 from pip._internal.utils.misc import redact_auth_from_url
 
 from .._compat import parse_requirements
 from ..cache import DependencyCache
 from ..exceptions import NoCandidateFound, PipToolsError
-from ..locations import CACHE_DIR, CONFIG_FILE_NAME
+from ..locations import CACHE_DIR, DEFAULT_CONFIG_FILE_NAMES
 from ..logging import log
 from ..repositories import LocalRequirementsRepository, PyPIRepository
 from ..repositories.base import BaseRepository
 from ..resolver import BacktrackingResolver, LegacyResolver
 from ..utils import (
     UNSAFE_PACKAGES,
     dedup,
@@ -222,17 +222,17 @@
         "Use --no-allow-unsafe to keep the old behavior. It is recommended to pass the "
         "--allow-unsafe now to adapt to the upcoming change.".format(
             ", ".join(sorted(UNSAFE_PACKAGES))
         )
     ),
 )
 @click.option(
-    "--strip-extras",
+    "--strip-extras/--no-strip-extras",
     is_flag=True,
-    default=False,
+    default=None,
     help="Assure output file is constraints compatible, avoiding use of extras.",
 )
 @click.option(
     "--generate-hashes",
     is_flag=True,
     default=False,
     help="Generate pip 8 style hashes in the resulting requirements file.",
@@ -310,16 +310,18 @@
         exists=True,
         file_okay=True,
         dir_okay=False,
         readable=True,
         allow_dash=False,
         path_type=str,
     ),
-    help=f"Read configuration from TOML file. By default, looks for a {CONFIG_FILE_NAME} or "
-    "pyproject.toml.",
+    help=(
+        f"Read configuration from TOML file. By default, looks for the following "
+        f"files in the given order: {', '.join(DEFAULT_CONFIG_FILE_NAMES)}."
+    ),
     is_eager=True,
     callback=override_defaults_from_config_file,
 )
 @click.option(
     "--no-config",
     is_flag=True,
     default=False,
@@ -361,15 +363,15 @@
     annotate: bool,
     annotation_style: str,
     upgrade: bool,
     upgrade_packages: tuple[str, ...],
     output_file: LazyFile | IO[Any] | None,
     newline: str,
     allow_unsafe: bool,
-    strip_extras: bool,
+    strip_extras: bool | None,
     generate_hashes: bool,
     reuse_hashes: bool,
     src_files: tuple[str, ...],
     max_rounds: int,
     build_isolation: bool,
     emit_find_links: bool,
     cache_dir: str,
@@ -672,14 +674,23 @@
 
     log.debug("")
 
     linesep = _determine_linesep(
         strategy=newline, filenames=(output_file.name, *src_files)
     )
 
+    if strip_extras is None:
+        strip_extras = False
+        log.warning(
+            "WARNING: --strip-extras is becoming the default "
+            "in version 8.0.0. To silence this warning, "
+            "either use --strip-extras to opt into the new default "
+            "or use --no-strip-extras to retain the existing behavior."
+        )
+
     ##
     # Output
     ##
 
     writer = OutputWriter(
         cast(BinaryIO, output_file),
         click_ctx=ctx,
```

### Comparing `pip-tools-7.2.0/piptools/scripts/sync.py` & `pip-tools-7.3.0/piptools/scripts/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.metadata import get_environment
 
 from .. import sync
 from .._compat import Distribution, parse_requirements
 from ..exceptions import PipToolsError
-from ..locations import CONFIG_FILE_NAME
+from ..locations import DEFAULT_CONFIG_FILE_NAMES
 from ..logging import log
 from ..repositories import PyPIRepository
 from ..utils import (
     flat_map,
     get_pip_version_for_python_executable,
     get_required_pip_specification,
     get_sys_path_for_python_executable,
@@ -94,16 +94,18 @@
         exists=True,
         file_okay=True,
         dir_okay=False,
         readable=True,
         allow_dash=False,
         path_type=str,
     ),
-    help=f"Read configuration from TOML file. By default, looks for a {CONFIG_FILE_NAME} or "
-    "pyproject.toml.",
+    help=(
+        f"Read configuration from TOML file. By default, looks for the following "
+        f"files in the given order: {', '.join(DEFAULT_CONFIG_FILE_NAMES)}."
+    ),
     is_eager=True,
     callback=override_defaults_from_config_file,
 )
 @click.option(
     "--no-config",
     is_flag=True,
     default=False,
```

### Comparing `pip-tools-7.2.0/piptools/subprocess_utils.py` & `pip-tools-7.3.0/piptools/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/sync.py` & `pip-tools-7.3.0/piptools/sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/piptools/utils.py` & `pip-tools-7.3.0/piptools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import os
 import re
 import shlex
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Iterator, TypeVar, cast
 
+from click.core import ParameterSource
+
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 import click
 from click.utils import LazyFile
@@ -27,15 +29,15 @@
 from pip._vendor.packaging.requirements import Requirement
 from pip._vendor.packaging.specifiers import SpecifierSet
 from pip._vendor.packaging.utils import canonicalize_name
 from pip._vendor.packaging.version import Version
 from pip._vendor.pkg_resources import get_distribution
 
 from piptools._compat import PIP_VERSION
-from piptools.locations import CONFIG_FILE_NAME
+from piptools.locations import DEFAULT_CONFIG_FILE_NAMES
 from piptools.subprocess_utils import run_python_snippet
 
 if TYPE_CHECKING:
     from typing import Protocol
 else:
     Protocol = object
 
@@ -151,15 +153,17 @@
 
     # Look for a relative file path, the direct reference currently does not work with it.
     if ireq.link.is_file and not ireq.link.path.startswith("/"):
         return cast(str, ireq.link.url)
 
     # If we get here then we have a requirement that supports direct reference.
     # We need to remove the egg if it exists and keep the rest of the fragments.
-    direct_reference = f"{ireq.name.lower()} @ {ireq.link.url_without_fragment}"
+    lowered_ireq_name = canonicalize_name(ireq.name)
+    extras = f"[{','.join(sorted(ireq.extras))}]" if ireq.extras else ""
+    direct_reference = f"{lowered_ireq_name}{extras} @ {ireq.link.url_without_fragment}"
     fragments = []
 
     # Check if there is any fragment to add to the URI.
     if ireq.link.subdirectory_fragment:
         fragments.append(f"subdirectory={ireq.link.subdirectory_fragment}")
 
     if ireq.link.has_hash:
@@ -363,16 +367,19 @@
         # Exclude one-off options (--upgrade/--upgrade-package/--rebuild/...)
         # or options that don't change compile behaviour (--verbose/--dry-run/...)
         if option_long_name in COMPILE_EXCLUDE_OPTIONS:
             continue
 
         # Exclude config option if it's the default one
         if option_long_name == "--config":
-            default_config = select_config_file(click_ctx.params.get("src_files", ()))
-            if value == default_config:
+            parameter_source = click_ctx.get_parameter_source(option_name)
+            if (
+                str(value) in DEFAULT_CONFIG_FILE_NAMES
+                or parameter_source == ParameterSource.DEFAULT
+            ):
                 continue
 
         # Skip options without a value
         if option.default is None and not value:
             continue
 
         # Skip options with a default value
@@ -650,15 +657,15 @@
         (working_directory / src_file).resolve() for src_file in src_files or (".",)
     )
     candidate_dirs = (src if src.is_dir() else src.parent for src in src_files_as_paths)
     config_file_path = next(
         (
             candidate_dir / config_file
             for candidate_dir in candidate_dirs
-            for config_file in (CONFIG_FILE_NAME, "pyproject.toml")
+            for config_file in DEFAULT_CONFIG_FILE_NAMES
             if (candidate_dir / config_file).is_file()
         ),
         None,
     )
     if config_file_path is None:
         return None
```

### Comparing `pip-tools-7.2.0/piptools/writer.py` & `pip-tools-7.3.0/piptools/writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/pyproject.toml` & `pip-tools-7.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/conftest.py` & `pip-tools-7.3.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from pip._internal.utils.direct_url_helpers import direct_url_from_link
 from pip._vendor.packaging.version import Version
 from pip._vendor.pkg_resources import Requirement
 
 from piptools._compat import PIP_VERSION, Distribution
 from piptools.cache import DependencyCache
 from piptools.exceptions import NoCandidateFound
-from piptools.locations import CONFIG_FILE_NAME
+from piptools.locations import DEFAULT_CONFIG_FILE_NAMES
 from piptools.logging import log
 from piptools.repositories import PyPIRepository
 from piptools.repositories.base import BaseRepository
 from piptools.resolver import BacktrackingResolver, LegacyResolver
 from piptools.utils import (
     as_tuple,
     is_url_requirement,
@@ -448,19 +448,22 @@
 def make_config_file(tmpdir_cwd):
     """
     Make a config file for pip-tools with a given parameter set to a specific
     value, returning a ``pathlib.Path`` to the config file.
     """
 
     def _maker(
-        pyproject_param: str, new_default: Any, config_file_name: str = CONFIG_FILE_NAME
+        pyproject_param: str,
+        new_default: Any,
+        config_file_name: str = DEFAULT_CONFIG_FILE_NAMES[0],
     ) -> Path:
-        # Make a config file with this one config default override
-        config_path = tmpdir_cwd / pyproject_param
-        config_file = config_path / config_file_name
-        config_path.mkdir(exist_ok=True)
+        # Create a nested directory structure if config_file_name includes directories
+        config_dir = (tmpdir_cwd / config_file_name).parent
+        config_dir.mkdir(exist_ok=True, parents=True)
 
+        # Make a config file with this one config default override
+        config_file = tmpdir_cwd / config_file_name
         config_to_dump = {"tool": {"pip-tools": {pyproject_param: new_default}}}
         config_file.write_text(tomli_w.dumps(config_to_dump))
         return cast(Path, config_file.relative_to(tmpdir_cwd))
 
     return _maker
```

### Comparing `pip-tools-7.2.0/tests/test_cache.py` & `pip-tools-7.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_cli_compile.py` & `pip-tools-7.3.0/tests/test_cli_compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,15 +775,18 @@
 def test_direct_reference_with_extras(runner):
     with open("requirements.in", "w") as req_in:
         req_in.write(
             "pip-tools[testing,coverage] @ git+https://github.com/jazzband/pip-tools@6.2.0"
         )
     out = runner.invoke(cli, ["-n", "--rebuild", "--no-build-isolation"])
     assert out.exit_code == 0
-    assert "pip-tools @ git+https://github.com/jazzband/pip-tools@6.2.0" in out.stderr
+    assert (
+        "pip-tools[coverage,testing] @ git+https://github.com/jazzband/pip-tools@6.2.0"
+        in out.stderr
+    )
     assert "pytest==" in out.stderr
     assert "pytest-cov==" in out.stderr
 
 
 def test_input_file_without_extension(pip_conf, runner):
     """
     piptools can compile a file without an extension,
@@ -2943,42 +2946,56 @@
         )
     )
     out = runner.invoke(
         cli,
         [
             "--no-header",
             "--no-annotate",
-            "--no-emit-find-links",
+            "--no-emit-options",
             "--extra",
             "dev",
             "--find-links",
             os.fspath(MINIMAL_WHEELS_PATH),
             os.fspath(tmp_path / "pyproject.toml"),
+            "--output-file",
+            "-",
         ],
     )
-    expected = rf"""foo @ {tmp_path.as_uri()}
+    expected = rf"""foo[footest] @ {tmp_path.as_uri()}
 small-fake-a==0.2
 small-fake-b==0.3
 """
     assert out.exit_code == 0
-    assert expected == out.stderr
+    assert expected == out.stdout
 
 
 def test_config_option(pip_conf, runner, tmp_path, make_config_file):
     config_file = make_config_file("dry-run", True)
 
     req_in = tmp_path / "requirements.in"
     req_in.touch()
 
     out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
 
     assert out.exit_code == 0
     assert "Dry-run, so nothing updated" in out.stderr
 
 
+def test_default_config_option(pip_conf, runner, make_config_file, tmpdir_cwd):
+    make_config_file("dry-run", True)
+
+    req_in = tmpdir_cwd / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli)
+
+    assert out.exit_code == 0
+    assert "Dry-run, so nothing updated" in out.stderr
+
+
 def test_no_config_option_overrides_config_with_defaults(
     pip_conf, runner, tmp_path, make_config_file
 ):
     config_file = make_config_file("dry-run", True)
 
     req_in = tmp_path / "requirements.in"
     req_in.touch()
@@ -3096,7 +3113,37 @@
     req_in = tmp_path / "requirements.in"
     req_in.touch()
 
     out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
 
     assert out.exit_code == 2
     assert "No such config key 'no_annnotate'." in out.stderr
+
+
+strip_extras_warning = (
+    "WARNING: --strip-extras is becoming the default in version 8.0.0."
+)
+
+
+def test_show_warning_on_default_strip_extras_option(
+    runner, make_package, make_sdist, tmp_path
+):
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, req_in.as_posix())
+
+    assert out.exit_code == 0
+    assert strip_extras_warning in out.stderr
+
+
+@pytest.mark.parametrize("option", ("--strip-extras", "--no-strip-extras"))
+def test_do_not_show_warning_on_explicit_strip_extras_option(
+    runner, make_package, make_sdist, tmp_path, option
+):
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, [option, req_in.as_posix()])
+
+    assert out.exit_code == 0
+    assert strip_extras_warning not in out.stderr
```

### Comparing `pip-tools-7.2.0/tests/test_cli_sync.py` & `pip-tools-7.3.0/tests/test_cli_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,27 @@
             "install",
             "-r",
         ]
     ]
 
 
 @mock.patch("piptools.sync.run")
+def test_default_config_option(run, runner, make_config_file, tmpdir_cwd):
+    make_config_file("dry-run", True)
+
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
+        reqs_txt.write("six==1.10.0")
+
+    out = runner.invoke(cli)
+
+    assert out.exit_code == 1
+    assert "Would install:" in out.stdout
+
+
+@mock.patch("piptools.sync.run")
 def test_config_option(run, runner, make_config_file):
     config_file = make_config_file("dry-run", True)
 
     with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
         reqs_txt.write("six==1.10.0")
 
     out = runner.invoke(cli, ["--config", config_file.as_posix()])
```

### Comparing `pip-tools-7.2.0/tests/test_data/fake-index.json` & `pip-tools-7.3.0/tests/test_data/fake-index.json`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.3.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_data/packages/fake_with_deps/setup.py` & `pip-tools-7.3.0/tests/test_data/packages/fake_with_deps/setup.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_fake_index.py` & `pip-tools-7.3.0/tests/test_fake_index.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_logging.py` & `pip-tools-7.3.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_minimal_upgrade.py` & `pip-tools-7.3.0/tests/test_minimal_upgrade.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_repository_local.py` & `pip-tools-7.3.0/tests/test_repository_local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_repository_pypi.py` & `pip-tools-7.3.0/tests/test_repository_pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_resolver.py` & `pip-tools-7.3.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_sync.py` & `pip-tools-7.3.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tests/test_utils.py` & `pip-tools-7.3.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import operator
 import os
 import shlex
 import sys
 from pathlib import Path
+from textwrap import dedent
 
 import pip
 import pytest
 from click import BadOptionUsage, Context, FileError
 from pip._vendor.packaging.version import Version
 
 from piptools.scripts.compile import cli as compile_cli
@@ -27,14 +28,15 @@
     get_sys_path_for_python_executable,
     is_pinned_requirement,
     is_url_requirement,
     key_from_ireq,
     lookup_table,
     lookup_table_from_tuples,
     override_defaults_from_config_file,
+    select_config_file,
 )
 
 
 def test_format_requirement(from_line):
     ireq = from_line("test==1.2")
     assert format_requirement(ireq) == "test==1.2"
 
@@ -76,14 +78,19 @@
         ),
         pytest.param(
             "example @ https://example.com/example.zip?egg=test",
             "example @ https://example.com/example.zip?egg=test",
             id="direct reference with egg in query",
         ),
         pytest.param(
+            "example[b,c,a] @ https://example.com/example.zip",
+            "example[a,b,c] @ https://example.com/example.zip",
+            id="direct reference with optional dependency",
+        ),
+        pytest.param(
             "file:./vendor/package.zip",
             "file:./vendor/package.zip",
             id="file scheme relative path",
         ),
         pytest.param(
             "file:vendor/package.zip",
             "file:vendor/package.zip",
@@ -406,14 +413,44 @@
     """Test that get_compile_command excludes or includes config file."""
     with open(config_file, "w"):
         pass
     with compile_cli.make_context("pip-compile", ["--config", config_file]) as ctx:
         assert get_compile_command(ctx) == expected_command
 
 
+@pytest.mark.parametrize("config_file", ("pyproject.toml", ".pip-tools.toml"))
+@pytest.mark.parametrize(
+    "config_file_content",
+    (
+        pytest.param("", id="empty config file"),
+        pytest.param("[tool.pip-tools]", id="empty config section"),
+        pytest.param("[tool.pip-tools]\ndry-run = true", id="non-empty config section"),
+    ),
+)
+def test_get_compile_command_does_not_include_default_config_if_reqs_file_in_subdir(
+    tmpdir_cwd, config_file, config_file_content
+):
+    """
+    Test that ``get_compile_command`` does not include default config file
+    if requirements file is in a subdirectory.
+    Regression test for issue GH-1903.
+    """
+    default_config_file = Path(config_file)
+    default_config_file.write_text(config_file_content)
+
+    (tmpdir_cwd / "subdir").mkdir()
+    req_file = Path("subdir/requirements.in")
+    req_file.touch()
+    req_file.write_bytes(b"")
+
+    # Make sure that the default config file is not included
+    with compile_cli.make_context("pip-compile", [req_file.as_posix()]) as ctx:
+        assert get_compile_command(ctx) == f"pip-compile {req_file.as_posix()}"
+
+
 def test_get_compile_command_escaped_filenames(tmpdir_cwd):
     """
     Test that get_compile_command output (re-)escapes ' -- '-escaped filenames.
     """
     with open("--requirements.in", "w"):
         pass
     with compile_cli.make_context("pip-compile", ["--", "--requirements.in"]) as ctx:
@@ -674,7 +711,56 @@
     ctx = Context(compile_cli)
     with pytest.raises(FileError, match="Could not read "):
         override_defaults_from_config_file(
             ctx,
             "config",
             "/dev/null/path/does/not/exist/my-config.toml",
         )
+
+
+def test_select_config_file_no_files(tmpdir_cwd):
+    assert select_config_file(()) is None
+
+
+@pytest.mark.parametrize("filename", ("pyproject.toml", ".pip-tools.toml"))
+def test_select_config_file_returns_config_in_cwd(make_config_file, filename):
+    config_file = make_config_file("dry-run", True, filename)
+    assert select_config_file(()) == config_file
+
+
+def test_select_config_file_returns_empty_config_file_in_cwd(tmpdir_cwd):
+    config_file = Path(".pip-tools.toml")
+    config_file.touch()
+
+    assert select_config_file(()) == config_file
+
+
+def test_select_config_file_cannot_find_config_in_cwd(tmpdir_cwd, make_config_file):
+    make_config_file("dry-run", True, "subdir/pyproject.toml")
+    assert select_config_file(()) is None
+
+
+def test_select_config_file_with_config_file_in_subdir(tmpdir_cwd, make_config_file):
+    config_file = make_config_file("dry-run", True, "subdir/.pip-tools.toml")
+
+    requirement_file = Path("subdir/requirements.in")
+    requirement_file.touch()
+
+    assert select_config_file((requirement_file.as_posix(),)) == config_file
+
+
+def test_select_config_file_prefers_pip_tools_toml_over_pyproject_toml(tmpdir_cwd):
+    pip_tools_file = Path(".pip-tools.toml")
+    pip_tools_file.touch()
+
+    pyproject_file = Path("pyproject.toml")
+    pyproject_file.write_text(
+        dedent(
+            """\
+            [build-system]
+            requires = ["setuptools>=63", "setuptools_scm[toml]>=7"]
+            build-backend = "setuptools.build_meta"
+            """
+        )
+    )
+
+    assert select_config_file(()) == pip_tools_file
```

### Comparing `pip-tools-7.2.0/tests/test_writer.py` & `pip-tools-7.3.0/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-7.2.0/tox.ini` & `pip-tools-7.3.0/tox.ini`

 * *Files identical despite different names*


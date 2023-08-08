# Comparing `tmp/lassen-0.2.7.tar.gz` & `tmp/lassen-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lassen-0.2.7.tar", max compression
+gzip compressed data, was "lassen-0.2.8.tar", max compression
```

## Comparing `lassen-0.2.7.tar` & `lassen-0.2.8.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.2.7/LICENSE
--rw-r--r--   0        0        0     3418 2023-07-23 17:12:41.829570 lassen-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.2.7/lassen/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.2.7/lassen/alembic/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.2.7/lassen/alembic/cli.py
--rw-r--r--   0        0        0     2839 2023-07-22 17:00:28.388594 lassen-0.2.7/lassen/alembic/io.py
--rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.2.7/lassen/alembic/runner.py
--rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.2.7/lassen/assets/__init__.py
--rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.2.7/lassen/assets/alembic.ini
--rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.2.7/lassen/assets/script.py.mako
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.2.7/lassen/core/__init__.py
--rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.2.7/lassen/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.2.7/lassen/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.2.7/lassen/core/config.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.2.7/lassen/datasets/__init__.py
--rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.2.7/lassen/datasets/dataset_helpers.py
--rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.2.7/lassen/datasets/pyarrow_schemas.py
--rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.2.7/lassen/db/__init__.py
--rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.2.7/lassen/db/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      422 2023-07-22 17:00:28.388869 lassen-0.2.7/lassen/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.2.7/lassen/db/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.2.7/lassen/db/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-310.pyc
--rw-r--r--   0        0        0     2138 2023-07-23 15:46:35.701193 lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-311.pyc
--rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.2.7/lassen/db/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0     1296 2023-07-22 17:00:28.389524 lassen-0.2.7/lassen/db/__pycache__/session.cpython-311.pyc
--rw-r--r--   0        0        0     1437 2023-07-23 15:46:28.626071 lassen-0.2.7/lassen/db/base_class.py
--rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.2.7/lassen/db/session.py
--rw-r--r--   0        0        0      302 2023-07-29 15:15:21.002859 lassen-0.2.7/lassen/enums.py
--rw-r--r--   0        0        0     1272 2023-07-22 17:00:28.389917 lassen-0.2.7/lassen/io.py
--rw-r--r--   0        0        0        0 2023-07-22 17:05:14.900856 lassen-0.2.7/lassen/py.typed
--rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.2.7/lassen/schema.py
--rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.2.7/lassen/shared.py
--rw-r--r--   0        0        0    10799 2023-07-29 15:15:21.003191 lassen-0.2.7/lassen/store.py
--rw-r--r--   0        0        0      201 2023-07-22 17:00:28.390303 lassen-0.2.7/lassen/stubs/__init__.py
--rw-r--r--   0        0        0     1294 2023-07-23 15:10:32.421607 lassen-0.2.7/lassen/stubs/base.py
--rw-r--r--   0        0        0      147 2023-07-23 04:25:54.115562 lassen-0.2.7/lassen/stubs/definition.py
--rw-r--r--   0        0        0     2448 2023-07-25 17:26:24.493945 lassen-0.2.7/lassen/stubs/field.py
--rw-r--r--   0        0        0     4856 2023-07-30 15:57:55.862739 lassen-0.2.7/lassen/stubs/generate.py
--rw-r--r--   0        0        0       96 2023-07-22 17:00:28.390790 lassen-0.2.7/lassen/stubs/generators/__init__.py
--rw-r--r--   0        0        0     9627 2023-07-30 15:57:55.863156 lassen-0.2.7/lassen/stubs/generators/common.py
--rw-r--r--   0        0        0     8064 2023-07-25 17:26:24.494192 lassen-0.2.7/lassen/stubs/generators/schema.py
--rw-r--r--   0        0        0    13343 2023-07-30 15:57:55.863592 lassen-0.2.7/lassen/stubs/generators/store.py
--rw-r--r--   0        0        0      177 2023-07-22 17:00:28.391343 lassen-0.2.7/lassen/stubs/templates/__init__.py
--rw-r--r--   0        0        0     1052 2023-07-22 17:00:28.391457 lassen-0.2.7/lassen/stubs/templates/schema.py.j2
--rw-r--r--   0        0        0      591 2023-07-23 15:31:38.606138 lassen-0.2.7/lassen/stubs/templates/sqlalchemy.py.j2
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.2.7/lassen/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.2.7/lassen/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.2.7/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.2.7/lassen/tests/__pycache__/fixtures.cpython-310.pyc
--rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.2.7/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.2.7/lassen/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.2.7/lassen/tests/datasets/__init__.py
--rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.2.7/lassen/tests/datasets/test_dataset_helpers.py
--rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.2.7/lassen/tests/datasets/test_pyarrow_schemas.py
--rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.2.7/lassen/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1181 2023-07-25 17:26:24.494365 lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema.py
--rw-r--r--   0        0        0      961 2023-07-25 17:26:24.494521 lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema_public.py
--rw-r--r--   0        0        0      926 2023-07-23 17:16:21.722018 lassen-0.2.7/lassen/tests/fixtures/stubs/expected_store.py
--rw-r--r--   0        0        0     1134 2023-07-25 17:26:24.494720 lassen-0.2.7/lassen/tests/fixtures/stubs/fixtures.py
--rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.2.7/lassen/tests/fixtures/test_harness/README.md
--rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.2.7/lassen/tests/fixtures/test_harness/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/__init__.py
--rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
--rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
--rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/models.py
--rw-r--r--   0        0        0      521 2023-07-23 15:10:32.425116 lassen-0.2.7/lassen/tests/model_fixtures.py
--rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392359 lassen-0.2.7/lassen/tests/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392464 lassen-0.2.7/lassen/tests/stubs/generators/__init__.py
--rw-r--r--   0        0        0     3788 2023-07-30 15:57:55.863980 lassen-0.2.7/lassen/tests/stubs/generators/test_common.py
--rw-r--r--   0        0        0     1221 2023-07-23 15:10:32.425828 lassen-0.2.7/lassen/tests/stubs/generators/test_schema.py
--rw-r--r--   0        0        0     3792 2023-07-30 15:57:55.864327 lassen-0.2.7/lassen/tests/stubs/generators/test_store.py
--rw-r--r--   0        0        0     2560 2023-07-22 17:00:28.393152 lassen-0.2.7/lassen/tests/stubs/test_generate.py
--rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.2.7/lassen/tests/test_alembic.py
--rw-r--r--   0        0        0     5422 2023-07-29 15:15:21.003403 lassen-0.2.7/lassen/tests/test_store.py
--rw-r--r--   0        0        0     1423 2023-07-30 15:58:38.629922 lassen-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 lassen-0.2.7/setup.py
--rw-r--r--   0        0        0     4389 1970-01-01 00:00:00.000000 lassen-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3418 2023-07-23 17:12:41.829570 lassen-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.2.8/lassen/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.2.8/lassen/alembic/__init__.py
+-rw-r--r--   0        0        0     3691 2023-07-30 16:40:39.835375 lassen-0.2.8/lassen/alembic/cli.py
+-rw-r--r--   0        0        0     2858 2023-07-30 16:40:39.835782 lassen-0.2.8/lassen/alembic/io.py
+-rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.2.8/lassen/alembic/runner.py
+-rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.2.8/lassen/assets/__init__.py
+-rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.2.8/lassen/assets/alembic.ini
+-rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.2.8/lassen/assets/script.py.mako
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.2.8/lassen/core/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.2.8/lassen/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.2.8/lassen/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.2.8/lassen/core/config.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.2.8/lassen/datasets/__init__.py
+-rw-r--r--   0        0        0     2404 2023-07-30 16:40:39.836025 lassen-0.2.8/lassen/datasets/dataset_helpers.py
+-rw-r--r--   0        0        0     3043 2023-07-30 16:40:39.836317 lassen-0.2.8/lassen/datasets/pyarrow_schemas.py
+-rw-r--r--   0        0        0      240 2023-07-30 16:40:39.836583 lassen-0.2.8/lassen/db/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.2.8/lassen/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      422 2023-08-08 23:48:52.604473 lassen-0.2.8/lassen/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.2.8/lassen/db/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.2.8/lassen/db/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.2.8/lassen/db/__pycache__/base_class.cpython-310.pyc
+-rw-r--r--   0        0        0     2138 2023-07-23 15:46:35.701193 lassen-0.2.8/lassen/db/__pycache__/base_class.cpython-311.pyc
+-rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.2.8/lassen/db/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0     1296 2023-07-22 17:00:28.389524 lassen-0.2.8/lassen/db/__pycache__/session.cpython-311.pyc
+-rw-r--r--   0        0        0     1437 2023-07-23 15:46:28.626071 lassen-0.2.8/lassen/db/base_class.py
+-rw-r--r--   0        0        0      213 2023-08-08 23:48:52.604577 lassen-0.2.8/lassen/db/columns.py
+-rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.2.8/lassen/db/session.py
+-rw-r--r--   0        0        0      302 2023-07-29 15:15:21.002859 lassen-0.2.8/lassen/enums.py
+-rw-r--r--   0        0        0     1272 2023-07-22 17:00:28.389917 lassen-0.2.8/lassen/io.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:05:14.900856 lassen-0.2.8/lassen/py.typed
+-rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.2.8/lassen/schema.py
+-rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.2.8/lassen/shared.py
+-rw-r--r--   0        0        0    10822 2023-08-08 23:48:52.604740 lassen-0.2.8/lassen/store.py
+-rw-r--r--   0        0        0      181 2023-07-30 16:40:39.837664 lassen-0.2.8/lassen/stubs/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-23 15:10:32.421607 lassen-0.2.8/lassen/stubs/base.py
+-rw-r--r--   0        0        0      147 2023-07-23 04:25:54.115562 lassen-0.2.8/lassen/stubs/definition.py
+-rw-r--r--   0        0        0     2456 2023-07-30 16:40:39.837902 lassen-0.2.8/lassen/stubs/field.py
+-rw-r--r--   0        0        0     4923 2023-07-30 16:40:39.838145 lassen-0.2.8/lassen/stubs/generate.py
+-rw-r--r--   0        0        0       86 2023-07-30 16:40:39.838633 lassen-0.2.8/lassen/stubs/generators/__init__.py
+-rw-r--r--   0        0        0     9700 2023-07-30 16:40:39.838990 lassen-0.2.8/lassen/stubs/generators/common.py
+-rw-r--r--   0        0        0     8090 2023-07-30 16:40:39.839254 lassen-0.2.8/lassen/stubs/generators/schema.py
+-rw-r--r--   0        0        0    13887 2023-08-08 23:48:52.604917 lassen-0.2.8/lassen/stubs/generators/store.py
+-rw-r--r--   0        0        0      177 2023-07-22 17:00:28.391343 lassen-0.2.8/lassen/stubs/templates/__init__.py
+-rw-r--r--   0        0        0     1052 2023-07-22 17:00:28.391457 lassen-0.2.8/lassen/stubs/templates/schema.py.j2
+-rw-r--r--   0        0        0      591 2023-07-23 15:31:38.606138 lassen-0.2.8/lassen/stubs/templates/sqlalchemy.py.j2
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.2.8/lassen/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.2.8/lassen/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.2.8/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.2.8/lassen/tests/__pycache__/fixtures.cpython-310.pyc
+-rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.2.8/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1915 2023-07-30 16:40:39.839871 lassen-0.2.8/lassen/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.2.8/lassen/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.2.8/lassen/tests/datasets/test_dataset_helpers.py
+-rw-r--r--   0        0        0     1649 2023-07-30 16:40:39.840179 lassen-0.2.8/lassen/tests/datasets/test_pyarrow_schemas.py
+-rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.2.8/lassen/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-30 16:37:31.430609 lassen-0.2.8/lassen/tests/fixtures/stubs/expected_schema.py
+-rw-r--r--   0        0        0      961 2023-07-30 16:37:31.430840 lassen-0.2.8/lassen/tests/fixtures/stubs/expected_schema_public.py
+-rw-r--r--   0        0        0      926 2023-07-30 16:37:31.431085 lassen-0.2.8/lassen/tests/fixtures/stubs/expected_store.py
+-rw-r--r--   0        0        0     1134 2023-07-25 17:26:24.494720 lassen-0.2.8/lassen/tests/fixtures/stubs/fixtures.py
+-rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.2.8/lassen/tests/fixtures/test_harness/README.md
+-rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.2.8/lassen/tests/fixtures/test_harness/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.2.8/lassen/tests/fixtures/test_harness/test_harness/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.2.8/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
+-rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.2.8/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
+-rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.2.8/lassen/tests/fixtures/test_harness/test_harness/models.py
+-rw-r--r--   0        0        0      521 2023-07-23 15:10:32.425116 lassen-0.2.8/lassen/tests/model_fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392359 lassen-0.2.8/lassen/tests/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392464 lassen-0.2.8/lassen/tests/stubs/generators/__init__.py
+-rw-r--r--   0        0        0     3788 2023-07-30 16:40:39.840612 lassen-0.2.8/lassen/tests/stubs/generators/test_common.py
+-rw-r--r--   0        0        0     1221 2023-07-23 15:10:32.425828 lassen-0.2.8/lassen/tests/stubs/generators/test_schema.py
+-rw-r--r--   0        0        0     3928 2023-08-08 23:48:52.605068 lassen-0.2.8/lassen/tests/stubs/generators/test_store.py
+-rw-r--r--   0        0        0     2560 2023-07-22 17:00:28.393152 lassen-0.2.8/lassen/tests/stubs/test_generate.py
+-rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.2.8/lassen/tests/test_alembic.py
+-rw-r--r--   0        0        0     5421 2023-07-30 16:40:39.841163 lassen-0.2.8/lassen/tests/test_store.py
+-rw-r--r--   0        0        0     1361 2023-08-08 23:48:54.887853 lassen-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 lassen-0.2.8/setup.py
+-rw-r--r--   0        0        0     4389 1970-01-01 00:00:00.000000 lassen-0.2.8/PKG-INFO
```

### Comparing `lassen-0.2.7/LICENSE` & `lassen-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/README.md` & `lassen-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/alembic/cli.py` & `lassen-0.2.8/lassen/alembic/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def patch_migrations(self, config: Config, offline_mode=False):
         # Interpret the config file for Python logging.
         # This line sets up loggers basically.
         fileConfig(str(config.config_file_name))
 
         # Exhaust the iterator to ensure that all sqlalchemy modules are mounted.
         found_models = list(get_sqlalchemy_base_subclasses(self.package_name))
-        print(f"Auto-detected models: {found_models}")
+        click.secho(f"Auto-detected models: {found_models}")
 
         def run_migration(self):
             if offline_mode:
                 run_migrations_offline()
             else:
                 run_migrations_online()
```

### Comparing `lassen-0.2.7/lassen/alembic/io.py` & `lassen-0.2.8/lassen/alembic/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 
     # Return the directory name, which is the name of the package
     return package_path.name
 
 
 def get_migration_path(package_name: str):
     """
-    By convention, client apps store their migrations in a sub-folder called `{package_name}.migrations`.
+    By convention, client apps store their migrations in a sub-folder
+    called `{package_name}.migrations`.
     """
     package = importlib.import_module(package_name)
     path = package.__path__
 
     migration_path = Path(path[0]) / "migrations"
     if not migration_path.exists():
         raise Exception(
-            f"Could not find migrations folder at `{migration_path}`. Did you forget to create it?"
+            f"Could not find migrations folder at `{migration_path}`."
+            " Did you forget to create it?"
         )
 
     return migration_path
 
 
 def iterate_regular_package_files(
     package_name: str, exclude_patterns: list | None = None
```

### Comparing `lassen-0.2.7/lassen/alembic/runner.py` & `lassen-0.2.8/lassen/alembic/runner.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/assets/alembic.ini` & `lassen-0.2.8/lassen/assets/alembic.ini`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/core/__pycache__/config.cpython-310.pyc` & `lassen-0.2.8/lassen/core/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/core/config.py` & `lassen-0.2.8/lassen/core/config.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/datasets/dataset_helpers.py` & `lassen-0.2.8/lassen/datasets/dataset_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 def batch_to_examples(batch: dict[str, list[Any]]) -> Iterator[dict[str, Any]]:
     """
     Batches are passed as dictionary-lists:
 
     {feature1: [values], feature2: [values]}
 
-    It's typically more natural to treat a batch as each example. This function reformats
-    into each separate examples in a streaming iterator.
+    It's typically more natural to treat a batch as each example. This function
+    reformats into each separate examples in a streaming iterator.
 
     """
     lengths = {len(v) for v in batch.values()}
     if len(lengths) != 1:
         raise ValueError("All lists in the batch must have the same length.")
 
     for i in range(next(iter(lengths))):
@@ -34,27 +34,32 @@
 ) -> dict[str, list[Any]] | Table:
     """
     This function takes an iterator of examples and converts it into a batch.
     Each example is a dictionary of features:
 
     {"feature1": value, "feature2": value}
 
-    The function returns a dictionary where each key corresponds to a feature and the value is a list of feature values for all examples.
+    The function returns a dictionary where each key corresponds to
+    a feature and the value is a list of feature values for all examples.
     """
-    # We create a placeholder series of lists here because `datasets` expects that each batch dictionary will
-    # have the same keys, even if there are no objects. Trying to build this up as we go based on the examples
+    # We create a placeholder series of lists here because `datasets`
+    # expects that each batch dictionary will
+    # have the same keys, even if there are no objects. Trying to build
+    # this up as we go based on the examples
     # results in a blank dictionary if the values are empty.
     batch: dict[str, list[Any]] = {field.name: [] for field in fields(data_class)}
 
     for example in examples:
         # For each example, iterate over its features.
         for feature, value in asdict(example).items():
             batch[feature].append(value)
 
     if explicit_schema and examples:
-        # If explicit_schema is specified without examples, the dataframe will have empty dtypes
-        # by default and the schema-dataframe mismatch will raise an exception.
+        # If explicit_schema is specified without examples, the dataframe
+        # will have empty dtypes
+        # by default and the schema-dataframe mismatch will raise
+        # an exception.
         schema = get_schema_from_dataclass(data_class)
         table = Table.from_pandas(pd.DataFrame(batch), schema=schema)
         return table
     else:
         return batch
```

### Comparing `lassen-0.2.7/lassen/datasets/pyarrow_schemas.py` & `lassen-0.2.8/lassen/datasets/pyarrow_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,16 @@
             fields = {
                 key: python_type_to_pyarrow_type(val)
                 for key, val in python_type.__annotations__.items()
             }
             return pa.struct(fields)
         elif python_type is np.ndarray:
             raise ValueError(
-                "ndarrays should be typehinted with their inner type, like np.ndarray[np.int32]"
+                "ndarrays should be typehinted with their inner type,"
+                " like np.ndarray[np.int32]"
             )
         else:
             raise ValueError(
                 f"Unsupported pyarrow field conversion type: {python_type}"
             )
     else:
         # This is a complex type, like list[str] or dict[str, str]
```

### Comparing `lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-310.pyc` & `lassen-0.2.8/lassen/db/__pycache__/base_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-311.pyc` & `lassen-0.2.8/lassen/db/__pycache__/base_class.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/db/__pycache__/session.cpython-310.pyc` & `lassen-0.2.8/lassen/db/__pycache__/session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/db/__pycache__/session.cpython-311.pyc` & `lassen-0.2.8/lassen/db/__pycache__/session.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/db/base_class.py` & `lassen-0.2.8/lassen/db/base_class.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/db/session.py` & `lassen-0.2.8/lassen/db/session.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/io.py` & `lassen-0.2.8/lassen/io.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/store.py` & `lassen-0.2.8/lassen/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pydantic import BaseModel
 from sqlalchemy import Column, Table
 from sqlalchemy.orm import Query, Session
 
 from lassen.db.base_class import Base
 from lassen.enums import FilterTypeEnum
+from uuid import UUID
 
 ModelType = TypeVar("ModelType", bound=Base)
 CreateSchemaType = TypeVar("CreateSchemaType", bound=BaseModel)
 UpdateSchemaType = TypeVar("UpdateSchemaType", bound=BaseModel)
 FilterSchemaType = TypeVar("FilterSchemaType", bound=BaseModel)
 
 
@@ -78,27 +79,28 @@
                 raise ValueError(f"Model `{self.model}` has no column `{field}`")
             setattr(db_obj, field, value)
         db.add(db_obj)
         db.commit()
         db.refresh(db_obj)
         return db_obj
 
-    def remove(self, db: Session, *, id: int) -> ModelType | None:
+    def remove(self, db: Session, *, id: int | UUID) -> ModelType | None:
         obj = db.query(self.model).get(id)
         if obj:
             db.delete(obj)
             db.commit()
         return obj
 
     def create_dependencies(
         self, db: Session, obj_in_data: dict[str, Any], obj_in: Any
     ):
         """
-        Creates nested objects that are contained within the primary. Note that this function
-        only creates one-depth of dependencies. If you have a dependency that has a dependency,
+        Creates nested objects that are contained within the primary.
+        Note that this function only creates one-depth of dependencies.
+        If you have a dependency that has a dependency,
         you will need to create that dependency separately.
 
         """
         # Iterate over the dependent relationships and attempt to create these first
         for relationship, relationship_class in self.relationship_attributes.items():
             if relationship not in obj_in_data:
                 continue
@@ -112,28 +114,29 @@
             database_value: list[Base] | Base | None = None
 
             # Determine if we should create a list
             # Otherwise assume this is an object
             if isinstance(static_value, list):
                 database_value = []
                 for value, original_value in zip(static_value, static_value_original):
-                    # print("ORIGINAL", original_value)
-                    # If this is a dict, we should cast it otherwise assume it's a SQLAlchemy object
+                    # If this is a dict, we should cast it otherwise
+                    # assume it's a SQLAlchemy object
                     if isinstance(original_value, Base):
                         database_value.append(value)
                     else:
                         database_object = relationship_class(**value)
                         # db.add(database_object)
                         # db.commit()
                         # db.refresh(database_object)
                         database_value.append(database_object)
 
                 obj_in_data[relationship] = database_value
             else:
-                # If this is a dict, we should cast it otherwise assume it's a SQLAlchemy object
+                # If this is a dict, we should cast it otherwise
+                # assume it's a SQLAlchemy object
                 if isinstance(value, dict):
                     # Create the relationship object
                     database_value = relationship_class(**static_value)
                     # db.add(database_value)
                     # db.commit()
                     # db.refresh(database_value)
                 else:
@@ -154,36 +157,37 @@
         if not base_class_args:
             raise ValueError("StoreBase must be subclassed with type arguments")
 
         _, create_schema, update_schema = get_args(base_class_args[0])
 
         def validate_arg_model_order(args):
             """
-            Ensure that models are declared before their SQLAlchemy counterparts. Otherwise
-            objects will be cast as schemas where we typically want them to remain as SQLAlchemy objects.
+            Ensure that models are declared before their SQLAlchemy
+            counterparts. Otherwise objects will be cast as schemas
+            where we typically want them to remain as SQLAlchemy objects.
             """
             index_of_model = [
                 i for i, x in enumerate(args) if isclass(x) and issubclass(x, Base)
             ]
             if index_of_model:
                 if min(index_of_model) > 0:
                     raise ValueError(
-                        f"SQLAlchemy Model must come first in a list of typehints, actual order: {args}"
+                        "SQLAlchemy Model must come first in a list of"
+                        " typehints, actual order: {args}"
                     )
 
             # Recursively do this for all union types
             for arg in args:
                 if isinstance(arg, types.UnionType):
                     validate_arg_model_order(arg.__args__)
 
         # Get all the nested elements that involve models and
         for schema in [create_schema, update_schema]:
             # Iterate over all typehints for the class
             schema_typehints = get_type_hints(schema)
-            print(schema_typehints)
 
             for typehint in schema_typehints.values():
                 if hasattr(typehint, "__args__"):
                     validate_arg_model_order(typehint.__args__)
 
 
 class StoreFilterMixin(
```

### Comparing `lassen-0.2.7/lassen/stubs/base.py` & `lassen-0.2.8/lassen/stubs/base.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/stubs/field.py` & `lassen-0.2.8/lassen/stubs/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,18 @@
     default: Any | Callable | UNSET_VALUE = UNSET_VALUE(),
 ) -> Any:
     """
     :param generators: By default, all class-associated generators are used
     :param default: If you want to set a more complex expression as your default
         you can use a lambda x: {my value} expression. This delays execution of
         the actual logic and we'll instead use the lambda values.
-    :param If set to True, enables regular equality expressions for this field. For additional
-        options, see the filter_extensions parameter.
-    :param filter_extensions: List of additional filter extensions to enable for this field.
+    :param If set to True, enables regular equality expressions for this field.
+        For additional options, see the filter_extensions parameter.
+    :param filter_extensions: List of additional filter extensions
+        to enable for this field.
 
     """
     return FieldDefinition(
         generators=generators,
         description=description,
         examples=examples or [],
         create=create,
```

### Comparing `lassen-0.2.7/lassen/stubs/generate.py` & `lassen-0.2.8/lassen/stubs/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     stub_models: list[tuple[Type[BaseStub], Path]] = []
 
     package = importlib.import_module(root_path.name)
 
     for _, module_name, _ in pkgutil.walk_packages(
         path=package.__path__, prefix=package.__name__ + "."
     ):
-        # Speed up the search by skipping modules that are clearly not in the stubs directory
+        # Speed up the search by skipping modules that are clearly not
+        # in the stubs directory
         if CLIENT_STUB_DIRECTORY not in module_name:
             continue
 
         definition_module = importlib.import_module(module_name)
 
         stub_models += [
             (val, Path(inspect.getfile(val)))
@@ -43,15 +44,15 @@
             if val != BaseStub
         ]
 
     if not stub_models:
         secho(f"No stub models found, checked: {root_path}", fg="red")
         return []
 
-    secho(f"Found stub models:", fg="blue")
+    secho("Found stub models:", fg="blue")
     for model, path in stub_models:
         secho(f"  {model.__name__} ({path.name})", fg="blue")
 
     model_generators: list[tuple[Type[BaseStub], Path, list[BaseGenerator]]] = [
         (
             model,
             path,
@@ -66,32 +67,34 @@
     ]
 
     unique_generators = set(
         generator for _, _, generators in model_generators for generator in generators
     )
 
     # Set up the base folders
-    # This includes a new __init__ stub in each directory that can be used to import dependency files
+    # This includes a new __init__ stub in each directory that can be
+    # used to import dependency files
     for generator in unique_generators:
         generator_output = root_path / generator.output_directory
         generator_output.mkdir(parents=True, exist_ok=True)
 
-        # Clear the old files, since the user might have deleted the underlying stubs in the meantime
+        # Clear the old files, since the user might have deleted the
+        # underlying stubs in the meantime
         for file in generator_output.iterdir():
             if file.is_file():
                 file.unlink()
 
         with open(generator_output / "__init__.py", "w") as f:
             f.write("")
 
     try:
         for model, path, generators in model_generators:
             # Extract the explicit import from the model and its user-defined parents
-            # Skip the lassen-internal base class itself since this won't have any imports
-            # that are relevant to the definitions
+            # Skip the lassen-internal base class itself since this won't have any
+            # imports that are relevant to the definitions
             parent_paths = [
                 Path(inspect.getfile(model))
                 for model in model.__bases__
                 if model != BaseStub
             ]
             stub_imports = extract_stub_imports([path] + parent_paths)
 
@@ -104,29 +107,31 @@
                     generator_output / f"{underscore(model.__name__)}.py", "w"
                 ) as f:
                     f.write(rendered.content)
 
                 with open(generator_output / "__init__.py", "a") as f:
                     formatted_class_names = ", ".join(rendered.created_classes)
                     f.write(
-                        f"from .{underscore(model.__name__)} import {formatted_class_names} # noqa: 401\n"
+                        f"from .{underscore(model.__name__)}"
+                        f" import {formatted_class_names} # noqa: 401\n"
                     )
 
             if generators:
                 secho(f"Generated files for {model.__name__}", fg="green")
             else:
                 secho(f"No generators found for {model.__name__}", fg="yellow")
     except Exception as e:
         secho("Exception encountered, cleaning up filesystem...", fg="red")
 
         for generator in unique_generators:
             generator_output = root_path / generator.output_directory
             generator_output.mkdir(parents=True, exist_ok=True)
 
-            # Clear the old files, since the user might have deleted the underlying stubs in the meantime
+            # Clear the old files, since the user might have deleted the underlying
+            # stubs in the meantime
             for file in generator_output.iterdir():
                 if file.is_file():
                     file.unlink()
 
             with open(generator_output / "__init__.py", "w") as f:
                 f.write("")
```

### Comparing `lassen-0.2.7/lassen/stubs/generators/common.py` & `lassen-0.2.8/lassen/stubs/generators/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         return None
     return f"from {module_name} import {class_name}"
 
 
 def extract_type_hints(cls, required_superclass: type):
     """
     :param required_superclass: Only extract type hints from fields that are instances
-        of the given class. Useful to limit typehints to only Field instances or Generator instances.
+        of the given class. Useful to limit typehints to only Field instances
+        or Generator instances.
     """
     if not issubclass(cls, BaseStub):
         raise ValueError("cls must be a subclass of BaseStub")
 
     # Explicitly don't resolve forward references (unlike typing.get_type_hints(cls))
     # to avoid possible circular dependencies
     type_hints = cls.__annotations__
@@ -68,15 +69,15 @@
     args = get_args(typehint)
 
     # Handle case for NoneType
     if typehint is type(None):
         return "None", []
 
     # Handle case for Unions, which might represent nullable fields
-    if origin is typing.Union or origin == types.UnionType:
+    if origin is typing.Union or origin == types.UnionType:  # noqa E721
         union_args = ", ".join([format_typehint_as_string(t)[0] for t in args])
         return f"Union[{union_args}]", [format_import(t) for t in args] + [
             format_import(typing.Union)
         ]
 
     # Handle case for Enum
     if isinstance(typehint, enum.EnumMeta):
@@ -118,15 +119,16 @@
         arg_types = ", ".join(arg_names)
         return f"{typehint_name}[{arg_types}]", arg_deps
 
     raise NotImplementedError(f"Type hint {typehint} not supported")
 
 
 def is_lambda(v):
-    LAMBDA = lambda: 0
+    LAMBDA = lambda: 0  # noqa
+
     return isinstance(v, type(LAMBDA)) and v.__name__ == LAMBDA.__name__
 
 
 def get_lambda_body(func: Callable) -> str:
     func_lines, start_number = inspect.getsourcelines(func)
     func_range = set(range(start_number, start_number + len(func_lines)))
 
@@ -157,16 +159,16 @@
         return ast.unparse(found_lambds[0].body).strip()
 
     raise ValueError("No lambda function found in provided function.")
 
 
 def format_dict_as_kwargs(dictionary: dict[str, Any]):
     """
-    Formats a dictionary as keyword arguments. If a dictionary value is a lambda function,
-    will attempt to extract its value as a string.
+    Formats a dictionary as keyword arguments. If a dictionary value is
+    a lambda function, will attempt to extract its value as a string.
 
     """
     # These representations can be explicitly cast
     # Everything else should be in a lambda
     allowed_representations = (str, int, float, bool, type(None))
     representation_dict: dict[str, str] = {}
 
@@ -176,21 +178,23 @@
         elif is_lambda(value):
             return f"lambda: {get_lambda_body(value)}"
         elif isinstance(value, list):
             # Convert the args
             converted_args: list[str] = [convert_value(arg) for arg in value]
             return f"[{', '.join(converted_args)}]"
         elif isinstance(value, allowed_representations):
-            # Allowed representation fallback should be the last in the chain, since these
-            # classes might be superclasses of other more specific targeting (StrEnum, for instance)
-            # that we would rather process by their targeted handler
+            # Allowed representation fallback should be the last in the chain, since
+            # these classes might be superclasses of other more specific targeting
+            # (StrEnum, for instance) that we would rather process by their
+            # targeted handler
             return repr(value)
         else:
             raise ValueError(
-                f"Value {value} is not a valid default; cast with `lambda` in your code to maintain its representation."
+                f"Value {value} is not a valid default; cast with `lambda` in your"
+                " code to maintain its representation."
             )
 
     for key, value in dictionary.items():
         representation_dict[key] = convert_value(value)
 
     return ", ".join(f"{k}={v}" for k, v in representation_dict.items())
 
@@ -237,15 +241,16 @@
     stub_imports: list[ImportDefinition] = []
 
     for path in paths:
         with open(path, "r") as file:
             file_content = file.read()
         module = ast.parse(file_content)
 
-        # Ignore lassen imports by default, since this often brings in conflicting type definitions
+        # Ignore lassen imports by default, since this often brings in conflicting
+        # type definitions
         stub_imports += [
             module_import
             for module_import in extract_imports(module)
             if "lassen" not in module_import.definition
         ]
 
     return ExtractedStubImports(
```

### Comparing `lassen-0.2.7/lassen/stubs/generators/schema.py` & `lassen-0.2.8/lassen/stubs/generators/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 from lassen.stubs.templates import get_template_path
 
 
 def is_optional(type_hint):
     origin = get_origin(type_hint)
     args = get_args(type_hint)
 
-    if origin is typing.Union or origin == types.UnionType:
+    if origin is typing.Union or origin == types.UnionType:  # noqa E721
         return any(arg is type(None) for arg in args)
     elif isinstance(type_hint, type):
         return type_hint is type(None)
     return False
 
 
 def make_optional(type_hint):
     if is_optional(type_hint):
         # The type hint is already Optional
         return type_hint
     else:
         origin = get_origin(type_hint)
         args = get_args(type_hint)
 
-        if origin is typing.Union or origin == types.UnionType:
+        if origin is typing.Union or origin == types.UnionType:  # noqa E721
             # Convert the Union to Optional by adding None as an argument
             return typing.Union[*args, type(None)]
         else:
             # If the type hint is not a Union, make it Optional
             return typing.Optional[type_hint]
```

### Comparing `lassen-0.2.7/lassen/stubs/generators/store.py` & `lassen-0.2.8/lassen/stubs/generators/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 import pydantic
 import sqlalchemy
 import sqlalchemy.ext.associationproxy
 import sqlalchemy.orm
 from inflection import underscore
 from jinja2 import Environment, FileSystemLoader, select_autoescape
+from uuid import UUID
 
+from lassen.db.columns import LassenUUID
 from lassen.db.base_class import Base as LassenBase
 from lassen.stubs.base import BaseDefinition, BaseGenerator, BaseStub, RenderedFile
 from lassen.stubs.definition import UniqueDefinition
 from lassen.stubs.field import UNSET_VALUE, FieldDefinition
 from lassen.stubs.generators.common import (
     ExtractedStubImports,
     extract_type_hints,
@@ -41,14 +43,15 @@
     int: sqlalchemy.Integer,
     float: sqlalchemy.Float,
     str: sqlalchemy.String,
     bool: sqlalchemy.Boolean,
     datetime: sqlalchemy.DateTime,
     Any: sqlalchemy.JSON,
     dict: sqlalchemy.JSON,
+    UUID: LassenUUID,
 }
 
 
 class StoreGenerator(BaseGenerator):
     origin_mapping = DEFAULT_ORIGIN_MAPPING
 
     def __init__(
@@ -117,21 +120,26 @@
                 if self not in field.generators:
                     continue
 
             typehint = typehints[name]
             mapped_typehint, dependencies1 = format_typehint_as_string(typehint)
             dependencies |= set(dependencies1)
 
-            # Since we want SQLAlchemy to translate the exact typehint into the column, we need to check
-            # for exact class equality (versus a subclass like with isinstance)
-            # One specific case where this happens is Enum - it is a VARCHAR in the backend, so isinstance(enum_field, sqlalchemy.String)
-            # is True. At runtime, SQLAlchemy won't auto resolve this Enum to a String and needs the explicit definition
-            # of the mapped_column(Enum(XX))
+            # Since we want SQLAlchemy to translate the exact typehint into the column,
+            # we need to check for exact class equality (versus a subclass like
+            # with isinstance)
+            # One specific case where this happens is Enum - it is a VARCHAR in the
+            # backend, so isinstance(enum_field, sqlalchemy.String) is True. At runtime,
+            # SQLAlchemy won't auto resolve this Enum to a String and needs the explicit
+            # definition of the mapped_column(Enum(XX))
             if not isinstance(field.association_proxy, UNSET_VALUE):
-                declaration = f"{name}: AssociationProxy[{mapped_typehint}] = association_proxy('{field.association_proxy[0]}', '{field.association_proxy[1]}')"
+                declaration = (
+                    f"{name}: AssociationProxy[{mapped_typehint}] = association_proxy"
+                    f"('{field.association_proxy[0]}', '{field.association_proxy[1]}')"
+                )
                 dependencies |= {
                     format_import(sqlalchemy.ext.associationproxy.AssociationProxy),
                     format_import(sqlalchemy.ext.associationproxy.association_proxy),
                 }
             elif field.is_relationship:
                 (
                     column_typehint,
@@ -139,42 +147,46 @@
                     dependencies2,
                 ) = self.format_column_for_sqlalchemy(typehint)
                 dependencies |= set(dependencies2)
 
                 mapped_typehint = mapped_typehint.strip("'")
                 declaration = f"{name}: Mapped['{mapped_typehint}']"
 
-                # The foreign key should point to another field on the model, which during runtime
-                # corresponds to a FieldDefinition instance
+                # The foreign key should point to another field on the model, which
+                # during runtime corresponds to a FieldDefinition instance
                 foreign_key_name = instance_to_name.get(id(field.foreign_key))
                 if not foreign_key_name:
                     raise ValueError(
                         f"Unable to find {field.foreign_key} in model {model.__name__}"
                     )
 
                 extra_kwargs: dict[str, Any] = {}
                 if not isinstance(field.backref, UNSET_VALUE):
                     extra_kwargs["backref"] = field.backref
 
                 dependencies.add(format_import(sqlalchemy.orm.relationship))
-                declaration += f" = relationship('{mapped_typehint}', foreign_keys=[{foreign_key_name}], {format_dict_as_kwargs(extra_kwargs)})"
+                declaration += (
+                    f" = relationship('{mapped_typehint}',"
+                    f" foreign_keys=[{foreign_key_name}],"
+                    f" {format_dict_as_kwargs(extra_kwargs)})"
+                )
             else:
                 (
                     column_typehint,
                     column_class,
                     dependencies2,
                 ) = self.format_column_for_sqlalchemy(typehint)
                 dependencies |= set(dependencies2)
 
                 declaration = f"{name}: Mapped[{mapped_typehint}]"
 
                 args = []
                 keyword_args = {}
 
-                if column_typehint and not column_class.__class__ in AUTO_CAST:
+                if column_typehint and column_class.__class__ not in AUTO_CAST:
                     args = [column_typehint]
 
                 if not isinstance(field.primary_key, UNSET_VALUE):
                     keyword_args["primary_key"] = True
                 if not isinstance(field.default, UNSET_VALUE):
                     keyword_args["default"] = field.default
                 if not isinstance(field.foreign_key, UNSET_VALUE):
@@ -213,15 +225,16 @@
         for _, definition in definitions:
             if isinstance(definition, UniqueDefinition):
                 field_names = [
                     f"'{instance_to_name[id(field)]}'" for field in definition.fields
                 ]
 
                 declarations.append(
-                    f"UniqueConstraint({', '.join(field_names)}, name='{definition.name}')"
+                    f"UniqueConstraint({', '.join(field_names)},"
+                    f" name='{definition.name}')"
                 )
                 dependencies.add(
                     format_import(sqlalchemy.UniqueConstraint),
                 )
 
         return declarations, list(dependencies)
 
@@ -233,15 +246,14 @@
         instance_variable: list[tuple[str, Any]] = list(inspect.getmembers(model))
 
         return {id(field): name for name, field in instance_variable}
 
     def format_column_for_sqlalchemy(
         self, typehint: Any
     ) -> tuple[str, Any, list[str | None]]:
-        print("GOT TYPEHINT", typehint)
         if inspect.isclass(typehint) and issubclass(typehint, enum.Enum):
             enum_handler = self.origin_mapping[enum.Enum]
             return (
                 f"{enum_handler.__name__}({typehint.__name__})",
                 enum_handler(typehint),
                 [format_import(enum_handler)],
             )
@@ -252,14 +264,21 @@
                 # Don't import other class dependencies for now
                 # TODO: Add typehinting only support here for their new file paths
                 [],
             )
         elif typehint in [int, float, str, bool, datetime, Any]:
             raw_class = self.origin_mapping[typehint]
             return (f"{raw_class.__name__}()", raw_class(), [format_import(raw_class)])
+        elif typehint == UUID:
+            raw_class = self.origin_mapping[typehint]
+            return (
+                f"{raw_class.__name__}(as_uuid=True)",
+                raw_class(as_uuid=True),
+                [format_import(raw_class)],
+            )
         elif isinstance(typehint, str):
             # Forward reference, assume this is to another class
             return (f"'{typehint}'", typehint, [])
         elif (
             inspect.isclass(typehint)
             and issubclass(typehint, pydantic.BaseModel)
             and not issubclass(typehint, BaseStub)
@@ -279,15 +298,16 @@
                 if len(unique_args) > 1:
                     raise ValueError("Lists with multiple types are not supported")
                 if (
                     args
                     and inspect.isclass(args[0])
                     and issubclass(args[0], pydantic.BaseModel)
                 ):
-                    # If the sub-model is a pydantic value we should format as a regular json blob
+                    # If the sub-model is a pydantic value we should format as a regular
+                    # json blob
                     return self.format_column_for_sqlalchemy(Any)
                 elif args and isinstance(args[0], type):
                     list_handler = self.origin_mapping[list]
                     (
                         cast_arg,
                         cast_class_arg,
                         dependencies,
@@ -301,15 +321,15 @@
             elif origin is dict or origin is Dict:
                 raw_class = self.origin_mapping[dict]
                 return (
                     f"{raw_class.__name__}()",
                     raw_class(),
                     [format_import(raw_class)],
                 )
-            elif origin is typing.Union or origin == types.UnionType:
+            elif origin is typing.Union or origin == types.UnionType:  # noqa E721
                 # Assumes that all Union types are nullable
                 nullable_args = [arg for arg in args if arg is not type(None)]
                 if len(nullable_args) > 1:
                     raise ValueError(
                         "Unions with multiple non-None types are not supported"
                     )
                 (
```

### Comparing `lassen-0.2.7/lassen/stubs/templates/schema.py.j2` & `lassen-0.2.8/lassen/stubs/templates/schema.py.j2`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/stubs/templates/sqlalchemy.py.j2` & `lassen-0.2.8/lassen/stubs/templates/sqlalchemy.py.j2`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc` & `lassen-0.2.8/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/__pycache__/fixtures.cpython-310.pyc` & `lassen-0.2.8/lassen/tests/__pycache__/fixtures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc` & `lassen-0.2.8/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/conftest.py` & `lassen-0.2.8/lassen/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,19 @@
     for key, value in settings.dict().items():
         if value:
             if isinstance(value, list):
                 value = json_dumps(value)
             else:
                 value = str(value)
 
-            print(f"Test Env: Will set `{key}` = `{value}`")
+            print(f"Test Env: Will set `{key}` = `{value}`")  # noqa
             environ[key] = value
 
-    # We don't have a client-specific settings object, so we'll just back-register the core settings
+    # We don't have a client-specific settings object, so we'll just back-register
+    # the core settings
     register_settings(CoreSettings)
 
 
 @pytest.fixture()
 def db_session():
     with get_db_context() as db:
         # Drop the alembic specific tables
```

### Comparing `lassen-0.2.7/lassen/tests/datasets/test_dataset_helpers.py` & `lassen-0.2.8/lassen/tests/datasets/test_dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/datasets/test_pyarrow_schemas.py` & `lassen-0.2.8/lassen/tests/datasets/test_pyarrow_schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,16 @@
             True,
         ),
     ],
 )
 def test_get_schema_from_dataclass(field_type: Any, field_value: Any):
     """
     Ensure we can correctly convert a dataclass to a pyarrow schema and then cast
-    the dataclass object into a table. If this fails it will raise a pyarrow.lib.ArrowInvalid.
+    the dataclass object into a table. If this fails it will raise a
+    pyarrow.lib.ArrowInvalid.
 
     """
 
     @dataclass
     class ExampleSchema:
         field: field_type
```

### Comparing `lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema.py` & `lassen-0.2.8/lassen/tests/fixtures/stubs/expected_schema.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema_public.py` & `lassen-0.2.8/lassen/tests/fixtures/stubs/expected_schema_public.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/fixtures/stubs/expected_store.py` & `lassen-0.2.8/lassen/tests/fixtures/stubs/expected_store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/fixtures/stubs/fixtures.py` & `lassen-0.2.8/lassen/tests/fixtures/stubs/fixtures.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py` & `lassen-0.2.8/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py` & `lassen-0.2.8/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/model_fixtures.py` & `lassen-0.2.8/lassen/tests/model_fixtures.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/stubs/generators/test_common.py` & `lassen-0.2.8/lassen/tests/stubs/generators/test_common.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/stubs/generators/test_schema.py` & `lassen-0.2.8/lassen/tests/stubs/generators/test_schema.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/stubs/generators/test_store.py` & `lassen-0.2.8/lassen/tests/stubs/generators/test_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import datetime
 from enum import Enum
 from typing import Any, Dict, List
 
 import pytest
 import sqlalchemy
 from pydantic import BaseModel
+from uuid import UUID
 
 from lassen.stubs.base import BaseStub
 from lassen.stubs.definition import UniqueDefinition
 from lassen.stubs.field import Field
 from lassen.stubs.generators.common import ExtractedStubImports
 from lassen.stubs.generators.store import DEFAULT_ORIGIN_MAPPING, StoreGenerator
+from lassen.db.columns import LassenUUID
 
 
 class SimpleEnum(Enum):
     TEST = "TEST"
 
 
 class SimplePydanticModel(BaseModel):
@@ -31,26 +33,28 @@
         (List[str], "ARRAY(String())", sqlalchemy.ARRAY(sqlalchemy.String())),
         (str | None, "String()", sqlalchemy.String()),
         (Any, "JSON()", sqlalchemy.JSON()),
         (dict[str, str], "JSON()", sqlalchemy.JSON()),
         (Dict[str, str], "JSON()", sqlalchemy.JSON()),
         (SimplePydanticModel, "JSON()", sqlalchemy.JSON()),
         (list[SimplePydanticModel], "JSON()", sqlalchemy.JSON()),
+        (UUID, "LassenUUID(as_uuid=True)", LassenUUID()),
     ],
 )
 def test_format_column_for_sqlalchemy(typehint, expected_str, expected_class):
     store_generator = StoreGenerator("test")
     (
         formatted_column,
         class_value,
         dependencies,
     ) = store_generator.format_column_for_sqlalchemy(typehint)
 
     assert formatted_column == expected_str
-    # Since the classes are fully instantiated separately and therefore fail exact equality, compare the string values
+    # Since the classes are fully instantiated separately and therefore fail exact
+    # equality, compare the string values
     assert str(class_value) == str(expected_class)
     assert len(dependencies) > 0
 
 
 def test_format_column_for_sqlalchemy_custom_type():
     # Assert that our custom class isn't in the default mapping, otherwise
     # this test doesn't verify the intended behavior
@@ -66,15 +70,16 @@
     (
         formatted_column,
         class_value,
         dependencies,
     ) = store_generator.format_column_for_sqlalchemy(datetime.date)
 
     assert formatted_column == "Date()"
-    # Since the classes are fully instantiated separately and therefore fail exact equality, compare the string values
+    # Since the classes are fully instantiated separately and therefore fail
+    # exact equality, compare the string values
     assert str(class_value) == str(sqlalchemy.Date())
     assert len(dependencies) > 0
 
 
 def test_generate_relationship() -> None:
     class MyParentModel(BaseStub):
         pass
@@ -89,17 +94,17 @@
     definition = store_generator(MyChildModel, ExtractedStubImports([], []))
 
     assert (
         "user_parent_id: Mapped[int] = mapped_column(ForeignKey('my_parent_model.id'))"
         in definition.content
     )
     assert (
-        "user_parent: Mapped['MyParentModel'] = relationship('MyParentModel', foreign_keys=[user_parent_id], )"
-        in definition.content
-    )
+        "user_parent: Mapped['MyParentModel'] ="
+        " relationship('MyParentModel', foreign_keys=[user_parent_id], )"
+    ) in definition.content
 
 
 def test_get_model_table_args() -> None:
     class MyModel(BaseStub):
         unique_text: str = Field()
 
         my_unique_constraint = UniqueDefinition(
```

### Comparing `lassen-0.2.7/lassen/tests/stubs/test_generate.py` & `lassen-0.2.8/lassen/tests/stubs/test_generate.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/test_alembic.py` & `lassen-0.2.8/lassen/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.7/lassen/tests/test_store.py` & `lassen-0.2.8/lassen/tests/test_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,18 +38,18 @@
     test_model_id = create_batch(db_session, quantity=1)[0]
 
     store = StoreBase[SampleModel, SampleSchemaCreate, SampleSchemaUpdate](SampleModel)
     # Test with a valid ID
     retrieved = store.get(db_session, id=test_model_id)
     assert retrieved is not None
     assert retrieved.id == test_model_id
-    assert retrieved.name == f"Test Model 0"
+    assert retrieved.name == "Test Model 0"
 
     # Test with an invalid ID
-    assert store.get(db_session, id=9999) == None
+    assert store.get(db_session, id=9999) is None
 
 
 def test_store_base_get_multi(db_session: Session, use_fixture_models):
     create_batch(db_session, quantity=5)
 
     store = StoreFilterMixin[SampleModel, SampleSchemaFilter](SampleModel)
     # Test without skip and limit
```

### Comparing `lassen-0.2.7/pyproject.toml` & `lassen-0.2.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "lassen"
-version = "0.2.7"
+version = "0.2.8"
 description = "Common webapp scaffolding."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
+[tool.ruff]
+select = ["E", "F", "T20"]
+
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.99.0"
 pydantic = "^1.10.2"
 inflection = "^0.5.1"
 click = "^8.1.3"
 alembic = "^1.11.1"
@@ -24,36 +27,30 @@
 Jinja2 = "^3.1.2"
 
 [tool.poetry.extras]
 datasets = ["datasets", "numpy", "pandas"]
 database = ["SQLAlchemy", "psycopg2"]
 
 [tool.poetry.group.dev.dependencies]
-isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
-autoflake = "^2.1.1"
 types-setuptools = "^67.8.0.0"
 pandas-stubs = "^2.0.2.230605"
+ruff = "^0.0.280"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 migrate = "lassen.alembic.cli:main"
 generate-lassen = "lassen.stubs.generate:cli"
 
-[tool.isort]
-profile = "black"
-known_first_party = "lassen"
-multi_line_output=3
-
 [tool.mypy]
 exclude = "fixtures"
 
 [[tool.mypy.overrides]]
 module = "pyarrow.*"
 ignore_missing_imports = true
```

### Comparing `lassen-0.2.7/setup.py` & `lassen-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 entry_points = \
 {'console_scripts': ['generate-lassen = lassen.stubs.generate:cli',
                      'migrate = lassen.alembic.cli:main']}
 
 setup_kwargs = {
     'name': 'lassen',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'Common webapp scaffolding.',
     'long_description': '# lassen\n\n**40.4881° N, 121.5049° W**\n\nCore utilities for MonkeySee web applications.\n\nNot guaranteed to be backwards compatible, use at your own risk.\n\n## Structure\n\n**Stores:** Each datamodel is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`\n- StoreBase: Base class for all stores\n- StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter\n\n**Schemas:** Each datamodel should define a Model class (SQLAlchemy base object) and a series of Schema objects (Pydantic) that allow the Store to serialize the models. These schemas are also often used for direct CRUD referencing in the API layer.\n\nWe use a base `Stub` file to generate these schemas from a centralized definition. When defining generators you should use a path that can be fully managed by lassen, since we will remove and regenerate these files on each run.\n\n```python\nSTORE_GENERATOR = StoreGenerator("models/auto")\nSCHEMA_GENERATOR = SchemaGenerator("schemas/auto")\n```\n\n```bash\npoetry run generate-lassen\n```\n\n**Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:\n\n- batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.\n- examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can\'t automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.\n\n```python\nfrom lassen.datasets import batch_to_examples, examples_to_batch\nimport pandas as pd\n\n@dataclass\nclass BatchInsertion:\n    texts: list[str]\n\ndef batch_process(examples):\n    new_examples : list[BatchInsertion] = []\n    for example in batch_to_examples(examples):\n        new_examples.append(\n            BatchInsertion(\n                example["raw_text"].split()\n            )\n        )\n\n    # datasets won\'t be able to typehint a dataset that starts with an empty example, so we use our explicit schema to cast the data\n    return examples_to_batch(new_examples, BatchInsertion, explicit_schema=True)\n\ndf = pd.DataFrame(\n    [\n        {"raw_text": ""},\n        {"raw_text": "This is a test"},\n        {"raw_text": "This is another test"},\n    ]\n)\n\ndataset = Dataset.from_pandas(df)\n\ndataset = dataset.map(\n    batch_process,\n    batched=True,\n    batch_size=1,\n    num_proc=1,\n    remove_columns=dataset.column_names,\n)\n```\n\n**Migrations:** Lassen includes a templated alembic.init and env.py file. Client applications just need to have a `migrations` folder within their project root. After this you can swap `poetry run alembic` with `poetry run migrate`.\n\n```sh\npoetry run migrate upgrade head\n```\n\n**Settings:** Application settings should subclass our core settings. This provides a standard way to load settings from environment variables and includes common database keys.\n\n```python\nfrom lassen.core.config import CoreSettings, register_settings\n\n@register_settings\nclass ClientSettings(CoreSettings):\n    pass\n```\n\n**Schemas:** For helper schemas when returning results via API, see [lassen.schema](./lassen/schema.py).\n\n## Development\n\n```sh\npoetry install --extras "datasets"\n\ncreateuser lassen\ncreatedb -O lassen lassen_db\ncreatedb -O lassen lassen_test_db\n```\n\nUnit Tests:\n\n```sh\npoetry run pytest\n```\n',
     'author': 'Pierce Freeman',
     'author_email': 'pierce@freeman.vc',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lassen-0.2.7/PKG-INFO` & `lassen-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lassen
-Version: 0.2.7
+Version: 0.2.8
 Summary: Common webapp scaffolding.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: database
 Provides-Extra: datasets
```


# Comparing `tmp/ursactl-0.6.0.tar.gz` & `tmp/ursactl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-ievhknl6/ursactl-0.6.0.tar", last modified: Tue Jul 25 12:15:45 2023, max compression
+gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-rag1gs69/ursactl-0.7.0.tar", last modified: Tue Aug  8 23:22:11 2023, max compression
```

## Comparing `ursactl-0.6.0.tar` & `ursactl-0.7.0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/
--rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.6.0/CHANGELOG.md
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.6.0/LICENSE.md
--rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.6.0/MANIFEST.in
--rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-07-25 12:15:45.000000 ursactl-0.6.0/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1675 2023-07-25 12:15:23.000000 ursactl-0.6.0/README.md
--rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.6.0/pyproject.toml
--rw-r--r--   0 jgsmith    (501) staff       (20)      168 2023-07-25 12:15:23.000000 ursactl-0.6.0/requirements-dev.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.6.0/requirements.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)     1287 2023-07-25 12:15:45.000000 ursactl-0.6.0/setup.cfg
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/tests/
--rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.6.0/tests/test_ursactl.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/airflow_provider/
--rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/airflow_provider/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/airflow_provider/hooks.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/controllers/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/controllers/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.6.0/ursactl/controllers/base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/create.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.6.0/ursactl/controllers/delete.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.6.0/ursactl/controllers/get.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1224 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/controllers/init.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.6.0/ursactl/controllers/list.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.6.0/ursactl/controllers/refresh.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2297 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/controllers/run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/controllers/send.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/show.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.6.0/ursactl/controllers/stop.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8140 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/controllers/sync.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/update.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/controllers/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.6.0/ursactl/controllers/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/utils/transforms.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/core/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/core/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/agent.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2345 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/core/dataset.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.6.0/ursactl/core/exc.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2023 2023-07-20 15:12:38.000000 ursactl-0.6.0/ursactl/core/pipeline.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1793 2023-07-20 12:42:32.000000 ursactl-0.6.0/ursactl/core/pipeline_run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1967 2023-07-20 12:42:32.000000 ursactl-0.6.0/ursactl/core/pipeline_sweep.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4578 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/core/project.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1010 2023-07-20 12:42:32.000000 ursactl-0.6.0/ursactl/core/running_agent.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/core/services/
--rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/core/services/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-25 12:10:01.000000 ursactl-0.6.0/ursactl/core/services/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    32379 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/core/services/ape_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/services/dss_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/services/iam_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/core/services/planning_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/core/services/project_client.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/core/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.6.0/ursactl/core/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.6.0/ursactl/core/utils/magic.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/core/version.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/ext/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/ext/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4269 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/main.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/plugins/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/plugins/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/templates/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/templates/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/
--rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1603 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/SOURCES.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/dependency_links.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/entry_points.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/requires.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/top_level.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.6.0/ursactl.egg-info/zip-safe
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/
+-rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.7.0/CHANGELOG.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.7.0/LICENSE.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.7.0/MANIFEST.in
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-08-08 23:22:11.000000 ursactl-0.7.0/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1675 2023-07-25 12:15:23.000000 ursactl-0.7.0/README.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.7.0/pyproject.toml
+-rw-r--r--   0 jgsmith    (501) staff       (20)      168 2023-07-25 12:15:23.000000 ursactl-0.7.0/requirements-dev.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.7.0/requirements.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1287 2023-08-08 23:22:11.000000 ursactl-0.7.0/setup.cfg
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/tests/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.7.0/tests/test_ursactl.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.7.0/ursactl/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/airflow_provider/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      434 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/airflow_provider/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-08-01 15:14:48.000000 ursactl-0.7.0/ursactl/airflow_provider/hooks.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/controllers/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.7.0/ursactl/controllers/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.7.0/ursactl/controllers/base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8647 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/create.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.7.0/ursactl/controllers/delete.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.7.0/ursactl/controllers/get.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1334 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/init.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8063 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/list.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.7.0/ursactl/controllers/refresh.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2297 2023-07-25 12:15:23.000000 ursactl-0.7.0/ursactl/controllers/run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.7.0/ursactl/controllers/send.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.7.0/ursactl/controllers/show.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.7.0/ursactl/controllers/stop.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     9517 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/sync.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     5853 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/update.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/controllers/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.7.0/ursactl/controllers/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1299 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/utils/pages.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     5427 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/controllers/utils/transforms.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/core/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.7.0/ursactl/core/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.7.0/ursactl/core/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.7.0/ursactl/core/agent.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2345 2023-07-20 19:45:48.000000 ursactl-0.7.0/ursactl/core/dataset.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.7.0/ursactl/core/exc.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2023 2023-07-20 15:12:38.000000 ursactl-0.7.0/ursactl/core/pipeline.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1793 2023-07-20 12:42:32.000000 ursactl-0.7.0/ursactl/core/pipeline_run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1967 2023-07-20 12:42:32.000000 ursactl-0.7.0/ursactl/core/pipeline_sweep.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4578 2023-07-25 12:15:23.000000 ursactl-0.7.0/ursactl/core/project.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1010 2023-07-20 12:42:32.000000 ursactl-0.7.0/ursactl/core/running_agent.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/core/services/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      931 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/core/services/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1843 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/core/services/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    33358 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/core/services/ape_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.7.0/ursactl/core/services/dss_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.7.0/ursactl/core/services/iam_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     6760 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/core/services/page_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.7.0/ursactl/core/services/planning_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.7.0/ursactl/core/services/project_client.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/core/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.7.0/ursactl/core/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.7.0/ursactl/core/utils/magic.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-08-08 23:22:03.000000 ursactl-0.7.0/ursactl/core/version.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/ext/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.7.0/ursactl/ext/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4269 2023-07-20 19:45:48.000000 ursactl-0.7.0/ursactl/main.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/plugins/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.7.0/ursactl/plugins/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl/templates/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.7.0/ursactl/templates/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1675 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/SOURCES.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/dependency_links.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/entry_points.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/requires.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-08-08 23:22:11.000000 ursactl-0.7.0/ursactl.egg-info/top_level.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.7.0/ursactl.egg-info/zip-safe
```

### Comparing `ursactl-0.6.0/PKG-INFO` & `ursactl-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.6.0
+Version: 0.7.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Home-page: https://ursafrontier.cloud/
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `ursactl-0.6.0/README.md` & `ursactl-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/setup.cfg` & `ursactl-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/airflow_provider/hooks.py` & `ursactl-0.7.0/ursactl/airflow_provider/hooks.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/base.py` & `ursactl-0.7.0/ursactl/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/create.py` & `ursactl-0.7.0/ursactl/controllers/create.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from cement import Controller, ex
 import json
 import yaml
 
 from ..core.services import client
 from ..core.utils.magic import magic
 from ursactl.controllers.utils.transforms import load_transform
+from ursactl.controllers.utils.pages import load_page
 
 
 def _yaml_load(fd):
     return list(yaml.load_all(fd, Loader=yaml.Loader))
 
 
 class Create(Controller):
@@ -39,20 +40,20 @@
         elif file.endswith('.json'):
             loader = json.load
         else:
             print("Only YAML and JSON files may be uploaded.")
             sys.exit(1)
 
         with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+            pages = loader(fd)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'name': content['name'],
                 'packages': content['packages'],
                 'behaviors': content['behaviors'],
                 'project_uuid': project_uuid,
             }
 
@@ -65,38 +66,35 @@
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def transform(self):
         project_uuid = self._project_scope
         ape_client = client('ape', self.app)
 
         file = self.app.pargs.file
-        documents = load_transform(file)
+        pages = load_transform(file)
 
-        if documents is None:
+        if pages is None:
             print(f"Unable to load transform from {file}")
             sys.exit(1)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'path': content['path'],
                 'name': content['name'],
                 'type': content['type'],
                 'implementation': content['implementation'],
                 'configuration_schema': content['configurationSchema'],
                 'project_uuid': project_uuid,
             }
-            if 'outputs' in content:
-                args['outputs'] = content['outputs']
-            if 'inputs' in content:
-                args['inputs'] = content['inputs']
-            if 'description' in content:
-                args['description'] = content['description']
+            for key in ['outputs', 'inputs', 'description', 'tags']:
+                if key in content:
+                    args[key] = content[key]
 
             result = ape_client.create_transform(**args)
             self._print(result)
 
     @ex(help='create dataset',
         arguments=[
             (['source'], {'help': 'dataset to upload', 'action': 'store'}),
@@ -109,14 +107,44 @@
         path = self.app.pargs.path
         source = self.app.pargs.source
         dss_client = client('dss', self.app)
         file_type = self.app.pargs.file_type or magic(source)
         result = dss_client.create_dataset(project_uuid=project_uuid, path=path, data=source, data_type=file_type)
         self._print(result)
 
+    @ex(help='create a new page',
+        arguments=[
+            (['file'], {'help': 'page definition file', 'action': 'store'}),
+            (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
+        ])
+    def page(self):
+        project_uuid = self._project_scope
+        page_client = client('page', self.app)
+
+        file = self.app.pargs.file
+        if file.endswith('.md'):
+            page = load_page(file)
+        else:
+            print("Only Markdown files may be uploaded.")
+            sys.exit(1)
+
+        args = {
+            'path': page['path'],
+            'content': page['content'],
+            'project_uuid': project_uuid,
+        }
+
+        if 'title' in page:
+            args['title'] = page['title']
+        if 'tags' in page:
+            args['tags'] = page['tags']
+
+        result = page_client.create_page(**args)
+        self._print(result)
+
     @ex(help='create a new package from a file',
         arguments=[
             (['file'], {'help': 'package definition file', 'action': 'store'}),
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def package(self):
         project_uuid = self._project_scope
@@ -157,29 +185,29 @@
         elif file.endswith('.json'):
             loader = json.load
         else:
             print("Only YAML and JSON files may be uploaded.")
             sys.exit(1)
 
         with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+            pages = loader(fd)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'path': content['path'],
                 'transform': content['transform']['path'],
                 'transform_configuration': content['transform']['configuration'],
                 'load': content['load'],
                 'project_uuid': self._project_scope
             }
 
-            for key in ['extract', 'description']:
+            for key in ['extract', 'description', 'tags']:
                 if key in content and content[key] is not None:
                     args[key] = content[key]
 
             result = ape_client.create_generator(**args)
             self._print(result)
 
     @ex(help='create a pipeline from a file',
@@ -196,26 +224,26 @@
         elif file.endswith('.json'):
             loader = json.load
         else:
             print("Only YAML and JSON files may be uploaded.")
             sys.exit(1)
 
         with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+            pages = loader(fd)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'path': content['path'],
                 'project_uuid': self._project_scope
             }
 
-            for key in ['seeders', 'generators', 'description']:
+            for key in ['seeders', 'generators', 'description', 'tags']:
                 if key in content and content[key] is not None:
                     args[key] = content[key]
 
             result = ape_client.create_pipeline(**args)
             self._print(result)
 
     def _print(self, data):
```

### Comparing `ursactl-0.6.0/ursactl/controllers/delete.py` & `ursactl-0.7.0/ursactl/controllers/delete.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/get.py` & `ursactl-0.7.0/ursactl/controllers/get.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/init.py` & `ursactl-0.7.0/ursactl/controllers/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,12 +31,15 @@
             sys.exit(1)
 
         for subdir in (
                        'data/transforms',
                        'data/generators',
                        'data/pipelines',
                        'data/datasets',
+                       'data/pages',
                        'planning/packages',
-                       'planning/agents'
+                       'planning/agents',
+                       'planning/pages',
+                       'pages'
         ):
             (root / subdir).mkdir(parents=True, exist_ok=True)
             (root / subdir / '.keep').touch()
```

### Comparing `ursactl-0.6.0/ursactl/controllers/list.py` & `ursactl-0.7.0/ursactl/controllers/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         planning_client = client('planning', self.app)
 
         agents = planning_client.list_agents(project_uuid=self._project_scope)
         if self.app.pargs.output is None:
             data = []
             for item in agents:
                 data.append(
-                    [item['name'], item['id']]
+                    [item['name']]
                 )
             data.sort()
-            self.app.render(data, headers=['Name', 'UUID'])
+            self.app.render(data, headers=['Name'])
         else:
             self._print(agents)
 
     @ex(help='list transforms',
         arguments=[
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
@@ -65,37 +65,60 @@
         dss_client = client('dss', self.app)
         datasets = dss_client.list_datasets(self._project_scope)
 
         if self.app.pargs.output is None:
             data = []
             for item in datasets:
                 data.append(
-                    [item['path'], item['id'], item['size'], item['content_type']]
+                    [item['path'], item['size'], item['content_type']]
                 )
             data.sort()
-            self.app.render(data, headers=['Path', 'UUID', 'Size', 'Type'])
+            self.app.render(data, headers=['Path', 'Size', 'Type'])
         else:
             self._print(list(datasets))
 
+    @ex(help='list pages',
+        arguments=[
+            (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
+        ])
+    def pages(self):
+        page_client = client('page', self.app)
+
+        pages = page_client.list_pages(project_uuid=self._project_scope)
+        if self.app.pargs.output is None:
+            data = []
+            for item in pages:
+                data.append(
+                    [item['path'], item['title']]
+                )
+            data.sort()
+            self.app.render(data, headers=['Path', 'Title'])
+        else:
+            self._print(pages)
+
     @ex(help='list generators',
         arguments=[
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def generators(self):
         ape_client = client('ape', self.app)
 
         generators = ape_client.list_generators(project_uuid=self._project_scope)
         if self.app.pargs.output is None:
             data = []
             for item in generators:
                 data.append(
-                    [item['path'], item['id'], item['transform']['type'], item['transform']['path']]
+                    [
+                        item['path'],
+                        item['transform']['type'],
+                        self._transform_name(item['transform'])
+                    ]
                 )
             data.sort()
-            self.app.render(data, headers=['Path', 'UUID', 'Type', 'transform'])
+            self.app.render(data, headers=['Path', 'Type', 'transform'])
         else:
             self._print(generators)
 
     @ex(help='list packages',
         arguments=[
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
@@ -103,18 +126,18 @@
         planning_client = client('planning', self.app)
 
         packages = planning_client.list_packages(project_uuid=self._project_scope)
         if self.app.pargs.output is None:
             data = []
             for item in packages:
                 data.append(
-                    [item['name'], item['id']]
+                    [item['name']]
                 )
             data.sort()
-            self.app.render(data, headers=['Name', 'UUID'])
+            self.app.render(data, headers=['Name'])
         else:
             self._print(packages)
 
     @ex(help='list pipelines',
         arguments=[
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
@@ -122,18 +145,18 @@
         ape_client = client('ape', self.app)
 
         if self.app.pargs.output is None:
             pipelines = ape_client.list_pipelines(project_uuid=self._project_scope)
             data = []
             for item in pipelines:
                 data.append(
-                    [item['path'], item['id'], item['description']]
+                    [item['path'], item['description']]
                 )
             data.sort()
-            self.app.render(data, headers=['Path', 'UUID', 'Description'])
+            self.app.render(data, headers=['Path', 'Description'])
         else:
             pipelines = ape_client.list_pipelines(
                 project_uuid=self._project_scope,
                 all=True)
             self._print(pipelines)
 
     @ex(help='list projects')
@@ -201,7 +224,10 @@
         return scope
 
     def _print(self, data):
         if self.app.pargs.output == 'json':
             print(json_dump(data))
         else:
             print(yaml_dump(data))
+
+    def _transform_name(self, transform):
+        return f"{transform['project']['user']['handle']}/{transform['project']['name']}:{transform['path']}"
```

### Comparing `ursactl-0.6.0/ursactl/controllers/run.py` & `ursactl-0.7.0/ursactl/controllers/run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/send.py` & `ursactl-0.7.0/ursactl/controllers/send.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/show.py` & `ursactl-0.7.0/ursactl/controllers/show.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/stop.py` & `ursactl-0.7.0/ursactl/controllers/stop.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/controllers/sync.py` & `ursactl-0.7.0/ursactl/controllers/sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from cement import Controller
 import json
 import yaml
 
 from ..core.services import client
 import ursactl.controllers.utils.transforms
+import ursactl.controllers.utils.pages
 
 
 class Sync(Controller):
     """
     Provides the 'sync' verb
     """
 
@@ -41,92 +42,120 @@
             print("Error: %s does not exist." % root)
             sys.exit(1)
         elif not root.is_dir():
             print("Error: %s exists and is not a directory." % root)
             sys.exit(1)
 
         ape_client = client('ape', self.app)
+        page_client = client('page', self.app)
 
         resources = self._load_resources(root)
 
         if self.app.pargs.dry_run:
             print("Would sync:")
             print(yaml.dump({k: list(v.keys()) for k, v in resources.items() if len(v) > 0}))
             return
 
         # now we can sync resources
+        self._sync_pages(page_client, resources['page'])
         self._sync_datasets(resources['dataset'])
         self._sync_transforms(ape_client, resources['transform'])
         self._sync_generators(ape_client, resources['generator'])
         self._sync_pipelines(ape_client, resources['pipeline'])
 
+    def _is_synced(self, collection, path):
+        if path not in collection:
+            return False
+        if 'published' in collection[path] and not collection[path]['published']:
+            return False
+        return True
+
     def _sync_datasets(self, datasets):
         pass
 
+    def _sync_pages(self, client, pages):
+        for item in client.list_pages(self._project_scope):
+            if item['isSynced']:
+                if not self._is_synced(pages, item['path']):
+                    client.delete_synced_page(item['id'])
+            elif item['path'] in pages and not item['isSynced']:
+                print(f"Unable to sync page #{item['path']} because it is not synced.")
+                pages.delete(item['path'])
+        for item in pages.values():
+            args = {
+                'path': item['path'],
+                'content': item['content'],
+                'project_uuid': self._project_scope,
+            }
+
+            for key in ['title', 'tags']:
+                if key in item:
+                    args[key] = item[key]
+
+            result = client.sync_page(**args)
+            self._print(result)
+
     def _sync_transforms(self, client, transforms):
         for item in client.list_transforms(self._project_scope):
-            if item['path'] not in transforms and item['isSynced']:
+            if not self._is_synced(transforms, item['path']):
                 client.delete_synced_transform(item['id'])
             elif item['path'] in transforms and not item['isSynced']:
                 print(f"Unable to sync transform #{item['path']} because it is not synced.")
                 transforms.delete(item['path'])
         for item in transforms.values():
             args = {
                 'path': item['path'],
                 'name': item['name'],
                 'type': item['type'],
                 'implementation': item['implementation'],
                 'configuration_schema': item['configurationSchema'],
                 'project_uuid': self._project_scope,
             }
-            if 'outputs' in item:
-                args['outputs'] = item['outputs']
-            if 'inputs' in item:
-                args['inputs'] = item['inputs']
-            if 'description' in item:
-                args['description'] = item['description']
+            for key in ['outputs', 'inputs', 'description', 'tags']:
+                if key in item:
+                    args[key] = item[key]
             result = client.sync_transform(**args)
             self._print(result)
 
     def _sync_generators(self, client, generators):
         for item in client.list_generators(self._project_scope):
-            if item['path'] not in generators and item['isSynced']:
+            if not self._is_synced(generators, item['path']):
                 client.delete_synced_generator(item['id'])
             elif item['path'] in generators and not item['isSynced']:
                 print(f"Unable to sync generator #{item['path']} because it is not synced.")
                 generators.delete(item['path'])
         for item in generators.values():
             args = {
                 'path': item['path'],
                 'transform': item['transform']['path'],
                 'transform_configuration': item['transform']['configuration'],
                 'load': item['load'],
                 'project_uuid': self._project_scope
             }
 
-            for key in ['extract', 'description']:
+            for key in ['extract', 'description', 'tags']:
                 if key in item and item[key] is not None:
                     args[key] = item[key]
 
             result = client.sync_generator(**args)
             self._print(result)
 
     def _sync_pipelines(self, client, pipelines):
         for item in client.list_pipelines(self._project_scope):
-            if item['path'] not in pipelines and item['isSynced']:
+            if not self._is_synced(pipelines, item['path']):
                 client.delete_synced_pipeline(item['id'])
             elif item['path'] in pipelines and not item['isSynced']:
                 print(f"Unable to sync pipeline #{item['path']} because it is not synced.")
                 pipelines.delete(item['path'])
         for item in pipelines.values():
             args = {
                 'path': item['path'],
                 'project_uuid': self._project_scope
             }
-            for key in ['seeders', 'generators', 'description']:
+            for key in ['seeders', 'generators', 'description', 'tags']:
                 if key in item and item[key] is not None:
                     args[key] = item[key]
 
             result = client.sync_pipeline(**args)
             self._print(result)
 
     def _load_resources(self, root):  # noqa: C901
@@ -140,14 +169,15 @@
         # datasets are special, but the same file with the .yaml extension can house
         # the metadata (so foo.csv has a foo.csv.yaml metadata file)
         #
         # OR, for datasets, we can have an index.yaml file that lists all of the datasets
         # we want to sync along with their metadata. Or both, until we find out which one
         # users find easiest to use.
         resources = {
+            'page': {},
             'transform': {},
             'generator': {},
             'pipeline': {},
             'dataset': {},
         }
 
         for file in root.rglob("*"):
@@ -155,18 +185,22 @@
                 continue
             if file.stat().st_size == 0:
                 continue
             if file.name.startswith('.'):
                 continue
             info = None
             suffix = file.suffix
+            default_kind = self._get_kind(root, file, {})
             if suffix == '.md':
-                # likely a transform
+                # likely a transform or a page
                 with open(file, "r") as fd:
-                    info = ursactl.controllers.utils.transforms.load_from_markdown(fd)
+                    if default_kind == 'transform':
+                        info = ursactl.controllers.utils.transforms.load_from_markdown(fd)
+                    else:
+                        info = ursactl.controllers.utils.pages.load_from_markdown(fd)
             elif suffix == '.lua':
                 # likely a transform
                 with open(file, "r") as fd:
                     info = ursactl.controllers.utils.transforms.load_from_lua(fd)
             elif suffix in ['.yaml', '.yml']:
                 with open(file, "r") as fd:
                     info = list(yaml.load_all(fd, Loader=yaml.Loader))
@@ -187,15 +221,15 @@
         if info is None:
             return 'unknown'
         if 'kind' in info and info['kind'] not in [None, '']:
             return info['kind']
         if file.suffix in ['.yaml', '.yml'] and file.with_name(file.stem).exists():
             return 'dataset'
         bits = file.relative_to(root).parts
-        for type in ['transforms', 'generators', 'pipelines', 'datasets']:
+        for type in ['pages', 'transforms', 'generators', 'pipelines', 'datasets']:
             if type in bits:
                 return type[:-1]
         return 'unknown'
 
     @property
     def _project_scope(self):
         return self.app.pargs.project or self.app.config.get('ursactl', 'project')
```

### Comparing `ursactl-0.6.0/ursactl/controllers/update.py` & `ursactl-0.7.0/ursactl/controllers/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,38 +42,35 @@
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'})
         ])
     def transform(self):
         project_uuid = self._project_scope
         ape_client = client('ape', self.app)
 
         file = self.app.pargs.file
-        documents = load_transform(file)
+        pages = load_transform(file)
 
-        if documents is None:
+        if pages is None:
             print(f"Unable to load transform from {file}")
             sys.exit(1)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'path': content['path'],
                 'type': content['type'],
                 'name': content['name'],
                 'implementation': content['implementation'],
                 'configuration_schema': content['configurationSchema'],
                 'project_uuid': project_uuid,
             }
-            if 'outputs' in content:
-                args['outputs'] = content['outputs']
-            if 'inputs' in content:
-                args['inputs'] = content['inputs']
-            if 'description' in content:
-                args['description'] = content['description']
+            for key in ['description', 'inputs', 'outputs', 'tags']:
+                if key in content:
+                    args[key] = content[key]
 
             result = ape_client.update_transform(**args)
             self._print(result)
 
     @ex(help='update an existing generator from a file',
         arguments=[
             (['file'], {'help': 'generator definition file', 'action': 'store'}),
@@ -88,29 +85,29 @@
         elif file.endswith('.json'):
             loader = json.load
         else:
             print("Only YAML and JSON files may be uploaded.")
             sys.exit(1)
 
         with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+            pages = loader(fd)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'path': content['path'],
                 'transform': content['transform']['path'],
                 'transform_configuration': content['transform']['configuration'],
                 'load': content['load'],
                 'project_uuid': self._project_scope
             }
 
-            for key in ['extract', 'description']:
+            for key in ['extract', 'description', 'tags']:
                 if key in content and content[key] is not None:
                     args[key] = content[key]
 
             result = ape_client.update_generator(**args)
             self._print(result)
 
     @ex(help='update an existing package from a file',
@@ -144,26 +141,26 @@
         elif file.endswith('.json'):
             loader = json.load
         else:
             print("Only YAML and JSON files may be uploaded.")
             sys.exit(1)
 
         with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+            pages = loader(fd)
 
-        if not isinstance(documents, list):
-            documents = [documents]
+        if not isinstance(pages, list):
+            pages = [pages]
 
-        for content in documents:
+        for content in pages:
             args = {
                 'path': content['path'],
             }
             args['project_uuid'] = self._project_scope
 
-            for key in ['seeders', 'generators', 'description']:
+            for key in ['seeders', 'generators', 'description', 'tags']:
                 if key in content and content[key] is not None:
                     args[key] = content[key]
 
             result = ape_client.update_pipeline(**args)
             self._print(result)
 
     def _print(self, data):
```

### Comparing `ursactl-0.6.0/ursactl/controllers/utils/transforms.py` & `ursactl-0.7.0/ursactl/controllers/utils/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     elif file.endswith('.lua'):
         loader = load_from_lua
     else:
         print("Only YAML, JSON, Lua, and Markdown files may be uploaded.")
         sys.exit(1)
 
     with open(file, 'r', encoding='utf-8') as fd:
-        documents = loader(fd)
-    return documents
+        pages = loader(fd)
+    return pages
 
 
 def _yaml_load(fd):
     return list(yaml.load_all(fd, Loader=yaml.Loader))
 
 
 def load_from_lua(source):  # noqa: C901
@@ -120,14 +120,16 @@
         chunks = chunks[1:]
 
     info['name'] = name
 
     for chunk in chunks:
         _update_info_from_chunk(info, chunk)
 
+    info['kind'] = 'transform'
+
     return info
 
 
 def _update_info_from_chunk(info, chunk):
     if chunk[0].startswith('## Metadata'):
         info.update(yaml.load("".join(chunk[1:]), Loader=yaml.Loader))
     if chunk[0].startswith('## Configuration Schema'):
```

### Comparing `ursactl-0.6.0/ursactl/core/_base.py` & `ursactl-0.7.0/ursactl/core/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/agent.py` & `ursactl-0.7.0/ursactl/core/agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/dataset.py` & `ursactl-0.7.0/ursactl/core/dataset.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/pipeline.py` & `ursactl-0.7.0/ursactl/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/pipeline_run.py` & `ursactl-0.7.0/ursactl/core/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/pipeline_sweep.py` & `ursactl-0.7.0/ursactl/core/pipeline_sweep.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/project.py` & `ursactl-0.7.0/ursactl/core/project.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/running_agent.py` & `ursactl-0.7.0/ursactl/core/running_agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/services/__init__.py` & `ursactl-0.7.0/ursactl/core/services/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Manages service discovery.
 """
 from typing import Optional
 
 from .ape_client import ApeClient
+from .page_client import PageClient
 from .iam_client import IamClient
 from .planning_client import PlanningClient
 from .project_client import ProjectClient
 from .dss_client import DssClient
 
 SERVICE_CLIENTS = {
     'ape': ApeClient,
     'dss': DssClient,
+    'page': PageClient,
     'iam': IamClient,
     'planning': PlanningClient,
     'projects': ProjectClient
 }
 
 
 def client(service: Optional[str] = None, app=None):
```

### Comparing `ursactl-0.6.0/ursactl/core/services/_base.py` & `ursactl-0.7.0/ursactl/core/services/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         try:
             result = self.client.execute(query=query, variables=variables, headers={
                 "authorization": f"Bearer {self.iam_client.get_token()}"
             })
 
             if 'errors' in result:
                 for error in result['errors']:
-                    if error['code'] == 'Forbidden':
+                    if 'code' in error and error['code'] == 'Forbidden':
                         if reauthorize:
                             self.iam_client.clear_token()
                             return self.raw_query(query, variables, reauthorize=False)
                         raise UrsaNotAuthorized("Not authorized")
                     else:
                         print(error['message'])
         except requests.exceptions.HTTPError as e:
```

### Comparing `ursactl-0.6.0/ursactl/core/services/ape_client.py` & `ursactl-0.7.0/ursactl/core/services/ape_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     project(handleName: $id) {
         transforms {
             id
             name
             path
             type
             isSynced
+            tags
         }
     }
 }
 """
 
 CREATE_TRANSFORM_MUTATION = """\
 mutation create_transform($input: CreateTransformInput!) {
@@ -75,27 +76,31 @@
 GET_TRANSFORM_BY_ID_QUERY = """\
 query get_transform($id: ID!) {
     transform(id: $id) {
         path
         description
         configurationSchema
         type
+        tags
+        isSynced
     }
 }
 """
 
 GET_TRANSFORM_BY_PATH_QUERY = """\
 query get_transform($path: String!, $project: String!) {
     project(handleName: $project) {
         transforms(limit: 1, filter: { path: { eq: $path } }) {
             id
             path
             description
             configurationSchema
             type
+            tags
+            isSynced
         }
     }
 }
 """
 
 DELETE_TRANSFORM_MUTATION = """\
 mutation delete_transform($id: ID!) {
@@ -180,15 +185,16 @@
 LIST_GENERATORS_FOR_PROJECT_QUERY = """\
 query list_generators($id: String!) {
     project(handleName: $id) {
         generators {
             id
             path
             isSynced
-            transform
+            transform { type path project { name user { handle } } }
+            tags
         }
     }
 }
 """
 
 GET_GENERATOR_BY_ID_QUERY = """\
 query get_generator($id: ID!) {
@@ -327,14 +333,15 @@
 query pipelines($id: String!) {
   project(handleName: $id) {
     pipelines {
       path
       id
       description
       isSynced
+      tags
     }
   }
 }
 """
 
 LIST_PIPELINES_FOR_PROJECT_FULL_QUERY = """\
 query pipelines($id: String!) {
@@ -342,14 +349,15 @@
     pipelines {
       path
       id
       isSynced
       description
       seeders
       generators
+      tags
     }
   }
 }
 """
 
 RUN_PIPELINE_MUTATION = """\
 mutation run_pipeline($input: RunPipelineInput!){
@@ -504,15 +512,16 @@
                          name=None,
                          path=None,
                          inputs=None,
                          outputs=None,
                          implementation=None,
                          description=None,
                          configuration_schema=None,
-                         type=None):
+                         type=None,
+                         tags=None):
         """
         Create a transform. This will do some light checking before sending the
         request. More extensive checking is done on the server.
         """
         if project_uuid is None:
             raise AttributeError("transforms must be assigned to a project.")
         if type not in ["seeder", "mapper", "reducer"]:
@@ -535,28 +544,31 @@
         }
         if outputs is not None:
             variables['input']['outputs'] = dumps(outputs)
         if inputs is not None:
             variables['input']['inputs'] = dumps(inputs)
         if description is not None:
             variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
         result = self.raw_query(query=CREATE_TRANSFORM_MUTATION, variables=variables)
 
         return result['data']['createTransform']['result']
 
     def sync_transform(self,
                        project_uuid=None,
                        name=None,
                        path=None,
                        inputs=None,
                        outputs=None,
                        implementation=None,
                        description=None,
                        configuration_schema=None,
-                       type=None):
+                       type=None,
+                       tags=None):
         """
         Sync a transform. This will do some light checking before sending the
         request. More extensive checking is done on the server.
         """
         if project_uuid is None:
             raise AttributeError("transforms must be assigned to a project.")
         if type not in ["seeder", "mapper", "reducer"]:
@@ -579,28 +591,31 @@
         }
         if outputs is not None:
             variables['input']['outputs'] = dumps(outputs)
         if inputs is not None:
             variables['input']['inputs'] = dumps(inputs)
         if description is not None:
             variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
         result = self.raw_query(query=SYNC_TRANSFORM_MUTATION, variables=variables)
 
         return result['data']['syncTransform']['result']
 
-    def update_transform(self,
+    def update_transform(self,  # noqa: C901
                          project_uuid=None,
                          name=None,
                          path=None,
                          inputs=None,
                          outputs=None,
                          implementation=None,
                          description=None,
                          configuration_schema=None,
-                         type=None):
+                         type=None,
+                         tags=None):
         """
         Update a transform. This will do some light checking before sending the
         request. More extensive checking is done on the server.
         """
         if project_uuid is None:
             raise AttributeError("transforms must be assigned to a project.")
         if type not in ["seeder", "mapper", "reducer"]:
@@ -622,14 +637,16 @@
         }
         if outputs is not None:
             variables['input']['outputs'] = dumps(outputs)
         if inputs is not None:
             variables['input']['inputs'] = dumps(inputs)
         if description is not None:
             variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
         algo = self.get_transform(path=path, project_uuid=project_uuid)
         if algo is None:
             return {}
         variables['id'] = algo['id']
         result = self.raw_query(query=UPDATE_TRANSFORM_MUTATION, variables=variables)
 
         return result['data']['updateTransform']
@@ -689,15 +706,16 @@
     def create_generator(self,
                          project_uuid=None,
                          path=None,
                          description=None,
                          transform=None,
                          transform_configuration=None,
                          extract=None,
-                         load=None):
+                         load=None,
+                         tags=None):
         """
         Creates a generator. This will do some checking before sending the request to make sure
         the request is reasonable.
         """
         transform_rec = self.get_transform(project_uuid=project_uuid, path=transform)
         if transform_rec is None:
             raise ValueError(f"The transform ({transform}) is not defined.")
@@ -712,27 +730,30 @@
                 'transform': transform,
                 'configuration': dumps(transform_configuration),
                 'extract': extract,
                 'load': load
             }
         }
         if description is not None:
-            variables['input']['generator']['description'] = description
+            variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
         result = self.raw_query(query=CREATE_GENERATOR_MUTATION, variables=variables)
 
         return result['data']['createGenerator']
 
     def sync_generator(self,
                        project_uuid=None,
                        path=None,
                        description=None,
                        transform=None,
                        transform_configuration=None,
                        extract=None,
-                       load=None):
+                       load=None,
+                       tags=None):
         """
         Syncs a generator. This will do some checking before sending the request to make sure
         the request is reasonable.
         """
         transform_rec = self.get_transform(project_uuid=project_uuid, path=transform)
         if transform_rec is None:
             raise ValueError(f"The transform ({transform}) is not defined.")
@@ -747,28 +768,30 @@
                 'transform': transform,
                 'configuration': dumps(transform_configuration),
                 'extract': extract,
                 'load': load
             }
         }
         if description is not None:
-            variables['input']['generator']['description'] = description
-
+            variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
         result = self.raw_query(query=SYNC_GENERATOR_MUTATION, variables=variables)
 
         return result['data']['syncGenerator']
 
     def update_generator(self,
                          project_uuid=None,
                          path=None,
                          description=None,
                          transform=None,
                          transform_configuration=None,
                          extract=None,
-                         load=None):
+                         load=None,
+                         tags=None):
         """
         Creates a generator. This will do some checking before sending the request to make sure
         the request is reasonable.
         """
         transform_rec = self.get_transform(project_uuid=project_uuid, path=transform)
         if transform_rec is None:
             raise ValueError(f"The transform ({transform}) is not defined.")
@@ -782,15 +805,17 @@
                 'transform': transform,
                 'configuration': dumps(transform_configuration),
                 'extract': extract,
                 'load': load
             }
         }
         if description is not None:
-            variables['input']['generator']['description'] = description
+            variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
         generator = self.get_generator(path=path, project_uuid=project_uuid)
         if generator is None:
             return {}
         variables['id'] = generator['id']
         result = self.raw_query(query=UPDATE_GENERATOR_MUTATION, variables=variables)
 
         return result['data']['updateGenerator']
@@ -864,15 +889,15 @@
         query_response = self.raw_query(query=query, variables=variables)
 
         if 'errors' in query_response:
             return []
 
         return query_response['data']['project']['pipelines']
 
-    def create_pipeline(self, project_uuid=None, description=None, path=None, seeders=None, generators=None):
+    def create_pipeline(self, project_uuid=None, description=None, path=None, seeders=None, generators=None, tags=None):
         """
         Creates a pipeline.
         """
         variables = {
             'input': {
                 'path': path,
                 'project': project_uuid,
@@ -884,22 +909,24 @@
         if generators is not None:
             variables['input']['generators'] = [
                 self._marshal_generator(label, generator) for label, generator in generators.items()]
         if seeders is not None:
             variables['input']['seeders'] = [self._marshal_seeder(seeder) for seeder in seeders]
         if description is not None:
             variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
 
         result = self.raw_query(query=CREATE_PIPELINE_MUTATION, variables=variables)
         if 'errors' in result:
             return {"accepted": False}
 
         return result['data']['createPipeline']
 
-    def sync_pipeline(self, project_uuid=None, description=None, path=None, seeders=None, generators=None):
+    def sync_pipeline(self, project_uuid=None, description=None, path=None, seeders=None, generators=None, tags=None):
         """
         Syncs a pipeline.
         """
         variables = {
             'input': {
                 'path': path,
                 'project': project_uuid,
@@ -911,14 +938,16 @@
         if generators is not None:
             variables['input']['generators'] = [
                 self._marshal_generator(label, generator) for label, generator in generators.items()]
         if seeders is not None:
             variables['input']['seeders'] = [self._marshal_seeder(seeder) for seeder in seeders]
         if description is not None:
             variables['input']['description'] = description
+        if tags is not None:
+            variables['input']['tags'] = tags
 
         result = self.raw_query(query=SYNC_PIPELINE_MUTATION, variables=variables)
         if 'errors' in result:
             return {"accepted": False}
 
         return result['data']['syncPipeline']
```

### Comparing `ursactl-0.6.0/ursactl/core/services/dss_client.py` & `ursactl-0.7.0/ursactl/core/services/dss_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/services/iam_client.py` & `ursactl-0.7.0/ursactl/core/services/iam_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/services/planning_client.py` & `ursactl-0.7.0/ursactl/core/services/planning_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/services/project_client.py` & `ursactl-0.7.0/ursactl/core/services/project_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/core/utils/magic.py` & `ursactl-0.7.0/ursactl/core/utils/magic.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl/main.py` & `ursactl-0.7.0/ursactl/main.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.6.0/ursactl.egg-info/PKG-INFO` & `ursactl-0.7.0/ursactl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.6.0
+Version: 0.7.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Home-page: https://ursafrontier.cloud/
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `ursactl-0.6.0/ursactl.egg-info/SOURCES.txt` & `ursactl-0.7.0/ursactl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 ursactl/controllers/run.py
 ursactl/controllers/send.py
 ursactl/controllers/show.py
 ursactl/controllers/stop.py
 ursactl/controllers/sync.py
 ursactl/controllers/update.py
 ursactl/controllers/utils/__init__.py
+ursactl/controllers/utils/pages.py
 ursactl/controllers/utils/transforms.py
 ursactl/core/__init__.py
 ursactl/core/_base.py
 ursactl/core/agent.py
 ursactl/core/dataset.py
 ursactl/core/exc.py
 ursactl/core/pipeline.py
@@ -46,14 +47,15 @@
 ursactl/core/running_agent.py
 ursactl/core/version.py
 ursactl/core/services/__init__.py
 ursactl/core/services/_base.py
 ursactl/core/services/ape_client.py
 ursactl/core/services/dss_client.py
 ursactl/core/services/iam_client.py
+ursactl/core/services/page_client.py
 ursactl/core/services/planning_client.py
 ursactl/core/services/project_client.py
 ursactl/core/utils/__init__.py
 ursactl/core/utils/magic.py
 ursactl/ext/__init__.py
 ursactl/plugins/__init__.py
 ursactl/templates/__init__.py
```


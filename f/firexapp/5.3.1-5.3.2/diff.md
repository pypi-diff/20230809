# Comparing `tmp/firexapp-5.3.1.tar.gz` & `tmp/firexapp-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexapp-5.3.1.tar", last modified: Mon Aug  7 22:54:28 2023, max compression
+gzip compressed data, was "firexapp-5.3.2.tar", last modified: Tue Aug  8 19:46:56 2023, max compression
```

## Comparing `firexapp-5.3.1.tar` & `firexapp-5.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.316801 firexapp-5.3.1/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-08-07 22:54:13.000000 firexapp-5.3.1/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-08-07 22:54:13.000000 firexapp-5.3.1/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 22:54:28.316801 firexapp-5.3.1/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-08-07 22:54:13.000000 firexapp-5.3.1/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-08-07 22:54:13.000000 firexapp-5.3.1/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.317801 firexapp-5.3.1/firexapp/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-07 22:54:28.317801 firexapp-5.3.1/firexapp/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7352 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/application.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.308801 firexapp-5.3.1/firexapp/broker_manager/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/broker_manager/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/broker_manager/broker_factory.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13497 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/broker_manager/redis_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/celery_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/discovery.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.309801 firexapp-5.3.1/firexapp/engine/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/celery.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/default_celery_config.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6851 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/logging.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.310801 firexapp-5.3.1/firexapp/events/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/broker_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/event_aggregator.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3571 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/model.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/fileregistry.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    15762 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/firex_subprocess.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/info.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/plugins.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.310801 firexapp-5.3.1/firexapp/reporters/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/reporters/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6049 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/reporters/json_reporter.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.313801 firexapp-5.3.1/firexapp/submit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/arguments.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/console.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/install_configs.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/report_trigger.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/reporting.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9662 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/shutdown.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    32000 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/submit.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/tracking_service.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4612 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/uid.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.314801 firexapp-5.3.1/firexapp/tasks/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/core_tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/example.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/root_tasks.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.316801 firexapp-5.3.1/firexapp/testing/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/config_base.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12807 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/config_interpreter.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/coverage_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/pydev_debug_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7451 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/test_infra.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.307801 firexapp-5.3.1/firexapp.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      201 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2023-08-07 22:54:28.317801 firexapp-5.3.1/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1731 2023-08-07 22:54:13.000000 firexapp-5.3.1/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-07 22:54:13.000000 firexapp-5.3.1/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.823705 firexapp-5.3.2/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-08-08 19:46:41.000000 firexapp-5.3.2/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-08-08 19:46:41.000000 firexapp-5.3.2/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-08 19:46:56.823705 firexapp-5.3.2/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-08-08 19:46:41.000000 firexapp-5.3.2/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-08-08 19:46:41.000000 firexapp-5.3.2/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.824705 firexapp-5.3.2/firexapp/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-08 19:46:56.824705 firexapp-5.3.2/firexapp/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7352 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/application.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.814705 firexapp-5.3.2/firexapp/broker_manager/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/broker_manager/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/broker_manager/broker_factory.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13497 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/broker_manager/redis_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/celery_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/discovery.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.816705 firexapp-5.3.2/firexapp/engine/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/engine/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/engine/celery.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/engine/default_celery_config.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6851 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/engine/logging.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.817705 firexapp-5.3.2/firexapp/events/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/events/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/events/broker_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/events/event_aggregator.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3571 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/events/model.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/fileregistry.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    15711 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/firex_subprocess.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/info.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/plugins.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.817705 firexapp-5.3.2/firexapp/reporters/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/reporters/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6049 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/reporters/json_reporter.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.820705 firexapp-5.3.2/firexapp/submit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/arguments.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/console.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/install_configs.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/report_trigger.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/reporting.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9662 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/shutdown.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    32000 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/submit.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/tracking_service.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4612 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/submit/uid.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.821705 firexapp-5.3.2/firexapp/tasks/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/tasks/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/tasks/core_tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/tasks/example.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/tasks/root_tasks.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.823705 firexapp-5.3.2/firexapp/testing/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/testing/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/testing/config_base.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    12807 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/testing/config_interpreter.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/testing/coverage_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/testing/pydev_debug_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7451 2023-08-08 19:46:41.000000 firexapp-5.3.2/firexapp/testing/test_infra.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 19:46:56.813705 firexapp-5.3.2/firexapp.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      201 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 19:46:56.000000 firexapp-5.3.2/firexapp.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2023-08-08 19:46:56.824705 firexapp-5.3.2/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1731 2023-08-08 19:46:41.000000 firexapp-5.3.2/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 19:46:41.000000 firexapp-5.3.2/versioneer.py
```

### Comparing `firexapp-5.3.1/LICENSE` & `firexapp-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/fastentrypoints.py` & `firexapp-5.3.2/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/application.py` & `firexapp-5.3.2/firexapp/application.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/broker_manager/__init__.py` & `firexapp-5.3.2/firexapp/broker_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/broker_manager/broker_factory.py` & `firexapp-5.3.2/firexapp/broker_manager/broker_factory.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/broker_manager/redis_manager.py` & `firexapp-5.3.2/firexapp/broker_manager/redis_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/celery_manager.py` & `firexapp-5.3.2/firexapp/celery_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/common.py` & `firexapp-5.3.2/firexapp/common.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/discovery.py` & `firexapp-5.3.2/firexapp/discovery.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/engine/celery.py` & `firexapp-5.3.2/firexapp/engine/celery.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/engine/default_celery_config.py` & `firexapp-5.3.2/firexapp/engine/default_celery_config.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/engine/logging.py` & `firexapp-5.3.2/firexapp/engine/logging.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/events/broker_event_consumer.py` & `firexapp-5.3.2/firexapp/events/broker_event_consumer.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/events/event_aggregator.py` & `firexapp-5.3.2/firexapp/events/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/events/model.py` & `firexapp-5.3.2/firexapp/events/model.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/fileregistry.py` & `firexapp-5.3.2/firexapp/fileregistry.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/firex_subprocess.py` & `firexapp-5.3.2/firexapp/firex_subprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,22 +223,23 @@
 
     def _get_output_from_file():
         if not file or not chars or os.fstat(f.fileno()).st_size < chars:
             f.seek(0)
         else:
             f.seek(-chars, 2)
 
-        return f.read().decode(encoding='utf-8', errors='ignore')
+        return f.read().decode(encoding='utf-8', errors='replace')
 
     def _log_output(contents, error=False):
         if not chars or len(contents) < chars:
             log_msg = '%s Returned String:\n%s' % (log_header, contents)
         else:
             log_msg = '%s Last %d chars of Returned String:\n%s' % (log_header, chars, contents[-chars:])
-        logger.log(log_level, log_msg.encode(encoding='ascii', errors='namereplace').decode(errors='ignore'),
+        logger.log(log_level,
+                   log_msg,
                    extra={'span_class': 'command_output command_output_error' if error else 'command_output'})
 
     def _kill_proc_gently(proc):
         try:
             proc.terminate()
             try:
                 proc.wait(timeout=60)
```

### Comparing `firexapp-5.3.1/firexapp/info.py` & `firexapp-5.3.2/firexapp/info.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/plugins.py` & `firexapp-5.3.2/firexapp/plugins.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/reporters/json_reporter.py` & `firexapp-5.3.2/firexapp/reporters/json_reporter.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/arguments.py` & `firexapp-5.3.2/firexapp/submit/arguments.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/console.py` & `firexapp-5.3.2/firexapp/submit/console.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/install_configs.py` & `firexapp-5.3.2/firexapp/submit/install_configs.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/report_trigger.py` & `firexapp-5.3.2/firexapp/submit/report_trigger.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/reporting.py` & `firexapp-5.3.2/firexapp/submit/reporting.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/shutdown.py` & `firexapp-5.3.2/firexapp/submit/shutdown.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/submit.py` & `firexapp-5.3.2/firexapp/submit/submit.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/tracking_service.py` & `firexapp-5.3.2/firexapp/submit/tracking_service.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/submit/uid.py` & `firexapp-5.3.2/firexapp/submit/uid.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/tasks/core_tasks.py` & `firexapp-5.3.2/firexapp/tasks/core_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/tasks/example.py` & `firexapp-5.3.2/firexapp/tasks/example.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/tasks/root_tasks.py` & `firexapp-5.3.2/firexapp/tasks/root_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/testing/config_base.py` & `firexapp-5.3.2/firexapp/testing/config_base.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/testing/config_interpreter.py` & `firexapp-5.3.2/firexapp/testing/config_interpreter.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/testing/coverage_plugin.py` & `firexapp-5.3.2/firexapp/testing/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/testing/pydev_debug_plugin.py` & `firexapp-5.3.2/firexapp/testing/pydev_debug_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp/testing/test_infra.py` & `firexapp-5.3.2/firexapp/testing/test_infra.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/firexapp.egg-info/SOURCES.txt` & `firexapp-5.3.2/firexapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/setup.py` & `firexapp-5.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.1/versioneer.py` & `firexapp-5.3.2/versioneer.py`

 * *Files identical despite different names*


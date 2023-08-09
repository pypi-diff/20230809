# Comparing `tmp/cooptools-1.8.tar.gz` & `tmp/cooptools-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooptools-1.8.tar", last modified: Mon Jul  3 20:10:57 2023, max compression
+gzip compressed data, was "cooptools-1.9.tar", last modified: Mon Jul  3 21:04:05 2023, max compression
```

## Comparing `cooptools-1.8.tar` & `cooptools-1.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.341726 cooptools-1.8/
--rw-rw-rw-   0        0        0      770 2023-07-03 20:10:57.340730 cooptools-1.8/PKG-INFO
--rw-rw-rw-   0        0        0       59 2022-06-02 21:34:30.000000 cooptools-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.272724 cooptools-1.8/cooptools/
--rw-rw-rw-   0        0        0        0 2021-08-29 04:28:10.000000 cooptools-1.8/cooptools/__init__.py
--rw-rw-rw-   0        0        0     2447 2022-11-21 16:49:49.000000 cooptools-1.8/cooptools/anchor.py
--rw-rw-rw-   0        0        0     7443 2023-04-11 17:52:54.000000 cooptools-1.8/cooptools/colors.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.298750 cooptools-1.8/cooptools/commandDesignPattern/
--rw-rw-rw-   0        0        0       66 2022-06-02 21:34:30.000000 cooptools-1.8/cooptools/commandDesignPattern/__init__.py
--rw-rw-rw-   0        0        0     3475 2022-11-10 20:52:38.000000 cooptools-1.8/cooptools/commandDesignPattern/commandController.py
--rw-rw-rw-   0        0        0      833 2022-11-10 20:53:28.000000 cooptools-1.8/cooptools/commandDesignPattern/commandProtocol.py
--rw-rw-rw-   0        0        0      410 2022-10-23 20:05:41.000000 cooptools-1.8/cooptools/commandDesignPattern/exceptions.py
--rw-rw-rw-   0        0        0     7136 2023-02-02 23:13:02.000000 cooptools-1.8/cooptools/common.py
--rw-rw-rw-   0        0        0     4843 2023-06-20 21:31:18.000000 cooptools-1.8/cooptools/config.py
--rw-rw-rw-   0        0        0     3836 2023-06-08 18:10:09.000000 cooptools-1.8/cooptools/coopEnum.py
--rw-rw-rw-   0        0        0      273 2023-02-09 23:59:03.000000 cooptools-1.8/cooptools/coopProtocols.py
--rw-rw-rw-   0        0        0     2863 2022-06-02 21:34:30.000000 cooptools-1.8/cooptools/coopthreading.py
--rw-rw-rw-   0        0        0     2570 2023-06-08 20:41:42.000000 cooptools-1.8/cooptools/currency.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.302752 cooptools-1.8/cooptools/dataRefresher/
--rw-rw-rw-   0        0        0       70 2022-06-02 21:34:30.000000 cooptools-1.8/cooptools/dataRefresher/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-02-07 17:35:24.000000 cooptools-1.8/cooptools/dataRefresher/dataHub.py
--rw-rw-rw-   0        0        0     8195 2023-02-13 23:36:35.000000 cooptools-1.8/cooptools/dataRefresher/dataRefresher.py
--rw-rw-rw-   0        0        0     4484 2023-05-25 14:18:36.000000 cooptools-1.8/cooptools/date_utils.py
--rw-rw-rw-   0        0        0     2677 2023-01-28 03:52:10.000000 cooptools-1.8/cooptools/decor.py
--rw-rw-rw-   0        0        0     2528 2022-09-19 22:09:44.000000 cooptools-1.8/cooptools/dictPolicies.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.304750 cooptools-1.8/cooptools/discreteEventSimulator/
--rw-rw-rw-   0        0        0        0 2023-01-19 21:18:55.000000 cooptools-1.8/cooptools/discreteEventSimulator/__init__.py
--rw-rw-rw-   0        0        0     5778 2023-01-23 18:26:37.000000 cooptools-1.8/cooptools/discreteEventSimulator/discreteEventSimulator.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.313724 cooptools-1.8/cooptools/geometry_utils/
--rw-rw-rw-   0        0        0        0 2023-03-07 18:24:21.000000 cooptools-1.8/cooptools/geometry_utils/__init__.py
--rw-rw-rw-   0        0        0     5532 2023-03-15 23:08:51.000000 cooptools-1.8/cooptools/geometry_utils/circle_utils.py
--rw-rw-rw-   0        0        0     8755 2023-03-07 18:29:32.000000 cooptools-1.8/cooptools/geometry_utils/curve_utils.py
--rw-rw-rw-   0        0        0     2753 2023-03-07 18:29:32.000000 cooptools-1.8/cooptools/geometry_utils/line_utils.py
--rw-rw-rw-   0        0        0     2381 2023-03-07 18:29:32.000000 cooptools-1.8/cooptools/geometry_utils/rect_utils.py
--rw-rw-rw-   0        0        0     2434 2023-03-07 18:29:32.000000 cooptools-1.8/cooptools/geometry_utils/triangle_utils.py
--rw-rw-rw-   0        0        0     8281 2023-03-15 21:44:53.000000 cooptools-1.8/cooptools/geometry_utils/vector_utils.py
--rw-rw-rw-   0        0        0     3480 2022-12-01 19:46:18.000000 cooptools-1.8/cooptools/jsonIO.py
--rw-rw-rw-   0        0        0     4137 2022-07-19 18:00:18.000000 cooptools-1.8/cooptools/marchingSquares.py
--rw-rw-rw-   0        0        0     5130 2021-08-29 04:28:10.000000 cooptools-1.8/cooptools/matrixManipulation.py
--rw-rw-rw-   0        0        0     5682 2022-06-22 22:18:21.000000 cooptools-1.8/cooptools/metrics.py
--rw-rw-rw-   0        0        0    11287 2023-05-30 16:47:59.000000 cooptools-1.8/cooptools/os_manip.py
--rw-rw-rw-   0        0        0    20839 2023-02-06 16:33:36.000000 cooptools-1.8/cooptools/pandasHelpers.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.316724 cooptools-1.8/cooptools/physics/
--rw-rw-rw-   0        0        0        0 2023-06-07 16:42:29.000000 cooptools-1.8/cooptools/physics/__init__.py
--rw-rw-rw-   0        0        0     5630 2023-06-07 16:46:12.000000 cooptools-1.8/cooptools/physics/movement.py
--rw-rw-rw-   0        0        0     5217 2023-06-07 16:46:12.000000 cooptools-1.8/cooptools/physics/orientation.py
--rw-rw-rw-   0        0        0     5928 2022-11-22 19:39:42.000000 cooptools-1.8/cooptools/plotting.py
--rw-rw-rw-   0        0        0     1421 2021-08-29 04:28:10.000000 cooptools-1.8/cooptools/printing.py
--rw-rw-rw-   0        0        0     3341 2023-04-11 17:19:06.000000 cooptools-1.8/cooptools/randoms.py
--rw-rw-rw-   0        0        0      684 2023-02-13 22:06:39.000000 cooptools-1.8/cooptools/register.py
--rw-rw-rw-   0        0        0     1694 2023-06-07 16:31:00.000000 cooptools-1.8/cooptools/retry.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.322723 cooptools-1.8/cooptools/sectors/
--rw-rw-rw-   0        0        0       20 2023-03-07 20:40:12.000000 cooptools-1.8/cooptools/sectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.330724 cooptools-1.8/cooptools/sectors/grids/
--rw-rw-rw-   0        0        0       78 2023-03-07 20:35:41.000000 cooptools-1.8/cooptools/sectors/grids/__init__.py
--rw-rw-rw-   0        0        0     1253 2022-09-19 21:08:23.000000 cooptools-1.8/cooptools/sectors/grids/gridState.py
--rw-rw-rw-   0        0        0     3529 2023-04-12 13:39:47.000000 cooptools-1.8/cooptools/sectors/grids/grid_base.py
--rw-rw-rw-   0        0        0     2394 2022-11-10 19:53:54.000000 cooptools-1.8/cooptools/sectors/grids/hexGrid.py
--rw-rw-rw-   0        0        0     3024 2023-03-07 20:35:41.000000 cooptools-1.8/cooptools/sectors/grids/rectGrid.py
--rw-rw-rw-   0        0        0     7122 2022-11-12 19:13:30.000000 cooptools-1.8/cooptools/sectors/hex_utils.py
--rw-rw-rw-   0        0        0     8027 2022-11-21 15:30:38.000000 cooptools-1.8/cooptools/sectors/rect_utils.py
--rw-rw-rw-   0        0        0      337 2022-10-13 14:34:53.000000 cooptools-1.8/cooptools/sectors/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.331724 cooptools-1.8/cooptools/statistics/
--rw-rw-rw-   0        0        0       47 2021-10-05 19:39:56.000000 cooptools-1.8/cooptools/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.335729 cooptools-1.8/cooptools/statistics/controlChart/
--rw-rw-rw-   0        0        0        0 2022-02-19 23:10:39.000000 cooptools-1.8/cooptools/statistics/controlChart/__init__.py
--rw-rw-rw-   0        0        0    13265 2022-11-10 23:04:03.000000 cooptools-1.8/cooptools/statistics/controlChart/controlChart.py
--rw-rw-rw-   0        0        0     7937 2022-11-12 19:13:30.000000 cooptools-1.8/cooptools/statistics/controlChart/plotting.py
--rw-rw-rw-   0        0        0     1677 2022-06-03 13:34:45.000000 cooptools-1.8/cooptools/timeWindow.py
--rw-rw-rw-   0        0        0     3247 2023-06-07 18:27:42.000000 cooptools-1.8/cooptools/timedDecay.py
--rw-rw-rw-   0        0        0     5204 2022-12-31 04:29:20.000000 cooptools-1.8/cooptools/toggles.py
--rw-rw-rw-   0        0        0     1553 2022-11-10 23:12:40.000000 cooptools-1.8/cooptools/trends.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.338764 cooptools-1.8/cooptools/triggerActionSystem/
--rw-rw-rw-   0        0        0        0 2023-02-09 23:42:35.000000 cooptools-1.8/cooptools/triggerActionSystem/__init__.py
--rw-rw-rw-   0        0        0      247 2023-02-10 00:02:03.000000 cooptools-1.8/cooptools/triggerActionSystem/trigger.py
--rw-rw-rw-   0        0        0     3098 2023-02-14 19:51:35.000000 cooptools-1.8/cooptools/typevalidation.py
--rw-rw-rw-   0        0        0     2375 2022-11-30 23:33:22.000000 cooptools-1.8/cooptools/version.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:10:57.292724 cooptools-1.8/cooptools.egg-info/
--rw-rw-rw-   0        0        0      770 2023-07-03 20:10:57.000000 cooptools-1.8/cooptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2216 2023-07-03 20:10:57.000000 cooptools-1.8/cooptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:10:57.000000 cooptools-1.8/cooptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-08-30 22:37:58.000000 cooptools-1.8/cooptools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      192 2023-07-03 20:10:57.000000 cooptools-1.8/cooptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 20:10:57.000000 cooptools-1.8/cooptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 20:10:57.341726 cooptools-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-07-03 19:56:33.000000 cooptools-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.103498 cooptools-1.9/
+-rw-rw-rw-   0        0        0      770 2023-07-03 21:04:05.102534 cooptools-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2022-06-02 21:34:30.000000 cooptools-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:04.852907 cooptools-1.9/cooptools/
+-rw-rw-rw-   0        0        0        0 2021-08-29 04:28:10.000000 cooptools-1.9/cooptools/__init__.py
+-rw-rw-rw-   0        0        0     2447 2022-11-21 16:49:49.000000 cooptools-1.9/cooptools/anchor.py
+-rw-rw-rw-   0        0        0     7443 2023-04-11 17:52:54.000000 cooptools-1.9/cooptools/colors.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:04.905910 cooptools-1.9/cooptools/commandDesignPattern/
+-rw-rw-rw-   0        0        0       66 2022-06-02 21:34:30.000000 cooptools-1.9/cooptools/commandDesignPattern/__init__.py
+-rw-rw-rw-   0        0        0     3475 2022-11-10 20:52:38.000000 cooptools-1.9/cooptools/commandDesignPattern/commandController.py
+-rw-rw-rw-   0        0        0      833 2022-11-10 20:53:28.000000 cooptools-1.9/cooptools/commandDesignPattern/commandProtocol.py
+-rw-rw-rw-   0        0        0      410 2022-10-23 20:05:41.000000 cooptools-1.9/cooptools/commandDesignPattern/exceptions.py
+-rw-rw-rw-   0        0        0     7136 2023-02-02 23:13:02.000000 cooptools-1.9/cooptools/common.py
+-rw-rw-rw-   0        0        0     6173 2023-07-03 20:45:31.000000 cooptools-1.9/cooptools/config.py
+-rw-rw-rw-   0        0        0     3836 2023-06-08 18:10:09.000000 cooptools-1.9/cooptools/coopEnum.py
+-rw-rw-rw-   0        0        0      273 2023-02-09 23:59:03.000000 cooptools-1.9/cooptools/coopProtocols.py
+-rw-rw-rw-   0        0        0     2863 2022-06-02 21:34:30.000000 cooptools-1.9/cooptools/coopthreading.py
+-rw-rw-rw-   0        0        0     2570 2023-06-08 20:41:42.000000 cooptools-1.9/cooptools/currency.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:04.927939 cooptools-1.9/cooptools/dataRefresher/
+-rw-rw-rw-   0        0        0       70 2022-06-02 21:34:30.000000 cooptools-1.9/cooptools/dataRefresher/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-02-07 17:35:24.000000 cooptools-1.9/cooptools/dataRefresher/dataHub.py
+-rw-rw-rw-   0        0        0     8195 2023-02-13 23:36:35.000000 cooptools-1.9/cooptools/dataRefresher/dataRefresher.py
+-rw-rw-rw-   0        0        0     4484 2023-05-25 14:18:36.000000 cooptools-1.9/cooptools/date_utils.py
+-rw-rw-rw-   0        0        0     2677 2023-01-28 03:52:10.000000 cooptools-1.9/cooptools/decor.py
+-rw-rw-rw-   0        0        0     2528 2022-09-19 22:09:44.000000 cooptools-1.9/cooptools/dictPolicies.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:04.936910 cooptools-1.9/cooptools/discreteEventSimulator/
+-rw-rw-rw-   0        0        0        0 2023-01-19 21:18:55.000000 cooptools-1.9/cooptools/discreteEventSimulator/__init__.py
+-rw-rw-rw-   0        0        0     5778 2023-01-23 18:26:37.000000 cooptools-1.9/cooptools/discreteEventSimulator/discreteEventSimulator.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:04.983561 cooptools-1.9/cooptools/geometry_utils/
+-rw-rw-rw-   0        0        0        0 2023-03-07 18:24:21.000000 cooptools-1.9/cooptools/geometry_utils/__init__.py
+-rw-rw-rw-   0        0        0     5532 2023-03-15 23:08:51.000000 cooptools-1.9/cooptools/geometry_utils/circle_utils.py
+-rw-rw-rw-   0        0        0     8755 2023-03-07 18:29:32.000000 cooptools-1.9/cooptools/geometry_utils/curve_utils.py
+-rw-rw-rw-   0        0        0     2753 2023-03-07 18:29:32.000000 cooptools-1.9/cooptools/geometry_utils/line_utils.py
+-rw-rw-rw-   0        0        0     2381 2023-03-07 18:29:32.000000 cooptools-1.9/cooptools/geometry_utils/rect_utils.py
+-rw-rw-rw-   0        0        0     2434 2023-03-07 18:29:32.000000 cooptools-1.9/cooptools/geometry_utils/triangle_utils.py
+-rw-rw-rw-   0        0        0     8281 2023-03-15 21:44:53.000000 cooptools-1.9/cooptools/geometry_utils/vector_utils.py
+-rw-rw-rw-   0        0        0     3480 2022-12-01 19:46:18.000000 cooptools-1.9/cooptools/jsonIO.py
+-rw-rw-rw-   0        0        0     4137 2022-07-19 18:00:18.000000 cooptools-1.9/cooptools/marchingSquares.py
+-rw-rw-rw-   0        0        0     5130 2021-08-29 04:28:10.000000 cooptools-1.9/cooptools/matrixManipulation.py
+-rw-rw-rw-   0        0        0     5682 2022-06-22 22:18:21.000000 cooptools-1.9/cooptools/metrics.py
+-rw-rw-rw-   0        0        0    11447 2023-07-03 20:44:59.000000 cooptools-1.9/cooptools/os_manip.py
+-rw-rw-rw-   0        0        0    20839 2023-02-06 16:33:36.000000 cooptools-1.9/cooptools/pandasHelpers.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.000497 cooptools-1.9/cooptools/physics/
+-rw-rw-rw-   0        0        0        0 2023-06-07 16:42:29.000000 cooptools-1.9/cooptools/physics/__init__.py
+-rw-rw-rw-   0        0        0     5630 2023-06-07 16:46:12.000000 cooptools-1.9/cooptools/physics/movement.py
+-rw-rw-rw-   0        0        0     5217 2023-06-07 16:46:12.000000 cooptools-1.9/cooptools/physics/orientation.py
+-rw-rw-rw-   0        0        0     5928 2022-11-22 19:39:42.000000 cooptools-1.9/cooptools/plotting.py
+-rw-rw-rw-   0        0        0     1421 2021-08-29 04:28:10.000000 cooptools-1.9/cooptools/printing.py
+-rw-rw-rw-   0        0        0     3341 2023-04-11 17:19:06.000000 cooptools-1.9/cooptools/randoms.py
+-rw-rw-rw-   0        0        0      684 2023-02-13 22:06:39.000000 cooptools-1.9/cooptools/register.py
+-rw-rw-rw-   0        0        0     1694 2023-06-07 16:31:00.000000 cooptools-1.9/cooptools/retry.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.028537 cooptools-1.9/cooptools/sectors/
+-rw-rw-rw-   0        0        0       20 2023-03-07 20:40:12.000000 cooptools-1.9/cooptools/sectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.063496 cooptools-1.9/cooptools/sectors/grids/
+-rw-rw-rw-   0        0        0       78 2023-03-07 20:35:41.000000 cooptools-1.9/cooptools/sectors/grids/__init__.py
+-rw-rw-rw-   0        0        0     1253 2022-09-19 21:08:23.000000 cooptools-1.9/cooptools/sectors/grids/gridState.py
+-rw-rw-rw-   0        0        0     3529 2023-04-12 13:39:47.000000 cooptools-1.9/cooptools/sectors/grids/grid_base.py
+-rw-rw-rw-   0        0        0     2394 2022-11-10 19:53:54.000000 cooptools-1.9/cooptools/sectors/grids/hexGrid.py
+-rw-rw-rw-   0        0        0     3024 2023-03-07 20:35:41.000000 cooptools-1.9/cooptools/sectors/grids/rectGrid.py
+-rw-rw-rw-   0        0        0     7122 2022-11-12 19:13:30.000000 cooptools-1.9/cooptools/sectors/hex_utils.py
+-rw-rw-rw-   0        0        0     8027 2022-11-21 15:30:38.000000 cooptools-1.9/cooptools/sectors/rect_utils.py
+-rw-rw-rw-   0        0        0      337 2022-10-13 14:34:53.000000 cooptools-1.9/cooptools/sectors/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.070499 cooptools-1.9/cooptools/statistics/
+-rw-rw-rw-   0        0        0       47 2021-10-05 19:39:56.000000 cooptools-1.9/cooptools/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.092533 cooptools-1.9/cooptools/statistics/controlChart/
+-rw-rw-rw-   0        0        0        0 2022-02-19 23:10:39.000000 cooptools-1.9/cooptools/statistics/controlChart/__init__.py
+-rw-rw-rw-   0        0        0    13265 2022-11-10 23:04:03.000000 cooptools-1.9/cooptools/statistics/controlChart/controlChart.py
+-rw-rw-rw-   0        0        0     7937 2022-11-12 19:13:30.000000 cooptools-1.9/cooptools/statistics/controlChart/plotting.py
+-rw-rw-rw-   0        0        0     1677 2022-06-03 13:34:45.000000 cooptools-1.9/cooptools/timeWindow.py
+-rw-rw-rw-   0        0        0     3247 2023-06-07 18:27:42.000000 cooptools-1.9/cooptools/timedDecay.py
+-rw-rw-rw-   0        0        0     5204 2022-12-31 04:29:20.000000 cooptools-1.9/cooptools/toggles.py
+-rw-rw-rw-   0        0        0     1553 2022-11-10 23:12:40.000000 cooptools-1.9/cooptools/trends.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:05.100533 cooptools-1.9/cooptools/triggerActionSystem/
+-rw-rw-rw-   0        0        0        0 2023-02-09 23:42:35.000000 cooptools-1.9/cooptools/triggerActionSystem/__init__.py
+-rw-rw-rw-   0        0        0      247 2023-02-10 00:02:03.000000 cooptools-1.9/cooptools/triggerActionSystem/trigger.py
+-rw-rw-rw-   0        0        0     3098 2023-02-14 19:51:35.000000 cooptools-1.9/cooptools/typevalidation.py
+-rw-rw-rw-   0        0        0     2375 2022-11-30 23:33:22.000000 cooptools-1.9/cooptools/version.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:04:04.876910 cooptools-1.9/cooptools.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-07-03 21:04:04.000000 cooptools-1.9/cooptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2216 2023-07-03 21:04:04.000000 cooptools-1.9/cooptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 21:04:04.000000 cooptools-1.9/cooptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-08-30 22:37:58.000000 cooptools-1.9/cooptools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      171 2023-07-03 21:04:04.000000 cooptools-1.9/cooptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 21:04:04.000000 cooptools-1.9/cooptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 21:04:05.103498 cooptools-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-07-03 21:04:00.000000 cooptools-1.9/setup.py
```

### Comparing `cooptools-1.8/PKG-INFO` & `cooptools-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cooptools
-Version: 1.8
+Version: 1.9
 Summary: Generic Tooling
 Home-page: https://github.com/tylertjburns/cooptools
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cooptools-1.8/cooptools/anchor.py` & `cooptools-1.9/cooptools/anchor.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/colors.py` & `cooptools-1.9/cooptools/colors.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/commandDesignPattern/commandController.py` & `cooptools-1.9/cooptools/commandDesignPattern/commandController.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/commandDesignPattern/commandProtocol.py` & `cooptools-1.9/cooptools/commandDesignPattern/commandProtocol.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/common.py` & `cooptools-1.9/cooptools/common.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/coopEnum.py` & `cooptools-1.9/cooptools/coopEnum.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/coopthreading.py` & `cooptools-1.9/cooptools/coopthreading.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/currency.py` & `cooptools-1.9/cooptools/currency.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/dataRefresher/dataHub.py` & `cooptools-1.9/cooptools/dataRefresher/dataHub.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/dataRefresher/dataRefresher.py` & `cooptools-1.9/cooptools/dataRefresher/dataRefresher.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/date_utils.py` & `cooptools-1.9/cooptools/date_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/decor.py` & `cooptools-1.9/cooptools/decor.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/dictPolicies.py` & `cooptools-1.9/cooptools/dictPolicies.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/discreteEventSimulator/discreteEventSimulator.py` & `cooptools-1.9/cooptools/discreteEventSimulator/discreteEventSimulator.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/geometry_utils/circle_utils.py` & `cooptools-1.9/cooptools/geometry_utils/circle_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/geometry_utils/curve_utils.py` & `cooptools-1.9/cooptools/geometry_utils/curve_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/geometry_utils/line_utils.py` & `cooptools-1.9/cooptools/geometry_utils/line_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/geometry_utils/rect_utils.py` & `cooptools-1.9/cooptools/geometry_utils/rect_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/geometry_utils/triangle_utils.py` & `cooptools-1.9/cooptools/geometry_utils/triangle_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/geometry_utils/vector_utils.py` & `cooptools-1.9/cooptools/geometry_utils/vector_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/jsonIO.py` & `cooptools-1.9/cooptools/jsonIO.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/marchingSquares.py` & `cooptools-1.9/cooptools/marchingSquares.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/matrixManipulation.py` & `cooptools-1.9/cooptools/matrixManipulation.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/metrics.py` & `cooptools-1.9/cooptools/metrics.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/os_manip.py` & `cooptools-1.9/cooptools/os_manip.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,29 @@
 
 filePathProvider = Union[str, Callable[[], str]]
 
 def resolve_absolute_filepath(file_path: filePathProvider):
     if file_path is None:
         return None
 
+    fp = None
     if type(file_path) == str:
-        return file_path
+        fp = file_path
+    else:
+        try:
+            fp = file_path()
+        except Exception as e:
+            logger.error(f"Unable to resolve the file path: {e}")
+            raise e
+
+    afp = os.path.abspath(fp)
+    logger.debug(f"The resolved absolute filepath to be used: {afp}")
+    return afp
+
 
-    try:
-        return file_path()
-    except Exception as e:
-        logger.error(f"Unable to resolve the file path: {e}")
-        return None
 
 def check_file_exists(file_path: filePathProvider):
     fp = resolve_absolute_filepath(file_path)
     return fp is not None and os.path.exists(fp)
 
 def verify_file_exists(file_path: filePathProvider):
     # verify path exists
```

### Comparing `cooptools-1.8/cooptools/pandasHelpers.py` & `cooptools-1.9/cooptools/pandasHelpers.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/physics/movement.py` & `cooptools-1.9/cooptools/physics/movement.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/physics/orientation.py` & `cooptools-1.9/cooptools/physics/orientation.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/plotting.py` & `cooptools-1.9/cooptools/plotting.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/printing.py` & `cooptools-1.9/cooptools/printing.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/randoms.py` & `cooptools-1.9/cooptools/randoms.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/register.py` & `cooptools-1.9/cooptools/register.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/retry.py` & `cooptools-1.9/cooptools/retry.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/sectors/grids/gridState.py` & `cooptools-1.9/cooptools/sectors/grids/gridState.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/sectors/grids/grid_base.py` & `cooptools-1.9/cooptools/sectors/grids/grid_base.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/sectors/grids/hexGrid.py` & `cooptools-1.9/cooptools/sectors/grids/hexGrid.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/sectors/grids/rectGrid.py` & `cooptools-1.9/cooptools/sectors/grids/rectGrid.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/sectors/hex_utils.py` & `cooptools-1.9/cooptools/sectors/hex_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/sectors/rect_utils.py` & `cooptools-1.9/cooptools/sectors/rect_utils.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/statistics/controlChart/controlChart.py` & `cooptools-1.9/cooptools/statistics/controlChart/controlChart.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/statistics/controlChart/plotting.py` & `cooptools-1.9/cooptools/statistics/controlChart/plotting.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/timeWindow.py` & `cooptools-1.9/cooptools/timeWindow.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/timedDecay.py` & `cooptools-1.9/cooptools/timedDecay.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/toggles.py` & `cooptools-1.9/cooptools/toggles.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/trends.py` & `cooptools-1.9/cooptools/trends.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/typevalidation.py` & `cooptools-1.9/cooptools/typevalidation.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools/version.py` & `cooptools-1.9/cooptools/version.py`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/cooptools.egg-info/PKG-INFO` & `cooptools-1.9/cooptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cooptools
-Version: 1.8
+Version: 1.9
 Summary: Generic Tooling
 Home-page: https://github.com/tylertjburns/cooptools
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cooptools-1.8/cooptools.egg-info/SOURCES.txt` & `cooptools-1.9/cooptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cooptools-1.8/setup.py` & `cooptools-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='cooptools',
-      version='1.08',
+      version='1.09',
       description='Generic Tooling',
       url='https://github.com/tylertjburns/cooptools',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```


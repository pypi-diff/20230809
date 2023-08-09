# Comparing `tmp/valorant.py-1.0.1.tar.gz` & `tmp/valorant.py-1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valorant.py-1.0.1.tar", last modified: Tue Aug  8 10:40:57 2023, max compression
+gzip compressed data, was "valorant.py-1.0.2a0.tar", last modified: Wed Aug  9 03:05:55 2023, max compression
```

## Comparing `valorant.py-1.0.1.tar` & `valorant.py-1.0.2a0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.449462 valorant.py-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-08 10:40:46.000000 valorant.py-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 10:40:46.000000 valorant.py-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-08 10:40:57.449462 valorant.py-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 10:40:46.000000 valorant.py-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 10:40:46.000000 valorant.py-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 10:40:46.000000 valorant.py-1.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 10:40:46.000000 valorant.py-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 10:40:57.449462 valorant.py-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-08 10:40:46.000000 valorant.py-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.437461 valorant.py-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-08 10:40:46.000000 valorant.py-1.0.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-08-08 10:40:46.000000 valorant.py-1.0.1/tests/test_valorant_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.441461 valorant.py-1.0.1/valorant/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17875 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/localization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.445461 valorant.py-1.0.1/valorant/models/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/buddies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/ceremonies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/competitive_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/content_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/gamemodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/gear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/level_borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/player_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/player_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/sprays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/models/weapons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.449462 valorant.py-1.0.1/valorant/types/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/buddies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/ceremonies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/competitive_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/content_tiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/gamemodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/gear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/level_borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/player_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/player_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/sprays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/types/weapons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-08 10:40:46.000000 valorant.py-1.0.1/valorant/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:40:57.441461 valorant.py-1.0.1/valorant.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 10:40:57.000000 valorant.py-1.0.1/valorant.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:05:55.452265 valorant.py-1.0.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-08-09 03:05:55.448265 valorant.py-1.0.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:05:55.452265 valorant.py-1.0.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:05:55.432265 valorant.py-1.0.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:05:55.436265 valorant.py-1.0.2a0/valorant/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28120 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17875 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/localization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:05:55.444265 valorant.py-1.0.2a0/valorant/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/buddies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/ceremonies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/competitive_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/content_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/gamemodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/gear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/level_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/player_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/player_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/sprays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/models/weapons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:05:55.448265 valorant.py-1.0.2a0/valorant/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/buddies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/ceremonies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/competitive_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/content_tiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/gamemodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/gear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/level_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/player_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/player_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/sprays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/types/weapons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-09 03:05:42.000000 valorant.py-1.0.2a0/valorant/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:05:55.440265 valorant.py-1.0.2a0/valorant.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-08-09 03:05:55.000000 valorant.py-1.0.2a0/valorant.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-09 03:05:55.000000 valorant.py-1.0.2a0/valorant.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:05:55.000000 valorant.py-1.0.2a0/valorant.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-09 03:05:55.000000 valorant.py-1.0.2a0/valorant.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-09 03:05:55.000000 valorant.py-1.0.2a0/valorant.py.egg-info/top_level.txt
```

### Comparing `valorant.py-1.0.1/LICENSE` & `valorant.py-1.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/PKG-INFO` & `valorant.py-1.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valorant.py
-Version: 1.0.1
+Version: 1.0.2a0
 Summary: An Asynchronous Unofficial Valorant API Wrapper for Python
 Home-page: https://github.com/staciax/valorant
 Author: STACiA
 License: MIT
 Project-URL: Issue tracker, https://github.com/staciax/valorant/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `valorant.py-1.0.1/README.md` & `valorant.py-1.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/pyproject.toml` & `valorant.py-1.0.2a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/setup.py` & `valorant.py-1.0.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/tests/test_client.py` & `valorant.py-1.0.2a0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/tests/test_valorant_api.py` & `valorant.py-1.0.2a0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/__init__.py` & `valorant.py-1.0.2a0/valorant/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'valorant'
 __author__ = 'STACiA'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present STACiA'
-__version__ = '1.0.1'
+__version__ = '1.0.2a'
 
 from typing import Literal, NamedTuple
 
 from . import models as models, utils as utils
 from .asset import *
 from .client import *
 from .enums import *
@@ -25,10 +25,10 @@
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     release: Literal["alpha", "beta", "final"]
 
 
-version_info: VersionInfo = VersionInfo(major=1, minor=0, micro=1, release='final')
+version_info: VersionInfo = VersionInfo(major=1, minor=0, micro=2, release='final')
 
 del NamedTuple, Literal, VersionInfo
```

### Comparing `valorant.py-1.0.1/valorant/asset.py` & `valorant.py-1.0.2a0/valorant/asset.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/cache.py` & `valorant.py-1.0.2a0/valorant/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,23 +97,20 @@
 #     def find(self):
 #         raise NotImplementedError
 
 _log = logging.getLogger(__name__)
 
 
 class CacheState:
-    def __init__(self, *, locale: Locale, http: HTTPClient, to_file: bool = False) -> None:
+    def __init__(self, *, locale: Locale, http: HTTPClient) -> None:
         self.locale = locale
         self.http = http
-        self.cache: bool = True
-        self._to_file: bool = to_file
         # -
         self._agents: Dict[str, Agent] = {}
         self._buddies: Dict[str, Buddy] = {}
-        self._buddy_levels: Dict[str, BuddyLevel] = {}
         self._bundles: Dict[str, Bundle] = {}
         self._ceremonies: Dict[str, Ceremony] = {}
         self._competitive_tiers: Dict[str, CompetitiveTier] = {}
         self._content_tiers: Dict[str, ContentTier] = {}
         self._contracts: Dict[str, Contract] = {}
         self._currencies: Dict[str, Currency] = {}
         self._events: Dict[str, Event] = {}
@@ -124,21 +121,17 @@
         self._maps: Dict[str, Map] = {}
         self._missions: Dict[str, Mission] = {}
         self._player_cards: Dict[str, PlayerCard] = {}
         self._player_titles: Dict[str, PlayerTitle] = {}
         self._seasons: Dict[str, Season] = {}
         self._competitive_seasons: Dict[str, CompetitiveSeason] = {}
         self._sprays: Dict[str, Spray] = {}
-        self._spray_levels: Dict[str, SprayLevel] = {}
         self._themes: Dict[str, Theme] = {}
         self._version: Version = MISSING
         self._weapons: Dict[str, Weapon] = {}
-        self._skins: Dict[str, Skin] = {}
-        self._skin_chromas: Dict[str, SkinChroma] = {}
-        self._skin_levels: Dict[str, SkinLevel] = {}
 
     async def init(self) -> None:
         tasks = [
             self.http.get_agents,
             self.http.get_buddies,
             self.http.get_bundles,
             self.http.get_ceremonies,
@@ -158,54 +151,22 @@
             self.http.get_seasons,
             self.http.get_competitive_seasons,
             self.http.get_sprays,
             self.http.get_themes,
             self.http.get_weapons,
             self.http.get_version,
         ]
-        # if self._to_file:
-
-        #     # read from file
-        #     for func in tasks:
-        #         funcname = func.__name__.split('_')[1:]
-        #         filename = '_'.join(funcname) + '.json'
-        #         # add_to_cache = getattr(self, f'add_{funcname}')
-        #         # if os.path.exists(filename):
-        #         #     with open(filename, 'r') as f:
-        #         #         data = json.load(f)
-        #         #         continue
-        #         # else:
-        #         #     data = await func()
-        #         #     self._add_to_file(data, filename)
-        #         # add_to_cache = getattr(self, f'add_{funcname}')
-        # else:
-        # results = await self._fetch_data_from_api(tasks)
-
         results = await asyncio.gather(*(task() for task in tasks))
         for func, result in zip(tasks, results):
             assert result is not None
             funcname = func.__name__.split('_')[1:]
             funcname = '_'.join(funcname)
             parse_func = getattr(self, f'_add_{funcname}')
             parse_func(result)
 
-    # async def _fetch_data_from_api(self, tasks: List[Callable[..., Coroutine[Any, Any, Any]]]) -> List[Any]:
-    #     results = await asyncio.gather(*[task() for task in tasks])
-    #     return results
-    # for func, result in zip(tasks, results):
-    #     assert result is not None
-    #     funcname = func.__name__.split('_')[1:]
-    #     funcname = '_'.join(funcname)
-    #     parse_func = getattr(self, f'add_{funcname}')
-    #     parse_func(result)
-
-    # def _add_to_file(self, data: Any, filename: str) -> None:
-    #     with open(filename, 'w') as f:
-    #         json.dump(data, f, indent=4)
-
     def clear(self) -> None:
         for key in self.__dict__.keys():
             if key.startswith('_') and isinstance(self.__dict__[key], dict):
                 self.__dict__[key].clear()
         self._version = MISSING
 
     # agents
@@ -238,27 +199,31 @@
 
     @property
     def buddies(self) -> List[Buddy]:
         return list(self._buddies.values())
 
     @property
     def buddy_levels(self) -> List[BuddyLevel]:
-        return list(self._buddy_levels.values())
+        levels = []
+        for buddy in self.buddies:
+            levels.extend(buddy.levels)
+        return levels
 
     def get_buddy(self, uuid: Optional[str], /) -> Optional[Buddy]:
         return self._buddies.get(uuid)  # type: ignore
 
     def get_buddy_level(self, uuid: Optional[str], /) -> Optional[BuddyLevel]:
-        return self._buddy_levels.get(uuid)  # type: ignore
+        for level in self.buddy_levels:
+            if level.uuid == uuid:
+                return level
+        return None
 
     def store_buddy(self, data: buddies.Buddy) -> Buddy:
         buddy_id = data['uuid']
         self._buddies[buddy_id] = buddy = Buddy(state=self, data=data)
-        for level in buddy.levels:
-            self._buddy_levels[level.uuid] = level
         return buddy
 
     def _add_buddies(self, data: buddies.Buddies) -> None:
         buddy_data = data['data']
         for buddy in buddy_data:
             buddy_existing = self.get_buddy(buddy['uuid'])
             if buddy_existing is None:
@@ -471,15 +436,16 @@
         game_mode_id = data['uuid']
         self._game_modes[game_mode_id] = game_mode = GameMode(state=self, data=data)
         return game_mode
 
     def store_game_mode_equippable(self, data: gamemodes.GameModeEquippable) -> GameModeEquippable:
         game_mode_equippable_id = data['uuid']
         self._game_mode_equippables[game_mode_equippable_id] = game_mode_equippable = GameModeEquippable(
-            state=self, data=data
+            state=self,
+            data=data,
         )
         return game_mode_equippable
 
     def _add_game_modes(self, data: gamemodes.GameModes) -> None:
         game_mode_data = data['data']
         for game_mode in game_mode_data:
             game_mode_existing = self.get_game_mode(game_mode['uuid'])
@@ -716,24 +682,28 @@
         return list(self._sprays.values())
 
     def get_spray(self, uuid: Optional[str], /) -> Optional[Spray]:
         return self._sprays.get(uuid)  # type: ignore
 
     @property
     def spray_levels(self) -> List[SprayLevel]:
-        return list(self._spray_levels.values())
+        levels = []
+        for spray in self.sprays:
+            levels.extend(spray.levels)
+        return levels
 
     def get_spray_level(self, uuid: Optional[str], /) -> Optional[SprayLevel]:
-        return self._spray_levels.get(uuid)  # type: ignore
+        for level in self.spray_levels:
+            if level.uuid == uuid:
+                return level
+        return
 
     def store_spray(self, data: sprays.Spray) -> Spray:
         spray_id = data['uuid']
         self._sprays[spray_id] = spray = Spray(state=self, data=data)
-        for level in spray.levels:
-            self._spray_levels[level.uuid] = level
         return spray
 
     def _add_sprays(self, data: sprays.Sprays) -> None:
         spray_data = data['data']
         for spray in spray_data:
             spray_existing = self.get_spray(spray['uuid'])
             if spray_existing is None:
@@ -791,42 +761,54 @@
         return list(self._weapons.values())
 
     def get_weapon(self, uuid: Optional[str], /) -> Optional[Weapon]:
         return self._weapons.get(uuid)  # type: ignore
 
     @property
     def skins(self) -> List[Skin]:
-        return list(self._skins.values())
+        skins = []
+        for weapon in self.weapons:
+            skins.extend(weapon.skins)
+        return skins
 
     def get_skin(self, uuid: Optional[str], /) -> Optional[Skin]:
-        return self._skins.get(uuid)  # type: ignore
+        for skin in self.skins:
+            if skin.uuid == uuid:
+                return skin
+        return None
 
     @property
     def skin_chromas(self) -> List[SkinChroma]:
-        return list(self._skin_chromas.values())
+        chromas = []
+        for skin in self.skins:
+            chromas.extend(skin.chromas)
+        return chromas
 
     def get_skin_chroma(self, uuid: Optional[str], /) -> Optional[SkinChroma]:
-        return self._skin_chromas.get(uuid)  # type: ignore
+        for chroma in self.skin_chromas:
+            if chroma.uuid == uuid:
+                return chroma
+        return None
 
     @property
     def skin_levels(self) -> List[SkinLevel]:
-        return list(self._skin_levels.values())
+        levels = []
+        for skin in self.skins:
+            levels.extend(skin.levels)
+        return levels
 
     def get_skin_level(self, uuid: Optional[str], /) -> Optional[SkinLevel]:
-        return self._skin_levels.get(uuid)  # type: ignore
+        for level in self.skin_levels:
+            if level.uuid == uuid:
+                return level
+        return None
 
     def store_weapon(self, data: weapons.Weapon) -> Weapon:
         weapon_id = data['uuid']
         self._weapons[weapon_id] = weapon = Weapon(state=self, data=data)
-        for skin in weapon.skins:
-            self._skins[skin.uuid] = skin
-            for chroma in skin.chromas:
-                self._skin_chromas[chroma.uuid] = chroma
-            for level in skin.levels:
-                self._skin_levels[level.uuid] = level
         return weapon
 
     def _add_weapons(self, data: weapons.Weapons) -> None:
         weapon_data = data['data']
         for weapon in weapon_data:
             weapon_existing = self.get_weapon(weapon['uuid'])
             if weapon_existing is None:
```

### Comparing `valorant.py-1.0.1/valorant/client.py` & `valorant.py-1.0.2a0/valorant/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,22 @@
 __all__ = (
     'Client',
 )
 # fmt: on
 
 
 class Client:
-    def __init__(self, locale: Locale = Locale.american_english) -> None:
+    def __init__(
+        self,
+        locale: Locale = Locale.american_english
+        # *,
+        # enable_cache: bool = True,
+    ) -> None:
+        self.locale: Locale = locale
+        # self.enable_cache: bool = enable_cache
         self.http: HTTPClient = HTTPClient()
         self.cache: CacheState = CacheState(locale=locale, http=self.http)
         self._ready: asyncio.Event = MISSING
         self._closed: bool = False
 
     async def __aenter__(self) -> Self:
         await self.init()
@@ -457,33 +464,32 @@
     @property
     def skins(self) -> List[Skin]:
         return self.cache.skins
 
     def get_skin(self, uuid: str, /) -> Optional[Skin]:
         return self.cache.get_skin(uuid)
 
-    async def fetch_skin(self, uuid: str, /) -> Optional[Skin[Weapon]]:
+    async def fetch_skin(self, uuid: str, /) -> Optional[Skin]:
         await self.cache.fetch_weapons()
-        a = await self.fetch_skin(uuid)
         return self.get_skin(uuid)
 
     @property
     def skin_chromas(self) -> List[SkinChroma]:
         return self.cache.skin_chromas
 
-    def get_skin_chroma(self, uuid: str, /) -> Optional[SkinChroma[Skin]]:
+    def get_skin_chroma(self, uuid: str, /) -> Optional[SkinChroma]:
         return self.cache.get_skin_chroma(uuid)
 
-    async def fetch_skin_chroma(self, uuid: str, /) -> Optional[SkinChroma[Skin]]:
+    async def fetch_skin_chroma(self, uuid: str, /) -> Optional[SkinChroma]:
         await self.cache.fetch_weapons()
         return self.get_skin_chroma(uuid)
 
     @property
-    def skin_levels(self) -> List[SkinLevel[Skin]]:
+    def skin_levels(self) -> List[SkinLevel]:
         return self.cache.skin_levels
 
-    def get_skin_level(self, uuid: str, /) -> Optional[SkinLevel[Skin]]:
+    def get_skin_level(self, uuid: str, /) -> Optional[SkinLevel]:
         return self.cache.get_skin_level(uuid)
 
-    async def fetch_skin_level(self, uuid: str, /) -> Optional[SkinLevel[Skin]]:
+    async def fetch_skin_level(self, uuid: str, /) -> Optional[SkinLevel]:
         await self.cache.fetch_weapons()
         return self.get_skin_level(uuid)
```

### Comparing `valorant.py-1.0.1/valorant/enums.py` & `valorant.py-1.0.2a0/valorant/enums.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/errors.py` & `valorant.py-1.0.2a0/valorant/errors.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/file.py` & `valorant.py-1.0.2a0/valorant/file.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/http.py` & `valorant.py-1.0.2a0/valorant/http.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/localization.py` & `valorant.py-1.0.2a0/valorant/localization.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/__init__.py` & `valorant.py-1.0.2a0/valorant/models/__init__.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/abc.py` & `valorant.py-1.0.2a0/valorant/models/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     __slots__ = ('_uuid',)
 
     def __init__(self, uuid: str) -> None:
         self._uuid = uuid
 
     @property
     def uuid(self) -> str:
+        # TODO: str to UUID
         return self._uuid
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} uuid={self.uuid!r}>'
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, self.__class__) and self.uuid == other.uuid
@@ -70,15 +71,15 @@
 
 class GridPosition:
     def __init__(self, data: GridPositionPayload) -> None:
         self.row: float = data['row']
         self.column: float = data['column']
 
     def __repr__(self) -> str:
-        return f"<GridPosition row={self.row} column={self.column}>"
+        return f'<GridPosition row={self.row} column={self.column}>'
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, GridPosition) and self.row == other.row and self.column == other.column
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
@@ -97,29 +98,34 @@
         self._image: Optional[str] = data['image']
         self._new_image: Optional[str] = data['newImage']
         self._new_image_2: Optional[str] = data['newImage2']
         self.asset_path: str = data['assetPath']
         self._category_text_localized: Localization = Localization(self._category_text, locale=self._state.locale)
 
     def __repr__(self) -> str:
-        return f"<ShopData category_text={self.category_text} cost={self.cost}>"
+        return f'<ShopData category_text={self.category_text} cost={self.cost}>'
 
     def __int__(self) -> int:
         return self.cost
 
     def __eq__(self, other: object) -> bool:
-        return isinstance(other, ShopData) and self._image == other._image and self.cost == other.cost
+        return isinstance(other, ShopData) and self.item == other.item and self.cost == other.cost
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     def category_text_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._category_text_localized.from_locale(locale)
 
     @property
+    def item(self) -> Union[Weapon, Gear]:
+        """:class: `Weapon` or :class: `Gear` Returns the item."""
+        return self._item
+
+    @property
     def category_text(self) -> Localization:
         """:class: `str` Returns the weapon's shop category text."""
         return self._category_text_localized
 
     @property
     def image(self) -> Optional[Asset]:
         """:class: `Asset` Returns the weapon's image."""
```

### Comparing `valorant.py-1.0.1/valorant/models/agents.py` & `valorant.py-1.0.2a0/valorant/models/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,14 @@
 
     def __repr__(self) -> str:
         return f'<Role display_name={self.display_name!r}>'
 
     def __str__(self) -> str:
         return self.display_name.locale
 
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, Role) and other.uuid == self.uuid
-
-    def __ne__(self, other: object) -> bool:
-        return not self.__eq__(other)
-
-    def __hash__(self) -> int:
-        return hash(self.uuid)
-
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     def description_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._description_localized.from_locale(locale)
 
     @property
```

### Comparing `valorant.py-1.0.1/valorant/models/buddies.py` & `valorant.py-1.0.2a0/valorant/models/buddies.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict, Generic, List, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from ..asset import Asset
 from ..enums import Locale
 from ..localization import Localization
 from .abc import BaseModel
 
 if TYPE_CHECKING:
@@ -39,16 +39,14 @@
     from .themes import Theme
 
 __all__ = (
     'Buddy',
     'BuddyLevel',
 )
 
-BuddyT = TypeVar('BuddyT', bound='Buddy')
-
 
 class Buddy(BaseModel):
     def __init__(self, *, state: CacheState, data: BuddyPayload) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._is_hidden_if_not_owned: bool = data['isHiddenIfNotOwned']
@@ -105,24 +103,24 @@
         self._display_icon = buddy._display_icon
         self.asset_path = buddy.asset_path
         self.levels = buddy.levels.copy()
         self._name_localized = buddy._name_localized
         return self
 
 
-class BuddyLevel(BaseModel, Generic[BuddyT]):
-    def __init__(self, *, state: CacheState, data: BuddyLevelPayload, parent: BuddyT) -> None:
+class BuddyLevel(BaseModel):
+    def __init__(self, *, state: CacheState, data: BuddyLevelPayload, parent: Buddy) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._data: BuddyLevelPayload = data
         self.charm_level: int = data['charmLevel']
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._display_icon: Optional[str] = data['displayIcon']
         self.asset_path: str = data['assetPath']
-        self.parent: BuddyT = parent
+        self.parent: Buddy = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
         return f'<BuddyLevel display_name={self.display_name!r}>'
```

### Comparing `valorant.py-1.0.1/valorant/models/bundles.py` & `valorant.py-1.0.2a0/valorant/models/bundles.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/ceremonies.py` & `valorant.py-1.0.2a0/valorant/models/ceremonies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/competitive_tiers.py` & `valorant.py-1.0.2a0/valorant/models/competitive_tiers.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/content_tiers.py` & `valorant.py-1.0.2a0/valorant/models/content_tiers.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/contracts.py` & `valorant.py-1.0.2a0/valorant/models/contracts.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/currencies.py` & `valorant.py-1.0.2a0/valorant/models/currencies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/events.py` & `valorant.py-1.0.2a0/valorant/models/events.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/gamemodes.py` & `valorant.py-1.0.2a0/valorant/models/gamemodes.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/gear.py` & `valorant.py-1.0.2a0/valorant/models/gear.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/level_borders.py` & `valorant.py-1.0.2a0/valorant/models/level_borders.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/maps.py` & `valorant.py-1.0.2a0/valorant/models/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 if TYPE_CHECKING:
     from ..cache import CacheState
     from ..types.maps import Callout as CalloutPayload, Location as LocationPayload, Map as MapPayload
 
 # fmt: off
 __all__ = (
     'Map',
-    'MapCallout',
-    'MapLocation',
+    'Callout',
+    'Location',
 )
 # fmt: on
 
 
 class Location:
     def __init__(self, data: LocationPayload) -> None:
         self.x: float = data['x']
@@ -149,11 +149,7 @@
 
     @property
     def splash(self) -> Optional[Asset]:
         """:class: `Asset` Returns the mission's splash."""
         if self._splash is None:
             return None
         return Asset._from_url(state=self._state, url=self._splash)
-
-
-MapLocation = Location
-MapCallout = Callout
```

### Comparing `valorant.py-1.0.1/valorant/models/missions.py` & `valorant.py-1.0.2a0/valorant/models/missions.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/player_cards.py` & `valorant.py-1.0.2a0/valorant/models/player_cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
-        return f"<PlayerCard display_name={self.display_name!r}>"
+        return f'<PlayerCard display_name={self.display_name!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     @property
     def display_name(self) -> Localization:
         """:class: `str` Returns the player card's name."""
```

### Comparing `valorant.py-1.0.1/valorant/models/player_titles.py` & `valorant.py-1.0.2a0/valorant/models/player_titles.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
         self._title_text_localized: Localization = Localization(self._title_text, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.text.locale
 
     def __repr__(self) -> str:
-        return f"<PlayerTitle display_name={self.display_name!r} text={self.text!r}>"
+        return f'<PlayerTitle display_name={self.display_name!r} text={self.text!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     def title_text_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._title_text_localized.from_locale(locale)
```

### Comparing `valorant.py-1.0.1/valorant/models/seasons.py` & `valorant.py-1.0.2a0/valorant/models/seasons.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         return isinstance(other, Season) and other.id == self.id
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     @property
     def id(self) -> str:
-        return self._uuid
+        return self.uuid
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     @property
     def display_name(self) -> Localization:
         """:class: `str` Returns the season's name."""
```

### Comparing `valorant.py-1.0.1/valorant/models/sprays.py` & `valorant.py-1.0.2a0/valorant/models/sprays.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict, Generic, List, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from .. import utils
 from ..asset import Asset
 from ..enums import Locale
 from ..localization import Localization
 from .abc import BaseModel
 
@@ -40,16 +40,14 @@
     from .themes import Theme
 
 __all__ = (
     'Spray',
     'SprayLevel',
 )
 
-SprayT = TypeVar('SprayT', bound='Spray')
-
 
 class Spray(BaseModel):
     def __init__(self, *, state: CacheState, data: SprayPayload) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._data: SprayPayload = data
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
@@ -65,15 +63,15 @@
         self.levels: List[SprayLevel] = [SprayLevel(state=self._state, data=level, parent=self) for level in data['levels']]
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
-        return f"<Spray display_name={self.display_name!r}>"
+        return f'<Spray display_name={self.display_name!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         return self._display_name_localized.from_locale(locale)
 
     @property
     def display_name(self) -> Localization:
         """:class: `str` Returns the skin's name."""
@@ -146,24 +144,24 @@
         self._animation_gif = spray._animation_gif
         self.asset_path = spray.asset_path
         self.levels = spray.levels.copy()
         self._display_name_localized = spray._display_name_localized
         return self
 
 
-class SprayLevel(BaseModel, Generic[SprayT]):
-    def __init__(self, state: CacheState, data: SprayLevelPayload, parent: SprayT) -> None:
+class SprayLevel(BaseModel):
+    def __init__(self, state: CacheState, data: SprayLevelPayload, parent: Spray) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._data: SprayLevelPayload = data
         self.spray_level: int = data['sprayLevel']
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._display_icon: Optional[str] = data['displayIcon']
         self.asset_path: str = data['assetPath']
-        self.parent: SprayT = parent
+        self.parent: Spray = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
         return f'<SprayLevel display_name={self.display_name!r}>'
```

### Comparing `valorant.py-1.0.1/valorant/models/themes.py` & `valorant.py-1.0.2a0/valorant/models/themes.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/version.py` & `valorant.py-1.0.2a0/valorant/models/version.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/models/weapons.py` & `valorant.py-1.0.2a0/valorant/models/weapons.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, Generic, List, Optional, TypeVar, Union  # overload
+from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from .. import utils
 from ..asset import Asset
 from ..enums import MELEE_WEAPON_ID, Locale
 from ..localization import Localization
 from .abc import BaseModel, ShopData
 
@@ -58,17 +58,14 @@
     'Skin',
     'SkinChroma',
     'SkinLevel',
     'Weapon',
     'WeaponStats',
 )
 
-WeaponT = TypeVar('WeaponT', bound='Weapon', covariant=True)
-SkinT = TypeVar('SkinT', bound='Skin[Any]')
-
 
 class AdsStats:
     def __init__(self, data: AdsStatsPayload) -> None:
         self.zoom_multiplier: float = data['zoomMultiplier']
         self.fire_rate: float = data['fireRate']
         self.run_speed_multiplier: float = data['runSpeedMultiplier']
         self.burst_count: float = data['burstCount']
@@ -210,15 +207,14 @@
             self.weapon_stats = WeaponStats(data['weaponStats'])
         self.shop_data: Optional[ShopData] = None
         if data['shopData'] is not None:
             self.shop_data = ShopData(state=self._state, item=self, data=data['shopData'])
         self.skins: List[Skin] = [Skin(state=self._state, data=skin, parent=self) for skin in data['skins']]
         self._is_melee: bool = True if self.uuid == MELEE_WEAPON_ID else False
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
-        self._is_random: bool = 'random' in self.asset_path.lower()
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
         return f"<Weapon display_name={self.display_name!r}>"
 
@@ -229,15 +225,14 @@
     def display_name(self) -> Localization:
         """:class: `str` Returns the weapon's name."""
         return self._display_name_localized
 
     @property
     def category(self) -> str:
         """:class: `str` Returns the weapon's category."""
-        #  self._category.removeprefix("EEquippableCategory::")
         return utils.removeprefix(self._category, "EEquippableCategory::")
 
     @property
     def display_icon(self) -> Asset:
         """:class: `Asset` Returns the weapon's icon."""
         return Asset._from_url(self._state, self._display_icon)
 
@@ -251,19 +246,14 @@
         return self._is_melee
 
     @property
     def stats(self) -> Optional[WeaponStats]:
         """:class: `Optional[WeaponStats]` alias for :attr: `weapon_stats`"""
         return self.weapon_stats
 
-    # helpers
-
-    def is_random(self) -> bool:
-        return self._is_random
-
     @classmethod
     def _copy(cls, weapon: Self) -> Self:
         self = cls.__new__(cls)  # bypass __init__
         self._uuid = weapon._uuid
         self._state = weapon._state
         self._data = weapon._data.copy()
         self._display_name = weapon._display_name
@@ -273,26 +263,24 @@
         self._kill_stream_icon = weapon._kill_stream_icon
         self.asset_path = weapon.asset_path
         self.weapon_stats = weapon.weapon_stats
         self.shop_data = weapon.shop_data
         self.skins = weapon.skins
         self._is_melee = weapon._is_melee
         self._display_name_localized = weapon._display_name_localized
-        self._is_random = weapon._is_random
         return self
 
-    # @classmethod
-    # def _from_uuid(cls, client: Client, uuid: str) -> Optional[Self]:
-    #     """Returns the weapon with the given UUID."""
-    #     data = client._assets.get_weapon(uuid)
-    #     return cls(client=client, data=data) if data else None
+    # helpers
+
+    def is_random(self) -> bool:
+        return 'random' in self.asset_path.lower()
 
 
-class Skin(BaseModel, Generic[WeaponT]):
-    def __init__(self, *, state: CacheState, data: SkinPayload, parent: WeaponT) -> None:
+class Skin(BaseModel):
+    def __init__(self, *, state: CacheState, data: SkinPayload, parent: Weapon) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._data: SkinPayload = data
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._theme_uuid: str = data['themeUuid']
         self._content_tier_uuid: Optional[str] = data['contentTierUuid']
         self._display_icon: str = data['displayIcon']
@@ -301,17 +289,16 @@
         self.chromas: List[SkinChroma] = [
             SkinChroma(state=self._state, data=chroma, parent=self) for chroma in data['chromas']
         ]
         self.levels: List[SkinLevel] = [
             SkinLevel(state=self._state, data=level, parent=self, level_number=index)
             for index, level in enumerate(data['levels'])
         ]
-        self.parent: WeaponT = parent
+        self.parent: Weapon = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
-        self._is_random: bool = 'random' in self.asset_path.lower()
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
         return f"<Skin display_name={self.display_name!r}>"
 
@@ -363,15 +350,15 @@
         return Asset._from_url(self._state, url=self._wallpaper)
 
     def is_melee(self) -> bool:
         """:class: `bool` Returns whether the bundle is a melee."""
         return self.parent.is_melee()
 
     def is_random(self) -> bool:
-        return self._is_random
+        return 'random' in self.asset_path.lower()
 
     @classmethod
     def _copy(cls, skin: Self) -> Self:
         self = cls.__new__(cls)  # bypass __init__
         self._uuid = skin._uuid
         self._state = skin._state
         self._data = skin._data.copy()
@@ -381,17 +368,18 @@
         self._display_icon = skin._display_icon
         self._wallpaper = skin._wallpaper
         self.asset_path = skin.asset_path
         self.chromas = skin.chromas.copy()
         self.levels = skin.levels.copy()
         self.parent = skin.parent
         self._display_name_localized = skin._display_name_localized
-        self._is_random = skin._is_random
         return self
 
+    # helpers
+
     def get_skin_level(self, level: int) -> Optional[SkinLevel]:
         """get the skin's level with the given level.
 
         Parameters
         ----------
         level: :class: `int`
             The level of the skin level to get.
@@ -400,34 +388,33 @@
         -------
         Optional[:class: `SkinLevel`]
             The skin level with the given level.
         """
         return next((skin_level for skin_level in self.levels if skin_level.level_number == level), None)
 
 
-class SkinChroma(BaseModel, Generic[SkinT]):
-    def __init__(self, *, state: CacheState, data: SkinChromaPayload, parent: SkinT) -> None:
+class SkinChroma(BaseModel):
+    def __init__(self, *, state: CacheState, data: SkinChromaPayload, parent: Skin) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._data: SkinChromaPayload = data
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._display_icon: Optional[str] = data['displayIcon']
         self._full_render: str = data['fullRender']
         self._swatch: Optional[str] = data['swatch']
         self._streamed_video: Optional[str] = data['streamedVideo']
         self.asset_path: str = data['assetPath']
-        self.parent: SkinT = parent
+        self.parent: Skin = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
-        self._is_random: bool = 'random' in self.asset_path.lower()
 
     def __str__(self) -> str:
         return self.display_name.locale
 
     def __repr__(self) -> str:
-        return f"<SkinChroma display_name={self.display_name!r}>"
+        return f'<SkinChroma display_name={self.display_name!r}>'
 
     def display_name_localized(self, locale: Optional[Union[Locale, str]] = None) -> str:
         """Returns the skin's display name localized to the given locale."""
         return self._display_name_localized.from_locale(locale=locale)
 
     @property
     def display_name(self) -> Localization:
@@ -486,15 +473,32 @@
         return Asset._from_url(self._state, url=self._streamed_video)
 
     @property
     def video(self) -> Optional[Asset]:
         """:class: `Asset` alias for streamed_video."""
         return self.streamed_video
 
-    # helper properties
+    @classmethod
+    def _copy(cls, skin_chroma: Self) -> Self:
+        """Copies the given skin_chroma with the given parent."""
+        self = cls.__new__(cls)  # bypass __init__
+        self._uuid = skin_chroma._uuid
+        self._state = skin_chroma._state
+        self._data = skin_chroma._data.copy()
+        self._display_name = skin_chroma._display_name
+        self._display_icon = skin_chroma._display_icon
+        self._full_render = skin_chroma._full_render
+        self._swatch = skin_chroma._swatch
+        self._streamed_video = skin_chroma._streamed_video
+        self.asset_path = skin_chroma.asset_path
+        self.parent = skin_chroma.parent
+        self._display_name_localized = skin_chroma._display_name_localized
+        return self
+
+    # helpers
 
     @property
     def theme(self) -> Optional[Theme]:
         """:class: `Theme` Returns the skin's theme uuid."""
         return self.parent.theme
 
     @property
@@ -507,48 +511,32 @@
         """:class: `ContentTier` alias for content_tier."""
         return self.content_tier
 
     def is_melee(self) -> bool:
         """:class: `bool` Returns whether the bundle is a melee."""
         return self.parent.is_melee()
 
-    @classmethod
-    def _copy(cls, skin_chroma: Self) -> Self:
-        """Copies the given skin_chroma with the given parent."""
-        self = cls.__new__(cls)  # bypass __init__
-        self._uuid = skin_chroma._uuid
-        self._state = skin_chroma._state
-        self._data = skin_chroma._data.copy()
-        self._display_name = skin_chroma._display_name
-        self._display_icon = skin_chroma._display_icon
-        self._full_render = skin_chroma._full_render
-        self._swatch = skin_chroma._swatch
-        self._streamed_video = skin_chroma._streamed_video
-        self.asset_path = skin_chroma.asset_path
-        self.parent = skin_chroma.parent
-        self._display_name_localized = skin_chroma._display_name_localized
-        self._is_random = skin_chroma._is_random
-        return self
+    def is_random(self) -> bool:
+        return 'random' in self.asset_path.lower()
 
 
-class SkinLevel(BaseModel, Generic[SkinT]):
-    def __init__(self, *, state: CacheState, data: SkinLevelPayload, parent: SkinT, level_number: int) -> None:
+class SkinLevel(BaseModel):
+    def __init__(self, *, state: CacheState, data: SkinLevelPayload, parent: Skin, level_number: int) -> None:
         super().__init__(data['uuid'])
         self._state: CacheState = state
         self._data: SkinLevelPayload = data
         self._display_name: Union[str, Dict[str, str]] = data['displayName']
         self._level: Optional[str] = data['levelItem']
         self._display_icon: Optional[str] = data['displayIcon']
         self._streamed_video: Optional[str] = data['streamedVideo']
         self.asset_path: str = data['assetPath']
         self._level_number: int = level_number
         self._is_level_one: bool = level_number == 0
-        self.parent: SkinT = parent
+        self.parent: Skin = parent
         self._display_name_localized: Localization = Localization(self._display_name, locale=self._state.locale)
-        self._is_random: bool = 'random' in self.asset_path.lower()
 
     def __str__(self) -> str:
         return str(self.display_name)
 
     def __repr__(self) -> str:
         return f"<SkinLevel display_name={self.display_name!r} level={self.level!r}>"
 
@@ -601,15 +589,33 @@
         """:class: `Asset` alias for streamed_video."""
         return self.streamed_video
 
     def is_level_one(self) -> bool:
         """:class: `bool` Returns whether the skin is level one."""
         return self._is_level_one
 
-    # helper properties
+    @classmethod
+    def _copy(cls, skin_level: Self) -> Self:
+        """Copies the given skin_level with the given parent."""
+        self = cls.__new__(cls)  # bypass __init__
+        self._uuid = skin_level._uuid
+        self._state = skin_level._state
+        self._data = skin_level._data.copy()
+        self._display_name = skin_level._display_name
+        self._level = skin_level._level
+        self._display_icon = skin_level._display_icon
+        self._streamed_video = skin_level._streamed_video
+        self.asset_path = skin_level.asset_path
+        self._level_number = skin_level._level_number
+        self._is_level_one = skin_level._is_level_one
+        self.parent = skin_level.parent._copy(skin_level.parent)
+        self._display_name_localized = skin_level._display_name_localized
+        return self
+
+    # helpers
 
     @property
     def level_number(self) -> int:
         """:class: `int` Returns the skin's level number."""
         return self._level_number
 
     @property
@@ -629,27 +635,8 @@
 
     def is_melee(self) -> bool:
         """:class: `bool` Returns whether the bundle is a melee."""
         return self.parent.is_melee()
 
     def is_random(self) -> bool:
         """:class: `bool` Returns whether the skin is random."""
-        return self._is_random
-
-    @classmethod
-    def _copy(cls, skin_level: Self) -> Self:
-        """Copies the given skin_level with the given parent."""
-        self = cls.__new__(cls)  # bypass __init__
-        self._uuid = skin_level._uuid
-        self._state = skin_level._state
-        self._data = skin_level._data.copy()
-        self._display_name = skin_level._display_name
-        self._level = skin_level._level
-        self._display_icon = skin_level._display_icon
-        self._streamed_video = skin_level._streamed_video
-        self.asset_path = skin_level.asset_path
-        self._level_number = skin_level._level_number
-        self._is_level_one = skin_level._is_level_one
-        self.parent = skin_level.parent._copy(skin_level.parent)
-        self._display_name_localized = skin_level._display_name_localized
-        self._is_random = skin_level._is_random
-        return self
+        return 'random' in self.asset_path.lower()
```

### Comparing `valorant.py-1.0.1/valorant/types/agents.py` & `valorant.py-1.0.2a0/valorant/types/agents.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/buddies.py` & `valorant.py-1.0.2a0/valorant/types/buddies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/bundles.py` & `valorant.py-1.0.2a0/valorant/types/bundles.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/ceremonies.py` & `valorant.py-1.0.2a0/valorant/types/ceremonies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/competitive_tiers.py` & `valorant.py-1.0.2a0/valorant/types/competitive_tiers.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/content_tiers.py` & `valorant.py-1.0.2a0/valorant/types/content_tiers.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/contracts.py` & `valorant.py-1.0.2a0/valorant/types/contracts.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/currencies.py` & `valorant.py-1.0.2a0/valorant/types/currencies.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/events.py` & `valorant.py-1.0.2a0/valorant/types/events.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/gamemodes.py` & `valorant.py-1.0.2a0/valorant/types/gamemodes.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/gear.py` & `valorant.py-1.0.2a0/valorant/types/gear.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/level_borders.py` & `valorant.py-1.0.2a0/valorant/types/level_borders.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/maps.py` & `valorant.py-1.0.2a0/valorant/types/maps.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/missions.py` & `valorant.py-1.0.2a0/valorant/types/missions.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/object.py` & `valorant.py-1.0.2a0/valorant/types/object.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/player_cards.py` & `valorant.py-1.0.2a0/valorant/types/player_cards.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/player_titles.py` & `valorant.py-1.0.2a0/valorant/types/player_titles.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/response.py` & `valorant.py-1.0.2a0/valorant/types/response.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/seasons.py` & `valorant.py-1.0.2a0/valorant/types/seasons.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/sprays.py` & `valorant.py-1.0.2a0/valorant/types/sprays.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/themes.py` & `valorant.py-1.0.2a0/valorant/types/themes.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/version.py` & `valorant.py-1.0.2a0/valorant/types/version.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/types/weapons.py` & `valorant.py-1.0.2a0/valorant/types/weapons.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant/utils.py` & `valorant.py-1.0.2a0/valorant/utils.py`

 * *Files identical despite different names*

### Comparing `valorant.py-1.0.1/valorant.py.egg-info/PKG-INFO` & `valorant.py-1.0.2a0/valorant.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valorant.py
-Version: 1.0.1
+Version: 1.0.2a0
 Summary: An Asynchronous Unofficial Valorant API Wrapper for Python
 Home-page: https://github.com/staciax/valorant
 Author: STACiA
 License: MIT
 Project-URL: Issue tracker, https://github.com/staciax/valorant/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `valorant.py-1.0.1/valorant.py.egg-info/SOURCES.txt` & `valorant.py-1.0.2a0/valorant.py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
 tests/test_client.py
-tests/test_valorant_api.py
+tests/test_models.py
 valorant/__init__.py
 valorant/asset.py
 valorant/cache.py
 valorant/client.py
 valorant/enums.py
 valorant/errors.py
 valorant/file.py
```


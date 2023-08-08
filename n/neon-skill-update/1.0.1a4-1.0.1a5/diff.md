# Comparing `tmp/neon-skill-update-1.0.1a4.tar.gz` & `tmp/neon-skill-update-1.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-1.0.1a4.tar", last modified: Mon Aug  7 21:10:15 2023, max compression
+gzip compressed data, was "neon-skill-update-1.0.1a5.tar", last modified: Tue Aug  8 23:48:03 2023, max compression
```

## Comparing `neon-skill-update-1.0.1a4.tar` & `neon-skill-update-1.0.1a5.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.211546 neon-skill-update-1.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-07 21:10:15.211546 neon-skill-update-1.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.199546 neon-skill-update-1.0.1a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.199546 neon-skill-update-1.0.1a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.207546 neon-skill-update-1.0.1a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/error_updating_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_downloading_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_downloading_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_os_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_update_failure.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_update_success.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/update_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/update_system.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.207546 neon-skill-update-1.0.1a4/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.207546 neon-skill-update-1.0.1a4/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.207546 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-07 21:10:15.000000 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-07 21:10:15.000000 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:10:15.000000 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 21:10:15.000000 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-07 21:10:15.000000 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 21:10:15.000000 neon-skill-update-1.0.1a4/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 21:10:15.211546 neon-skill-update-1.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:10:15.211546 neon-skill-update-1.0.1a4/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-07 21:10:11.000000 neon-skill-update-1.0.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.187320 neon-skill-update-1.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-08 23:48:03.187320 neon-skill-update-1.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23832 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.175320 neon-skill-update-1.0.1a5/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.175320 neon-skill-update-1.0.1a5/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.183320 neon-skill-update-1.0.1a5/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/error_updating_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/help_online.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/help_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_downloading_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_downloading_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_os_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/update_initramfs_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/update_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/update_system.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.183320 neon-skill-update-1.0.1a5/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.183320 neon-skill-update-1.0.1a5/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.183320 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-08 23:48:03.000000 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-08 23:48:03.000000 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:48:03.000000 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 23:48:03.000000 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-08 23:48:03.000000 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 23:48:03.000000 neon-skill-update-1.0.1a5/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:48:03.187320 neon-skill-update-1.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:03.183320 neon-skill-update-1.0.1a5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-08 23:47:58.000000 neon-skill-update-1.0.1a5/version.py
```

### Comparing `neon-skill-update-1.0.1a4/LICENSE.md` & `neon-skill-update-1.0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a4/PKG-INFO` & `neon-skill-update-1.0.1a5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 1.0.1a4
+Version: 1.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-1.0.1a4/README.md` & `neon-skill-update-1.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a4/__init__.py` & `neon-skill-update-1.0.1a5/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,62 +189,70 @@
         if get_user_prefs(message)['response_mode'].get('hesitation'):
             self.speak_dialog("check_updates")
         initramfs_available = False
         squashfs_available = False
 
         if self.check_initramfs:
             initramfs_available = self._check_initramfs_update(message)
+            LOG.info(f"initramfs_available={initramfs_available}")
         if self.check_squashfs:
             squashfs_available = self._check_squashfs_update(message)
+            LOG.info(f"squashfs_available={squashfs_available}")
 
         if initramfs_available or squashfs_available:
             resp = self.ask_yesno("update_system")
             if resp == "yes":
                 self.speak_dialog("starting_update", wait=True)
-
+                self.gui.show_controlled_notification(
+                    self.translate("notify_downloading_update"))
                 if initramfs_available:
                     LOG.info("Updating initramfs")
+                    # Force update since we already checked for updates
                     resp = self.bus.wait_for_response(
-                        message.forward("neon.update_initramfs"), timeout=30)
+                        message.forward("neon.update_initramfs",
+                                        {"force_update": True}), timeout=60)
                     if resp and resp.data.get("updated"):
                         LOG.info("initramfs updated")
-                        # TODO: Speak?
+                        self.speak_dialog("update_initramfs_success")
                     else:
                         error = resp.data.get("error")
                         LOG.error(f"initramfs update failed: {error}")
-                        self.speak_dialog("error_updating_os")
+                        self.speak_dialog("error_updating_os",
+                                          {"help":
+                                           self.translate("help_support")})
+                        self.gui.remove_controlled_notification()
                         return
                 if squashfs_available:
                     self._write_update_signal("squashfs")
 
-                    self.gui.show_controlled_notification(
-                        self.translate("notify_downloading_update"))
-
                     LOG.info("Updating squashfs")
                     resp = self.bus.wait_for_response(
                         message.forward("neon.update_squashfs"), timeout=1800)
                     if not resp:
                         LOG.warning(f"Timed out waiting for download")
                         self.gui.remove_controlled_notification()
-                        self.speak_dialog("error_updating_os")
+                        self.speak_dialog("error_updating_os",
+                                          {"help":
+                                           self.translate("help_online")})
+                        self.gui.remove_controlled_notification()
                         return
                     self.gui.remove_controlled_notification()
                     if resp.data.get("new_version"):
                         LOG.info("squashfs updated")
                         self.speak_dialog("update_restarting", wait=True)
                         self.bus.emit(message.forward("system.reboot"))
                     else:
                         error = "no response"
                         if resp:
                             error = resp.data.get("error")
                         LOG.error(f"squashfs update failed: {error}")
                         self.speak_dialog("error_updating_os")
+                        self.gui.remove_controlled_notification()
                         return
-
-                return
+                self.gui.remove_controlled_notification()
         # No OS update available or user declined, check core updates
         self._check_package_update(message)
 
     def _check_initramfs_update(self, message) -> bool:
         """
         Check for an updated initramfs image
         """
```

### Comparing `neon-skill-update-1.0.1a4/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-1.0.1a5/neon_skill_update.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 1.0.1a4
+Version: 1.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-1.0.1a4/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-1.0.1a5/neon_skill_update.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 locale/en-us/dialog/confirm_no_change_update_track.dialog
 locale/en-us/dialog/core_version.dialog
 locale/en-us/dialog/downloading_image.dialog
 locale/en-us/dialog/drive_instructions.dialog
 locale/en-us/dialog/error_installing_os.dialog
 locale/en-us/dialog/error_offline.dialog
 locale/en-us/dialog/error_updating_os.dialog
+locale/en-us/dialog/help_online.dialog
+locale/en-us/dialog/help_support.dialog
 locale/en-us/dialog/installation_complete.dialog
 locale/en-us/dialog/not_updating.dialog
 locale/en-us/dialog/notify_download_complete.dialog
 locale/en-us/dialog/notify_download_failed.dialog
 locale/en-us/dialog/notify_downloading_os.dialog
 locale/en-us/dialog/notify_downloading_update.dialog
 locale/en-us/dialog/notify_installation_complete.dialog
@@ -33,14 +35,15 @@
 locale/en-us/dialog/notify_update_success.dialog
 locale/en-us/dialog/notify_writing_image.dialog
 locale/en-us/dialog/point.dialog
 locale/en-us/dialog/starting_installation.dialog
 locale/en-us/dialog/starting_update.dialog
 locale/en-us/dialog/up_to_date.dialog
 locale/en-us/dialog/update_core.dialog
+locale/en-us/dialog/update_initramfs_success.dialog
 locale/en-us/dialog/update_restarting.dialog
 locale/en-us/dialog/update_system.dialog
 locale/en-us/dialog/update_track_already_set.dialog
 locale/en-us/dialog/word_beta.dialog
 locale/en-us/dialog/word_stable.dialog
 locale/en-us/intent/core_version.intent
 locale/en-us/intent/update_configuration.intent
```

### Comparing `neon-skill-update-1.0.1a4/setup.py` & `neon-skill-update-1.0.1a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a4/skill.json` & `neon-skill-update-1.0.1a5/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a4/test/test_skill.py` & `neon-skill-update-1.0.1a5/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-1.0.1a4/version.py` & `neon-skill-update-1.0.1a5/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a4"
+__version__ = "1.0.1a5"
```


# Comparing `tmp/inhandtest-0.0.63.tar.gz` & `tmp/inhandtest-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.63.tar", last modified: Wed Aug  2 06:09:21 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.64.tar", last modified: Wed Aug  9 01:56:57 2023, max compression
```

## Comparing `inhandtest-0.0.63.tar` & `inhandtest-0.0.64.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.63/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-08-02 06:09:21.000000 inhandtest-0.0.63/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.63/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.63/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.63/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.63/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.63/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.63/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    66800 2023-07-28 06:14:30.000000 inhandtest-0.0.63/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    27535 2023-08-01 07:15:28.000000 inhandtest-0.0.63/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.63/inhandtest/exception.py
--rw-rw-rw-   0        0        0     6365 2023-08-01 03:34:58.000000 inhandtest-0.0.63/inhandtest/file.py
--rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.63/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.63/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.63/inhandtest/inmqtt.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/inrequest/
--rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.63/inhandtest/inrequest/__init__.py
--rw-rw-rw-   0        0        0    10424 2023-07-20 10:21:59.000000 inhandtest-0.0.63/inhandtest/inrequest/console.py
--rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.63/inhandtest/inrequest/dm.py
--rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.63/inhandtest/inrequest/dn.py
--rw-rw-rw-   0        0        0    14989 2023-07-24 08:32:31.000000 inhandtest-0.0.63/inhandtest/inrequest/er_default_config.py
--rw-rw-rw-   0        0        0    37418 2023-07-27 06:47:07.000000 inhandtest-0.0.63/inhandtest/inrequest/er_device.py
--rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.63/inhandtest/inrequest/ics.py
--rw-rw-rw-   0        0        0    11198 2023-08-02 01:37:41.000000 inhandtest-0.0.63/inhandtest/inrequest/inrequest.py
--rw-rw-rw-   0        0        0    53371 2023-08-02 01:43:31.000000 inhandtest-0.0.63/inhandtest/inrequest/nezha.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.63/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.63/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.63/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.63/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.63/inhandtest/log.py
--rw-rw-rw-   0        0        0    15229 2023-07-18 03:57:23.000000 inhandtest-0.0.63/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.63/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.63/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    68401 2023-07-28 06:15:35.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    75780 2023-07-28 06:11:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3617 2023-07-28 06:11:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    12188 2023-07-24 09:42:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.63/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.63/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    35543 2023-07-27 03:55:47.000000 inhandtest-0.0.63/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    30974 2023-07-27 05:13:54.000000 inhandtest-0.0.63/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:09:21.000000 inhandtest-0.0.63/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1919 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 06:09:20.000000 inhandtest-0.0.63/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      155 2023-07-24 08:29:33.000000 inhandtest-0.0.63/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 06:09:21.000000 inhandtest-0.0.63/setup.cfg
--rw-rw-rw-   0        0        0     1625 2023-08-02 06:09:07.000000 inhandtest-0.0.63/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.64/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-08-09 01:56:57.000000 inhandtest-0.0.64/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.64/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.64/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.64/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43266 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.64/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.64/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    68503 2023-08-09 01:16:15.000000 inhandtest-0.0.64/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    26502 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.64/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     6365 2023-08-01 03:34:58.000000 inhandtest-0.0.64/inhandtest/file.py
+-rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.64/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.64/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.64/inhandtest/inmqtt.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/inrequest/
+-rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.64/inhandtest/inrequest/__init__.py
+-rw-rw-rw-   0        0        0    10424 2023-07-20 10:21:59.000000 inhandtest-0.0.64/inhandtest/inrequest/console.py
+-rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.64/inhandtest/inrequest/dm.py
+-rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.64/inhandtest/inrequest/dn.py
+-rw-rw-rw-   0        0        0    14989 2023-07-24 08:32:31.000000 inhandtest-0.0.64/inhandtest/inrequest/er_default_config.py
+-rw-rw-rw-   0        0        0    37676 2023-08-09 01:23:51.000000 inhandtest-0.0.64/inhandtest/inrequest/er_device.py
+-rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.64/inhandtest/inrequest/ics.py
+-rw-rw-rw-   0        0        0    11198 2023-08-02 01:37:41.000000 inhandtest-0.0.64/inhandtest/inrequest/inrequest.py
+-rw-rw-rw-   0        0        0    66708 2023-08-09 01:56:10.000000 inhandtest-0.0.64/inhandtest/inrequest/nezha.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.64/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.64/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.64/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.64/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.64/inhandtest/log.py
+-rw-rw-rw-   0        0        0    17122 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.64/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.64/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    69571 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    76675 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3957 2023-08-09 01:15:46.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    12497 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    88185 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    31244 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.64/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    35473 2023-08-08 10:35:19.000000 inhandtest-0.0.64/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    31148 2023-08-08 10:26:39.000000 inhandtest-0.0.64/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-09 01:56:57.000000 inhandtest-0.0.64/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      155 2023-07-24 08:29:33.000000 inhandtest-0.0.64/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 01:56:57.000000 inhandtest-0.0.64/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2023-08-09 01:56:42.000000 inhandtest-0.0.64/setup.py
```

### Comparing `inhandtest-0.0.63/PKG-INFO` & `inhandtest-0.0.64/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.63
+Version: 0.0.64
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.63/README.md` & `inhandtest-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.64/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                                    'docker_manager': 'Docker Manager', 'cloud_edge_computing': 'Cloud Edge Computing',
                                    'device_supervisor': 'Device Supervisor', 'measure_monitor': 'Measure Monitor',
                                    'monitoring_list': 'Monitoring List', 'group': 'Group',
                                    'controller_template': 'Controller Template',
                                    'alarm': 'Alarm', 'realtime_alarms': 'Realtime Alarms', 'alarm_rules': 'Alarm Rules',
                                    'history_alarms': 'History Alarms', 'alarm_label': 'Alarm Label',
                                    'cloud': 'Cloud', 'mqtt_cloud_service': 'MQTT Cloud Service',
-                                   'whitehawk_energy_manager': 'Whitehawk Energy Manager', 'protocol': 'Protocol',
+                                   'whiteeagle_energy_manager': 'WhiteEagle Energy Manager', 'protocol': 'Protocol',
                                    'parameter_settings': 'Parameter Settings',
                                    'custom_quickfunctions': 'Custom QuickFunctions',
                                    'system': 'System', 'system_time': 'System Time', 'system_log': 'Log',
                                    'clear_history_log': 'Clear History Log',
                                    'system_config': 'Configuration Management', 'system_cloud': 'InHand Cloud',
                                    'system_firmware': 'Firmware Upgrade', 'system_tools': 'Access Tools',
                                    'system_user_management': 'User Management', 'system_reboot': 'Reboot',
@@ -76,15 +76,15 @@
                                    'edge': '边缘计算', 'python_edge': 'Python边缘计算', 'docker_manager': 'Docker 管理',
                                    'cloud_edge_computing': '公有云边缘计算', 'device_supervisor': '设备监控',
                                    'measure_monitor': '测点监控', 'monitoring_list': '监控列表', 'group': '分组',
                                    'controller_template': '控制器模板',
                                    'alarm': '告警', 'realtime_alarms': '实时告警', 'alarm_rules': '告警规则',
                                    'history_alarms': '历史告警', 'alarm_label': '告警标签',
                                    'cloud': '云服务', 'mqtt_cloud_service': 'MQTT云服务',
-                                   'whitehawk_energy_manager': '白鹰能源管家', 'protocol': '协议转换',
+                                   'whiteeagle_energy_manager': '白鹰能源管家', 'protocol': '协议转换',
                                    'parameter_settings': '参数设置', 'custom_quickfunctions': '自定义快函数',
                                    'system': '系统管理', 'system_time': '系统时间', 'system_log': '系统日志',
                                    'clear_history_log': '清除历史日志',
                                    'system_config': '配置管理', 'system_cloud': '设备云平台',
                                    'system_firmware': '固件升级', 'system_tools': '管理工具',
                                    'system_user_management': '用户管理', 'system_reboot': '重启',
                                    'system_network_tools': '工具', 'system_3rd_party': '第三方软件声明',
@@ -603,20 +603,20 @@
                                             'aria-selected': 'true'}},
                                     'wait_locator': [
                                         self.page.locator('.ant-modal-content').locator('.ant-table-content')]
                                 },
 
                             }
                         },
-                        'whitehawk_energy_manager': {
+                        'whiteeagle_energy_manager': {
                             'menu': self.page.locator(
-                                f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'),
+                                f'div:text-is("{self.__locale.get("whiteeagle_energy_manager")}")'),
                             'attributes': {
                                 self.page.locator(
-                                    f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'): {
+                                    f'div:text-is("{self.__locale.get("whiteeagle_energy_manager")}")'): {
                                     'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('//label[@for="enable.form"]')]
                         }
                     },
                     'protocol': {
                         'default': 'modbus_tcp_slave',
                         'menu': self.protocol_menu,
```

### Comparing `inhandtest-0.0.63/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.64/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.64/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/base_page/base_page.py` & `inhandtest-0.0.64/inhandtest/base_page/base_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @Author  : Pane Li
 # @File    : base_page.py
 """
 base_page
 
 """
 import os.path
+import time
 from os import path
 import playwright
 from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
 from inhandtest.tools import replace_str
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
@@ -37,26 +38,29 @@
         :param model: 'VG710'|'ER805'|'ER605'|'IR302'|'IG502'|'IG902'|'IR305'|'IR615'
         :param page: 当page为None时，自动打开浏览器及页面，否则使用传入的page
         :param kwargs:
                       browser: 当没有传入page时，可以选择浏览器
                       locale: dict 国际化
                       bring_to_front: bool 是否将浏览器窗口置顶
                       viewport: {'width': 1366, 'height': 768}  浏览器窗口大小
+                      web_login_timeout: int  登录超时时间 默认300， 单位秒 即5分钟， 监测到登录超时后，会自动重新登录
         """
         self.page = page
         self.host = host
         self.model = model.upper()
         self.protocol = protocol
         self.port = port
         self.username = username
         self.password = password
         self.language = language
         self.bring_to_front = kwargs.get('bring_to_front', False)
         self.__browser_type = kwargs.get('browser')
         self.__http_credentials_model = ('VG710',)  # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
+        self.__web_login_timeout = kwargs.get('web_login_timeout', 300)
+        self.__logout_time = None
         self.viewport = kwargs.get('viewport', {'width': 1366, 'height': 768})
         if self.page is None:
             self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IG902', 'IG502'):
             self.content_locator = IGContentsLocators(self.page, language).tags_menu
@@ -69,14 +73,22 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def call_web_login_timeout(self, response):
+        if response.status == 401:
+            # 当页面的token过期时，可能会连续几个API返回401，这里只处理一次，避免重复登录
+            if self.__logout_time is None or (int(time.time()) - self.__logout_time) > self.__web_login_timeout:
+                logging.warning(f'login timeout, try to login again')
+                self.__logout_time = int(time.time())
+                self.login(self.username, self.password)
+
     @property
     def __login_locator(self) -> dict:
         if self.model == 'VG710':
             return {'wait_locator': self.page.locator('#logo')}
         elif self.model in ('ER805', 'ER605'):
             return {'username': self.page.locator('#username'), 'password': self.page.locator('#password'),
                     'submit': self.page.locator('button'),
@@ -151,35 +163,34 @@
                 logging.debug('Device %s fill password %s' % (self.host, password))
                 self.__login_locator.get('submit').click()
                 logging.info("Device %s  login" % self.host)
                 if status == 'success':
                     self.__login_locator.get('wait_locator').wait_for(state='visible')
                     self.page.wait_for_timeout(500)
 
-        for i in range(0, 10):
-            if self.__login_locator.get('username') and self.__login_locator.get(
-                    'username').is_visible():
-                _login()
-                break
-            elif self.__login_locator.get('wait_locator') and self.__login_locator.get(
-                    'wait_locator').is_visible():
-                break
-            elif self.page.url == 'about:blank':
-                goto_router()
-                _login()
-                break
-            else:
-                try:
-                    logging.debug(f"Device %s refresh page {i + 1} times" % self.host)
-                    self.page.reload()
-                except TimeoutError:
-                    pass
+        self.page.wait_for_load_state('domcontentloaded', timeout=15 * 1000)
+        if self.__login_locator.get('username') and self.__login_locator.get('username').is_visible():
+            _login()
+        elif self.__login_locator.get('wait_locator') and self.__login_locator.get(
+                'wait_locator').is_visible():
+            pass
+        elif self.page.url == 'about:blank':
+            goto_router()
+            _login()
         else:
-            logging.exception(f'Device {self.host} page error')
-            raise Exception(f'Device {self.host} page error')
+            try:
+                self.page.reload()
+                logging.debug(f"Device %s refresh page" % self.host)
+                self.__login_locator.get('wait_locator').wait_for(state='visible', timeout=10 * 1000)
+            except TimeoutError:
+                if self.__login_locator.get('username') and self.__login_locator.get(
+                        'username').is_visible():
+                    _login()
+                else:
+                    logging.error(f"Device {self.host} page is error")
 
     @allure.step('页面抓取接口返回结果')
     def wait_for_response(self, url: str, timeout=30) -> dict:
         """
 
         :param url:  pattern 匹配的正则表达式,
         :param timeout: 默认30秒
@@ -696,15 +707,16 @@
         """
         if messages:
             if isinstance(messages, str):
                 tip_messages = [self.locale.get(messages)] if self.locale.get(messages) else [messages]
             elif isinstance(messages, re.Pattern):
                 tip_messages = [messages]  # 正则表达式 时需要自己做国际化转换
             elif isinstance(messages, list):
-                tip_messages = [self.locale.get(message) if self.locale.get(message) else message for message in messages]
+                tip_messages = [self.locale.get(message) if self.locale.get(message) else message for message in
+                                messages]
             else:
                 raise Exception("messages type error")
             for message in tip_messages:
                 expect(self.page.get_by_text(message)).to_be_visible(timeout=timeout * 1000)
                 expect(self.page.get_by_text(message)).to_be_hidden(timeout=timeout * 1000)
                 logging.info(f'{self.host} assert tip {message} visible success')
 
@@ -718,15 +730,15 @@
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             if isinstance(messages, str):
                 messages = [self.locale.get(messages)] if self.locale.get(messages) else [messages]
             elif isinstance(messages, re.Pattern):
-                messages = [messages]    # 正则表达式 时需要自己做国际化转换
+                messages = [messages]  # 正则表达式 时需要自己做国际化转换
             elif isinstance(messages, list):
                 messages = [self.locale.get(message) if self.locale.get(message) else message for message in messages]
             else:
                 raise Exception("messages type error")
             text_messages = Counter(messages)  # 处理多个相同的文本
             for message, count in text_messages.items():
                 for i_ in range(0, count):
@@ -916,14 +928,15 @@
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
                     $type: 操作项的类型 text|select|select_multi|select_more|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|fill_date|
                                      multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|monaco|value_mapping
                             select value值可以是label|Value
                             multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
+                    "always_do": True|False: 操作项是否必须操作, 哪怕是报异常也会做
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
             if param_locator.get('type') == 'text':
@@ -1051,38 +1064,48 @@
                     elif wait_for_.get('type') == 'tip_messages':
                         timeout = wait_for_.get('timeout') if wait_for_.get('timeout') else 30
                         self.tip_messages(wait_for_.get('messages'), timeout)
             if param_locator.get('mouse_move'):
                 self.page.mouse.move(param_locator.get('mouse_move')[0], param_locator.get('mouse_move')[1])
 
         if action_dict:
-            for option in locators:
-                assert type(option) in (tuple, list) and len(option) == 2, "type of option is incorrect"
-                if option[0] in [key for key, value in action_dict.items() if value is not None]:
-                    if isinstance(option[1], dict):
-                        if option[1].get("relation") and option[1].get("relation") not in relations:
-                            # 对关系项操作之前检查关系项
-                            for relation_ in option[1].get("relation"):
-                                relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
-                                operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
-                            relations.append(option[1].get("relation"))
-                        operation(option[0], option[1], action_dict.get(option[0]))  # 本身操作
-                    elif isinstance(option[1], list) and isinstance(action_dict.get(option[0]),
-                                                                    list):  # 当使用一个变量传多个元素的值时
-                        for option_, action_value in zip(option[1], action_dict.get(option[0])):
-                            if option_.get("relation") and option_.get("relation") not in relations:
+            always_do_value = None
+            always_do_all = [(option[0], option[1]) for option in locators if option[1].get("always_do")]
+            if len(always_do_all) >= 1 and action_dict.get(always_do_all[0][0]) is not None:  # always_do 始终要做的操作
+                always_do_value = action_dict.pop(always_do_all[0][0])
+            try:
+                for option in locators:
+                    assert type(option) in (tuple, list) and len(option) == 2, "type of option is incorrect"
+                    if option[0] in [key for key, value in action_dict.items() if value is not None]:
+                        if isinstance(option[1], dict):
+                            if option[1].get("relation") and option[1].get("relation") not in relations:
                                 # 对关系项操作之前检查关系项
-                                for relation_ in option_.get("relation"):
+                                for relation_ in option[1].get("relation"):
                                     relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
                                     operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
-                                relations.append(option_.get("relation"))
-                            operation(option[0], option_, action_value)  # 本身操作
-                    else:
-                        logging.exception("type of option is incorrect")
-                        raise Exception("type of option is incorrect")
+                                relations.append(option[1].get("relation"))
+                            operation(option[0], option[1], action_dict.get(option[0]))  # 本身操作
+                        elif isinstance(option[1], list) and isinstance(action_dict.get(option[0]),
+                                                                        list):  # 当使用一个变量传多个元素的值时
+                            for option_, action_value in zip(option[1], action_dict.get(option[0])):
+                                if option_.get("relation") and option_.get("relation") not in relations:
+                                    # 对关系项操作之前检查关系项
+                                    for relation_ in option_.get("relation"):
+                                        relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
+                                        operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
+                                    relations.append(option_.get("relation"))
+                                operation(option[0], option_, action_value)  # 本身操作
+                        else:
+                            logging.exception("type of option is incorrect")
+                            raise Exception("type of option is incorrect")
+            except Exception as e:
+                raise e
+            finally:
+                if always_do_value is not None:
+                    operation(always_do_all[0][0], always_do_all[0][1], always_do_value)
 
     @allure.step("计算元素表达式")
     def eval_locator_attribute(self, expect_: dict, locators: list) -> bool:
         """对页面特定元素值做判断
 
         :param expect_: {$status: $expressions}
                         status: 状态名称， 比如可以传定义好的 current_sim
```

### Comparing `inhandtest-0.0.63/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.64/inhandtest/base_page/table_tr.py`

 * *Files 4% similar despite different names*

```diff
@@ -312,47 +312,30 @@
 
         :param agg_in: function, 导致该方法不能单独使用
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
             kwargs['save'] = True
-        cancel = kwargs.pop('cancel') if kwargs.get('cancel') is not None else False
         try:
             add_button = list(filter(lambda x: x[0] == 'add', self.columns))[0][1].get('locator')
         except Exception:
             add_button = self.table_locator.locator('//button').first
         if kwargs.get('is_exists'):
             is_exists = kwargs.pop('is_exists')
             if not self.exist(is_exists, self.locale):
                 add_button.click()
-                if not cancel:
-                    agg_in(self.columns, kwargs)
-                    logging.debug(f'table resource {kwargs} add success')
-                else:
-                    try:
-                        agg_in(self.columns, kwargs)
-                    except Exception:
-                        raise
-                    finally:
-                        agg_in(self.columns, {'cancel': True})
+                agg_in(self.columns, kwargs)
+                logging.debug(f'table resource {kwargs} add success')
             else:
                 logging.debug(f'table resource {kwargs} exist')
         else:
             add_button.click()
-            if not cancel:
-                agg_in(self.columns, kwargs)
-                logging.debug(f'table resource {kwargs} add success')
-            else:
-                try:
-                    agg_in(self.columns, kwargs)
-                except Exception:
-                    raise
-                finally:
-                    agg_in(self.columns, {'cancel': True})
+            agg_in(self.columns, kwargs)
+            logging.debug(f'table resource {kwargs} add success')
 
     def edit(self, agg_in, old_value, **kwargs) -> None:
         """ 只能编辑匹配到的第一条记录
 
         :param agg_in: function, 导致该方法不能单独使用
         :param old_value: str, 旧值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :param kwargs str, 待添加列 及对应值
@@ -363,25 +346,16 @@
         if exist_tr.count() > 0:
             if exist_tr.first.locator('//i[@class="anticon anticon-form"]').count() == 1:
                 exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
             else:
                 exist_tr.first.locator('//i[@class="anticon anticon-edit"]').click()
             if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                 kwargs['save'] = True
-            cancel = kwargs.pop('cancel') if kwargs.get('cancel') is not None else False
-            if not cancel:
-                agg_in(self.columns, kwargs)
-                logging.debug(f'table resource {kwargs} edit success')
-            else:
-                try:
-                    agg_in(self.columns, kwargs)
-                except Exception:
-                    raise
-                finally:
-                    agg_in(self.columns, {'cancel': True})
+            agg_in(self.columns, kwargs)
+            logging.debug(f'table resource {kwargs} edit success')
         else:
             logging.debug(f'table resource {old_value} not exist')
 
     def delete(self, value: str) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
```

### Comparing `inhandtest-0.0.63/inhandtest/exception.py` & `inhandtest-0.0.64/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/file.py` & `inhandtest-0.0.64/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inmodbus.py` & `inhandtest-0.0.64/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inmongodb.py` & `inhandtest-0.0.64/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inmqtt.py` & `inhandtest-0.0.64/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/__init__.py` & `inhandtest-0.0.64/inhandtest/inrequest/__init__.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/console.py` & `inhandtest-0.0.64/inhandtest/inrequest/console.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/dm.py` & `inhandtest-0.0.64/inhandtest/inrequest/dm.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/dn.py` & `inhandtest-0.0.64/inhandtest/inrequest/dn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/er_default_config.py` & `inhandtest-0.0.64/inhandtest/inrequest/er_default_config.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/er_device.py` & `inhandtest-0.0.64/inhandtest/inrequest/er_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.port = port
         self.model = model
         self.api = ErRequest(host=self.host, username=self.username, password=self.password, type_='device',
                              protocol=self.protocol, port=self.port, device_model=self.model)
         self.default_config = {'ER805': er805_default_config}.get(self.model)
 
     @property
-    def path(self) -> dict:
+    def path_url(self) -> dict:
         """
         :return: 返回设备的url
         """
         return {'ER805': {'import_firmware': '/api/v1/import/firmware',
                           'import_config': '/api/v1/config/import',
                           'upgrade_config': '/api/v1/config/update',
                           'upgrade_firmware': '/api/v1/upgrade',
@@ -80,30 +80,31 @@
                           'login': '/api/v1/user/login',
                           'basic': '/api/v1/basic',
                           'diagnose': '/api/v1/diagnose',
                           'download': '/api/v1/syslog/download',
                           'events_url': '/api/v1/events/get',
                           'adjust_url': '/api/v1/data_usage/adjust'}}.get(self.model)
 
-    def _get_config(self, fields: str):
+    def get_config(self, fields: str, expect: dict = None) -> dict:
         """
 
+        :param expect: 对期望的内容做判断，以字典形式传入，注意匹配大小写并保证key和value的值需完全匹配
         :param fields: cellular| wlan_ap| lan| switch_port| data_usage| wan| clients| system| ntp| data_usage| l2tp| ipsec|
                          可根据配置层级使用.来获取，例'cellular.modem'，
                          也可使用逗号分隔获取多个状态，例'wlan_ap,lan,wlan_sta'
         """
-        return self.api.send_request(self.path.get('config_url'), method='get',
-                                     param={'fields': fields}).json().get('result').get('config')
+        return self.api.send_request(self.path_url.get('config_url'), method='get',
+                                     param={'fields': fields}, expect=expect).json().get('result').get('config')
 
     def get_status(self, path: str):
         """获取设备状态
 
-        :param fields: cellular| wlan_ap| lan| wan| system| signal_history_info| data_usage| ipsec| l2tp|
+        :param path: cellular| wlan_ap| lan| wan| system| signal_history_info| data_usage| ipsec| l2tp|
         """
-        return self.api.send_request(f"{self.path.get('status_url')}{path}", method='get').json().get('result')
+        return self.api.send_request(f"{self.path_url.get('status_url')}{path}", method='get').json().get('result')
 
     def get_uuid_config(self, fields: str, condition: dict) -> List or None:
         """根据条件返回当前配置的uuid
 
 
         :param fields: cellular| wlan_ap| lan| static_route4| uplink| wan| admin| system| ntp| data_usage| record| alerts|
                          ipsec| email| ippt| l2tp| link_quality| uplink| dhcp| admin_access| firewall| policy_route| qos|
@@ -117,15 +118,15 @@
                          {"0000f0804da7846f": {
                          "interface": "wan1",
                          "egress_rate": "0Mbps",
                          "ingress_rate": "0Mbps"}
                          fields传参为'qos.uplink_rules'，condition传参为{'interface': 'wan1'}
         :return: 如存在uuid则返回uuid及匹配的config，否则返回None
         """
-        config = self._get_config(fields)
+        config = self.get_config(fields)
         con = (fields, condition)
         try:
             for k in con[0].split('.'):
                 config = config.get(k)
             for uuid_, v in config.items():
                 for ex_k, ex_v in con[1].items():
                     if v.get(ex_k) != ex_v:
@@ -154,15 +155,15 @@
                         auth: 'WPA2-PSK'|'OPEN'|'WPA-PSK'|'WPA-PSK/WPA2-PSK' 安全方式,只支持大写
                         encrypt: 'CCMP'|'CCMP/TKIP' 加密方式,只支持大写
                         vlan: int, 默认为1
                         channel: 信道，只能在主wifi中编辑 'Auto'或数字
                         ap_isolate: True| False 启用或者禁用
         :return:
         """
-        wlan_ap = self._get_config('wlan_ap').get('wlan_ap')
+        wlan_ap = self.get_config('wlan_ap').get('wlan_ap')
         band = band.upper()
         is_primary = False
         body = {}
         if kwargs.get('new_ssid'):
             kwargs.update({'ssid': kwargs.pop('new_ssid')})
         if action in ('edit', 'delete'):
             try:
@@ -192,15 +193,15 @@
                     name = [un_name for un_name in ('wlan2.1', 'wlan2.2', 'wlan2.3') if un_name not in list_5][0]
             except IndexError:
                 raise ParameterValueError(f'the {band} wifi is full')
             config_ap = self.default_config.get('wlan_ap').get(band)
             config_ap.update(kwargs)
             config_ap.update({'ssid': ssid, 'band': band, 'name': name})
             body = {'wlan_ap': {'$id': config_ap}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body,
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body,
                               expect={'result': 'ok'})
         logging.info(f'{action} wifi {band} {ssid}  ap success')
 
     def config_wan(self, interface='wan1', status='enable', **kwargs):
         """
         :param interface: 'wan1'|'wan2'
         :param status: 'enable'|'disable'|'delete'
@@ -237,15 +238,15 @@
             else:
                 if status == 'disable':
                     body = {'wan': {config_wan[0]: {'enabled': False}}}
                 else:
                     body = {'wan': {config_wan[0]: None}}
         else:
             raise ParameterValueError(f'status:{status} is not support')
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'{status} wan {interface} success')
 
     def config_wifi_sta(self, status='enable', **kwargs):
         """编辑wifi_sta
 
         :param status: 'enable'|'disable'|'delete'
         :param kwargs: dict
@@ -260,15 +261,15 @@
                         dhcpc: True | False
                         ip: str
                         prefix_len: int, 0-32, 掩码长度
                         gateway: str
                         dns1: str
                         dns2: str
         """
-        config_wlan = ['wlan_sta', self._get_config('wlan_sta').get('wlan_sta')] if self._get_config('wlan_sta').get(
+        config_wlan = ['wlan_sta', self.get_config('wlan_sta').get('wlan_sta')] if self.get_config('wlan_sta').get(
             'wlan_sta') else ['$id', self.default_config.get('wlan_sta')]
         if status == 'enable':
             kwargs.update({'enabled': True})
             config_wlan[1].update(kwargs)
             body = {config_wlan[0].replace('$id', 'wlan_sta'): config_wlan[1]}
         elif status in ('disable', 'delete'):
             if config_wlan[0] == '$id':
@@ -276,15 +277,15 @@
             else:
                 if status == 'disable':
                     body = {config_wlan[0].replace('$id', 'wlan_sta'): {'enabled': False}}
                 else:
                     body = {config_wlan[0].replace('$id', 'wlan_sta'): None}
         else:
             raise ParameterValueError(f'status:{status} is not support')
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'{status} wlan_ap success')
 
     def mac_filter(self, mac: str = None, action: str = None, **kwargs):
         """编辑mac地址过滤
 
         :param mac: str, 新增和删除时必填, 只变更过滤模式可为None
         :param action: 'edit'|'add'|'delete', 只变更过滤模式可为None
@@ -312,15 +313,15 @@
                 body = {'mac_filter': {'mac_list': {'$id': config_mac_filter}}}
         if 'mode' in kwargs.keys():
             if body:
                 body.get('mac_filter').update({'mode': kwargs.get('mode')})
                 action = 'change_mode'
             else:
                 body = {'mac_filter': {'mode': kwargs.get('mode')}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body,
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body,
                               expect={'result': 'ok'})
         logging.info(f'{action} mac_filter success')
 
     def config_cellular(self, **kwargs):
         """
         :param kwargs: dict
                     cellular: dict, cellular配置
@@ -385,15 +386,15 @@
                             adjust_usage_unit: 'GB'|'MB'|'KB'
                             adjust_usage: str
 
         """
 
         if 'adjust_usage' in kwargs.keys():
             config_adjust_usage = kwargs.get('adjust_usage')
-            self.api.send_request(self.path.get('adjust_url'), method='post', body=config_adjust_usage,
+            self.api.send_request(self.path_url.get('adjust_url'), method='post', body=config_adjust_usage,
                                   expect={'result': 'ok'})
             logging.info(f'config adjust usage success')
         if kwargs.get('cellular'):
             config_cellular = kwargs.get('cellular')
         else:
             config_cellular = {}
         if 'cellular:modem:dual_sim:enabled' in dict_flatten(kwargs).keys():
@@ -406,15 +407,15 @@
                     'sim1': {'monthly_data_plan': {'over_threshold_oper': 'alert'}},
                     'sim2': {'monthly_data_plan': {'over_threshold_oper': 'alert'}}}
         else:
             config_data_usage = {}
         if kwargs.get('data_usage'):
             config_data_usage.update(kwargs.get('data_usage'))
         body = {'cellular': config_cellular, 'data_usage': config_data_usage}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'config cellular success')
 
     def config_uplink(self, **kwargs):
         """
 
         :param kwargs: dict
                     mode: 'failover'|'load-balance', 链路备份|负载均衡
@@ -442,15 +443,15 @@
                     interface.update({config_interface_[0]: {'name': k, 'priority': v.get('priority')}})
                 except ResourceNotFoundError:
                     logging.info(f'interface {k} not found')
             uplink.update({'interface': interface})
             kwargs.pop('interface')
         uplink.update(kwargs)
         body = {'uplink': uplink}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'config uplink success')
 
     def config_lan(self, alias: str, action: str, **kwargs):
         """配置lan
 
         :param alias: str, lan名称
         :param action: str, 'edit'|'add'|'delete'
@@ -513,15 +514,15 @@
             lan_config = self.default_config.get('lan')
             lan_config.update({'alias': alias})
             lan_config.update(kwargs.get('lan'))
             dhcp_config = self.default_config.get('dhcp').get('server')
             dhcp_config.update({'alias': alias})
             dhcp_config.update(kwargs.get('dhcp').get('server'))
             body = {'lan': {'$id': lan_config}, 'dhcp': {'server': {'$id': dhcp_config}}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'{action} lan {alias} success')
 
     def config_route(self, destination: str, next_hop: dict, action: str, **kwargs):
         """配置静态路由
 
         :param destination: str, 目的地址, 格式'0.0.0.0/0'
         :param next_hop: dict
@@ -558,15 +559,15 @@
             except ResourceNotFoundError:
                 raise ResourceNotFoundError(f'route {destination} not found')
         else:
             route_config = self.default_config.get('static_route4')
             route_config.update({'destination': destination, 'next_hop': next_hop})
             route_config.update(kwargs)
             body = {'static_route4': {'$id': route_config}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'{action} route {destination} success')
 
     def config_ipsec(self, name: str, action: str, **kwargs):
         """配置ipsec
 
         :param name: str, ipsec名称
         :param action: str, 'edit'|'add'|'delete'
@@ -608,15 +609,15 @@
             except ResourceNotFoundError:
                 raise ResourceNotFoundError(f'ipsec {name} not found')
         else:
             ipsec_config = self.default_config.get('ipsec')
             ipsec_config.update({'name': name})
             ipsec_config.update(kwargs)
             body = {'ipsec': {'$id': ipsec_config}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'{action} ipsec {name} success')
 
     def config_l2tp(self, character: str, **kwargs):
         """配置l2tp
 
         :param character: str, 'server'|'client'
         :param kwargs: dict
@@ -646,14 +647,15 @@
                         password: str, 密码
                         ppp_auth: str, 'auto'|'pap'|'chap'
                         tunnel_auth: dict
                             enabled: bool, True|False
                             server: str, 认证服务器地址
                             password: str, 密码
         """
+        body = None
         if character == 'server':
             l2tp_server = self.default_config.get('l2tp').get('server')
             l2tp_server.update(kwargs)
             body = {'l2tp': {'server': l2tp_server}}
         else:
             if kwargs.get('alias') and kwargs.get('action'):
                 if kwargs.get('clients') and 'new_alias' in kwargs.get('clients'):
@@ -667,32 +669,32 @@
                         elif kwargs.get('action') == 'delete':
                             body = {'l2tp': {'clients': {l2tp_client[0]: None}}}
                         else:
                             pass
                     except ResourceNotFoundError:
                         raise ResourceNotFoundError(f'l2tp client {kwargs.get("alias")} not found')
                 else:
-                    l2tp_now = self._get_config('l2tp.clients').get('l2tp').get('clients')
+                    l2tp_now = self.get_config('l2tp.clients').get('l2tp').get('clients')
                     l2tp_list = [v.get('name') for k, v in l2tp_now.items() if 'l2tp' in v.get('name')]
                     un_name = \
                         [un_name_ for un_name_ in [f'l2tp{i}' for i in range(1, 10)] if un_name_ not in l2tp_list][0]
                     l2tp_client = self.default_config.get('l2tp').get('clients')
                     l2tp_client.update(kwargs.get('clients'))
                     l2tp_client.update({'alias': kwargs.get('alias'), 'name': un_name})
                     body = {'l2tp': {'clients': {'$id': l2tp_client}}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'config l2tp {character} success')
 
     def config_inbound_default(self, action: str):
         """配置防火墙入站默认规则
 
         :param action: str, 'permit'|'deny'
         """
         body = {'firewall': {'inbound_default': {'action': action}}}
-        self.api.send_request(self.path.get('config_url'), method='put', body=body, expect={'result': 'ok'})
+        self.api.send_request(self.path_url.get('config_url'), method='put', body=body, expect={'result': 'ok'})
         logging.info(f'config inbound default {action} success')
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
```

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/ics.py` & `inhandtest-0.0.64/inhandtest/inrequest/ics.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/inrequest.py` & `inhandtest-0.0.64/inhandtest/inrequest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inrequest/nezha.py` & `inhandtest-0.0.64/inhandtest/inrequest/nezha.py`

 * *Files 15% similar despite different names*

```diff
@@ -708,15 +708,15 @@
         if commit:
             resp = self.api.send_request('/api/v1/config/commit', 'post', header=header).json()
             assert resp == {'result': 'ok'}, 'commit config failed'
             logging.info(f'the device {sn} config commit success')
         return payload
 
     @allure.step("获取配置")
-    def get(self, sn: str, expect: dict, type_='actual') -> dict or None:
+    def get(self, sn: str, expect: dict = None, type_='actual') -> dict or None:
         """获取校验备配置
 
         :param sn: 设备序列号
         :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
         :param type_: actual 实际设备上传的配置
                       group 设备所在组的配置
                       pending 正在下发的配置
@@ -732,14 +732,54 @@
         if expect is not None:
             self.api.send_request(f'/api/v1/devices/{self.__device.info(sn).get("_id")}/config', 'get',
                                   expect=expect)
         else:
             return self.api.send_request(f'/api/v1/devices/{self.__device.info(sn).get("_id")}/config',
                                          'get').json().get('result').get(type_)
 
+    def get_uuid_config(self, sn: str, fields: str, condition: dict) -> list or None:
+        """根据条件返回当前配置的uuid
+
+        :param sn: 设备序列号
+        :param fields: cellular| wlan_ap| lan| static_route4| uplink| wan| admin| system| ntp| data_usage| record| alerts|
+                         ipsec| email| ippt| l2tp| link_quality| uplink| dhcp| admin_access| firewall| policy_route| qos|
+                         port_mapping| wlan_sta| switch_port
+                         可根据配置层级使用.来获取，例'cellular.modem'，不可获取多个配置项
+                         传参时需写到uuid前一级
+        :param condition: 查找uuid的条件，以字典形式传入，注意匹配大小写并保证key和value的值需完全匹配
+                            例当需要查找ssid=test且band=2.4G的wifi时可传入{'ssid': 'test', 'band': '2.4G'}
+                例当需要匹配qos中interface=wan1的uuid时
+                         "qos": {"uplink_rules":
+                         {"0000f0804da7846f": {
+                         "interface": "wan1",
+                         "egress_rate": "0Mbps",
+                         "ingress_rate": "0Mbps"}
+                         fields传参为'qos.uplink_rules'，condition传参为{'interface': 'wan1'}
+        :return: 如存在uuid则返回uuid及匹配的config，否则返回None
+        """
+        config = self.get(sn, None).get(fields)
+        con = (fields, condition)
+        try:
+            for k in con[0].split('.'):
+                config = config.get(k)
+            for uuid_, v in config.items():
+                for ex_k, ex_v in con[1].items():
+                    if v.get(ex_k) != ex_v:
+                        break
+                else:
+                    id_ = uuid_
+                    config_ = v
+                    break
+            else:
+                raise ResourceNotFoundError('not find uuid, please check the condition')
+        except Exception:
+            raise ResourceNotFoundError('not find key, please check the fields')
+        logging.info(f'find the matched uuid: {id_}')
+        return [id_, config_]
+
     @allure.step("清除配置")
     def clear_config(self, sn: str):
         """清除设备配置
 
         :param sn:
         :return:
         """
@@ -1077,14 +1117,115 @@
         _id = self.info(group_name, group_id).get('_id')
         if expect is not None:
             self.api.send_request(f'/api/v1/config/layer/group/{_id}', 'get', expect=expect)
         else:
             return self.api.send_request(f'/api/v1/config/layer/group/{_id}', 'get').json().get('result').get(type_)
 
 
+class Alert(Base):
+    def __init__(self, api, email, host):
+        super().__init__(api, email, host)
+        self.__group = Group(api, email, host)
+        self.__device = Device(api, email, host)
+        self.__org = Org(api, email, host)
+
+    @allure.step("创建告警规则")
+    def create_rule(self, rules: dict or list, users: list, groups: list, channels=None, expect=None) -> str:
+        """
+
+        :param rules: {"type": "reboot"}, or [{"type": "connected", "param": {retention: 600}}]
+        :param users:  用户邮箱列表
+        :param channels: 通知渠道列表 ["email"]  sms app
+        :param groups: 分组名列表, 需保障分组名唯一
+        :param expect: 预期结果
+        :return:  rule_id
+        """
+        rules = [rules] if isinstance(rules, dict) else rules
+        user_ids = [self.__org.user_info(email=user).get('_id') for user in users]
+        channels = ['email'] if channels is None else channels
+        groups_id = [self.__group.info(name=group).get('_id') for group in groups]
+        body = {"rules": rules, "notify": {"users": user_ids, "channels": channels},
+                "groupIds": groups_id}
+        return self.api.send_request('/api/v1/alerts/rules', 'post', body=body, expect=expect).json().get('result').get(
+            '_id')
+
+    @allure.step("编辑告警规则")
+    def edit_rule(self, _id: str, rules: dict or list, users: list, groups: list, channels=None, expect=None):
+        """
+
+        :param _id: rule_id
+        :param rules: {"type": "reboot"}, or [{"type": "connected", "param": {retention: 600}}]
+        :param users:  用户邮箱列表
+        :param channels: 通知渠道列表 ["email"]  sms app
+        :param groups: 分组名列表, 需保障分组名唯一
+        :param expect: 预期结果
+        :return:  rule_id
+        """
+        rules = [rules] if isinstance(rules, dict) else rules
+        user_ids = [self.__org.user_info(email=user).get('_id') for user in users]
+        channels = ['email'] if channels is None else channels
+        groups_id = [self.__group.info(name=group).get('_id') for group in groups]
+        body = {"rules": rules, "notify": {"users": user_ids, "channels": channels},
+                "groupIds": groups_id}
+        self.api.send_request(f'/api/v1/alerts/rules/{_id}', 'put', body=body, expect=expect)
+
+    @allure.step("删除告警规则")
+    def delete_rule(self, ids: list, expect=None):
+        self.api.send_request(f'/api/v1/alerts/rules/bulk-delete', 'post', body={"ids": ids}, expect=expect)
+
+    @allure.step("查询告警规则")
+    def find_rule(self, expect=None) -> list:
+        """
+        :param expect: 预期结果
+        :return:  返回符合查询条件的所有告警规则id
+        """
+        result = self.api.send_request('/api/v1/alerts/rules', 'get', param={"limit": 100, "page": 0},
+                                       expect=expect).json().get('result')
+        if result:
+            return [alert.get('_id') for alert in result]
+        else:
+            return []
+
+    @allure.step("查询告警")
+    def find_alert(self, params=None, expect=None) -> list:
+        """
+        :param expect: 预期结果
+        :param params: 查询参数 ack=false
+                                from=2023-08-02T16:00:00.000Z
+                                to=2023-08-03T16:00:00.000Z
+                                type=connected
+                                deviceId=64c85ab3b51c32731f029155
+                                deviceGroupId=64ba5b5e4718687c71936feb
+                                expand=deviceGroup,org  默认
+                                app=nezha 默认
+                                limit=100 默认
+                                page=0 默认
+        :return:  返回符合查询条件的所有告警id
+        """
+        params = dict_merge({"expand": "deviceGroup,org", "app": "nezha", "limit": 100, "page": 0}, params)
+        result = self.api.send_request('/api/v1/alerts', 'get', param=params, expect=expect).json().get('result')
+        if result:
+            return [alert.get('_id') for alert in result]
+        else:
+            return []
+
+    @allure.step("确认告警")
+    def ack_alert(self, ids: list, expect=None):
+        """
+
+        :param ids: 当list为空时，确认所有告警， 如果不为空时，确认指定告警
+        :param expect:
+        :return:
+        """
+        if ids:
+            self.api.send_request('/api/v1/alerts/acknowledge', 'put', body={"ids": ids, "app": "nezha"}, expect=expect)
+        else:
+            self.api.send_request('/api/v1/alerts/acknowledge/all', 'put', body={"app": "nezha"}, expect=expect)
+
+
 class Firmware(Base):
 
     def info(self, product: str, version=None) -> dict or list:
         """查询账号下对应产品 已发布版本
 
         :param product: ER805
         :param version: None 当版本为None返回所有的已发布版本
@@ -1167,14 +1308,137 @@
             if executions.get('total') == 0:
                 break
             else:
                 for execution in executions.get('result'):
                     self.api.send_request(f'api/v1/job/executions/{execution.get("_id")}/cancel', 'put')
 
 
+class Report(Base):
+
+    @allure.step("创建报表")
+    def create_policies(self, period: str, name: str, _format: str, schedule: dict, apply_to='all', templates='all',
+                        recipient=None, description=None, expect=None):
+        """
+        :param templates: 模板列表    'all', TOTAL_DEVICES, DEVICE_DISTRIBUTION, FIRMWARE_STATUS,
+                                    CONFIGURATION_STATUS, NETWORKING_METHOD, OFFLINE_TIMES_TOP_10,
+                                    USAGE_SUMMARY, TOTAL_USAGE_TOP_10, USAGE_TOP_10_BY_CELLULAR,
+                                    USAGE_TOP_10_BY_WIRED, USAGE_TOP_10_BY_WIRELESS, ALERTS_TOP_10_BY_DEVICE,
+                                    ALERT_TOP_10_BY_TYPE
+        :param apply_to: 适用对象，支持填入长度为1的字典   {"org": [ids]}, {"group": [ids]}
+        :param period: 周期   LAST_1_DAY，LAST_3_DAYS，LAST_7_DAYS，LAST_30_DAYS
+        :param name: 报表名称
+        :param _format: 报表格式    PDF，XLSX
+        :param schedule: 定时任务   定时任务字段：dayOfWeek, dayOfMonth, hourOfDay, minuteOfHour
+        :param recipient: 收件人
+        :param description: 描述
+        :param expect: 预期结果
+        :return:  report_id
+        """
+        tmp = {}
+        if isinstance(apply_to, dict):
+            for k, v in apply_to.items():
+                tmp["type"] = k
+                tmp["ids"] = v
+        else:
+            tmp["type"] = apply_to
+        if isinstance(templates, list):
+            templates = templates
+        elif isinstance(templates, str):
+            if templates == 'all':
+                templates = ['TOTAL_DEVICES', 'DEVICE_DISTRIBUTION', 'FIRMWARE_STATUS', 'CONFIGURATION_STATUS',
+                             'NETWORKING_METHOD', 'OFFLINE_TIMES_TOP_10', 'USAGE_SUMMARY', 'TOTAL_USAGE_TOP_10',
+                             'USAGE_TOP_10_BY_CELLULAR', 'USAGE_TOP_10_BY_WIRED', 'USAGE_TOP_10_BY_WIRELESS',
+                             'ALERTS_TOP_10_BY_DEVICE', 'ALERT_TOP_10_BY_TYPE']
+        body = {"templates": templates, "applyTo": tmp, "period": period, "name": name, "format": _format,
+                "scheduled": False, "recipient": recipient, "description": description}
+        if schedule:
+            body['scheduled'] = True
+            body['schedule'] = schedule
+        return self.api.send_request('/api/v1/incloud/report/policies', 'post', body=body, expect=expect).json().get(
+            'result')
+
+    @allure.step("获取历史报表")
+    def history_list(self, name=None, date_from=None, date_to=None, expect=None):
+        """
+        :param name: 报表名称
+        :param date_from: 开始时间
+        :param date_to: 结束时间
+        :param expect: 预期结果
+        :return:
+        """
+        param = {
+            "name": name,
+            "dateFrom": date_from,
+            "dateTo": date_to,
+            "limit": 100,
+            "page": 0
+        }
+        return self.api.send_request(f'/api/v1/incloud/reports', 'get', param=param, expect=expect).json().get('result')
+
+    @allure.step("编辑报表规则")
+    def edit_policies(self, report_id: str, period: str, name: str, _format: str, schedule: dict, apply_to='all',
+                      templates='all', recipient=None, description=None, expect=None):
+        tmp = {}
+        if isinstance(apply_to, dict):
+            for k, v in apply_to.items():
+                tmp["type"] = k
+                tmp["ids"] = v
+        else:
+            tmp["type"] = apply_to
+        if isinstance(templates, list):
+            templates = templates
+        elif isinstance(templates, str):
+            if templates == 'all':
+                templates = ['TOTAL_DEVICES', 'DEVICE_DISTRIBUTION', 'FIRMWARE_STATUS', 'CONFIGURATION_STATUS',
+                             'NETWORKING_METHOD', 'OFFLINE_TIMES_TOP_10', 'USAGE_SUMMARY', 'TOTAL_USAGE_TOP_10',
+                             'USAGE_TOP_10_BY_CELLULAR', 'USAGE_TOP_10_BY_WIRED', 'USAGE_TOP_10_BY_WIRELESS',
+                             'ALERTS_TOP_10_BY_DEVICE', 'ALERT_TOP_10_BY_TYPE']
+        body = {"templates": templates, "applyTo": tmp, "period": period, "name": name, "format": _format,
+                "scheduled": False, "recipient": recipient, "description": description}
+        if schedule:
+            body['scheduled'] = True
+            body['schedule'] = schedule
+        return self.api.send_request(f'/api/v1/incloud/report/policies/{report_id}', 'put', body=body,
+                                     expect=expect).json().get('result')
+
+    @allure.step("删除报表规则")
+    def delete_policies(self, report_id: str, expect=None):
+        return self.api.send_request(f'/api/v1/incloud/report/policies/{report_id}', 'delete', expect=expect).json()
+
+    @allure.step("获取报表")
+    def get_policies(self, _type="list", name=None, report_id=None, expect=None):
+        param = {
+            "name": name,
+            "limit": 100,
+            "page": 0
+        }
+        if _type == "list":
+            return self.api.send_request(f'/api/v1/incloud/report/policies', 'get', param=param,
+                                         expect=expect).json().get('result')
+        elif _type == "detail" and report_id:
+            return self.api.send_request(f'/api/v1/incloud/report/policies/{report_id}', 'get',
+                                         expect=expect).json().get('result')
+
+    @allure.step("删除报表")
+    def delete(self, report_id: str, expect=None):
+        return self.api.send_request(f'/api/v1/incloud/reports/{report_id}', 'delete', expect=expect).json()
+
+    @allure.step("下载报表")
+    def download(self, report_id: str, expect=None):
+        return self.api.send_request(f'/api/v1/incloud/reports/{report_id}/download', 'get', expect=expect).json()
+
+    @allure.step("重新生成报表")
+    def regenerate(self, report_id: str, expect=None):
+        return self.api.send_request(f'/api/v1/incloud/reports/{report_id}/regenerate', 'post', expect=expect).json()
+
+    @allure.step("获取报表详情")
+    def detail(self, report_id: str, expect=None):
+        return self.api.send_request(f'/api/v1/incloud/reports/{report_id}', 'get', expect=expect).json().get('result')
+
+
 class StarInterface:
 
     def __init__(self, email, password, host='star.inhandcloud.cn'):
         """ 须确保用户关闭了多因素认证
 
         :param email  平台用户名
         :param password  平台密码
@@ -1184,18 +1448,21 @@
         self.overview = Overview(self.api, email, host)
         self.device = Device(self.api, email, host)
         self.firmware = Firmware(self.api, email, host)
         self.config = Config(self.api, email, host)
         self.org = Org(self.api, email, host)
         self.group = Group(self.api, email, host)
         self.log = Log(self.api, email, host)
+        self.alert = Alert(self.api, email, host)
+        self.report = Report(self.api, email, host)
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
-    # star = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.design')
+
+
     # for i in range(2001, 3000):
     #     sn = f'EC94212345{str(i).rjust(5, "0")}'
     #     star.device.add(sn=sn, mac_or_imei='00:18:05:00:00:00', name=sn)
     #     star.group.move([sn], group_name='', group_id='64b8d9a90e1b8d1d245d79bf')
```

### Comparing `inhandtest-0.0.63/inhandtest/inserial.py` & `inhandtest-0.0.64/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/insocket.py` & `inhandtest-0.0.64/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/inssh.py` & `inhandtest-0.0.64/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/ip.py` & `inhandtest-0.0.64/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/log.py` & `inhandtest-0.0.64/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/mail.py` & `inhandtest-0.0.64/inhandtest/mail.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,34 +107,34 @@
         r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
                                         'password': mail_from[1]},
                          render=render)
         assert r.status_code == 250, 'send email failed'
         logging.info(f'send {mail_to} result success!')
 
 
-@loop_inspector('receive last email', 120, 5)
+@loop_inspector('receive last email', 20, 5)
 def receive_last_mail(receiver: tuple, mail_from: tuple, subject: str, **kwargs):
     """收取符合条件的邮件做校验，如果匹配到多个邮件，只校验最近的一封邮件
        当邮箱中邮件较多时，会耗时很长，所以建议匹配未读的邮件进行分析，分析完后，将邮件标记为已读
 
     :param receiver: 接收者('test@inhand.com.cn', '1111124') email, password
     :param mail_from: 发送者('映翰通网络', 'iot_console@inhand.com.cn') name, email
     :param subject: 邮件主题， 如：'VG710自动化测试'
     :param kwargs:
-                  before_date: 匹配发送日期早于指定日期的邮件，格式：'2021-04-12 10:10:43'
-                  after_date: 匹配发送日期晚于或等于指定日期的邮件，格式：'2021-04-12 10:10:43'
+                  before_date: 匹配发送日期早于指定日期的邮件，格式：'2021-03-12 10:10:43' 本地时间
+                  after_date: 匹配发送日期晚于或等于指定日期的邮件，格式：'2021-04-12 10:10:43'  本地时间
                   unseen: True| False 匹配未读邮件
                   seen_flag: True| False 对匹配到的所有邮件设置已读标记
-                  body: str or list 对匹配到的邮件内容做校验，整个邮件的内容是text形式, 判断邮件内容是否包含body中的内容, 且html_body和body只能有一个
-                  html_body: dict, {$xpath: $text()}对匹配到的邮件内容做校验，整个邮件的内容是html形式，example: {'//*[@id="mailContentContainer"]/div[1]': 'VG710自动化测试'}
-                  html_attribute: tuple or list, ($xpath, $attribute)对匹配到的邮件内容做校验，整个邮件的内容是html形式，example: ('//td[@align="center"]/a', 'href')
+                  assert_body: str or list 对匹配到的邮件内容做校验，整个邮件的内容是text形式, 判断邮件内容是否包含body中的内容, 且html_body和body只能有一个
+                  assert_html_attr: dict or list, {'xpath': '', 'attr': 'src', 'value':''}对匹配到的邮件内容做校验，整个邮件的内容是html形式，
+                                       xpath: str,  attr: text|src|href|value|id|class|name   value: str
+                  get_html_attr: tuple ($xpath, $attr)对匹配到的邮件内容做校验，整个邮件的内容是html形式，example: ('//td[@align="center"]/a', 'href')
                                    xpath: str,
-                                   attribute： str只能匹配一个属性
+                                   attr： str只能匹配一个属性  需要获取文本时 就传text  text|src|href|value|id|class|name
                                    return str
-                  html_text: str,  $xpath,  return str
                   timeout: 超时时间，单位秒
                   interval: 每隔多久检查一次，单位秒
     :return:
     """
 
     def decode_str(s):
         """解码邮件标题"""
@@ -162,39 +162,40 @@
     status, data = imap_server.search(None, type_)
     result = False
     # 循环处理每个邮件
     if status == 'OK':
         all_email = data[0].split()
         all_email.reverse()  # 从最新的邮件开始处理
         for num in all_email:
+            logging.info(f'查询第{all_email.index(num) + 1}封邮件')
             # 获取邮件内容
             if kwargs.get('seen_flag'):
                 imap_server.store(num, '+FLAGS', '\\Seen')
             status_, data = imap_server.fetch(num, '(RFC822)')
             raw_email = data[0][1]
             email_message = email.message_from_bytes(raw_email)
 
             # 解析邮件头
             receiver_time = str(decode_header(email_message['Date'])[0][0])
             receiver_time = datetime.datetime.strptime(receiver_time,
                                                        f'%a, %d %b %Y %H:%M:%S {receiver_time.split(" ", 5)[-1]}')
             if kwargs.get('before_date'):
-                if receiver_time < datetime.datetime.strptime(kwargs.get('before_date'), '%Y-%m-%d %H:%M:%S'):
-                    continue
+                if receiver_time <= datetime.datetime.strptime(kwargs.get('before_date'), '%Y-%m-%d %H:%M:%S'):
+                    break  # 邮件是按照时间倒序排列的，如果匹配到的邮件时间早于指定时间，就不用再匹配了
             if kwargs.get('after_date'):
-                if receiver_time > datetime.datetime.strptime(kwargs.get('after_date'), '%Y-%m-%d %H:%M:%S'):
-                    continue
+                if receiver_time >= datetime.datetime.strptime(kwargs.get('after_date'), '%Y-%m-%d %H:%M:%S'):
+                    continue  # 不符合条件的邮件，直接跳过
             subject_ = decode_str(email_message['Subject'])
             sender_from = decode_str(email_message['From'])
             if not ((subject in subject_) and (mail_from[0] in sender_from and mail_from[1] in sender_from)):
                 continue
             else:
                 logging.debug(f'get email success! subject: {subject_}, sender: {sender_from}')
             # 解析邮件正文
-            if not kwargs.get('body') and not kwargs.get('html_body') and not kwargs.get('html_attribute') and not kwargs.get('html_text'):
+            if not kwargs.get('assert_body') and not kwargs.get('assert_html_attr') and not kwargs.get('get_html_attr'):
                 result = True
                 break
             else:
                 body = html_body = None
                 if email_message.is_multipart():
                     for part in email_message.walk():
                         content_type = part.get_content_type()
@@ -207,53 +208,69 @@
                         elif content_type == 'text/html' and 'attachment' not in content_disposition:
                             html_body = part.get_payload(decode=True).decode('utf-8')
                 else:
                     try:
                         body = email_message.get_payload(decode=True).decode('utf-8')
                     except UnicodeDecodeError:
                         body = email_message.get_payload(decode=True).decode('gbk')
-                if kwargs.get('body'):
+                if kwargs.get('assert_body'):
                     if not body:
                         break
                     else:
-                        expect_body = kwargs.get('body') if isinstance(kwargs.get('body'), list) else [
-                            kwargs.get('body')]
+                        expect_body = kwargs.get('assert_body') if isinstance(kwargs.get('assert_body'), list) else [
+                            kwargs.get('assert_body')]
                         for expect_ in expect_body:
                             if expect_ not in body:
                                 logging.warning(f'assert email body failed!')
                                 break
                         else:
                             result = True
                             logging.debug(f'assert email body success!')
                         break  # 无论是否包含期望的邮件内容，都跳出循环
-                if kwargs.get('html_body'):
+                if kwargs.get('assert_html_attr'):
                     if not html_body:
                         break
                     else:
                         html_body = etree.HTML(html_body)
-                        for xpath_, text_ in kwargs.get('html_body').items():
-                            for _ in html_body.xpath(xpath_):
-                                if text_ in _.text:
-                                    break
+                        assert_html = [kwargs.get('assert_html_attr')] if isinstance(kwargs.get('assert_html_attr'), dict) else kwargs.get('assert_html_attr')
+                        for html_ in assert_html:
+                            if html_.get('attr') is None or html_.get('attr') == 'text':
+                                text = html_body.xpath(html_.get('xpath'))[0].text
                             else:
-                                logging.warning(f'assert email html_body failed!')
-                                break
+                                text = html_body.xpath(html_.get('xpath'))[0].get(html_.get('attr'))
+                            try:
+                                if '${value}' in html_.get('value'):
+                                    expression = html_.get('value').replace('${value}', text).replace('\n', ' ')
+                                else:
+                                    ex_ = html_.get('value').replace("'", "\'")
+                                    value = text.replace("'", "\'")
+                                    expression = f'"""{ex_}""" == """{value}"""'  # 默认使用等于判断
+                                if eval(expression):
+                                    logging.info(f'Check {html_.get("xpath")} , {expression} is success')
+                                else:
+                                    logging.info(f'Check {html_.get("xpath")} , {expression} is failed')
+                                    return False
+                            except TypeError:
+                                logging.error(f'get {html_.get("xpath")} value failed')
+                                return False
                         else:
                             result = True
-                            logging.warning(f'assert email html_body success!')
                         break
-                if kwargs.get('html_attribute'):
+                if kwargs.get('get_html_attr'):
                     if not html_body:
                         break
                     else:
                         html_body = etree.HTML(html_body)
-                        if isinstance(kwargs.get('html_attribute'), tuple):
+                        if isinstance(kwargs.get('get_html_attr'), tuple):
                             try:
-                                return html_body.xpath(kwargs.get('html_attribute')[0])[0].get(
-                                    kwargs.get('html_attribute')[1])
+                                if kwargs.get('get_html_attr')[1] == 'text':
+                                    return html_body.xpath(kwargs.get('get_html_attr')[0])[0].text
+                                else:
+                                    return html_body.xpath(kwargs.get('get_html_attr')[0])[0].get(
+                                        kwargs.get('get_html_attr')[1])
                             except IndexError:
                                 logging.warning(f'not found html_attribute failed!')
                                 pass
         else:
             logging.debug(f'not found {subject} email')
     else:
         logging.error(f'get email failed: {status}')
@@ -288,13 +305,16 @@
     # 关闭连接
     logging.info('delete all emails')
     imap_server.close()
     imap_server.logout()
 
 
 if __name__ == '__main__':
+    from inhandtest.log import enable_log
+    enable_log(console_level='debug')
     # 设置日志
-    delete_all_mail(('test@inhand.com.cn', 'ABc124'))
-    a = receive_last_mail(receiver=('test@inhand.com.cn', 'ABc124'),
-                          mail_from=('映翰通网络', 'iot_console@inhand.com.cn'), subject='邀请加入新组织',
-                          html_attribute=('//td[@align="center"]/a', 'href'))
-    print(a)
+    a = receive_last_mail(receiver=('test@inhand.com.cn', '2222222'),
+                          before_date='2023-08-03 16:05:00',
+                          after_date='2023-08-03 16:08:00',
+                          mail_from=('映翰通网络', 'iot_console@inhand.com.cn'), subject='MR8051234500001 与平台断开连接',
+                          assert_html_attr=[{'xpath': '//td[@align="center"]/a', 'value': 'https://star.dev.inhandjx.design/devices', 'attr': 'href'}])
+
```

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             ('submit_portainer_manager',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(1),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]').nth(1),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class PythonEdgeComputingLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -121,21 +121,21 @@
                      '.ant-btn.ant-btn-primary.ant-btn-sm').first,
                  "columns": [
                      ('app_package',
                       {'locator': self.pop_up.locator('.anticon.anticon-upload'), 'type': 'upload_file'}),
                      ('log_file_size', {'locator': self.pop_up.locator('#log_size'), 'type': 'text'}),
                      ('number_of_log', {'locator': self.pop_up.locator('#log_file_num'), 'type': 'text'}),
                      ('start_args', {'locator': self.pop_up.locator('#start_args'), 'type': 'text'}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                 'type': 'button'}),
                      ('save', {'locator': self.pop_up.locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                          'wait_for': {'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000}}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
+                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button',
+                                 "always_do": True}),
                  ]},
                  'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
             ('app_status',
              {'locator': {
                  'locator': self.app_status_table,
                  'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
                      '.ant-btn.ant-btn-primary.ant-btn-sm').first,
@@ -143,17 +143,17 @@
                  'type': 'table_tr', 'relation': [('python_engine', 'enable')]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
-            ('cancel', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                        'type': 'button'}),
+                       'type': 'button', "always_do": True}),
+            ('cancel', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'), 'type': 'button',
+                        "always_do": True}),
         ]
 
 
 class DeviceSupervisorLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -269,28 +269,28 @@
                 ('store_communication_message',
                  {'locator': self.pop_up.locator('#enableDebug'), 'type': 'switch_button',
                   'relation': [('advanced_settings', 'expand')]}),
                 ('submit', {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                             'type': 'button'}),
                 ('text_messages', {'type': 'text_messages'}),
                 ('tip_messages', {'type': 'tip_messages'}),
-                ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                            'type': 'button'}),
+                ('cancel',
+                 {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]
 
     @property
     def set_as_template(self) -> list:
         return [
             ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
             ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
             ('submit', {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                         'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
-            ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
+            ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
         ]
 
     def controller_card(self, name) -> list:
         controller_name = f'//div[@class="ant-list-item"]//div[text()="{name}"]'
         controllers = [('select', {'locator': self.page.locator(controller_name), 'type': 'button'}),
                        ('check', {'locator': self.page.locator(f'{controller_name}/../../../../div[1]/label/span'),
                                   'type': 'check'}),
@@ -382,16 +382,15 @@
                        'type': 'text'}),
             ('value_select', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]').locator(
                 '.ant-select.ant-select-enabled'), 'type': 'select'}),
             ('submit', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//i[2]'),
                         'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
-            ('cancel', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//i[1]'),
-                        'type': 'button'}),
+            ('cancel', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//i[1]'), 'type': 'button', "always_do": True}),
         ]
 
     def measure_card_status(self, name) -> list:
         measure_name = f'//div[@class="ant-table-body"]//div[text()="{name}"]'
         measures = [
             ('online_', {'locator': self.page.locator(f'{measure_name}/../../span/span[1]'), 'type': 'class'}),
             ('group', {'locator': self.page.locator(f'{measure_name}/../../../../td[3]'), 'type': 'text'}),
@@ -418,22 +417,23 @@
                     '.antd-pro-components-app-reg-addr-input-index-wrapper >> .ant-input-group-addon'),
                     'type': 'select'},
                     {'locator': self.pop_up.locator(
                         '.antd-pro-components-app-reg-addr-input-index-wrapper >> .ant-input'), 'type': 'text'}]),
                 ('register_address', {'locator': self.pop_up.locator('#regAddr'), 'type': 'text'}),
                 ('data_type', {'locator': self.pop_up.locator('#dataType'), 'type': 'select',
                                'param': {'bit': self.locale.get('bit'), 'word': self.locale.get('word'),
+                                         'sint': self.locale.get('sint'), 'byte': self.locale.get('byte'),
                                          'int': self.locale.get('int'), 'dword': self.locale.get('dword'),
                                          'dint': self.locale.get('dint'), 'bcd32': self.locale.get('bcd32'),
                                          'float': self.locale.get('float'), 'double': self.locale.get('double'),
                                          'string': self.locale.get('string'), 'bcd16': self.locale.get('bcd16'),
                                          'ulong': self.locale.get('ulong'), 'long': self.locale.get('long')}}),
                 ('decimal_places', {'locator': self.pop_up.locator('#decimal'), 'type': 'text'}),
                 ('read_bit_data', {'locator': self.pop_up.locator('#enableBit'), 'type': 'switch_button'}),
-                ('register_bit', {'locator': self.pop_up.locator('#bitIndex'), 'type': 'text'}),
+                ('register_bit', {'locator': self.pop_up.locator('#regBit'), 'type': 'text'}),
                 ('data_register_bit', {'locator': self.pop_up.locator('#bitIndex'), 'type': 'text'}),
                 ('negative_value', {'locator': self.pop_up.locator('#reverseBit'), 'type': 'switch_button'}),
                 ('size', {'locator': self.pop_up.locator('#len'), 'type': 'text'}),
                 ('encoding_format', {'locator': self.pop_up.locator('#codeType'), 'type': 'select',
                                      'param': {'ascii': 'ASCII', 'utf-8': 'UTF-8', 'utf-16': 'UTF-16',
                                                'utf-16-big': 'UTF-16-BIG', 'gb2312': 'GB2312'}}),
                 ('is_array', {'locator': self.pop_up.locator('#isArr'), 'type': 'switch_button'}),
@@ -470,16 +470,15 @@
                 ('ct', {'locator': self.pop_up.locator('#ct'), 'type': 'text'}),
                 ('package_reporting', {'locator': self.pop_up.locator('#msecSample'), 'type': 'switch_button'}),
                 ('value_mapping', {'locator': self.value_mapping, 'type': 'value_mapping'}),
                 ('submit', {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                             'type': 'button'}),
                 ('text_messages', {'type': 'text_messages'}),
                 ('tip_messages', {'type': 'tip_messages'}),
-                ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                            'type': 'button'}),
+                ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]
 
     @property
     def value_mapping(self) -> dict:
         return {'add': self.pop_up.locator('.ant-btn.ant-btn-primary.ant-btn-background-ghost.ant-btn-block'),
                 'table': self.pop_up.locator('//table'),
                 'ok': self.page.locator('.ant-popover-content').locator('.ant-btn.ant-btn-primary.ant-btn-sm')}
@@ -512,18 +511,17 @@
                      ('storage_method', {'locator': self.pop_up.locator('#historyDataPath'), 'type': 'select',
                                          'param': {'gateway': self.locale.gateway_store, 'usb': self.locale.usb,
                                                    'sd_card': self.locale.sd_card, }}),
                      ('storage_path', {'locator': self.pop_up.locator('#dataPath'), 'type': 'text'}),
                      ('save', {'locator': self.pop_up.locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                          'wait_for': {'type': 'hidden', 'locator': self.pop_up, 'timeout': 300 * 1000}}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
+                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                  ]},
                  'type': 'table_tr', }),
             ('delete_bulk', {'locator': self.page.locator('.anticon.anticon-delete').first,
                              'type': 'button'}),
             ('delete_bulk_confirm', {'locator': self.page.locator('.ant-popover-content').locator(
                 '.ant-btn.ant-btn-primary.ant-btn-sm').first, 'type': 'button'}),
         ]
@@ -540,17 +538,17 @@
                  'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
                      '.ant-btn.ant-btn-primary.ant-btn-sm').first,
                  "columns": [
                      ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                      ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
                      ('save', {'locator': self.pop_up.locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
+                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                  ]},
                  'type': 'table_tr', }),
             ('delete_bulk', {'locator': self.page.locator('.anticon.anticon-delete').first, 'type': 'button',
                              'mouse_move': (-100, 0)}),  # 鼠标移动开，防止遮挡
             ('delete_bulk_confirm', {'locator': self.page.locator('.ant-popover-content').locator(
                 '.ant-btn.ant-btn-primary.ant-btn-sm'), 'type': 'button'}),
         ]
@@ -586,17 +584,17 @@
                        {'locator': self.pop_up.locator('.ant-select.ant-select-enabled').nth(5), 'type': 'select'},
                        {'locator': self.pop_up.locator('.ant-input').nth(2), 'type': 'text'}]),
                      ('content', {'locator': self.pop_up.locator('#content'), 'type': 'text'}),
                      ('label', {'locator': self.pop_up.locator('#alarmLable'), 'type': 'select'}),
                      ('save', {'locator': self.pop_up.locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                          'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
+                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                  ]},
                  'type': 'table_tr', }),
 
             ('delete_bulk', {'locator': self.page.locator('.anticon.anticon-delete').first,
                              'type': 'button'}),
             ('delete_bulk_confirm', {'locator': self.page.locator('.ant-popover-content').locator(
                 '.ant-btn.ant-btn-primary.ant-btn-sm'), 'type': 'button'}),
@@ -630,17 +628,17 @@
                      '.ant-btn.ant-btn-primary.ant-btn-sm').first,
                  "columns": [
                      ('add', {'locator': self.page.locator('.anticon.anticon-plus-circle').first, 'type': 'button'}),
                      ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                      ('save', {'locator': self.pop_up.locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                          'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
-                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
+                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                  ]}, 'type': 'table_tr'}),
             ('delete_bulk', {'locator': self.page.locator('.anticon.anticon-delete').first,
                              'type': 'button'}),
             ('delete_bulk_confirm', {'locator': self.page.locator('.ant-popover-content').locator(
                 '.ant-btn.ant-btn-primary.ant-btn-sm'), 'type': 'button'}),
         ]
 
@@ -721,22 +719,35 @@
                 "columns": [
                     ('key', {'locator': self.pop_up.locator('#key'), 'type': 'text'}),
                     ('value', {'locator': self.pop_up.locator('#value'), 'type': 'text'}),
                     ('save', {'locator': self.pop_up.locator(
                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                         'wait_for': {'type': 'hidden', 'locator': self.pop_up,
                                      'timeout': 30 * 1000}}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
                     ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', })
         ]
 
     @property
+    def cloud_status_locator(self) -> list:
+        return [
+            ('status', {'locator': self.page.locator('//div').get_by_text(self.locale.cloud_status, exact=True).locator(
+                '../div[2]'), 'type': 'text',
+                'param': {'not_enable': self.locale.not_enable, 'connecting': self.locale.connecting,
+                          'connection_successful': self.locale.connection_successful,
+                          'unknown_error': self.locale.unknown_error,
+                          'registering': self.locale.registering_, 'registered': self.locale.registered}}),
+            ('connection_time', {'locator': self.page.locator('//div').get_by_text(self.locale.connection_time,
+                                                                                   exact=True).locator(
+                '../div[2]'), 'type': 'text', 'param': {'day': self.locale.day}}),
+        ]
+
+    @property
     def cloud_locator(self) -> list:
         return [
             ('enable', {'locator': self.page.locator('#enable'), 'type': 'switch_button'}),
             ('clear_offline_cache',
              {'locator': self.page.locator('.ant-btn.ant-btn-danger.ant-btn-sm'), 'type': 'button',
               'relation': [('enable', True)]}),
             ('cache_confirm',
@@ -807,43 +818,43 @@
              {'locator': self.page.locator('#args\.clientId'), 'type': 'text', 'relation': [('enable', True)]}),
             ('mqtt_auth',
              {'locator': self.page.locator('#args\.auth'), 'type': 'switch_button', 'relation': [('enable', True)]}),
             ('mqtt_user', {'locator': self.page.locator('#args\.username'), 'type': 'text',
                            'relation': [('enable', True), ('mqtt_auth', True)]}),
             ('mqtt_password', {'locator': self.page.locator('#args\.passwd'), 'type': 'text',
                                'relation': [('enable', True), ('mqtt_auth', True)]}),
-            ('advanced_settings',
+            ('mqtt_advanced_settings',
              {'locator': self.locale.advanced_settings, 'type': 'expand', 'relation': [('enable', True)]}),
             ('port', {'locator': self.page.locator('#args\.port'), 'type': 'text',
-                      'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+                      'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('keep_alive', {'locator': self.page.locator('#args\.keepalive'), 'type': 'text',
-                            'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+                            'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('tls', {'locator': self.page.locator('#args\.tls'), 'type': 'radio_select',
-                     'relation': [('enable', True), ('mqtt_advanced_settings', True)],
+                     'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')],
                      'param': {'enable': self.locale.enable, 'disable': self.locale.disable_}}),
             ('verify_method', {'locator': self.page.locator('#args\.tlsAuth'), 'type': 'select',
-                               'relation': [('enable', True), ('mqtt_advanced_settings', True)],
+                               'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')],
                                'param': {'verify_client_ca': self.locale.verify_client_ca,
                                          'verify_client_certificate_and_key': self.locale.verify_client_certificate_and_key}}),
             ('verify_server_certificate',
              {'locator': self.page.locator('#args\.verifyServer'), 'type': 'switch_button',
-              'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+              'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('root_ca', {'locator': self.page.locator('.anticon.anticon-upload').nth(1), 'type': 'upload_file',
-                         'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+                         'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('client_private_key',
              {'locator': self.page.locator('.anticon.anticon-upload').nth(2), 'type': 'upload_file',
-              'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+              'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('client_certificate',
              {'locator': self.page.locator('.anticon.anticon-upload').nth(3), 'type': 'upload_file',
-              'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+              'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('clean_session', {'locator': self.page.locator('#args\.cleanSession'), 'type': 'radio_select',
-                               'relation': [('enable', True), ('mqtt_advanced_settings', True)],
+                               'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')],
                                'param': {'no': self.locale.no.upper(), 'yes': self.locale.yes.upper()}}),
             ('mqtt_version', {'locator': self.page.locator('args\.mqttVersion'), 'type': 'radio_select',
-                              'relation': [('enable', True), ('mqtt_advanced_settings', True)]}),
+                              'relation': [('enable', True), ('mqtt_advanced_settings', 'expand')]}),
             ('mqtt_last_will', {'locator': self.locale.last_will, 'type': 'expand',
                                 'relation': [('enable', True), ]}),
             ('mqtt_last_will_topic', {'locator': self.page.locator('args\.willTopic'), 'type': 'text',
                                       'relation': [('enable', True), ('mqtt_last_will', 'expand')]}),
             ('mqtt_last_will_qos', {'locator': self.page.locator('args\.willQos'), 'type': 'select',
                                     'relation': [('enable', True), ('mqtt_last_will', 'expand')]}),
             ('mqtt_last_will_retain', {'locator': self.page.locator('args\.willRetain'), 'type': 'select',
@@ -871,18 +882,17 @@
                     ('entry_function', {'locator': self.pop_up.locator('#funcName'), 'type': 'text'}),
                     ('quick_function',
                      {'locator': self.pop_up.locator('.react-monaco-editor-container'), 'type': 'monaco'}),
                     ('save', {'locator': self.pop_up.locator(
                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                         'wait_for': {'type': 'hidden', 'locator': self.pop_up,
                                      'timeout': 30 * 1000}}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
                     ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'relation': [('enable', True)]}),
             ('subscribe', {'locator': {
                 'locator': self.page.locator('.antd-pro-pages-cloud-service-message-index-addButton').nth(1).locator(
                     '..'),
                 'pop_up_locator': self.pop_up,
                 'action_confirm': self.page.locator('.ant-popover-inner-content').locator(
                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
@@ -894,18 +904,17 @@
                     ('payload_type', {'locator': self.pop_up.locator('#payload_type'), 'type': 'select', }),
                     ('quick_function',
                      {'locator': self.pop_up.locator('.react-monaco-editor-container'), 'type': 'monaco'}),
                     ('save', {'locator': self.pop_up.locator(
                         '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                         'wait_for': {'type': 'hidden', 'locator': self.pop_up,
                                      'timeout': 30 * 1000}}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
-                                'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
                     ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'relation': [('enable', True)]})
         ]
 
     @property
     def cloud_measuring_point(self) -> list:
         return [
             ('page_number', {'locator': self.pop_up.locator('.ant-pagination-options-size-changer'), 'type': 'select',
```

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 2% similar despite different names*

```diff
@@ -726,14 +726,26 @@
                     self.__measure_point(cloud_measure=None, mute_measure=[('check', x, True) for x in all_measure])
                     self.agg_in(self.edge_locators.cloud_measuring_point, {'add_bulk': True, 'bulk_confirm': True})
                 else:
                     pass
         if (cloud_measure or mute_measure) and close:
             self.agg_in(self.edge_locators.cloud_measuring_point, {'close': True})
 
+    @allure.step('断言Cloud状态')
+    @loop_inspector('cloud_status')
+    def assert_status(self, cloud='mqtt_cloud_service', **kwargs):
+        """
+        :param cloud: mqtt_cloud_service, whiteeagle_energy_manager
+        :param kwargs:
+               status: not_enable|connecting|connection_successful|unknown_error|registering|registered ex: status='"${value}"=="connecting"'
+               connection_time: day ex: connection_time='"${value}"=="day"'
+        """
+        self.access_menu(f'edge_computing.device_supervisor.cloud.{cloud}')
+        return self.eval_locator_attribute(kwargs, self.edge_locators.cloud_status_locator)
+
     @allure.step('配置Device Supervisor Cloud')
     def config(self, **kwargs):
         """
 
         :param kwargs:
                 enable: bool True | False 是否启用
                 clear_offline_cache: bool True | False 是否清除离线缓存
@@ -795,15 +807,15 @@
                 azure_auth_method: Symmetric key|X.509 Self-Signed|X.509 CA-Signed
                 azure_connection_string: str
                 azure_hub_name: str
                 azure_device_id: str
                 azure_device_certificate: str, 文件路径
                 azure_device_key: str, 文件路径
 
-                advanced_settings: True|False
+                mqtt_advanced_settings: True|False
                 port: int
                 keep_alive: int
                 tls: 'enable'|'disable'
                 verify_method: verify_client_ca|verify_client_certificate_and_key
                 verify_server_certificate: True|False
                 root_ca: str, 文件路径
                 client_private_key: str, 文件路径
@@ -1233,15 +1245,19 @@
             gain_value = value_range + scale_range
             logging.info('config parameter: {}'.format(gain_value))
             return gain_value
         elif transform_type == 2:
             zoom_range = [round(random.uniform(-9999, 9999), 6) for i in range(2)]
             return zoom_range
         elif transform_type == 3:
-            bit_range = sorted([random.randint(digit_list[type_][0], digit_list[type_][1]) for i in range(2)])
+            start_bit = random.randint(digit_list[type_][0], digit_list[type_][1])
+            end_bit = random.randint(digit_list[type_][0], digit_list[type_][1])
+            while end_bit == start_bit:
+                end_bit = random.randint(digit_list[type_][0], digit_list[type_][1])
+            bit_range = sorted([start_bit, end_bit])
             return bit_range
         else:
             pt_range = [round(random.uniform(-999, 999), 6) for i in range(4)]
             return pt_range
 
     @allure.step('根据数据类型生成随机值')
     def generate_random_value(self, datatype, magnification=1, offset=0, pt=1, ct=1):
```

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/ingateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 import dynaconf
 import os
 
 
 class InGateway(BasePage):
 
     def __init__(self, host: str, super_user: str, super_password: str, page: Page = None, model='IG902',
-                 language='en', protocol='https', port=443, username='adm', password='123456',
-                 bring_to_front=False, **kwargs):
+                 language='en', protocol='https', port=443, username='adm', password='123456', **kwargs):
         """
 
         :param host:   设备主机地址
         :param super_user:  超级用户
         :param super_password: 超级用户密码
         :param page:  playwright page
         :param model:  设备型号  IG902 IG502
@@ -35,45 +34,48 @@
         :param username: 用户名
         :param password: 密码
         :param kwargs:
             telnet: 是否开启telnet, 默认为True 开启
             locale_yaml_path: 本地国际化文件路径
             bring_to_front: 是否将浏览器窗口置顶  默认为False 不置顶
             viewport: {'width': 1366, 'height': 768}  窗口大小
+            web_login_timeout: int  登录超时时间 默认300， 单位秒 即5分钟， 监测到登录超时后，会自动重新登录
         """
         telnet = kwargs.get('telnet', True)
         locale_yaml_path = kwargs.get('locale_yaml_path', None)
         bring_to_front = kwargs.get('bring_to_front', False)
+        web_login_timeout = kwargs.get('web_login_timeout', 300)
         viewport = kwargs.get('viewport', {'width': 1366, 'height': 768})
         if locale_yaml_path:
             in_setting = dynaconf.Dynaconf(
                 settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml'), locale_yaml_path],
                 merge_enabled=True)
         else:
             in_setting = dynaconf.Dynaconf(
                 settings_files=[os.path.join(os.path.dirname(__file__), 'locale.yml')])
         super().__init__(host, username, password, protocol, port, model, language, page, locale=in_setting,
-                         bring_to_front=bring_to_front, viewport=viewport)
+                         bring_to_front=bring_to_front, viewport=viewport, web_login_timeout=web_login_timeout)
         if telnet:
             self.telnet = Telnet(model, host, super_user, super_password)
         else:
             self.telnet = None
         if self.language == 'en':
             self.telnet.send_cli(command='language English', type_='user')
         else:
             self.telnet.send_cli(command='language Chinese', type_='user')
         self.login()
+        self.page.on("response", self.call_web_login_timeout)
         self.overview = Overview(host, username, password, protocol, port, model, language, self.page, self.locale)
         self.network: Network = Network(host, username, password, protocol, port, model, language, self.page,
                                         self.locale)
         self.edge = EdgeComputing(host, username, password, protocol, port, model, language, self.page, self.locale)
         self.system = System(host, username, password, protocol, port, model, language, self.page, self.locale)
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
     with InGateway('10.5.23.160', 'inhand', '64391099@inhand') as device:
-        device.edge.device_supervisor.cloud.config(
-            cloud_measure=[('export', './'), ])
+        device.edge.device_supervisor.cloud.assert_status(cloud='whiteeagle_energy_manager',
+                                                          status='not_enable')
         device.page.wait_for_timeout(10 * 1000)
```

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.64/inhandtest/pages/ingateway/locale.yml`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,16 @@
   connecting: Connecting
   custom: Custom
   current_version: Current Version
   start_capture: Start Capture
   download_capture_file: Download Capture File
   submit_successful: Submit successful
   bit: BIT
+  sint: SINT
+  byte: BYTE
   word: WORD
   dword: DWORD
   int: INT
   dint: DINT
   float: FLOAT
   double: DOUBLE
   string: STRING
@@ -199,14 +201,17 @@
   anonymous: Anonymous
   username_password: Username & Password
   certificate_auth: Certificate Authentication
   automatic_detection: Automatic detection
   sign: Sign
   sign_encrypt: Sign & Encrypt
   siemens_plc: Siemens PLC
+  cloud_status: Cloud Status
+  connection_successful: Connection Successful
+  unknown_error: Unknown Error
 cn:
   client: 客户端
   server: 服务器
   ap: 接入端
   edit: 编辑
   delete: 删除
   set_as_template: 设为模板
@@ -356,14 +361,16 @@
   connecting: 正在连接
   custom: 自定义
   current_version: 当前版本
   start_capture: 开始抓包
   download_capture_file: 下载抓包文件
   submit_successful: 提交成功
   bit: BIT(位：0/1)
+  sint: SINT(8位有符号整数)
+  byte: BYTE(8位无符号整数)
   word: WORD(16位无符号整数)
   dword: DWORD(32位无符号整数)
   int: INT(16位有符号整数)
   dint: DINT(32位有符号整数)
   float: FLOAT(单精度浮点数)
   double: DOUBLE(64位浮点数)
   string: STRING(8位字符串)
@@ -404,9 +411,11 @@
   anonymous: 匿名登录
   username_password: 用户名和密码
   certificate_auth: 证书认证
   automatic_detection: 自动检测
   sign: 签名
   sign_encryption: 签名和加密
   siemens_plc: Siemens Plc（西门子）
-
+  cloud_status: 云服务状态
+  connection_successful: 连接成功
+  unknown_error: 未知错误
```

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,21 @@
                     ('network_type', {'locator': self.pop_up.locator('#network_type'), 'type': 'select'}),
                     ('apn', {'locator': self.pop_up.locator('#apn'), 'type': 'text'}),
                     ('access_number', {'locator': self.pop_up.locator('#access_number'), 'type': 'text'}),
                     ('auth_method', {'locator': self.pop_up.locator('#auth_method'), 'type': 'select',
                                      'param': {'auto': self.locale.auto}}),
                     ('username', {'locator': self.pop_up.locator('#username'), 'type': 'text'}),
                     ('password', {'locator': self.pop_up.locator('#password'), 'type': 'text'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
-                    ('save',
-                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'relation': [('cellular_enable', 'enable')]}),
             ('dual_sim_enable', {'locator': self.page.locator('#enable_dual_sim'), 'type': 'switch_button',
                                  'relation': [('cellular_enable', 'enable')]}),
             ('main_sim', {'locator': self.page.locator('#main_sim'), 'type': 'select',
                           'param': {'Random': self.locale.random, 'Sequence': self.locale.sequence},
                           'relation': [('cellular_enable', 'enable'), ('dual_sim_enable', 'enable')]}),
             ('max_number_of_dial', {'locator': self.page.locator('#max_dial_times'), 'type': 'text',
@@ -183,15 +184,15 @@
               'type': 'button'}),
             ('confirm',
              {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn ant-btn-primary"]'),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class EthernetLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -247,28 +248,28 @@
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.pop_up.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.pop_up.locator('#netmask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class BridgeLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -304,30 +305,31 @@
             ('netmask', {'locator': self.page.locator('#netmask'), 'type': 'text'}),
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.pop_up.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask', {'locator': self.pop_up.locator('#netmask'), 'type': 'text'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
-                    ('save',
-                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('ge_01', {'locator': self.page.locator('//button[@id="gigabitethernet 0/1"]'), 'type': 'switch_button'}),
             ('ge_02', {'locator': self.page.locator('//button[@id="gigabitethernet 0/2"]'), 'type': 'switch_button'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class WlanLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -443,15 +445,15 @@
                                    'relation': [('enable_wifi', 'enable'), ('station_role', 'ap')]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'text_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class WanLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -506,29 +508,30 @@
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class LanLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -565,29 +568,30 @@
             ('shutdown', {'locator': self.page.locator('#shutdown'), 'type': 'switch_button'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class LoopbackLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -608,29 +612,30 @@
         return [
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class DhcpLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -648,42 +653,44 @@
                      {'locator': self.page.locator('.ant-modal-content').locator('#interface'), 'type': 'select'}),
                     ('start_address',
                      {'locator': self.page.locator('.ant-modal-content').locator('#start_addr'), 'type': 'text'}),
                     ('end_address',
                      {'locator': self.page.locator('.ant-modal-content').locator('#end_addr'), 'type': 'text'}),
                     ('lease',
                      {'locator': self.page.locator('.ant-modal-content').locator('#lease'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('windows_name_server', {'locator': self.page.locator('#windows_name_server'), 'type': 'text'}),
             ('static_ip_setting', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox').nth(1),
                 "columns": [
                     ('mac_address', {'locator': self.pop_up.locator('#mac_addr'), 'type': 'text'}),
                     ('ip_address', {'locator': self.pop_up.locator('#ip_addr'), 'type': 'text'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
-                    ('save',
-                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'param': {'enable': self.locale.enable, 'not_enable': self.locale.not_enable}}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class DnsLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -702,29 +709,30 @@
             ('domain_ip_address_pair', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('host',
                      {'locator': self.pop_up.locator('#host'), 'type': 'text'}),
                     ('ip_address1', {'locator': self.pop_up.locator('#ip_addr1'), 'type': 'text'}),
                     ('ip_address2', {'locator': self.pop_up.locator('#ip_addr2'), 'type': 'text'}),
+                    ('save',
+                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                     ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
-                    ('save',
-                     {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit_domain_ip_address_pair',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(1),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class GpsLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -798,29 +806,30 @@
             ('destination_ip_address', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('server',
                      {'locator': self.page.locator('.ant-modal-content').locator('#server_ip'), 'type': 'text'}),
                     ('port',
                      {'locator': self.page.locator('.ant-modal-content').locator('#server_port'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
     @property
     def gps_serial_forwarding_locators(self) -> list:
         return [
             ('enable', {'locator': self.page.locator('#enable'), 'type': 'switch_button'}),
             ('serial_type',
@@ -847,15 +856,15 @@
                              'relation': [('enable', True)]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class HostListLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -911,32 +920,33 @@
                                {'locator': self.page.locator('.ant-modal-content').locator('#gateway'),
                                 'type': 'text'}),
                               ('distance',
                                {'locator': self.page.locator('.ant-modal-content').locator('#distance'),
                                 'type': 'text'}),
                               ('track_id',
                                {'locator': self.page.locator('.ant-modal-content').locator('#track'), 'type': 'text'}),
+                              ('save',
+                               {'locator': self.page.locator('.ant-modal-content').locator(
+                                   '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                               ('text_messages', {'type': 'text_messages'}),
+                              ('tip_messages', {'type': 'tip_messages'}),
                               ('cancel',
                                {'locator': self.page.locator('.ant-modal-content').locator(
-                                   '//button[@class="ant-btn"]'),
-                                   'type': 'button'}),
-                              ('save',
-                               {'locator': self.page.locator('.ant-modal-content').locator(
-                                   '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})]},
+                                   '//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
+                          ]},
               'param': {'all': self.locale.all, 'connected_routing': self.locale.connected_routing,
                         'static_routing': self.locale.static_routing, 'ospf': 'OSPF', 'bgp': 'BGP',
                         'rip': 'RIP'}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class AclLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -990,49 +1000,52 @@
                                     'type': 'switch_button'}),
                      ('established', {'locator': self.page.locator('.ant-modal-content').locator('#established'),
                                       'type': 'switch_button'}),
                      ('log', {'locator': self.page.locator('.ant-modal-content').locator('#log'),
                               'type': 'switch_button'}),
                      ('description', {'locator': self.page.locator('.ant-modal-content').locator('#description'),
                                       'type': 'text'}),
+                     ('save',
+                      {'locator': self.page.locator('.ant-modal-content').locator(
+                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
+                     ('tip_messages', {'type': 'tip_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                       'type': 'button'}),
-                     ('save',
-                      {'locator': self.page.locator('.ant-modal-content').locator(
-                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})]},
+                       'type': 'button', "always_do": True}),
+                 ]},
                  'type': 'table_tr'}),
             ('access_control_list',
              {'locator': {
                  'locator': self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox'),
                  "columns": [
                      ('interface', {'locator': self.page.locator('#interface'), 'type': 'select'}),
                      ('in_acl',
                       {'locator': self.page.locator('.ant-modal-content').locator('#inbound_acl'), 'type': 'select'}),
                      ('out_acl',
                       {'locator': self.page.locator('.ant-modal-content').locator('#outbound_acl'), 'type': 'select'}),
                      ('admin_acl',
                       {'locator': self.page.locator('.ant-modal-content').locator('#admin_acl'), 'type': 'select'}),
+                     ('save',
+                      {'locator': self.page.locator('.ant-modal-content').locator(
+                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
                      ('tip_messages', {'type': 'tip_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                       'type': 'button'}),
-                     ('save',
-                      {'locator': self.page.locator('.ant-modal-content').locator(
-                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})]},
+                       'type': 'button', "always_do": True}),
+                 ]},
                  'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class NatLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -1077,45 +1090,48 @@
                       {'locator': self.pop_up.locator('//div[@id="transmit_dest.interface"]'), 'type': 'select'}),
                      ('translated_port',
                       {'locator': self.pop_up.locator('//input[@id="transmit_dest.port"]'), 'type': 'text'}),
                      ('translated_end_port',
                       {'locator': self.pop_up.locator('//input[@id="transmit_dest.end_port"]'), 'type': 'text'}),
                      ('log', {'locator': self.pop_up.locator('#log'), 'type': 'switch_button'}),
                      ('description', {'locator': self.pop_up.locator('#description'), 'type': 'text'}),
+                     ('save',
+                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
+                       'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
+                     ('tip_messages', {'type': 'tip_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                       'type': 'button'}),
-                     ('save',
-                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
-                       'type': 'button'})]},
+                       'type': 'button', "always_do": True}),
+                 ]},
                  'type': 'table_tr', 'param': {'inside': self.locale.inside, 'outside': self.locale.outside}}),
             ('network_interface',
              {'locator': {
                  'locator': self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox').nth(1),
                  "columns": [
                      ('interface', {'locator': self.page.locator('#interface'), 'type': 'select'}),
                      ('interface_type',
                       {'locator': self.pop_up.locator('#type'), 'type': 'radio_select',
                        'param': {'inside': self.locale.inside, 'outside': self.locale.outside}}),
+                     ('save',
+                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                      ('text_messages', {'type': 'text_messages'}),
+                     ('tip_messages', {'type': 'tip_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                       'type': 'button'}),
-                     ('save',
-                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
-                       'type': 'button'})]},
+                       'type': 'button', "always_do": True}),
+                 ]},
                  'type': 'table_tr', 'param': {'inside': self.locale.inside, 'outside': self.locale.outside}}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class L2tpLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -1144,89 +1160,94 @@
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(0),
                 "columns": [
                     ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                     ('auth', {'locator': self.pop_up.locator('#authentication'), 'type': 'radio_select',
                               'param': {'yes': self.locale.yes, 'no': self.locale.no}}),
                     ('hostname', {'locator': self.pop_up.locator('#hostname'), 'type': 'text'}),
                     ('challenge_secret', {'locator': self.pop_up.locator('#challenge_secret'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr',
                 'param': {'yes': self.locale.yes, 'no': self.locale.no}}),
             ('pseudowire_class', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(1),
                 "columns": [
                     ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                     ('l2tp_class', {'locator': self.pop_up.locator('#class'), 'type': 'select'}),
                     ('source_interface', {'locator': self.pop_up.locator('#source_interface'), 'type': 'select'}),
                     ('data_encapsulation_method',
                      {'locator': self.pop_up.locator('#data_encapsulation_method'), 'type': 'select'}),
                     ('tunnel_management_protocol',
                      {'locator': self.pop_up.locator('#tunnel_management_protocol'), 'type': 'select'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('l2tpv2_tunnel', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(2),
                 "columns": [
                     ('enable', {'locator': self.pop_up.locator('#enable'), 'type': 'switch_button'}),
                     ('id', {'locator': self.pop_up.locator('#id'), 'type': 'text'}),
                     ('l2tp_server', {'locator': self.pop_up.locator('#server'), 'type': 'text'}),
                     ('pseudowire_class', {'locator': self.pop_up.locator('#pseudowire_class'), 'type': 'select'}),
                     ('auth_type', {'locator': self.pop_up.locator('#authentication_type'), 'type': 'select',
                                    'param': {'AUTO': self.locale.auto}}),
                     ('username', {'locator': self.pop_up.locator('#username'), 'type': 'text'}),
                     ('password', {'locator': self.pop_up.locator('#password'), 'type': 'text'}),
                     ('local_ip_address', {'locator': self.pop_up.locator('#local_ip_address'), 'type': 'text'}),
                     ('remote_ip_address', {'locator': self.pop_up.locator('#remote_ip_address'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('l2tpv3_tunnel', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(3),
                 "columns": [
                     ('enable', {'locator': self.pop_up.locator('#enable'), 'type': 'switch_button'}),
                     ('id', {'locator': self.pop_up.locator('#id'), 'type': 'text'}),
                     ('peer_id', {'locator': self.pop_up.locator('#peer_id'), 'type': 'text'}),
                     ('pseudowire_class', {'locator': self.pop_up.locator('#pseudowire_class'), 'type': 'select'}),
                     ('protocol', {'locator': self.pop_up.locator('#protocol'), 'type': 'select'}),
                     ('source_port', {'locator': self.pop_up.locator('#source_port'), 'type': 'text'}),
                     ('destination_port', {'locator': self.pop_up.locator('#destination_port'), 'type': 'text'}),
                     ('xconnect_interface', {'locator': self.pop_up.locator('#xconnect_interface'), 'type': 'select'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('l2tpv3_session', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(4),
                 "columns": [
                     ('local_session_id', {'locator': self.pop_up.locator('#local_session_id'), 'type': 'text'}),
                     ('remote_session_id', {'locator': self.pop_up.locator('#remote_session_id'), 'type': 'text'}),
                     ('local_tunnel_id', {'locator': self.pop_up.locator('#local_tunnel_id'), 'type': 'select'}),
                     ('local_session_ip_address',
                      {'locator': self.pop_up.locator('#local_session_ip_address'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
     @property
     def l2tp_service_locators(self) -> list:
         return [
             ('enable', {'locator': self.page.locator('#enable'), 'type': 'switch_button'}),
             ('username', {'locator': self.page.locator('#username'), 'type': 'text', 'relation': [('enable', True)]}),
@@ -1258,15 +1279,15 @@
              {'locator': self.page.locator('#export_options'), 'type': 'text', 'relation': [('enable', True)]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
-                       'type': 'button'}),
+                       'type': 'button', "always_do": True}),
         ]
 
 
 class NetworkLocators(EthernetLocators, CellularLocators, BridgeLocators, WlanLocators, WanLocators, LanLocators,
                       LoopbackLocators, DhcpLocators, DnsLocators, GpsLocators, HostListLocators,
                       RoutingStatusLocators, StaticRoutingLocators, AclLocators, NatLocators, L2tpLocators):
     pass
```

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.64/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,19 @@
             ('sntp_interval', {'locator': self.page.locator('#update_interval'), 'type': 'text',
                                'relation': [('enable_sntp_clients', True)]}),
             ('sntp_servers', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
                     ('port', {'locator': self.pop_up.locator('#port'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'relation': [('enable_sntp_clients', True)]}),
             ('submit_sntp',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(0),
               'type': 'button'}),
             ('enable_ntp_server', {'locator': self.page.locator('#enable').nth(1), 'type': 'switch_button'}),
             ('pre_ntp_server', {'locator': self.page.locator('#master'), 'type': 'text',
@@ -74,18 +75,19 @@
                            'relation': [('enable_ntp_server', True)]}),
             ('ntp_servers', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox'),
                 'action_confirm': self.page.locator('.ant-popover-inner').locator(
                     '.ant-btn.ant-btn-primary.ant-btn-sm'),
                 "columns": [
                     ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
             ('submit_ntp',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(1),
               'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
@@ -129,18 +131,19 @@
         return [
             ('enable_remote_server', {'locator': self.page.locator('#log_to_remote_enable'), 'type': 'check'}),
             ('remote_server', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
                     ('port', {'locator': self.pop_up.locator('#server_port'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'relation': [('enable_remote_server', True)]}),
             ('log_to_console', {'locator': self.page.locator('#log_to_console'), 'type': 'check'}),
             ('history_log_file_size',
              {'locator': self.page.locator('//input[@class="ant-input-number-input"]'), 'type': 'text'}),
             ('history_log_level',
              {'locator': self.page.locator('.ant-select.ant-select-enabled'), 'type': 'select',
               'param': {'emergency': self.locale.emergency, 'alarm': self.locale.alarm,
@@ -323,21 +326,22 @@
                 "locator": self.page.locator('//label[@for="https.enable.form"]').locator('../../..').locator(
                     '.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('source_network',
                      {'locator': self.pop_up.locator('#source_network'), 'type': 'text'}),
                     ('ip_wildcard',
                      {'locator': self.pop_up.locator('#wildcard_mask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr', 'relation': [('https_remote_access', 'enable')]}),
 
             ('enable_telnet',
              {'locator': self.page.locator('//button[@id="telnet.enable"]'), 'type': 'switch_button'}),
             ('telnet_listen_ip',
              {'locator': self.page.locator('//div[@id="telnet.listen_ip_addr"]'), 'type': 'select',
               'relation': [('enable_telnet', 'enable')]}),
@@ -350,21 +354,22 @@
                 "locator": self.page.locator('//label[@for="telnet.enable.form"]').locator('../../..').locator(
                     '.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('source_network',
                      {'locator': self.pop_up.locator('#source_network'), 'type': 'text'}),
                     ('ip_wildcard',
                      {'locator': self.pop_up.locator('#wildcard_mask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr',
                 'relation': [('telnet_remote_access', 'enable')]}),
 
             ('enable_ssh',
              {'locator': self.page.locator('//button[@id="ssh.enable"]'), 'type': 'switch_button'}),
             ('ssh_listen_ip',
              {'locator': self.page.locator('//div[@id="ssh.listen_ip_addr"]'), 'type': 'select',
@@ -382,21 +387,22 @@
                 "locator": self.page.locator('//label[@for="ssh.enable.form"]').locator('../../..').locator(
                     '.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('source_network',
                      {'locator': self.pop_up.locator('#source_network'), 'type': 'text'}),
                     ('ip_wildcard',
                      {'locator': self.pop_up.locator('#wildcard_mask'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr',
                 'relation': [('ssh_remote_access', 'enable')]}),
 
             ('enable_developer',
              {'locator': self.page.locator('//button[@id="devlopMode.debug_enable"]'), 'type': 'switch_button'}),
             ('enable_fixed_password',
              {'locator': self.page.locator('//button[@id="devlopMode.fixed_passwd"]'), 'type': 'switch_button',
@@ -428,22 +434,23 @@
                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
                 "columns": [
                     ('username',
                      {'locator': self.pop_up.locator('#username'), 'type': 'text'}),
                     ('permission', {'locator': self.pop_up.locator('#privilege'), 'type': 'select'}),
                     ('password', {'locator': self.pop_up.locator('#password'), 'type': 'text'}),
                     ('confirm_password', {'locator': self.pop_up.locator('#passwordConfirm'), 'type': 'text'}),
-                    ('text_messages', {'type': 'text_messages'}),
-                    ('cancel',
-                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
-                      'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                          'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
+                    ('text_messages', {'type': 'text_messages'}),
+                    ('tip_messages', {'type': 'tip_messages'}),
+                    ('cancel',
+                     {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
+                      'type': 'button', "always_do": True}),
                 ]}, 'type': 'table_tr'}),
         ]
 
 
 class RebootLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
```

### Comparing `inhandtest-0.0.63/inhandtest/pytest_email.html` & `inhandtest-0.0.64/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/inhandtest/telnet.py` & `inhandtest-0.0.64/inhandtest/telnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,9 +687,8 @@
         self.tn.close()
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
     # enable_log('./log.log', 'DEBUG')
-    # a = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
     # a.assert_cli('ifconfig', 'fe80::67f:eff:fe01:92be/64')
```

### Comparing `inhandtest-0.0.63/inhandtest/tools.py` & `inhandtest-0.0.64/inhandtest/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,16 +397,19 @@
     :param diff: int 允许的误差 more为0  正整数
     :param time_format: str 时间格式
     :param order_by: bool True 传入的时间列表是按时间从小到大排列， False 传入的时间列表是按时间从大到小排列
     :return:
     """
     tmp = []
     for each in time_list:
-        each = time.strptime(each, time_format)
-        tmp.append(int(time.mktime(each)))
+        if isinstance(each, int):
+            tmp.append(each)
+        else:
+            each = time.strptime(each, time_format)
+            tmp.append(int(time.mktime(each)))
     t0 = tmp[0]
     for i_ in tmp[1:]:
         if not order_by:
             assert delta-diff <= t0 - i_ <= delta + diff, f'The time error between {t0} and {i_} is large'
         else:
             assert delta-diff <= i_ - t0 <= delta + diff, f'The time error between {t0} and {i_} is large'
         t0 = i_
@@ -506,15 +509,15 @@
         elif type_ == 'lowercase':
             return ''.join(random.choice(string.ascii_lowercase) for _ in range(length_))
         elif type_ == 'uppercase':
             return ''.join(random.choice(string.ascii_uppercase) for _ in range(length_))
         elif type_ == 'special_chars':
             return ''.join(random.choice(string.punctuation) for _ in range(length_))
         elif type_ == 'chinese_chars':
-            length_ = int(length_ / 2) if peer_chinese_chars_len != 1 else length_
+            length_ = int(length_ / peer_chinese_chars_len) if peer_chinese_chars_len != 1 else length_
             return ''.join(random_chinese_character() for _ in range(length_))
 
     # 定义字符集
     def split_number(num, n, contain_even_=True):
         """
         将一个数字拆分成n个数字相加得来
         :param num: 要拆分的数字
@@ -523,15 +526,15 @@
         :return: 拆分后的数字列表
         """
         value = []
         for i in range(n, 0, -1):
             if i != 1:
                 if num - i > 0:
                     if contain_even_:
-                        one = random.randrange(2, num - i, 2)
+                        one = random.randrange(peer_chinese_chars_len, num - i, peer_chinese_chars_len)
                         contain_even_ = False
                     else:
                         one = random.randint(1, num - i)
                     num = num - one
                 elif num - i == 0:
                     if contain_even_:
                         logging.exception('The minimum generated string does not support the inclusion of Chinese char')
@@ -706,8 +709,8 @@
             raise AttributeError(key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
 
 if __name__ == '__main__':
-    print(get_time_stamp('2022-02-18T13:39:32Z', -2))
+    print(generate_string(20, chinese_chars=True, peer_chinese_chars_len=3))
```

### Comparing `inhandtest-0.0.63/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.64/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.63
+Version: 0.0.64
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.63/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.64/inhandtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.63/setup.py` & `inhandtest-0.0.64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.63',
+    version='0.0.64',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```


# Comparing `tmp/ultrasync-0.9.8.tar.gz` & `tmp/ultrasync-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultrasync-0.9.8.tar", last modified: Mon Jun  5 02:45:19 2023, max compression
+gzip compressed data, was "ultrasync-0.9.9.tar", last modified: Mon Aug  7 16:23:03 2023, max compression
```

## Comparing `ultrasync-0.9.8.tar` & `ultrasync-0.9.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.755961 ultrasync-0.9.8/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1090 2023-06-05 02:41:15.000000 ultrasync-0.9.8/LICENSE
--rw-r--r--   0 l2g       (1000) l2g       (1000)      191 2023-06-05 02:41:15.000000 ultrasync-0.9.8/MANIFEST.in
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7188 2023-06-05 02:45:19.755961 ultrasync-0.9.8/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6235 2023-06-05 02:41:15.000000 ultrasync-0.9.8/README.md
--rw-r--r--   0 l2g       (1000) l2g       (1000)       43 2023-06-05 02:41:15.000000 ultrasync-0.9.8/dev-requirements.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-06-05 02:41:15.000000 ultrasync-0.9.8/requirements.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      335 2023-06-05 02:45:19.755961 ultrasync-0.9.8/setup.cfg
--rwxr-xr-x   0 l2g       (1000) l2g       (1000)     3031 2023-06-05 02:41:43.000000 ultrasync-0.9.8/setup.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.748961 ultrasync-0.9.8/tests/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5121 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7424 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_106.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6360 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_108-zone-check.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6635 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_108.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4922 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_comnav_0_108_burglar_alarm_on.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3873 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_config.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4828 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_xgen8_bypass.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7289 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_xgen8_nxg8zbo.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7984 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_xgen_general.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4590 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_zerowire_armed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6543 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/test_zerowire_general.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/comnav/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.749961 ultrasync-0.9.8/tests/var/comnav/0.106/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1892 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)    36123 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/master.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/seq.w.update.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/seq.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21526 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/status.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)      436 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/status.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1832 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       82 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zstate.bank0.w.update.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)       81 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zstate.bank4.w.update.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)       82 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.106/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.750961 ultrasync-0.9.8/tests/var/comnav/0.108/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1971 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23023 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/master.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/seq.w.update.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/seq.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18114 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/status.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)      436 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/status.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2793 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       98 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.751961 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1983 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23026 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/master.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/seq.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18114 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/status.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/status.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2791 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.751961 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2044 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       97 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/seq.w.update.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)       97 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/seq.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)      458 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/status.xml
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2327 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       91 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/xgen/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.752961 ultrasync-0.9.8/tests/var/xgen/general/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1862 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13088 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/master.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)      130 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/seq.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)      130 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/seq.w.update.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18618 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/status.js
--rw-r--r--   0 l2g       (1000) l2g       (1000)      188 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/status.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2071 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       76 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/zstate.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)       76 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen/general/zstate.w.update.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/xgen8/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.752961 ultrasync-0.9.8/tests/var/xgen8/bypass/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2217 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)      326 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/seq.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)       73 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/zonefunction.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2054 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       73 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/bypass/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.753961 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2282 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/seq.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/seq.w.update.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)      563 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/status.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2088 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       75 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zstate.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)       75 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zstate.w.update.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.746960 ultrasync-0.9.8/tests/var/zerowire/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.753961 ultrasync-0.9.8/tests/var/zerowire/armed/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1848 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)      165 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/seq.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)      196 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/status.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2582 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       94 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/armed/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.754961 ultrasync-0.9.8/tests/var/zerowire/general/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1848 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/area.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)      160 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/seq.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)      196 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/status.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2574 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/zones.htm
--rw-r--r--   0 l2g       (1000) l2g       (1000)       94 2023-06-05 02:41:15.000000 ultrasync-0.9.8/tests/var/zerowire/general/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.754961 ultrasync-0.9.8/ultrasync/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1793 2023-06-05 02:41:59.000000 ultrasync-0.9.8/ultrasync/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8954 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8351 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6747 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/config.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2282 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/logger.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    82964 2023-06-05 02:41:15.000000 ultrasync-0.9.8/ultrasync/main.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-06-05 02:45:19.755961 ultrasync-0.9.8/ultrasync.egg-info/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7188 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3085 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/SOURCES.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/dependency_links.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       49 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/entry_points.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/requires.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       10 2023-06-05 02:45:19.000000 ultrasync-0.9.8/ultrasync.egg-info/top_level.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.471238 ultrasync-0.9.9/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1090 2023-06-05 02:41:15.000000 ultrasync-0.9.9/LICENSE
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      191 2023-06-05 02:41:15.000000 ultrasync-0.9.9/MANIFEST.in
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7447 2023-08-07 16:23:03.471238 ultrasync-0.9.9/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6494 2023-08-07 15:33:29.000000 ultrasync-0.9.9/README.md
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       43 2023-06-05 02:41:15.000000 ultrasync-0.9.9/dev-requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-06-05 02:41:15.000000 ultrasync-0.9.9/requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-08-07 16:23:03.472238 ultrasync-0.9.9/setup.cfg
+-rwxr-xr-x   0 l2g       (1000) l2g       (1000)     3031 2023-08-07 15:23:29.000000 ultrasync-0.9.9/setup.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.465238 ultrasync-0.9.9/tests/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5135 2023-08-07 15:53:35.000000 ultrasync-0.9.9/tests/test_cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7802 2023-08-07 16:20:17.000000 ultrasync-0.9.9/tests/test_comnav_0_106.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6738 2023-08-07 16:19:26.000000 ultrasync-0.9.9/tests/test_comnav_0_108-zone-check.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7013 2023-08-07 16:18:30.000000 ultrasync-0.9.9/tests/test_comnav_0_108.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5300 2023-08-07 16:16:14.000000 ultrasync-0.9.9/tests/test_comnav_0_108_burglar_alarm_on.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3873 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/test_config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4842 2023-08-07 15:47:33.000000 ultrasync-0.9.9/tests/test_xgen8_bypass.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7303 2023-08-07 15:47:36.000000 ultrasync-0.9.9/tests/test_xgen8_nxg8zbo.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7998 2023-08-07 15:47:39.000000 ultrasync-0.9.9/tests/test_xgen_general.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4604 2023-08-07 15:47:43.000000 ultrasync-0.9.9/tests/test_zerowire_armed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6557 2023-08-07 15:47:48.000000 ultrasync-0.9.9/tests/test_zerowire_general.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.463238 ultrasync-0.9.9/tests/var/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.463238 ultrasync-0.9.9/tests/var/comnav/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.466238 ultrasync-0.9.9/tests/var/comnav/0.106/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1892 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    36123 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/seq.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21526 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      436 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1832 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       82 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/zstate.bank0.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       81 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/zstate.bank4.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       82 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.106/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.467238 ultrasync-0.9.9/tests/var/comnav/0.108/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1971 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23023 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/seq.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18114 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      436 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2793 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       98 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.467238 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1983 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23026 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       92 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18114 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2791 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       96 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.468238 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2044 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       97 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/seq.w.update.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       97 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/seq.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      458 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/status.xml
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2327 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       91 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.463238 ultrasync-0.9.9/tests/var/xgen/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.469238 ultrasync-0.9.9/tests/var/xgen/general/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1862 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13088 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/master.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      130 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      130 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/seq.w.update.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18618 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/status.js
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      188 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2071 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       76 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/zstate.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       76 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen/general/zstate.w.update.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.463238 ultrasync-0.9.9/tests/var/xgen8/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.469238 ultrasync-0.9.9/tests/var/xgen8/bypass/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2217 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/bypass/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      326 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/bypass/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       73 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/bypass/zonefunction.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2054 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/bypass/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       73 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/bypass/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.469238 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2282 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      321 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/seq.w.update.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      563 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2088 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       75 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/zstate.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       75 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/zstate.w.update.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.463238 ultrasync-0.9.9/tests/var/zerowire/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.470238 ultrasync-0.9.9/tests/var/zerowire/armed/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1848 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/armed/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      165 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/armed/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      196 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/armed/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2582 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/armed/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       94 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/armed/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.470238 ultrasync-0.9.9/tests/var/zerowire/general/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1848 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/general/area.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      160 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/general/seq.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      196 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/general/status.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2574 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/general/zones.htm
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       94 2023-06-05 02:41:15.000000 ultrasync-0.9.9/tests/var/zerowire/general/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.471238 ultrasync-0.9.9/ultrasync/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1793 2023-08-07 15:24:48.000000 ultrasync-0.9.9/ultrasync/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9562 2023-08-07 16:08:24.000000 ultrasync-0.9.9/ultrasync/cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8351 2023-06-05 02:41:15.000000 ultrasync-0.9.9/ultrasync/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6747 2023-06-05 02:41:15.000000 ultrasync-0.9.9/ultrasync/config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2282 2023-06-05 02:41:15.000000 ultrasync-0.9.9/ultrasync/logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    86250 2023-08-07 16:08:30.000000 ultrasync-0.9.9/ultrasync/main.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-08-07 16:23:03.471238 ultrasync-0.9.9/ultrasync.egg-info/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7447 2023-08-07 16:23:03.000000 ultrasync-0.9.9/ultrasync.egg-info/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3085 2023-08-07 16:23:03.000000 ultrasync-0.9.9/ultrasync.egg-info/SOURCES.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-08-07 16:23:03.000000 ultrasync-0.9.9/ultrasync.egg-info/dependency_links.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       49 2023-08-07 16:23:03.000000 ultrasync-0.9.9/ultrasync.egg-info/entry_points.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-08-07 16:23:03.000000 ultrasync-0.9.9/ultrasync.egg-info/requires.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       10 2023-08-07 16:23:03.000000 ultrasync-0.9.9/ultrasync.egg-info/top_level.txt
```

### Comparing `ultrasync-0.9.8/LICENSE` & `ultrasync-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/PKG-INFO` & `ultrasync-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultrasync
-Version: 0.9.8
+Version: 0.9.9
 Summary: Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync ZeroWire
 Home-page: https://github.com/caronc/ultrasync
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: MIT
 Keywords: XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire Security Panel
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,24 +17,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# NX-595E Output Control Fork
+This fork is designated to implementing the "Output Control" section of the NX-595E. The main objective is to enable communication with the outputs and ensure its proper implementation.
+
 # NX-595E UltraSync Hub
 
 Compatible with both NX-595E [Hills](https://www.hills.com.au/) ComNav, xGen, xGen8 (such as [NXG-8-Z-BO](https://firesecurityproducts.com/en/product/intrusion/NXG_8_Z_BO/82651)), [Interlogix](https://www.interlogix.com/), and [ZeroWire](https://www.interlogix.com/intrusion/product/ultrasync-selfcontained-hub) UltraSync solutions.
 
 ![ZeroWire Hub Image](https://raw.githubusercontent.com/caronc/ultrasync/master/static/zerowire_hub.jpeg)
 
 [![Paypal](https://img.shields.io/badge/paypal-donate-green.svg)](https://paypal.me/lead2gold?locale.x=en_US)
 [![Follow](https://img.shields.io/twitter/follow/l2gnux)](https://twitter.com/l2gnux/)<br/>
 [![Python](https://img.shields.io/pypi/pyversions/ultrasync.svg?style=flat-square)](https://pypi.org/project/ultrasync/)
-[![Build Status](https://travis-ci.org/caronc/ultrasync.svg?branch=master)](https://travis-ci.org/caronc/ultrasync)
+[![Build Status](https://github.com/caronc/ultrasync/actions/workflows/tests.yml/badge.svg)](https://github.com/caronc/ultrasync/actions/workflows/tests.yml)
 [![CodeCov Status](https://codecov.io/github/caronc/ultrasync/branch/master/graph/badge.svg)](https://codecov.io/github/caronc/ultrasync)
 [![Downloads](http://pepy.tech/badge/ultrasync)](https://pypi.org/project/ultrasync/)
 
 ## How Does It Work?
 
 1. First you need to install it; this part is easy:
```

### Comparing `ultrasync-0.9.8/README.md` & `ultrasync-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+# NX-595E Output Control Fork
+This fork is designated to implementing the "Output Control" section of the NX-595E. The main objective is to enable communication with the outputs and ensure its proper implementation.
+
 # NX-595E UltraSync Hub
 
 Compatible with both NX-595E [Hills](https://www.hills.com.au/) ComNav, xGen, xGen8 (such as [NXG-8-Z-BO](https://firesecurityproducts.com/en/product/intrusion/NXG_8_Z_BO/82651)), [Interlogix](https://www.interlogix.com/), and [ZeroWire](https://www.interlogix.com/intrusion/product/ultrasync-selfcontained-hub) UltraSync solutions.
 
 ![ZeroWire Hub Image](https://raw.githubusercontent.com/caronc/ultrasync/master/static/zerowire_hub.jpeg)
 
 [![Paypal](https://img.shields.io/badge/paypal-donate-green.svg)](https://paypal.me/lead2gold?locale.x=en_US)
 [![Follow](https://img.shields.io/twitter/follow/l2gnux)](https://twitter.com/l2gnux/)<br/>
 [![Python](https://img.shields.io/pypi/pyversions/ultrasync.svg?style=flat-square)](https://pypi.org/project/ultrasync/)
-[![Build Status](https://travis-ci.org/caronc/ultrasync.svg?branch=master)](https://travis-ci.org/caronc/ultrasync)
+[![Build Status](https://github.com/caronc/ultrasync/actions/workflows/tests.yml/badge.svg)](https://github.com/caronc/ultrasync/actions/workflows/tests.yml)
 [![CodeCov Status](https://codecov.io/github/caronc/ultrasync/branch/master/graph/badge.svg)](https://codecov.io/github/caronc/ultrasync)
 [![Downloads](http://pepy.tech/badge/ultrasync)](https://pypi.org/project/ultrasync/)
 
 ## How Does It Work?
 
 1. First you need to install it; this part is easy:
```

### Comparing `ultrasync-0.9.8/setup.py` & `ultrasync-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 else:
     # Load our CLI
     console_scripts = ['ultrasync = ultrasync.cli:main']
 
 setup(
     name='ultrasync',
-    version='0.9.8',
+    version='0.9.9',
     description='Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync '
                 'ZeroWire',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/caronc/ultrasync',
     keywords='XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire '
```

### Comparing `ultrasync-0.9.8/tests/test_cli.py` & `ultrasync-0.9.9/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 from importlib import reload
 import requests
 from os.path import join
 from os.path import dirname
 from click.testing import CliRunner
 from ultrasync import cli
 from ultrasync.common import NX595EVendor
```

### Comparing `ultrasync-0.9.8/tests/test_comnav_0_106.py` & `ultrasync-0.9.9/tests/test_comnav_0_106.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
 
@@ -83,16 +83,23 @@
     ast_obj = mock.Mock()
 
     # Simulate initial area status fetch configuration
     with open(join(ULTRASYNC_TEST_VAR_DIR, 'status.xml'), 'rb') as f:
         ast_obj.content = f.read()
     ast_obj.status_code = requests.codes.ok
 
+    # A Control response object (for garage door handling)
+    # At the time, i did not have a sample to work with, so we will use empty
+    # data for now to satisfy tests
+    crobj = mock.Mock()
+    crobj.status_code = requests.codes.ok
+    crobj.content = b''
+
     # Assign our response object to our mocked instance of requests
-    mock_post.side_effect = (arobj, zrobj)
+    mock_post.side_effect = (arobj, zrobj, crobj)
 
     uobj = UltraSync()
 
     # Perform a login which under the hood queries both area.htm and zones.htm
     # (in that order)
     assert uobj.login()
     assert uobj.vendor is NX595EVendor.COMNAV
@@ -135,19 +142,21 @@
         assert uobj.zones[entry['bank']]['name'] == entry['name']
         assert uobj.zones[entry['bank']]['sequence'] == 1
         assert uobj.zones[entry['bank']]['status'] == \
             entry.get('status', 'Ready')
         assert uobj.zones[entry['bank']]['can_bypass'] is True
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
-    assert mock_post.call_count == 2
+    assert mock_post.call_count == 3
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
+    assert mock_post.call_args_list[2][0][0] == \
+        'http://zerowire/user/outputs.htm'
 
     # Reset our mock object
     mock_post.reset_mock()
 
     # Update our side effects
     mock_post.side_effect = (seq_obj, ast_obj, zst_obj)
```

### Comparing `ultrasync-0.9.8/tests/test_comnav_0_108-zone-check.py` & `ultrasync-0.9.9/tests/test_comnav_0_108-zone-check.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
 
@@ -83,16 +83,23 @@
     ast_obj = mock.Mock()
 
     # Simulate initial area status fetch configuration
     with open(join(ULTRASYNC_TEST_VAR_DIR, 'status.xml'), 'rb') as f:
         ast_obj.content = f.read()
     ast_obj.status_code = requests.codes.ok
 
+    # A Control response object (for garage door handling)
+    # At the time, i did not have a sample to work with, so we will use empty
+    # data for now to satisfy tests
+    crobj = mock.Mock()
+    crobj.status_code = requests.codes.ok
+    crobj.content = b''
+
     # Assign our response object to our mocked instance of requests
-    mock_post.side_effect = (arobj, zrobj)
+    mock_post.side_effect = (arobj, zrobj, crobj)
 
     uobj = UltraSync()
 
     # Perform a login which under the hood queries both area.htm and zones.htm
     # (in that order)
     assert uobj.login()
     assert uobj.vendor is NX595EVendor.COMNAV
@@ -114,19 +121,21 @@
 
     assert isinstance(uobj.zones, dict)
     # our total zones defined (we want to be sure we don't
     # include the '%2D' or '-')
     assert len(uobj.zones) == 17
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
-    assert mock_post.call_count == 2
+    assert mock_post.call_count == 3
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
+    assert mock_post.call_args_list[2][0][0] == \
+        'http://zerowire/user/outputs.htm'
 
     # Reset our mock object
     mock_post.reset_mock()
 
     # Update our side effects
     mock_post.side_effect = (seq_obj, ast_obj, zst_obj)
```

### Comparing `ultrasync-0.9.8/tests/test_comnav_0_108.py` & `ultrasync-0.9.9/tests/test_comnav_0_108.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
 
@@ -83,16 +83,23 @@
     ast_obj = mock.Mock()
 
     # Simulate initial area status fetch configuration
     with open(join(ULTRASYNC_TEST_VAR_DIR, 'status.xml'), 'rb') as f:
         ast_obj.content = f.read()
     ast_obj.status_code = requests.codes.ok
 
+    # A Control response object (for garage door handling)
+    # At the time, i did not have a sample to work with, so we will use empty
+    # data for now to satisfy tests
+    crobj = mock.Mock()
+    crobj.status_code = requests.codes.ok
+    crobj.content = b''
+
     # Assign our response object to our mocked instance of requests
-    mock_post.side_effect = (arobj, zrobj)
+    mock_post.side_effect = (arobj, zrobj, crobj)
 
     uobj = UltraSync()
 
     # Perform a login which under the hood queries both area.htm and zones.htm
     # (in that order)
     assert uobj.login()
     assert uobj.vendor is NX595EVendor.COMNAV
@@ -134,19 +141,21 @@
         assert uobj.zones[entry['bank']]['name'] == entry['name']
         assert uobj.zones[entry['bank']]['sequence'] == 1
         assert uobj.zones[entry['bank']]['status'] == \
             entry.get('status', 'Ready')
         assert uobj.zones[entry['bank']]['can_bypass'] is True
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
-    assert mock_post.call_count == 2
+    assert mock_post.call_count == 3
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
+    assert mock_post.call_args_list[2][0][0] == \
+        'http://zerowire/user/outputs.htm'
 
     # Reset our mock object
     mock_post.reset_mock()
 
     # Update our side effects
     mock_post.side_effect = (seq_obj, ast_obj, zst_obj)
```

### Comparing `ultrasync-0.9.8/tests/test_comnav_0_108_burglar_alarm_on.py` & `ultrasync-0.9.9/tests/test_comnav_0_108_burglar_alarm_on.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
 
@@ -83,16 +83,23 @@
     ast_obj = mock.Mock()
 
     # Simulate initial area status fetch configuration
     with open(join(ULTRASYNC_TEST_VAR_DIR, 'status.xml'), 'rb') as f:
         ast_obj.content = f.read()
     ast_obj.status_code = requests.codes.ok
 
+    # A Control response object (for garage door handling)
+    # At the time, i did not have a sample to work with, so we will use empty
+    # data for now to satisfy tests
+    crobj = mock.Mock()
+    crobj.status_code = requests.codes.ok
+    crobj.content = b''
+
     # Assign our response object to our mocked instance of requests
-    mock_post.side_effect = (arobj, zrobj)
+    mock_post.side_effect = (arobj, zrobj, crobj)
 
     uobj = UltraSync()
 
     # Perform a login which under the hood queries both area.htm and zones.htm
     # (in that order)
     assert uobj.login()
     assert uobj.vendor is NX595EVendor.COMNAV
@@ -134,12 +141,14 @@
         assert uobj.zones[entry['bank']]['name'] == entry['name']
         assert uobj.zones[entry['bank']]['sequence'] == 1
         assert uobj.zones[entry['bank']]['status'] == \
             entry.get('status', 'Ready')
         assert uobj.zones[entry['bank']]['can_bypass'] is True
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
-    assert mock_post.call_count == 2
+    assert mock_post.call_count == 3
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
+    assert mock_post.call_args_list[2][0][0] == \
+        'http://zerowire/user/outputs.htm'
```

### Comparing `ultrasync-0.9.8/tests/test_config.py` & `ultrasync-0.9.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/test_xgen8_bypass.py` & `ultrasync-0.9.9/tests/test_xgen8_bypass.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
```

### Comparing `ultrasync-0.9.8/tests/test_xgen8_nxg8zbo.py` & `ultrasync-0.9.9/tests/test_xgen8_nxg8zbo.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
```

### Comparing `ultrasync-0.9.8/tests/test_xgen_general.py` & `ultrasync-0.9.9/tests/test_xgen_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
```

### Comparing `ultrasync-0.9.8/tests/test_zerowire_armed.py` & `ultrasync-0.9.9/tests/test_zerowire_armed.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
```

### Comparing `ultrasync-0.9.8/tests/test_zerowire_general.py` & `ultrasync-0.9.9/tests/test_zerowire_general.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import mock
+from unittest import mock
 import requests
 from os.path import join
 from os.path import dirname
 
 from ultrasync import UltraSync
 from ultrasync.common import NX595EVendor
```

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.106/area.htm` & `ultrasync-0.9.9/tests/var/comnav/0.106/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.106/master.js` & `ultrasync-0.9.9/tests/var/comnav/0.106/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.106/status.js` & `ultrasync-0.9.9/tests/var/comnav/0.106/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.106/zones.htm` & `ultrasync-0.9.9/tests/var/comnav/0.106/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108/area.htm` & `ultrasync-0.9.9/tests/var/comnav/0.108/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108/master.js` & `ultrasync-0.9.9/tests/var/comnav/0.108/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108/status.js` & `ultrasync-0.9.9/tests/var/comnav/0.108/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108/zones.htm` & `ultrasync-0.9.9/tests/var/comnav/0.108/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/area.htm` & `ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/master.js` & `ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/status.js` & `ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108-burglar-alarm-on/zones.htm` & `ultrasync-0.9.9/tests/var/comnav/0.108-burglar-alarm-on/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/area.htm` & `ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/comnav/0.108-zone-test/zones.htm` & `ultrasync-0.9.9/tests/var/comnav/0.108-zone-test/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen/general/area.htm` & `ultrasync-0.9.9/tests/var/xgen/general/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen/general/master.js` & `ultrasync-0.9.9/tests/var/xgen/general/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen/general/status.js` & `ultrasync-0.9.9/tests/var/xgen/general/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen/general/zones.htm` & `ultrasync-0.9.9/tests/var/xgen/general/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen8/bypass/area.htm` & `ultrasync-0.9.9/tests/var/xgen8/bypass/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen8/bypass/zones.htm` & `ultrasync-0.9.9/tests/var/xgen8/bypass/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/area.htm` & `ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/status.json` & `ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/status.json`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/xgen8/nxg8zbo/zones.htm` & `ultrasync-0.9.9/tests/var/xgen8/nxg8zbo/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/zerowire/armed/area.htm` & `ultrasync-0.9.9/tests/var/zerowire/armed/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/zerowire/armed/zones.htm` & `ultrasync-0.9.9/tests/var/zerowire/armed/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/zerowire/general/area.htm` & `ultrasync-0.9.9/tests/var/zerowire/general/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/tests/var/zerowire/general/zones.htm` & `ultrasync-0.9.9/tests/var/zerowire/general/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/ultrasync/__init__.py` & `ultrasync-0.9.9/ultrasync/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 __title__ = 'ultrasync'
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 __author__ = 'Chris Caron'
 __license__ = 'MIT'
 __copywrite__ = 'Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>'
 __email__ = 'lead2gold@gmail.com'
 __status__ = 'Production'
 
 from .main import UltraSync
```

### Comparing `ultrasync-0.9.8/ultrasync/cli.py` & `ultrasync-0.9.9/ultrasync/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,26 +101,32 @@
 @click.option('--area', '-a', default=0, type=int, metavar='AREA',
               help='Specify the Area you wish to target with a --scene (-s) '
               'action. If no area is specified, then *all* areas are '
               'targeted.')
 @click.option('--zone', type=int, metavar='ZONE',
               help='Specify the Zone you wish to target with a --bypass '
               'action.')
+@click.option('--output', type=int, metavar='OUTPUT',
+              help='Specify the Output you wish to control with a '
+              '--switch action.')
+@click.option('--switch', type=int,
+              metavar='STATE',
+              help='Set to 1 to turn on an output, set to 0 to turn it off.')
 @click.option('--full-debug-dump', is_flag=True,
               help='Dump a full set of tracing files to a archive for '
               'comparison/debug purposes. Usually the --debug-dump is '
               'satisfactory enough.')
 @click.option('--debug-dump', is_flag=True,
               help='Dump tracing files to a archive for comparison/debug '
               'purposes.')
 @click.option('--verbose', '-v', count=True)
 @click.option('--version', '-V', is_flag=True,
               help='Display the version of the ultrasync library and exit.')
 def main(config, debug_dump, full_debug_dump, scene, bypass, details, watch,
-         area, zone, verbose, version):
+         area, zone, output, switch, verbose, version):
     """
     Wrapper to ultrasync library.
     """
     # Note: Click ignores the return values of functions it wraps, If you
     #       want to return a specific error code, you must call sys.exit()
     #       as you will see below.
 
@@ -198,14 +204,22 @@
         actioned = True
 
     if bypass is not None:
         if not usync.set_zone_bypass(zone=zone, state=bypass):
             sys.exit(1)
         actioned = True
 
+    if output is not None and switch is not None:
+        if switch not in (0, 1):
+            logger.error('Switch state should be either 0 or 1')
+            sys.exit(1)
+        if not usync.set_output_control(output=output, state=switch):
+            sys.exit(1)
+        actioned = True
+
     if watch:
         area_delta = {}
         zone_delta = {}
         while True:
             # Get our details
             results = usync.details()
             if not results:
```

### Comparing `ultrasync-0.9.8/ultrasync/common.py` & `ultrasync-0.9.9/ultrasync/common.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/ultrasync/config.py` & `ultrasync-0.9.9/ultrasync/config.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/ultrasync/logger.py` & `ultrasync-0.9.9/ultrasync/logger.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.8/ultrasync/main.py` & `ultrasync-0.9.9/ultrasync/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,17 @@
         # Virtual bank for tracking individual sensor
         self._zvbank = {}
 
         # Our areas get populated after we connect
         self.areas = {}
         self._asequence = None
 
+        # Our output controls get populated after we connect
+        self.outputs = {}
+
         # Track the time our information was polled from our panel
         self.__updated = None
 
         # Track the Panel URL path
         self.__panel_url_path = None
 
     def login(self):
@@ -219,14 +222,17 @@
         ))
 
         if not self._areas(response=response) or not self._zones():
             # No match and/or bad login
             logger.error('Failed to authenticate to {}'.format(self.host))
             return False
 
+        # Prepare output control (if supported)
+        self.output_control()
+
         # Update our time reference
         self.__updated = datetime.now()
 
         # We're good
         return True if self.session_id else False
 
     def logout(self):
@@ -275,14 +281,19 @@
             },
 
             # Zones URL
             'zones.htm': {
                 'path': '/user/zones.htm',
             },
 
+            # Output Control URL
+            'outputs.htm': {
+                'path': '/user/outputs.htm',
+            },
+
             # Config Main Screen
             'config2.htm': {
                 'path': '/muser/config2.htm',
             },
 
             # Additional useful queries
             'master.js': {
@@ -590,54 +601,53 @@
 
         # Start our payload off with our session identifier
         payload = {
             'sess': self.session_id,
         }
 
         if self.vendor in (NX595EVendor.ZEROWIRE, NX595EVendor.XGEN8):
-                payload.update({
+            payload.update({
                 'cmd': 5,
                 'opt': int(state),
                 'zone': zone - 1,
             })
-            
-                # Send our response
-                response = self.__get(
-                    '/user/zonefunction.cgi', payload=payload)
+
+            # Send our response
+            response = self.__get(
+                '/user/zonefunction.cgi', payload=payload)
 
         elif self.vendor in (NX595EVendor.COMNAV):
             # Call comnav_process_zones to update can_bypass attribute
             self.comnav_process_zones
 
             # Get the current can_bypass state of the zone
             can_bypass = self.zones[zone - 1]['can_bypass']
 
-            # If the current can_bypass state does not match the desired bypass state,
-            # toggle the bypass state
+            # If the current can_bypass state does not match the desired
+            # bypass state, toggle the bypass state
             if can_bypass == state:
                 # Start our payload off with our session identifier
                 payload = {
                     'sess': self.session_id,
                     'comm': 82,
                     'data0': zone - 1,
                 }
-            else: 
+            else:
                 payload = {}
 
             # Send our response
             response = self.__get(
                 '/user/zonefunction.cgi', payload=payload)
- 
+
         else:   # self.vendor is NX595EVendor.{ZEROWIRE, XGEN}
 
             logger.error(
                 'Bypass not implemented for vendor {}'.format(self.vendor))
             return False
 
-
         if not response:
             logger.info(
                 'Failed to set bypass={} for zone {}'.format(state, zone))
             has_error = True
 
         logger.info(
             'Set bypass={} for zone {} Successfully'.format(state, zone))
@@ -668,27 +678,28 @@
 
         # Update our time reference
         self.__updated = datetime.now()
         return True
 
     def details(self, max_age_sec=1):
         """
-        Arranges the areas and zones into an easy to manage dictionary
+        Arranges the areas, zones and outputs into an easy to manage dictionary
         """
         if not self.update(max_age_sec=max_age_sec):
             return {}
 
         # Build our response object
         response = {
             'user': {
                 'is_installer': self.__is_installer,
                 'is_master': self.__is_master,
             },
             'zones': [z for z in self.zones.values()],
             'areas': [a for a in self.areas.values()],
+            'outputs': [o for o in self.outputs.values()],
             'date': self.__updated.strftime('%Y-%m-%d %H:%M:%S'),
         }
 
         return response
 
     def _areas(self, response=None):
         """
@@ -2087,14 +2098,105 @@
 
         except AttributeError:
             # <zdat> stanza was not found
             return None
 
         return response
 
+    def output_control(self):
+        """
+        Parses the Output Control from the UltraSync panel
+
+        At this time, this feature is only supported by the COMNAV panels
+        """
+
+        if self.vendor is not NX595EVendor.COMNAV:
+            # Only vendor that supports this right now is COMNAV
+            # Silently returned a positive status
+            return True
+
+        if not self.session_id and not self.login():
+            return False
+
+        logger.info('Retrieving initial Output Control information.')
+
+        # Perform our Query
+        response = self.__get('/user/outputs.htm', rtype=HubResponseType.RAW)
+        if not response:
+            return False
+
+            # Regex to capture output names and states
+            name_pattern = re.compile(
+                r'var oname(\d) = decodeURIComponent'
+                r'\(decode_utf8\("([^"]*)"\)\);')
+            state_pattern = re.compile(r'var ostate(\d) = "(\d)";')
+
+            # Extract names and states
+            names = {int(m.group(1)): unquote(m.group(2))
+                     for m in name_pattern.finditer(response)}
+            states = {int(m.group(1)): m.group(2)
+                      for m in state_pattern.finditer(response)}
+
+            # Store our outputs:
+            for i in range(1, max(len(names), len(states)) + 1):
+                self.outputs[i] = {
+                    'name': names.get(i, ''),
+                    'state': states.get(i, '0'),
+                }
+            return False
+
+        return True
+
+    def set_output_control(self, output, state):
+        """
+        Sets output control on/off
+
+        At this time, this feature is only supported by the COMNAV panels
+        """
+        if self.vendor is not NX595EVendor.COMNAV:
+            # Only vendor that supports this right now is COMNAV
+            logger.error(
+                'Output control not implemented for vendor {}'.format(
+                    self.vendor))
+            return False
+
+        if not self.session_id and not self.login():
+            return False
+
+        if not isinstance(output, int) or output not in self.outputs.keys():
+            logger.error(
+                '{} is not valid output'.format(output))
+            return False
+
+        # A boolean for tracking any errors
+        has_error = False
+
+        # Start our payload off with our session identifier
+        payload = {
+            'sess': self.session_id,
+        }
+
+        # Update payload with variables
+        payload.update({
+            'onum': output,
+            'ostate': state
+        })
+
+        # Send our response
+        response = self.__get('/user/output.cgi', payload=payload)
+        if not response:
+            logger.info(
+                'Failed to set state={} for output {}'.format(state, output))
+            has_error = True
+
+        logger.info(
+            'Set state={} for output {} successfully'.format(state, output))
+
+        return not has_error
+
     def _sequence(self):
         """
         Returns the sequences for both the zones, entries, and areas
         """
         return getattr(self, '_{}_sequence'.format(self.vendor))()
 
     def _zerowire_sequence(self):
```

### Comparing `ultrasync-0.9.8/ultrasync.egg-info/PKG-INFO` & `ultrasync-0.9.9/ultrasync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultrasync
-Version: 0.9.8
+Version: 0.9.9
 Summary: Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync ZeroWire
 Home-page: https://github.com/caronc/ultrasync
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: MIT
 Keywords: XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire Security Panel
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,24 +17,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# NX-595E Output Control Fork
+This fork is designated to implementing the "Output Control" section of the NX-595E. The main objective is to enable communication with the outputs and ensure its proper implementation.
+
 # NX-595E UltraSync Hub
 
 Compatible with both NX-595E [Hills](https://www.hills.com.au/) ComNav, xGen, xGen8 (such as [NXG-8-Z-BO](https://firesecurityproducts.com/en/product/intrusion/NXG_8_Z_BO/82651)), [Interlogix](https://www.interlogix.com/), and [ZeroWire](https://www.interlogix.com/intrusion/product/ultrasync-selfcontained-hub) UltraSync solutions.
 
 ![ZeroWire Hub Image](https://raw.githubusercontent.com/caronc/ultrasync/master/static/zerowire_hub.jpeg)
 
 [![Paypal](https://img.shields.io/badge/paypal-donate-green.svg)](https://paypal.me/lead2gold?locale.x=en_US)
 [![Follow](https://img.shields.io/twitter/follow/l2gnux)](https://twitter.com/l2gnux/)<br/>
 [![Python](https://img.shields.io/pypi/pyversions/ultrasync.svg?style=flat-square)](https://pypi.org/project/ultrasync/)
-[![Build Status](https://travis-ci.org/caronc/ultrasync.svg?branch=master)](https://travis-ci.org/caronc/ultrasync)
+[![Build Status](https://github.com/caronc/ultrasync/actions/workflows/tests.yml/badge.svg)](https://github.com/caronc/ultrasync/actions/workflows/tests.yml)
 [![CodeCov Status](https://codecov.io/github/caronc/ultrasync/branch/master/graph/badge.svg)](https://codecov.io/github/caronc/ultrasync)
 [![Downloads](http://pepy.tech/badge/ultrasync)](https://pypi.org/project/ultrasync/)
 
 ## How Does It Work?
 
 1. First you need to install it; this part is easy:
```

### Comparing `ultrasync-0.9.8/ultrasync.egg-info/SOURCES.txt` & `ultrasync-0.9.9/ultrasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*


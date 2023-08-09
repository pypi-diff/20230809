# Comparing `tmp/appPublic-5.1.8.tar.gz` & `tmp/appPublic-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appPublic-5.1.8.tar", last modified: Tue May 10 09:53:00 2022, max compression
+gzip compressed data, was "appPublic-5.1.9.tar", last modified: Thu Jun  9 07:40:35 2022, max compression
```

## Comparing `appPublic-5.1.8.tar` & `appPublic-5.1.9.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-05-10 09:53:00.945156 appPublic-5.1.8/
--rw-r--r--   0 ymq        (501) admin       (80)      400 2022-05-10 09:53:00.944522 appPublic-5.1.8/PKG-INFO
--rwxr-xr-x   0 ymq        (501) admin       (80)       61 2022-03-05 09:04:03.000000 appPublic-5.1.8/README.md
-drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-05-10 09:53:00.939747 appPublic-5.1.8/appPublic/
--rw-r--r--   0 ymq        (501) admin       (80)     1434 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/CSVData.py
--rw-r--r--   0 ymq        (501) admin       (80)     1038 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/Config.py
--rw-r--r--   0 ymq        (501) admin       (80)     2372 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/ExecFile.py
--rw-r--r--   0 ymq        (501) admin       (80)     1179 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/FiniteStateMachine.py
--rw-r--r--   0 ymq        (501) admin       (80)     3269 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/MiniI18N.py
--rw-r--r--   0 ymq        (501) admin       (80)     1165 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/ObjectCache.py
--rw-r--r--   0 ymq        (501) admin       (80)     2444 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/RSAutils.py
--rw-r--r--   0 ymq        (501) admin       (80)     4732 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/SQLite3Utils.py
--rw-r--r--   0 ymq        (501) admin       (80)      874 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/Singleton.py
--rw-r--r--   0 ymq        (501) admin       (80)        0 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/__init__.py
--rw-r--r--   0 ymq        (501) admin       (80)     2977 2022-03-05 14:55:14.000000 appPublic-5.1.8/appPublic/across_nat.bak.py
--rw-r--r--   0 ymq        (501) admin       (80)     3101 2022-05-10 08:30:43.000000 appPublic-5.1.8/appPublic/across_nat.py
--rw-r--r--   0 ymq        (501) admin       (80)     1126 2022-04-06 02:18:50.000000 appPublic-5.1.8/appPublic/app_logger.py
--rw-r--r--   0 ymq        (501) admin       (80)     5071 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/argsConvert.py
--rw-r--r--   0 ymq        (501) admin       (80)      246 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/background.py
--rw-r--r--   0 ymq        (501) admin       (80)     1139 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/csv_Data.py
--rw-r--r--   0 ymq        (501) admin       (80)     4400 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/dataencoder.py
--rw-r--r--   0 ymq        (501) admin       (80)      841 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/datamapping.py
--rw-r--r--   0 ymq        (501) admin       (80)      686 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/dictExt.py
--rw-r--r--   0 ymq        (501) admin       (80)     3528 2022-03-07 11:47:30.000000 appPublic-5.1.8/appPublic/dictObject.old.py
--rw-r--r--   0 ymq        (501) admin       (80)     3528 2022-03-07 11:54:08.000000 appPublic-5.1.8/appPublic/dictObject.py
--rw-r--r--   0 ymq        (501) admin       (80)     2362 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/easyExcel.py
--rw-r--r--   0 ymq        (501) admin       (80)     8044 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/exceldata.py
--rw-r--r--   0 ymq        (501) admin       (80)     4330 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/excelwriter.py
--rw-r--r--   0 ymq        (501) admin       (80)     1560 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/find_player.py
--rw-r--r--   0 ymq        (501) admin       (80)     4674 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/folderUtils.py
--rw-r--r--   0 ymq        (501) admin       (80)     1047 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/genetic.py
--rw-r--r--   0 ymq        (501) admin       (80)     2874 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/http_client.py
--rw-r--r--   0 ymq        (501) admin       (80)     2135 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/httpclient.py
--rw-r--r--   0 ymq        (501) admin       (80)     3562 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/i18n.py
--rw-r--r--   0 ymq        (501) admin       (80)     1577 2022-05-09 10:23:18.000000 appPublic-5.1.8/appPublic/iplocation.py
--rw-r--r--   0 ymq        (501) admin       (80)     1651 2022-03-11 08:22:46.000000 appPublic-5.1.8/appPublic/jsonConfig.py
--rw-r--r--   0 ymq        (501) admin       (80)     1005 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/jsonIO.py
--rw-r--r--   0 ymq        (501) admin       (80)     1050 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/localefunc.py
--rw-r--r--   0 ymq        (501) admin       (80)     1003 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/macAddress.py
--rw-r--r--   0 ymq        (501) admin       (80)      184 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/myImport.py
--rw-r--r--   0 ymq        (501) admin       (80)     1996 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/myTE.py
--rw-r--r--   0 ymq        (501) admin       (80)      304 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/myjson.py
--rw-r--r--   0 ymq        (501) admin       (80)     2024 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/mylog.py
--rw-r--r--   0 ymq        (501) admin       (80)     1268 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/objectAction.py
--rw-r--r--   0 ymq        (501) admin       (80)      286 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/pickleUtils.py
--rwxr-xr-x   0 ymq        (501) admin       (80)      866 2022-04-22 05:36:03.000000 appPublic-5.1.8/appPublic/process_workers.py
--rw-r--r--   0 ymq        (501) admin       (80)     4723 2022-03-18 15:07:55.000000 appPublic-5.1.8/appPublic/rc4.py
--rw-r--r--   0 ymq        (501) admin       (80)     2794 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/receiveMail.py
--rw-r--r--   0 ymq        (501) admin       (80)      750 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/registerfunction.py
--rw-r--r--   0 ymq        (501) admin       (80)      779 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/restrictedEnv.py
--rw-r--r--   0 ymq        (501) admin       (80)     5087 2022-03-17 08:07:49.000000 appPublic-5.1.8/appPublic/rsa.py
--rw-r--r--   0 ymq        (501) admin       (80)     2906 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/rsaPeer.py
--rw-r--r--   0 ymq        (501) admin       (80)     3109 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/sockPackage.py
--rw-r--r--   0 ymq        (501) admin       (80)      300 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/strUtils.py
--rw-r--r--   0 ymq        (501) admin       (80)      143 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/testdict.py
--rw-r--r--   0 ymq        (501) admin       (80)      878 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/thread_workers.py
--rw-r--r--   0 ymq        (501) admin       (80)     3990 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/timeUtils.py
--rw-r--r--   0 ymq        (501) admin       (80)      660 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/timecost.py
--rw-r--r--   0 ymq        (501) admin       (80)     1346 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/tworkers.py
--rw-r--r--   0 ymq        (501) admin       (80)     2036 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/udp_comm.py
--rw-r--r--   0 ymq        (501) admin       (80)      773 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/unicoding.py
--rw-r--r--   0 ymq        (501) admin       (80)      130 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/uniqueID.py
--rw-r--r--   0 ymq        (501) admin       (80)     1019 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/worker.py
--rwxr-xr-x   0 ymq        (501) admin       (80)     3359 2022-03-09 08:18:25.000000 appPublic-5.1.8/appPublic/zmq_reqrep.py
--rw-r--r--   0 ymq        (501) admin       (80)     3652 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/zmq_topic.py
--rw-r--r--   0 ymq        (501) admin       (80)     4178 2022-03-05 09:04:03.000000 appPublic-5.1.8/appPublic/zmqapi.py
-drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-05-10 09:53:00.942016 appPublic-5.1.8/appPublic.egg-info/
--rw-r--r--   0 ymq        (501) admin       (80)      400 2022-05-10 09:53:00.000000 appPublic-5.1.8/appPublic.egg-info/PKG-INFO
--rw-r--r--   0 ymq        (501) admin       (80)     1639 2022-05-10 09:53:00.000000 appPublic-5.1.8/appPublic.egg-info/SOURCES.txt
--rw-r--r--   0 ymq        (501) admin       (80)        1 2022-05-10 09:53:00.000000 appPublic-5.1.8/appPublic.egg-info/dependency_links.txt
--rw-r--r--   0 ymq        (501) admin       (80)       10 2022-05-10 09:53:00.000000 appPublic-5.1.8/appPublic.egg-info/top_level.txt
--rw-r--r--   0 ymq        (501) admin       (80)       38 2022-05-10 09:53:00.945411 appPublic-5.1.8/setup.cfg
--rwxr-xr-x   0 ymq        (501) admin       (80)      976 2022-05-10 09:52:22.000000 appPublic-5.1.8/setup.py
-drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-05-10 09:53:00.943496 appPublic-5.1.8/test/
--rw-r--r--   0 ymq        (501) admin       (80)      400 2022-03-05 09:04:03.000000 appPublic-5.1.8/test/test_across_nat.py
--rw-r--r--   0 ymq        (501) admin       (80)      760 2022-03-05 09:04:03.000000 appPublic-5.1.8/test/test_aioupnp.py
+drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-06-09 07:40:35.388533 appPublic-5.1.9/
+-rw-r--r--   0 ymq        (501) admin       (80)      400 2022-06-09 07:40:35.388168 appPublic-5.1.9/PKG-INFO
+-rwxr-xr-x   0 ymq        (501) admin       (80)       61 2022-03-05 09:04:03.000000 appPublic-5.1.9/README.md
+drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-06-09 07:40:35.383907 appPublic-5.1.9/appPublic/
+-rw-r--r--   0 ymq        (501) admin       (80)     1434 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/CSVData.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1038 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/Config.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2384 2022-05-20 07:27:40.000000 appPublic-5.1.9/appPublic/ExecFile.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1179 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/FiniteStateMachine.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3269 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/MiniI18N.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1165 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/ObjectCache.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2444 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/RSAutils.py
+-rw-r--r--   0 ymq        (501) admin       (80)     4732 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/SQLite3Utils.py
+-rw-r--r--   0 ymq        (501) admin       (80)      874 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/Singleton.py
+-rw-r--r--   0 ymq        (501) admin       (80)       33 2022-06-09 04:58:35.000000 appPublic-5.1.9/appPublic/__init__.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2977 2022-03-05 14:55:14.000000 appPublic-5.1.9/appPublic/across_nat.bak.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3101 2022-05-10 08:30:43.000000 appPublic-5.1.9/appPublic/across_nat.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1126 2022-04-06 02:18:50.000000 appPublic-5.1.9/appPublic/app_logger.py
+-rw-r--r--   0 ymq        (501) admin       (80)     5071 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/argsConvert.py
+-rw-r--r--   0 ymq        (501) admin       (80)      246 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/background.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1139 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/csv_Data.py
+-rw-r--r--   0 ymq        (501) admin       (80)     4400 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/dataencoder.py
+-rw-r--r--   0 ymq        (501) admin       (80)      841 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/datamapping.py
+-rw-r--r--   0 ymq        (501) admin       (80)      686 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/dictExt.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3528 2022-03-07 11:47:30.000000 appPublic-5.1.9/appPublic/dictObject.old.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3528 2022-03-07 11:54:08.000000 appPublic-5.1.9/appPublic/dictObject.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2362 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/easyExcel.py
+-rw-r--r--   0 ymq        (501) admin       (80)     8044 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/exceldata.py
+-rw-r--r--   0 ymq        (501) admin       (80)     4330 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/excelwriter.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1560 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/find_player.py
+-rw-r--r--   0 ymq        (501) admin       (80)     4674 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/folderUtils.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1047 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/genetic.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3071 2022-05-16 02:42:09.000000 appPublic-5.1.9/appPublic/http_client.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2135 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/httpclient.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3592 2022-05-20 12:04:48.000000 appPublic-5.1.9/appPublic/i18n.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1577 2022-05-09 10:23:18.000000 appPublic-5.1.9/appPublic/iplocation.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1651 2022-03-11 08:22:46.000000 appPublic-5.1.9/appPublic/jsonConfig.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1005 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/jsonIO.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1050 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/localefunc.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1003 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/macAddress.py
+-rw-r--r--   0 ymq        (501) admin       (80)      184 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/myImport.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1996 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/myTE.py
+-rw-r--r--   0 ymq        (501) admin       (80)      304 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/myjson.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2024 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/mylog.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1268 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/objectAction.py
+-rw-r--r--   0 ymq        (501) admin       (80)      286 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/pickleUtils.py
+-rwxr-xr-x   0 ymq        (501) admin       (80)      866 2022-04-22 05:36:03.000000 appPublic-5.1.9/appPublic/process_workers.py
+-rw-r--r--   0 ymq        (501) admin       (80)     4719 2022-06-07 05:59:58.000000 appPublic-5.1.9/appPublic/rc4.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2794 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/receiveMail.py
+-rw-r--r--   0 ymq        (501) admin       (80)      750 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/registerfunction.py
+-rw-r--r--   0 ymq        (501) admin       (80)      779 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/restrictedEnv.py
+-rw-r--r--   0 ymq        (501) admin       (80)     5087 2022-03-17 08:07:49.000000 appPublic-5.1.9/appPublic/rsa.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2906 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/rsaPeer.py
+-rw-r--r--   0 ymq        (501) admin       (80)      527 2022-06-09 04:44:57.000000 appPublic-5.1.9/appPublic/set_fgcolor.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3109 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/sockPackage.py
+-rw-r--r--   0 ymq        (501) admin       (80)      300 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/strUtils.py
+-rw-r--r--   0 ymq        (501) admin       (80)      143 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/testdict.py
+-rw-r--r--   0 ymq        (501) admin       (80)      878 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/thread_workers.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3990 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/timeUtils.py
+-rw-r--r--   0 ymq        (501) admin       (80)      660 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/timecost.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1346 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/tworkers.py
+-rw-r--r--   0 ymq        (501) admin       (80)     2036 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/udp_comm.py
+-rw-r--r--   0 ymq        (501) admin       (80)      773 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/unicoding.py
+-rw-r--r--   0 ymq        (501) admin       (80)      130 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/uniqueID.py
+-rw-r--r--   0 ymq        (501) admin       (80)       22 2022-06-09 04:58:00.000000 appPublic-5.1.9/appPublic/version.py
+-rw-r--r--   0 ymq        (501) admin       (80)     1019 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/worker.py
+-rwxr-xr-x   0 ymq        (501) admin       (80)     3359 2022-03-09 08:18:25.000000 appPublic-5.1.9/appPublic/zmq_reqrep.py
+-rw-r--r--   0 ymq        (501) admin       (80)     3652 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/zmq_topic.py
+-rw-r--r--   0 ymq        (501) admin       (80)     4178 2022-03-05 09:04:03.000000 appPublic-5.1.9/appPublic/zmqapi.py
+drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-06-09 07:40:35.386052 appPublic-5.1.9/appPublic.egg-info/
+-rw-r--r--   0 ymq        (501) admin       (80)      400 2022-06-09 07:40:34.000000 appPublic-5.1.9/appPublic.egg-info/PKG-INFO
+-rw-r--r--   0 ymq        (501) admin       (80)     1685 2022-06-09 07:40:35.000000 appPublic-5.1.9/appPublic.egg-info/SOURCES.txt
+-rw-r--r--   0 ymq        (501) admin       (80)        1 2022-06-09 07:40:34.000000 appPublic-5.1.9/appPublic.egg-info/dependency_links.txt
+-rw-r--r--   0 ymq        (501) admin       (80)       10 2022-06-09 07:40:35.000000 appPublic-5.1.9/appPublic.egg-info/top_level.txt
+-rw-r--r--   0 ymq        (501) admin       (80)       38 2022-06-09 07:40:35.388655 appPublic-5.1.9/setup.cfg
+-rwxr-xr-x   0 ymq        (501) admin       (80)     1022 2022-06-09 07:40:00.000000 appPublic-5.1.9/setup.py
+drwxr-xr-x   0 ymq        (501) admin       (80)        0 2022-06-09 07:40:35.387299 appPublic-5.1.9/test/
+-rw-r--r--   0 ymq        (501) admin       (80)      400 2022-03-05 09:04:03.000000 appPublic-5.1.9/test/test_across_nat.py
+-rw-r--r--   0 ymq        (501) admin       (80)      760 2022-03-05 09:04:03.000000 appPublic-5.1.9/test/test_aioupnp.py
```

### Comparing `appPublic-5.1.8/appPublic/CSVData.py` & `appPublic-5.1.9/appPublic/CSVData.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/Config.py` & `appPublic-5.1.9/appPublic/Config.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/ExecFile.py` & `appPublic-5.1.9/appPublic/ExecFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,12 +96,12 @@
 			raise Exception('exec file is none')
 		f = open(self.__file,'r')
 		buf = f.read()
 		f.close()
 		try :
 			exec(buf,globals(),self.__object.__dict__)
 		except Exception as e:
-			print("ExecFile()",e)
+			print("ExecFile()",e,self.__file)
 			return (False,e)
 		return (True,'')
```

### Comparing `appPublic-5.1.8/appPublic/FiniteStateMachine.py` & `appPublic-5.1.9/appPublic/FiniteStateMachine.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/MiniI18N.py` & `appPublic-5.1.9/appPublic/MiniI18N.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/ObjectCache.py` & `appPublic-5.1.9/appPublic/ObjectCache.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/RSAutils.py` & `appPublic-5.1.9/appPublic/RSAutils.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/SQLite3Utils.py` & `appPublic-5.1.9/appPublic/SQLite3Utils.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/Singleton.py` & `appPublic-5.1.9/appPublic/Singleton.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/across_nat.bak.py` & `appPublic-5.1.9/appPublic/across_nat.bak.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/across_nat.py` & `appPublic-5.1.9/appPublic/across_nat.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/app_logger.py` & `appPublic-5.1.9/appPublic/app_logger.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/argsConvert.py` & `appPublic-5.1.9/appPublic/argsConvert.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/csv_Data.py` & `appPublic-5.1.9/appPublic/csv_Data.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/dataencoder.py` & `appPublic-5.1.9/appPublic/dataencoder.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/datamapping.py` & `appPublic-5.1.9/appPublic/datamapping.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/dictExt.py` & `appPublic-5.1.9/appPublic/dictExt.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/dictObject.old.py` & `appPublic-5.1.9/appPublic/dictObject.old.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/dictObject.py` & `appPublic-5.1.9/appPublic/dictObject.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/easyExcel.py` & `appPublic-5.1.9/appPublic/easyExcel.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/exceldata.py` & `appPublic-5.1.9/appPublic/exceldata.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/excelwriter.py` & `appPublic-5.1.9/appPublic/excelwriter.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/find_player.py` & `appPublic-5.1.9/appPublic/find_player.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/folderUtils.py` & `appPublic-5.1.9/appPublic/folderUtils.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/genetic.py` & `appPublic-5.1.9/appPublic/genetic.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/http_client.py` & `appPublic-5.1.9/appPublic/http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 
 hostsessions = {}
 
 class Http_Client:
 	def __init__(self):
 		self.s = requests.Session()
 		self.s.verify = False
+		self.s.hooks['response'].append(self.response_handler)
+
+	def prepped_handler(self, prepped):
+		pass
+
+	def response_handler(self, resp, *args, **kw):
+		return resp
 		
 	def url2domain(self,url):
 		parts = url.split('/')[:3]
 		pre = '/'.join(parts)
 		return pre
 
 	def _webcall(self,url,method="GET",
@@ -43,14 +50,15 @@
 		if method in ['GET']:
 			req = requests.Request(method,url,
 					params=params,headers=headers)
 		else:
 			req = requests.Request(method,url,
 					data=params,files=files,headers=headers)
 		prepped = self.s.prepare_request(req)
+		self.prepped_handler(prepped)
 		resp = self.s.send(prepped)
 		if resp.status_code == 200:
 			h = resp.headers.get('Set-Cookie',None)
 			if h:
 				sessionid = h.split(';')[0]
 				hostsessions[domain] = sessionid
```

### Comparing `appPublic-5.1.8/appPublic/httpclient.py` & `appPublic-5.1.9/appPublic/httpclient.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/i18n.py` & `appPublic-5.1.9/appPublic/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,12 +149,13 @@
 
 	def getCurrentLang(self) :
 		"""
 		"""
 		threadid = threading.currentThread()
 		return self.clientLangs[threadid]['lang']
 
-def getI18N(coding='utf8'):
-	path = ProgramPath()
+def getI18N(path=None, coding='utf8'):
+	if path is None:
+		path = ProgramPath()
 	i18n = MiniI18N(path,coding)
 	return i18n
```

### Comparing `appPublic-5.1.8/appPublic/iplocation.py` & `appPublic-5.1.9/appPublic/iplocation.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/jsonConfig.py` & `appPublic-5.1.9/appPublic/jsonConfig.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/jsonIO.py` & `appPublic-5.1.9/appPublic/jsonIO.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/localefunc.py` & `appPublic-5.1.9/appPublic/localefunc.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/macAddress.py` & `appPublic-5.1.9/appPublic/macAddress.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/myTE.py` & `appPublic-5.1.9/appPublic/myTE.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/mylog.py` & `appPublic-5.1.9/appPublic/mylog.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/objectAction.py` & `appPublic-5.1.9/appPublic/objectAction.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/process_workers.py` & `appPublic-5.1.9/appPublic/process_workers.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/rc4.py` & `appPublic-5.1.9/appPublic/rc4.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 	def is_near_bottom(self, indicator=None):
 		ts = self.get_timestamp()
 		i = indicator
 		if i is None:
 			i = self.get_indicator(ts)
 		if i + self.threshold > ts:
 			return True
-		return FalseTrue
+		return False
 
 	def is_near_top(self, indicator=None):
 		ts = self.get_timestamp()
 		i = indicator
 		if i is None:
 			i = self.get_indicator(ts)
 		if i + self.period - self.threshold < ts:
```

### Comparing `appPublic-5.1.8/appPublic/receiveMail.py` & `appPublic-5.1.9/appPublic/receiveMail.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/registerfunction.py` & `appPublic-5.1.9/appPublic/registerfunction.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/restrictedEnv.py` & `appPublic-5.1.9/appPublic/restrictedEnv.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/rsa.py` & `appPublic-5.1.9/appPublic/rsa.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/rsaPeer.py` & `appPublic-5.1.9/appPublic/rsaPeer.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/sockPackage.py` & `appPublic-5.1.9/appPublic/sockPackage.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/thread_workers.py` & `appPublic-5.1.9/appPublic/thread_workers.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/timeUtils.py` & `appPublic-5.1.9/appPublic/timeUtils.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/timecost.py` & `appPublic-5.1.9/appPublic/timecost.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/tworkers.py` & `appPublic-5.1.9/appPublic/tworkers.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/udp_comm.py` & `appPublic-5.1.9/appPublic/udp_comm.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/unicoding.py` & `appPublic-5.1.9/appPublic/unicoding.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/worker.py` & `appPublic-5.1.9/appPublic/worker.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/zmq_reqrep.py` & `appPublic-5.1.9/appPublic/zmq_reqrep.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/zmq_topic.py` & `appPublic-5.1.9/appPublic/zmq_topic.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic/zmqapi.py` & `appPublic-5.1.9/appPublic/zmqapi.py`

 * *Files identical despite different names*

### Comparing `appPublic-5.1.8/appPublic.egg-info/SOURCES.txt` & `appPublic-5.1.9/appPublic.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,24 +44,26 @@
 appPublic/process_workers.py
 appPublic/rc4.py
 appPublic/receiveMail.py
 appPublic/registerfunction.py
 appPublic/restrictedEnv.py
 appPublic/rsa.py
 appPublic/rsaPeer.py
+appPublic/set_fgcolor.py
 appPublic/sockPackage.py
 appPublic/strUtils.py
 appPublic/testdict.py
 appPublic/thread_workers.py
 appPublic/timeUtils.py
 appPublic/timecost.py
 appPublic/tworkers.py
 appPublic/udp_comm.py
 appPublic/unicoding.py
 appPublic/uniqueID.py
+appPublic/version.py
 appPublic/worker.py
 appPublic/zmq_reqrep.py
 appPublic/zmq_topic.py
 appPublic/zmqapi.py
 appPublic.egg-info/PKG-INFO
 appPublic.egg-info/SOURCES.txt
 appPublic.egg-info/dependency_links.txt
```

### Comparing `appPublic-5.1.8/setup.py` & `appPublic-5.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
-
+from  appPublic.version import __version__
 try:
 	from setuptools import setup
 except ImportError:
 	from distutils.core import setup
 
 # usage:
 # python setup.py bdist_wininst generate a window executable file
 # python setup.py bdist_egg generate a egg file
 # Release information about eway
 
-version = "5.1.8"
+version = __version__
 name = "appPublic"
 description = "appPublic"
 author = "yumoqing"
 email = "yumoqing@gmail.com"
 
 package_data = {}
```

### Comparing `appPublic-5.1.8/test/test_aioupnp.py` & `appPublic-5.1.9/test/test_aioupnp.py`

 * *Files identical despite different names*


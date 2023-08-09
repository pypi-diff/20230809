# Comparing `tmp/apicrud-0.2.9.tar.gz` & `tmp/apicrud-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicrud-0.2.9.tar", last modified: Mon May 23 21:34:09 2022, max compression
+gzip compressed data, was "apicrud-0.3.0.tar", last modified: Wed Aug  9 02:06:12 2023, max compression
```

## Comparing `apicrud-0.2.9.tar` & `apicrud-0.3.0.tar`

### file list

```diff
@@ -1,74 +1,160 @@
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.127345 apicrud-0.2.9/
--rw-rw-rw-   0 build     (1001) docker     (485)    11358 2022-05-23 21:29:27.000000 apicrud-0.2.9/LICENSE.txt
--rw-------   0 build     (1001) docker     (485)     4213 2022-05-23 21:34:09.126345 apicrud-0.2.9/PKG-INFO
--rw-rw-rw-   0 build     (1001) docker     (485)     3346 2022-05-23 21:29:27.000000 apicrud-0.2.9/README.md
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.113344 apicrud-0.2.9/apicrud/
--rw-rw-rw-   0 build     (1001) docker     (485)      745 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/__init__.py
--rw-rw-rw-   0 build     (1001) docker     (485)       61 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/_version.py
--rw-rw-rw-   0 build     (1001) docker     (485)    15698 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/access.py
--rw-rw-rw-   0 build     (1001) docker     (485)     4866 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/account_settings.py
--rw-rw-rw-   0 build     (1001) docker     (485)     2648 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/aes_encrypt.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.118345 apicrud-0.2.9/apicrud/auth/
--rw-rw-rw-   0 build     (1001) docker     (485)      180 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/__init__.py
--rw-rw-rw-   0 build     (1001) docker     (485)     3770 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/apikey.py
--rw-rw-rw-   0 build     (1001) docker     (485)     6294 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/ldap_func.py
--rw-rw-rw-   0 build     (1001) docker     (485)     2218 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/local_func.py
--rw-rw-rw-   0 build     (1001) docker     (485)     6350 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/local_user.py
--rw-rw-rw-   0 build     (1001) docker     (485)     5821 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/oauth2.py
--rw-rw-rw-   0 build     (1001) docker     (485)     2004 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/oauth2_func.py
--rw-rw-rw-   0 build     (1001) docker     (485)     3794 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/totp.py
--rw-rw-rw-   0 build     (1001) docker     (485)     3967 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/auth/totp_func.py
--rw-rw-rw-   0 build     (1001) docker     (485)    27360 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/basic_crud.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1184 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/const.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.123345 apicrud-0.2.9/apicrud/controllers/
--rw-rw-rw-   0 build     (1001) docker     (485)     2667 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/account.py
--rw-rw-rw-   0 build     (1001) docker     (485)      754 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/apikey.py
--rw-rw-rw-   0 build     (1001) docker     (485)     2001 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/auth.py
--rw-rw-rw-   0 build     (1001) docker     (485)      139 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/category.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1692 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/contact.py
--rw-rw-rw-   0 build     (1001) docker     (485)      232 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/credential.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1618 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/grant.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1784 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/location.py
--rw-rw-rw-   0 build     (1001) docker     (485)      618 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/metric.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1130 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/person.py
--rw-rw-rw-   0 build     (1001) docker     (485)      211 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/profile.py
--rw-rw-rw-   0 build     (1001) docker     (485)      228 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/scope.py
--rw-rw-rw-   0 build     (1001) docker     (485)      781 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/settings.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1012 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/trashcan.py
--rw-rw-rw-   0 build     (1001) docker     (485)      127 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/controllers/tz.py
--rw-rw-rw-   0 build     (1001) docker     (485)    10952 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/database.py
--rw-rw-rw-   0 build     (1001) docker     (485)      268 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/exceptions.py
--rw-rw-rw-   0 build     (1001) docker     (485)     2787 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/geocode.py
--rw-rw-rw-   0 build     (1001) docker     (485)     6063 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/grants.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1627 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/health.py
--rw-rw-rw-   0 build     (1001) docker     (485)     6821 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/initialize.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.123345 apicrud-0.2.9/apicrud/media/
--rw-rw-rw-   0 build     (1001) docker     (485)    20445 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/media/storage.py
--rw-rw-rw-   0 build     (1001) docker     (485)    10838 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/media/worker_processing.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.125345 apicrud-0.2.9/apicrud/messaging/
--rw-rw-rw-   0 build     (1001) docker     (485)     4517 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/messaging/confirmation.py
--rw-rw-rw-   0 build     (1001) docker     (485)     5796 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/messaging/format.py
--rw-rw-rw-   0 build     (1001) docker     (485)     8567 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/messaging/send.py
--rw-rw-rw-   0 build     (1001) docker     (485)    12392 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/metrics.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.126345 apicrud-0.2.9/apicrud/models/
--rw-rw-rw-   0 build     (1001) docker     (485)      161 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/models/__init__.py
--rw-rw-rw-   0 build     (1001) docker     (485)    18750 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/models/api.py
--rw-rw-rw-   0 build     (1001) docker     (485)     1149 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/models/base.py
--rw-rw-rw-   0 build     (1001) docker     (485)     3778 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/ratelimit.py
--rw-rw-rw-   0 build     (1001) docker     (485)     8389 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/service_config.py
--rw-rw-rw-   0 build     (1001) docker     (485)     6149 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/service_registry.py
--rw-rw-rw-   0 build     (1001) docker     (485)    19054 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/session_auth.py
--rw-rw-rw-   0 build     (1001) docker     (485)     7040 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/session_manager.py
--rw-rw-rw-   0 build     (1001) docker     (485)      191 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/state.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.126345 apicrud-0.2.9/apicrud/test/
--rw-rw-rw-   0 build     (1001) docker     (485)     8185 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/test/base.py
--rw-rw-rw-   0 build     (1001) docker     (485)    12630 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/trashcan.py
--rw-rw-rw-   0 build     (1001) docker     (485)     2972 2022-05-23 21:29:27.000000 apicrud-0.2.9/apicrud/utils.py
-drwx------   0 build     (1001) docker     (485)        0 2022-05-23 21:34:09.115344 apicrud-0.2.9/apicrud.egg-info/
--rw-------   0 build     (1001) docker     (485)     4213 2022-05-23 21:34:09.000000 apicrud-0.2.9/apicrud.egg-info/PKG-INFO
--rw-------   0 build     (1001) docker     (485)     1574 2022-05-23 21:34:09.000000 apicrud-0.2.9/apicrud.egg-info/SOURCES.txt
--rw-------   0 build     (1001) docker     (485)        1 2022-05-23 21:34:09.000000 apicrud-0.2.9/apicrud.egg-info/dependency_links.txt
--rw-------   0 build     (1001) docker     (485)      489 2022-05-23 21:34:09.000000 apicrud-0.2.9/apicrud.egg-info/requires.txt
--rw-------   0 build     (1001) docker     (485)        8 2022-05-23 21:34:09.000000 apicrud-0.2.9/apicrud.egg-info/top_level.txt
--rw-------   0 build     (1001) docker     (485)       38 2022-05-23 21:34:09.127345 apicrud-0.2.9/setup.cfg
--rw-rw-rw-   0 build     (1001) docker     (485)     3006 2022-05-23 21:29:27.000000 apicrud-0.2.9/setup.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.132465 apicrud-0.3.0/
+-rw-rw-rw-   0 build     (1001) docker     (485)    11358 2023-08-09 02:05:46.000000 apicrud-0.3.0/LICENSE.txt
+-rw-------   0 build     (1001) docker     (485)     4193 2023-08-09 02:06:12.131465 apicrud-0.3.0/PKG-INFO
+-rw-rw-rw-   0 build     (1001) docker     (485)     3346 2023-08-09 02:05:46.000000 apicrud-0.3.0/README.md
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.110465 apicrud-0.3.0/apicrud/
+-rw-rw-rw-   0 build     (1001) docker     (485)      745 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/__init__.py
+-rw-rw-rw-   0 build     (1001) docker     (485)       61 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/_version.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    15845 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/access.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     4866 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/account_settings.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2648 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/aes_encrypt.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.112465 apicrud-0.3.0/apicrud/alembic/
+-rw-rw-rw-   0 build     (1001) docker     (485)       52 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/alembic/README.txt
+-rw-rw-rw-   0 build     (1001) docker     (485)     3602 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/alembic/env.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      494 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/alembic/script.py.mako
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.112465 apicrud-0.3.0/apicrud/alembic/versions/
+-rw-rw-rw-   0 build     (1001) docker     (485)    17204 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/alembic/versions/cac2000912a5_initialize.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1548 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/alembic.ini
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.114465 apicrud-0.3.0/apicrud/auth/
+-rw-rw-rw-   0 build     (1001) docker     (485)      180 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/__init__.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3770 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/apikey.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     6294 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/ldap_func.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2218 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/local_func.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     6350 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/local_user.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     5821 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/oauth2.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2004 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/oauth2_func.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3793 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/totp.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3967 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/auth/totp_func.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    27358 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/basic_crud.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1184 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/const.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.118465 apicrud-0.3.0/apicrud/controllers/
+-rw-rw-rw-   0 build     (1001) docker     (485)     2667 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/account.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      754 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/apikey.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2001 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/auth.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      139 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/category.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1692 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/contact.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      232 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/credential.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1618 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/grant.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1784 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/location.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      618 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/metric.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1130 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/person.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      211 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/profile.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      228 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/scope.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      781 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/settings.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1012 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/trashcan.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      127 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/controllers/tz.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    10942 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/database.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      268 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/exceptions.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2787 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/geocode.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     6063 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/grants.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1627 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/health.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.101466 apicrud-0.3.0/apicrud/i18n/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.097466 apicrud-0.3.0/apicrud/i18n/ar/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.118465 apicrud-0.3.0/apicrud/i18n/ar/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4824 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/ar/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.097466 apicrud-0.3.0/apicrud/i18n/de/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.118465 apicrud-0.3.0/apicrud/i18n/de/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4269 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/de/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.098466 apicrud-0.3.0/apicrud/i18n/en/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.119465 apicrud-0.3.0/apicrud/i18n/en/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)      465 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/en/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.098466 apicrud-0.3.0/apicrud/i18n/es/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.119465 apicrud-0.3.0/apicrud/i18n/es/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4207 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/es/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.098466 apicrud-0.3.0/apicrud/i18n/fil/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.119465 apicrud-0.3.0/apicrud/i18n/fil/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4298 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/fil/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.099465 apicrud-0.3.0/apicrud/i18n/fr/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.119465 apicrud-0.3.0/apicrud/i18n/fr/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4209 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/fr/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.099465 apicrud-0.3.0/apicrud/i18n/it/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.120465 apicrud-0.3.0/apicrud/i18n/it/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4170 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/it/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.099465 apicrud-0.3.0/apicrud/i18n/ja/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.120465 apicrud-0.3.0/apicrud/i18n/ja/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4687 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/ja/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.100466 apicrud-0.3.0/apicrud/i18n/ko/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.120465 apicrud-0.3.0/apicrud/i18n/ko/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4286 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/ko/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.100466 apicrud-0.3.0/apicrud/i18n/pt/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.120465 apicrud-0.3.0/apicrud/i18n/pt/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4117 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/pt/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.100466 apicrud-0.3.0/apicrud/i18n/ru/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.121465 apicrud-0.3.0/apicrud/i18n/ru/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     5505 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/ru/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.100466 apicrud-0.3.0/apicrud/i18n/vi/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.121465 apicrud-0.3.0/apicrud/i18n/vi/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     4580 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/vi/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.101466 apicrud-0.3.0/apicrud/i18n/zh/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.121465 apicrud-0.3.0/apicrud/i18n/zh/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     3803 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/zh/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.101466 apicrud-0.3.0/apicrud/i18n/zh_Hans/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.121465 apicrud-0.3.0/apicrud/i18n/zh_Hans/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     3803 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/zh_Hans/LC_MESSAGES/messages.mo
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.101466 apicrud-0.3.0/apicrud/i18n/zh_Hant/
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.122465 apicrud-0.3.0/apicrud/i18n/zh_Hant/LC_MESSAGES/
+-rw-------   0 build     (1001) docker     (485)     3824 2023-08-09 02:05:49.000000 apicrud-0.3.0/apicrud/i18n/zh_Hant/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0 build     (1001) docker     (485)     6821 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/initialize.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.122465 apicrud-0.3.0/apicrud/media/
+-rw-rw-rw-   0 build     (1001) docker     (485)    20445 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/media/storage.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    10838 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/media/worker_processing.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.123465 apicrud-0.3.0/apicrud/messaging/
+-rw-rw-rw-   0 build     (1001) docker     (485)     4517 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/messaging/confirmation.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     5704 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/messaging/format.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     8567 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/messaging/send.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    12392 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/metrics.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.124465 apicrud-0.3.0/apicrud/models/
+-rw-rw-rw-   0 build     (1001) docker     (485)      161 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/models/__init__.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    18750 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/models/api.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1148 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/models/base.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3778 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/ratelimit.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     8389 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/service_config.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    25003 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/service_config.yaml
+-rw-rw-rw-   0 build     (1001) docker     (485)     6149 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/service_registry.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    19054 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/session_auth.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     7040 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/session_manager.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      191 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/state.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.125465 apicrud-0.3.0/apicrud/templates/
+-rw-rw-rw-   0 build     (1001) docker     (485)     1604 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/confirm_new.j2
+-rw-rw-rw-   0 build     (1001) docker     (485)     1463 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/contact_add.j2
+-rw-rw-rw-   0 build     (1001) docker     (485)     1242 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/footer.j2
+-rw-rw-rw-   0 build     (1001) docker     (485)      372 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/moderator.j2
+-rw-rw-rw-   0 build     (1001) docker     (485)     1328 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/password_reset.j2
+-rw-rw-rw-   0 build     (1001) docker     (485)      794 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/reset_invalid.j2
+-rw-rw-rw-   0 build     (1001) docker     (485)      627 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/templates/usage_notify.j2
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.126465 apicrud-0.3.0/apicrud/test/
+-rw-rw-rw-   0 build     (1001) docker     (485)     8185 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/test/base.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2243 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/timezones.yaml
+-rw-rw-rw-   0 build     (1001) docker     (485)    12628 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/trashcan.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2972 2023-08-09 02:05:46.000000 apicrud-0.3.0/apicrud/utils.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.111465 apicrud-0.3.0/apicrud.egg-info/
+-rw-------   0 build     (1001) docker     (485)     4193 2023-08-09 02:06:12.000000 apicrud-0.3.0/apicrud.egg-info/PKG-INFO
+-rw-------   0 build     (1001) docker     (485)     3114 2023-08-09 02:06:12.000000 apicrud-0.3.0/apicrud.egg-info/SOURCES.txt
+-rw-------   0 build     (1001) docker     (485)        1 2023-08-09 02:06:12.000000 apicrud-0.3.0/apicrud.egg-info/dependency_links.txt
+-rw-------   0 build     (1001) docker     (485)      489 2023-08-09 02:06:12.000000 apicrud-0.3.0/apicrud.egg-info/requires.txt
+-rw-------   0 build     (1001) docker     (485)        8 2023-08-09 02:06:12.000000 apicrud-0.3.0/apicrud.egg-info/top_level.txt
+-rw-------   0 build     (1001) docker     (485)       38 2023-08-09 02:06:12.132465 apicrud-0.3.0/setup.cfg
+-rw-rw-rw-   0 build     (1001) docker     (485)     3006 2023-08-09 02:05:46.000000 apicrud-0.3.0/setup.py
+drwx------   0 build     (1001) docker     (485)        0 2023-08-09 02:06:12.131465 apicrud-0.3.0/tests/
+-rw-rw-rw-   0 build     (1001) docker     (485)    18215 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_accounts.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     9861 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_apikeys.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3733 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_auth.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     1709 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_base.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    10231 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_contacts.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     4834 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_credentials.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     7370 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_grants.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     4200 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_lists.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     5469 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_locations.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     4187 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_main.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     4076 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_messages.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     8429 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_messaging.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     7292 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_metrics.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    20514 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_oauth2.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     8829 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_people.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     4828 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_profile.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     2964 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_ratelimit.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3940 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_service_config.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     3003 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_service_registry.py
+-rw-rw-rw-   0 build     (1001) docker     (485)     7859 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_totp.py
+-rw-rw-rw-   0 build     (1001) docker     (485)    14885 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_trashcan.py
+-rw-rw-rw-   0 build     (1001) docker     (485)      554 2023-08-09 02:05:46.000000 apicrud-0.3.0/tests/test_utils.py
```

### Comparing `apicrud-0.2.9/LICENSE.txt` & `apicrud-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/PKG-INFO` & `apicrud-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: apicrud
-Version: 0.2.9
+Version: 0.3.0
 Summary: Flask REST framework for role-based access
 Home-page: https://github.com/instantlinux/apicrud
 Author: Rich Braun
 Author-email: docker@instantlinux.net
 License: Apache License Version 2.0
 Keywords: api flask rbac rest
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -47,9 +46,7 @@
 ### Contributions
 
 Your pull-requests and bug-reports are welcome here. See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ### License
 
 Software copyright &copy; 2021 by Richard Braun &bull; <a href="https://www.apache.org/licenses/LICENSE-2.0">Apache 2.0</a> license <p />
-
-
```

### Comparing `apicrud-0.2.9/README.md` & `apicrud-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/__init__.py` & `apicrud-0.3.0/apicrud/__init__.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/access.py` & `apicrud-0.3.0/apicrud/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,22 @@
             self.resource = model.__name__.lower() if model else None
             self.auth = self.auth_method = None
             header_auth = ServiceConfig().config.HEADER_AUTH_APIKEY
             self.apikey_id = None
             if header_auth in request.headers:
                 # TODO: add support for HMAC request signing in place
                 # of this plain-text X-Api-Key header method
-                prefix, secret = request.headers.get(header_auth).split('.')
-                item = g.session.get(None, self.apikey_hash(secret)[:8],
-                                     key_id=prefix)
+                try:
+                    prefix, secret = request.headers.get(
+                        header_auth).split('.')
+                except ValueError:
+                    item = None
+                else:
+                    item = g.session.get(None, self.apikey_hash(secret)[:8],
+                                         key_id=prefix)
                 if item:
                     self.auth = item.get('auth').split(':')
                     self.uid = uid = item.get('sub')
                     self.apikey_id = prefix
             elif request.authorization:
                 uid = self.uid = request.authorization.username
                 secret = request.authorization.password
```

### Comparing `apicrud-0.2.9/apicrud/account_settings.py` & `apicrud-0.3.0/apicrud/account_settings.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/aes_encrypt.py` & `apicrud-0.3.0/apicrud/aes_encrypt.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/apikey.py` & `apicrud-0.3.0/apicrud/auth/apikey.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/ldap_func.py` & `apicrud-0.3.0/apicrud/auth/ldap_func.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/local_func.py` & `apicrud-0.3.0/apicrud/auth/local_func.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/local_user.py` & `apicrud-0.3.0/apicrud/auth/local_user.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/oauth2.py` & `apicrud-0.3.0/apicrud/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/oauth2_func.py` & `apicrud-0.3.0/apicrud/auth/oauth2_func.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/auth/totp.py` & `apicrud-0.3.0/apicrud/auth/totp.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         if account.totp_secret:
             logging.info(dict(message='attempt to regenerate before revoke',
                               **logmsg))
             return dict(message=_(u'access denied')), 403
         totp = pyotp.random_base32()
         uri = pyotp.totp.TOTP(totp).provisioning_uri(
             name=account.owner.identity, issuer_name=self.config.APPNAME)
-        return(dict(g.session.create(acc.uid, ['pendingtotp'],
-                                     totp=totp, ttl=120, uri=uri))), 200
+        return dict(g.session.create(acc.uid, ['pendingtotp'],
+                                     totp=totp, ttl=120, uri=uri)), 200
 
     def register(self, body):
         acc = AccessControl()
         config = self.config
         logmsg = dict(action='totp_register', identity=acc.identity)
         totp_secret = g.session.get(acc.uid, body.get('nonce'), arg='totp')
         if not totp_secret:
```

### Comparing `apicrud-0.2.9/apicrud/auth/totp_func.py` & `apicrud-0.3.0/apicrud/auth/totp_func.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/basic_crud.py` & `apicrud-0.3.0/apicrud/basic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
         retval = record.as_dict()
         if hasattr(self.model, 'uid') and hasattr(self.model, 'owner'):
             retval['owner'] = record.owner.name
         if hasattr(self.model, 'category_id') and retval['category_id']:
             retval['category'] = record.category.name
         if 'modified' in retval and not retval['modified']:
-            del(retval['modified'])
+            del retval['modified']
         eid = None if hasattr(self.model, 'event_id') else (
             acc.auth_ids[acc.primary_resource] or [None])[0]
         retval['rbac'] = ''.join(sorted(list(
             acc.rbac_permissions(query=query, membership=acc.primary_resource,
                                  id=eid) - set('c'))))
         if 'geolat' in retval:
             access = 'r' if 'r' in retval['rbac'] else None
@@ -371,15 +371,15 @@
             # TODO: this seems a bit hackish, try to remember what
             # use-case this supports. The del() use-case is to
             # enable get:guest?filter{id:null,event_id=foo}
             if not filter.get('id'):
                 if len(filter) == 1:
                     return dict(count=0, items=[]), 200
                 else:
-                    del(filter['id'])
+                    del filter['id']
         elif 'filter' in kwargs and not filter:
             return dict(count=0, items=[]), 200
         if filter.get('account_id') and not hasattr(self.model, 'account_id'):
             try:
                 account = g.db.query(self.models.Account).filter_by(
                     id=filter['account_id']).one()
             except NoResultFound:
```

### Comparing `apicrud-0.2.9/apicrud/const.py` & `apicrud-0.3.0/apicrud/const.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/account.py` & `apicrud-0.3.0/apicrud/controllers/account.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/apikey.py` & `apicrud-0.3.0/apicrud/controllers/apikey.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/auth.py` & `apicrud-0.3.0/apicrud/controllers/auth.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/contact.py` & `apicrud-0.3.0/apicrud/controllers/contact.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/grant.py` & `apicrud-0.3.0/apicrud/controllers/grant.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/location.py` & `apicrud-0.3.0/apicrud/controllers/location.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/metric.py` & `apicrud-0.3.0/apicrud/controllers/metric.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/person.py` & `apicrud-0.3.0/apicrud/controllers/person.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/settings.py` & `apicrud-0.3.0/apicrud/controllers/settings.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/controllers/trashcan.py` & `apicrud-0.3.0/apicrud/controllers/trashcan.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/database.py` & `apicrud-0.3.0/apicrud/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 created 31-mar-2019 by richb@instantlinux.net
 """
 
 import alembic.config
 import alembic.script
 from alembic.runtime.environment import EnvironmentContext
-from flask import _app_ctx_stack, g
+from flask import g
 from flask_babel import _
+import greenlet
 import logging
 import os.path
 from sqlalchemy import create_engine
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.event import listen
 from sqlalchemy.exc import NoReferencedTableError, OperationalError, \
@@ -50,15 +51,15 @@
     global db_engine
     if not engine:
         # This is where init_db is invoked under celery
         engine = db_engine or _init_db(db_url=db_url)
     if scoped:
         global Session
         if scopefunc is None:
-            scopefunc = _app_ctx_stack.__ident_func__
+            scopefunc = greenlet.getcurrent
         Session = scoped_session(sessionmaker(autocommit=False,
                                               autoflush=False,
                                               bind=engine),
                                  scopefunc=scopefunc)
         if engine.url.drivername == 'sqlite':
             Session.execute('PRAGMA foreign_keys=on')
         return Session
```

### Comparing `apicrud-0.2.9/apicrud/geocode.py` & `apicrud-0.3.0/apicrud/geocode.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/grants.py` & `apicrud-0.3.0/apicrud/grants.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/health.py` & `apicrud-0.3.0/apicrud/health.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/initialize.py` & `apicrud-0.3.0/apicrud/initialize.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/media/storage.py` & `apicrud-0.3.0/apicrud/media/storage.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/media/worker_processing.py` & `apicrud-0.3.0/apicrud/media/worker_processing.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/messaging/confirmation.py` & `apicrud-0.3.0/apicrud/messaging/confirmation.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/messaging/format.py` & `apicrud-0.3.0/apicrud/messaging/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,15 @@
         trans = []
         for dir in config.BABEL_TRANSLATION_DIRECTORIES.split(';'):
             trans.append(Translations.load(dir, locale))
         if not jinja2Env:
             for folder in config.TEMPLATE_FOLDERS:
                 jinja2Env.append(jinja2.Environment(
                     loader=jinja2.FileSystemLoader(searchpath=folder),
-                    extensions=['jinja2.ext.i18n', 'jinja2.ext.autoescape'],
-                    autoescape=jinja2.select_autoescape(['html'])
+                    extensions=['jinja2.ext.i18n']
                 ))
 
         kwargs.update(dict(siteurl=self.siteurl, appname=self.config.APPNAME))
         for env in jinja2Env:
             try:
                 for x in trans:
                     env.install_gettext_translations(x)
```

### Comparing `apicrud-0.2.9/apicrud/messaging/send.py` & `apicrud-0.3.0/apicrud/messaging/send.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/metrics.py` & `apicrud-0.3.0/apicrud/metrics.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/models/api.py` & `apicrud-0.3.0/apicrud/models/api.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/models/base.py` & `apicrud-0.3.0/apicrud/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         A list of related records' ids can be attached by defining
         one or more resource names in a __rest_related__ tuple
         """
 
         retval = self.__dict__.copy()
         if hasattr(self, '__rest_exclude__'):
             for col in self.__rest_exclude__:
-                del(retval[col])
+                del retval[col]
         if hasattr(self, '__rest_related__'):
             for key in self.__rest_related__:
                 retval[key] = [rec.id for rec in getattr(self, key)]
         if hasattr(self, '__rest_hybrid__'):
             for key in self.__rest_hybrid__:
                 retval[key] = getattr(self, key)
         retval.pop('_sa_instance_state', None)
```

### Comparing `apicrud-0.2.9/apicrud/ratelimit.py` & `apicrud-0.3.0/apicrud/ratelimit.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/service_config.py` & `apicrud-0.3.0/apicrud/service_config.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/service_registry.py` & `apicrud-0.3.0/apicrud/service_registry.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/session_auth.py` & `apicrud-0.3.0/apicrud/session_auth.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/session_manager.py` & `apicrud-0.3.0/apicrud/session_manager.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/test/base.py` & `apicrud-0.3.0/apicrud/test/base.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud/trashcan.py` & `apicrud-0.3.0/apicrud/trashcan.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             msg = _(u'not found') if 'No row was found' in str(ex) else str(ex)
             return dict(id=id, message=msg), 404
 
         retval = record.as_dict()
         if hasattr(model, 'uid') and hasattr(model, 'owner'):
             retval['owner'] = record.owner.name
         if 'modified' in retval and not retval['modified']:
-            del(retval['modified'])
+            del retval['modified']
         eid = None if hasattr(model, 'event_id') else (
             acc.auth_ids[acc.primary_resource] or [None])[0]
         retval['rbac'] = ''.join(sorted(list(
             acc.rbac_permissions(query=query, membership=acc.primary_resource,
                                  id=eid) - set('c'))))
         if 'r' in retval['rbac']:
             logging.info(dict(
@@ -222,15 +222,15 @@
                     405
             resources = [
                 key for key in state.controllers.keys()
                 if key not in ('auth', 'scope', 'settings', 'trashcan', 'tz')
                 and key >= start_resource]
         if 'id' in filter and not filter.get('id'):
             # allow get:foo?filter{id:null,key=val,etc}
-            del(filter['id'])
+            del filter['id']
         limit = logmsg['limit'] = int(kwargs.get(
             'limit', Constants.PER_PAGE_DEFAULT))
         retval = dict(items=[], count=0)
         for resource in resources:
             if resource == 'apikey':
                 model = self.models.APIkey
             else:
```

### Comparing `apicrud-0.2.9/apicrud/utils.py` & `apicrud-0.3.0/apicrud/utils.py`

 * *Files identical despite different names*

### Comparing `apicrud-0.2.9/apicrud.egg-info/PKG-INFO` & `apicrud-0.3.0/apicrud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: apicrud
-Version: 0.2.9
+Version: 0.3.0
 Summary: Flask REST framework for role-based access
 Home-page: https://github.com/instantlinux/apicrud
 Author: Rich Braun
 Author-email: docker@instantlinux.net
 License: Apache License Version 2.0
 Keywords: api flask rbac rest
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -47,9 +46,7 @@
 ### Contributions
 
 Your pull-requests and bug-reports are welcome here. See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ### License
 
 Software copyright &copy; 2021 by Richard Braun &bull; <a href="https://www.apache.org/licenses/LICENSE-2.0">Apache 2.0</a> license <p />
-
-
```

### Comparing `apicrud-0.2.9/apicrud.egg-info/SOURCES.txt` & `apicrud-0.3.0/apicrud.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,43 @@
 README.md
 setup.py
 apicrud/__init__.py
 apicrud/_version.py
 apicrud/access.py
 apicrud/account_settings.py
 apicrud/aes_encrypt.py
+apicrud/alembic.ini
 apicrud/basic_crud.py
 apicrud/const.py
 apicrud/database.py
 apicrud/exceptions.py
 apicrud/geocode.py
 apicrud/grants.py
 apicrud/health.py
 apicrud/initialize.py
 apicrud/metrics.py
 apicrud/ratelimit.py
 apicrud/service_config.py
+apicrud/service_config.yaml
 apicrud/service_registry.py
 apicrud/session_auth.py
 apicrud/session_manager.py
 apicrud/state.py
+apicrud/timezones.yaml
 apicrud/trashcan.py
 apicrud/utils.py
 apicrud.egg-info/PKG-INFO
 apicrud.egg-info/SOURCES.txt
 apicrud.egg-info/dependency_links.txt
 apicrud.egg-info/requires.txt
 apicrud.egg-info/top_level.txt
+apicrud/alembic/README.txt
+apicrud/alembic/env.py
+apicrud/alembic/script.py.mako
+apicrud/alembic/versions/cac2000912a5_initialize.py
 apicrud/auth/__init__.py
 apicrud/auth/apikey.py
 apicrud/auth/ldap_func.py
 apicrud/auth/local_func.py
 apicrud/auth/local_user.py
 apicrud/auth/oauth2.py
 apicrud/auth/oauth2_func.py
@@ -48,16 +55,60 @@
 apicrud/controllers/metric.py
 apicrud/controllers/person.py
 apicrud/controllers/profile.py
 apicrud/controllers/scope.py
 apicrud/controllers/settings.py
 apicrud/controllers/trashcan.py
 apicrud/controllers/tz.py
+apicrud/i18n/ar/LC_MESSAGES/messages.mo
+apicrud/i18n/de/LC_MESSAGES/messages.mo
+apicrud/i18n/en/LC_MESSAGES/messages.mo
+apicrud/i18n/es/LC_MESSAGES/messages.mo
+apicrud/i18n/fil/LC_MESSAGES/messages.mo
+apicrud/i18n/fr/LC_MESSAGES/messages.mo
+apicrud/i18n/it/LC_MESSAGES/messages.mo
+apicrud/i18n/ja/LC_MESSAGES/messages.mo
+apicrud/i18n/ko/LC_MESSAGES/messages.mo
+apicrud/i18n/pt/LC_MESSAGES/messages.mo
+apicrud/i18n/ru/LC_MESSAGES/messages.mo
+apicrud/i18n/vi/LC_MESSAGES/messages.mo
+apicrud/i18n/zh/LC_MESSAGES/messages.mo
+apicrud/i18n/zh_Hans/LC_MESSAGES/messages.mo
+apicrud/i18n/zh_Hant/LC_MESSAGES/messages.mo
 apicrud/media/storage.py
 apicrud/media/worker_processing.py
 apicrud/messaging/confirmation.py
 apicrud/messaging/format.py
 apicrud/messaging/send.py
 apicrud/models/__init__.py
 apicrud/models/api.py
 apicrud/models/base.py
-apicrud/test/base.py
+apicrud/templates/confirm_new.j2
+apicrud/templates/contact_add.j2
+apicrud/templates/footer.j2
+apicrud/templates/moderator.j2
+apicrud/templates/password_reset.j2
+apicrud/templates/reset_invalid.j2
+apicrud/templates/usage_notify.j2
+apicrud/test/base.py
+tests/test_accounts.py
+tests/test_apikeys.py
+tests/test_auth.py
+tests/test_base.py
+tests/test_contacts.py
+tests/test_credentials.py
+tests/test_grants.py
+tests/test_lists.py
+tests/test_locations.py
+tests/test_main.py
+tests/test_messages.py
+tests/test_messaging.py
+tests/test_metrics.py
+tests/test_oauth2.py
+tests/test_people.py
+tests/test_profile.py
+tests/test_ratelimit.py
+tests/test_service_config.py
+tests/test_service_registry.py
+tests/test_totp.py
+tests/test_trashcan.py
+tests/test_utils.py
```

### Comparing `apicrud-0.2.9/setup.py` & `apicrud-0.3.0/setup.py`

 * *Files identical despite different names*


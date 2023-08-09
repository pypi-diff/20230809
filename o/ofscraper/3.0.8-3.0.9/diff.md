# Comparing `tmp/ofscraper-3.0.8.tar.gz` & `tmp/ofscraper-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.0.8.tar", max compression
+gzip compressed data, was "ofscraper-3.0.9.tar", max compression
```

## Comparing `ofscraper-3.0.8.tar` & `ofscraper-3.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-08-07 23:28:18.500726 ofscraper-3.0.8/LICENSE
--rw-r--r--   0        0        0     2863 2023-08-07 23:28:18.500726 ofscraper-3.0.8/README.md
--rwxr-xr-x   0        0        0      291 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/__main__.py
--rw-r--r--   0        0        0     1016 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/__version__.pye
--rw-r--r--   0        0        0     8736 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9895 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1029 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/init.py
--rw-r--r--   0        0        0     7568 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2946 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/me.py
--rw-r--r--   0        0        0     9518 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9687 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5730 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4497 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3384 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9312 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/api/timeline.py
--rw-r--r--   0        0        0      804 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8779 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/media.py
--rw-r--r--   0        0        0     1795 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0     8068 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3734 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4849 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29784 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14816 2023-08-07 23:28:18.508726 ofscraper-3.0.8/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5347 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    15354 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     7246 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10129 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4851 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      773 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     6241 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     7227 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7848 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    30812 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     3812 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    14095 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/args.py
--rw-r--r--   0        0        0    10673 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    14736 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/config.py
--rw-r--r--   0        0        0      395 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    41393 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     3386 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5665 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/filters.py
--rw-r--r--   0        0        0    11133 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/logger.py
--rw-r--r--   0        0        0      189 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/misc.py
--rw-r--r--   0        0        0    10913 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7251 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4221 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1215 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      893 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5773 2023-08-07 23:28:18.512726 ofscraper-3.0.8/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     2073 2023-08-07 23:28:49.520794 ofscraper-3.0.8/pyproject.toml
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 ofscraper-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 01:51:03.965648 ofscraper-3.0.9/LICENSE
+-rw-r--r--   0        0        0     2863 2023-08-08 01:51:03.965648 ofscraper-3.0.9/README.md
+-rwxr-xr-x   0        0        0      291 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1016 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/__version__.pye
+-rw-r--r--   0        0        0     8736 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9895 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1029 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7568 2023-08-08 01:51:03.973647 ofscraper-3.0.9/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2946 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9518 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9687 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5730 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4497 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3384 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9312 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0      804 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8779 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     1795 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0     8068 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3734 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4849 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29784 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14816 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5347 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    15355 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     7246 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10129 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4851 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      773 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     6241 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     7227 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7848 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    30812 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     3812 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    14095 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/args.py
+-rw-r--r--   0        0        0    10673 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    14774 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      395 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    41645 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-08-08 01:51:03.977647 ofscraper-3.0.9/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     3386 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5665 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0    11133 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0      189 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/misc.py
+-rw-r--r--   0        0        0    10913 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7251 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4209 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1215 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      893 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5773 2023-08-08 01:51:03.981647 ofscraper-3.0.9/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     2073 2023-08-08 01:51:47.557657 ofscraper-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 ofscraper-3.0.9/PKG-INFO
```

### Comparing `ofscraper-3.0.8/LICENSE` & `ofscraper-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/README.md` & `ofscraper-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/__version__.py` & `ofscraper-3.0.9/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/__version__.pye` & `ofscraper-3.0.9/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/archive.py` & `ofscraper-3.0.9/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/highlights.py` & `ofscraper-3.0.9/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/init.py` & `ofscraper-3.0.9/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/labels.py` & `ofscraper-3.0.9/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/me.py` & `ofscraper-3.0.9/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/messages.py` & `ofscraper-3.0.9/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/paid.py` & `ofscraper-3.0.9/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/pinned.py` & `ofscraper-3.0.9/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/profile.py` & `ofscraper-3.0.9/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/subscriptions.py` & `ofscraper-3.0.9/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/api/timeline.py` & `ofscraper-3.0.9/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/labels.py` & `ofscraper-3.0.9/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/media.py` & `ofscraper-3.0.9/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.0.9/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/placeholder.py` & `ofscraper-3.0.9/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/posts.py` & `ofscraper-3.0.9/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/sessionbuilder.py` & `ofscraper-3.0.9/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/classes/table.py` & `ofscraper-3.0.9/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/commands/check.py` & `ofscraper-3.0.9/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/commands/manual.py` & `ofscraper-3.0.9/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/commands/scraper.py` & `ofscraper-3.0.9/ofscraper/commands/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         profiles.print_current_profile()
         init.print_sign_status()
         userdata=userselector.getselected_usernames(rescan=False)
         length=len(userdata)
         for count,ele in enumerate(userdata):
             log.info(f"Progress {count+1}/{length} model")
             if args_.getargs().posts:
-                log.info(f"Getting {','.join(args_.getargs().posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+                log.error(f"Getting {','.join(args_.getargs().posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
             try:
                 model_id = profile.get_id( ele["name"])
                 operations.create_tables(model_id,ele['name'])
                 operations.write_profile_table(model_id,ele['name'])
                 combined_urls=OF.process_areas( ele, model_id)
                 download.process_dicts(
                 ele["name"],
```

### Comparing `ofscraper-3.0.8/ofscraper/constants.py` & `ofscraper-3.0.9/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/db/operations.py` & `ofscraper-3.0.9/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/db/queries.py` & `ofscraper-3.0.9/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/interaction/like.py` & `ofscraper-3.0.9/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/prompts/keybindings.py` & `ofscraper-3.0.9/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/prompts/promptConvert.py` & `ofscraper-3.0.9/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.0.9/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.0.9/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/prompts/prompts.py` & `ofscraper-3.0.9/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/start.py` & `ofscraper-3.0.9/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/args.py` & `ofscraper-3.0.9/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/auth.py` & `ofscraper-3.0.9/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/binaries.py` & `ofscraper-3.0.9/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/config.py` & `ofscraper-3.0.9/ofscraper/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     if config==None:
         return constants.SAVE_PATH_DEFAULT   
     return config.get('save_location') or constants.SAVE_PATH_DEFAULT
 
 def get_main_profile(config=None):
     if config==None:
         return constants.PROFILE_DEFAULT   
-    return config.get('main_profile',constants.PROFILE_DEFAULT)
+    return config.get(constants.mainProfile,constants.PROFILE_DEFAULT) or constants.PROFILE_DEFAULT  
 
 def get_filesize_limit(config=None):
     if config==None:
         return constants.FILE_SIZE_LIMIT_DEFAULT      
     try:
         return parse_size(config.get('file_size_limit', constants.FILE_SIZE_LIMIT_DEFAULT  ))
     except:
```

### Comparing `ofscraper-3.0.8/ofscraper/utils/dates.py` & `ofscraper-3.0.9/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/download.py` & `ofscraper-3.0.9/ofscraper/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,18 +95,21 @@
     data=0
     global total_data
     total_data=0
     global desc
     desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios, {forced_skipped} skipped, {skipped} failed || {sumcount}/{mediacount}||{data}/{total})'   
     global count_lock
     count_lock=aioprocessing.AioLock()
-    global dir_lock
-    dir_lock=aioprocessing.AioLock()
     global chunk_lock
     chunk_lock=aioprocessing.AioLock()
+    global dirSet
+    dirSet=set()
+    global dir_lock
+    dir_lock=aioprocessing.AioLock()
+
 #start other thread here
 def process_dicts(username,model_id,medialist):
     #reset globals
     reset_globals()
     log=logging.getLogger("shared")
     random.shuffle(medialist)
     if len(medialist)==0:
@@ -146,17 +149,18 @@
                 [thread.start() for thread in queue_threads]
                 while len(list(filter(lambda x:x.is_alive(),queue_threads)))>0: 
                     for thread in queue_threads:
                         thread.join(1)
                         time.sleep(5)
         [logthread.join() for logthread in logthreads]
         [process.join(timeout=1) for process in processes]    
-        [process.terminate() for process in processes]    
+        [process.terminate() for process in processes]
         overall_progress.remove_task(task1)
         progress_group.renderables[1].height=0
+        setDirectoriesDate()    
         log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios, {forced_skipped} skipped, {skipped} failed)' )
         return photo_count,video_count,audio_count,forced_skipped,skipped
     except KeyboardInterrupt as E:
             try:
                 with exit.DelayedKeyboardInterrupt():
                     [process.terminate() for process in processes]  
                     raise KeyboardInterrupt
@@ -169,43 +173,41 @@
                     raise E
             except KeyboardInterrupt:
                
                   raise KeyboardInterrupt  
 def queue_process(pipe_,overall_progress,job_progress,task1,total):
     count=0
     downloadprogress=config_.get_show_downloadprogress(config_.read_config()) or args_.getargs().downloadbars
-    #shared globals
+        #shared globals
     global total_bytes_downloaded
     global total_bytes
     global video_count
     global audio_count
     global photo_count
     global skipped
     global forced_skipped
     global data
     global total_data
     global desc
 
-    
-
     while True:
         if count==1 or overall_progress.tasks[task1].total==overall_progress.tasks[task1].completed:
             break
         results = pipe_.recv()
         if not isinstance(results,list):
             results=[results]
 
         for result in results:
             if result is None:
                 count=count+1
-
                 continue 
             if isinstance(result,dict) and not downloadprogress:
                 continue
-            
+            if isinstance(result,set):
+                addGlobalDir(result)
             if isinstance(result,dict):
                 job_progress_helper(job_progress,result)
                 continue
             media_type, num_bytes_downloaded,total_size = result
             with count_lock:
                 total_bytes_downloaded=total_bytes_downloaded+num_bytes_downloaded
                 total_bytes=total_bytes+total_size
@@ -279,16 +281,16 @@
  
     medialist=list(medialist)
     # This need to be here: https://stackoverflow.com/questions/73599594/asyncio-works-in-python-3-10-but-not-in-python-3-8
     global sem
     sem = semaphoreDelayed(config_.get_download_semaphores(config_.read_config()))
     global total_sem
     total_sem= semaphoreDelayed(config_.get_download_semaphores(config_.read_config())*2)
-    global dirSet
-    dirSet=set()
+    global localdirSet
+    localdirSet=set()
     global split_log
     split_log=logCopy
     global log_trace
     log_trace=True if "TRACE" in set([args_.getargs().log,args_.getargs().output,args_.getargs().discord]) else False
     global pipe_
     pipe_=pipecopy
     
@@ -328,18 +330,17 @@
                 except Exception as e:
                     split_log.traceback(e)
                     split_log.traceback(traceback.format_exc())
                     media_type = "skipped"
                     num_bytes_downloaded = 0
                     await pipe_.coro_send(  (media_type, num_bytes_downloaded,0))
             
-
-    setDirectoriesDate()
     split_log.debug(f"{pid_log_helper()} download process thread closing")
     split_log.critical(None)
+    await pipe_.coro_send(localdirSet)
     await pipe_.coro_send(None)
     other_thread.join()
  
 
 def retry_required(value):
     return value == ('skipped', 1)
 
@@ -389,15 +390,15 @@
         innerlog.get().debug(f"{get_medialog(ele)} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         innerlog.get().debug(f"{get_medialog(ele)} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(temp).absolute()} -> {path_to_file}")   
         #move temp file
         if not path_to_file.exists():
             shutil.move(temp,path_to_file)
         elif pathlib.Path(temp).absolute().stat().st_size>=pathlib.Path(path_to_file).absolute().stat().st_size: 
             shutil.move(temp,path_to_file)
-        addGlobalDir(path)
+        addLocalDir(path)
         if ele.postdate:
             newDate=dates.convert_local_time(ele.postdate)
             innerlog.get().debug(f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
             set_time(path_to_file,newDate )
             innerlog.get().debug(f"{get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
         if ele.id:
             await operations.write_media_table(ele,path_to_file,model_id,username)
@@ -555,15 +556,15 @@
         innerlog.get().debug(f"{get_medialog(ele)} ffmpeg {t.stderr.decode()}")
         innerlog.get().debug(f"{get_medialog(ele)} ffmpeg {t.stdout.decode()}")
 
     video["path"].unlink(missing_ok=True)
     audio["path"].unlink(missing_ok=True)
     innerlog.get().debug(f"Moving intermediate path {temp_path} to {path_to_file}")
     shutil.move(temp_path,path_to_file)
-    addGlobalDir(path_to_file)
+    addLocalDir(path_to_file)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         innerlog.get().debug(f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
         innerlog.get().debug(f"{get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
         await operations.write_media_table(ele,path_to_file,model_id,username)
@@ -850,24 +851,29 @@
     cache = Cache(paths.getcachepath())
 
     if  ele.postid and ele.responsetype_=="profile":
         cache.set(ele.postid ,True)
         cache.close()
 
 
-def addGlobalDir(path):
-    dirSet.add(path.resolve().parent)
-def setDirectoriesDate():
+def addLocalDir(path):
+    localdirSet.add(path.resolve().parent)
+def addGlobalDir(newSet):
+    global dirSet
     global dir_lock
-    split_log.info( f" {pid_log_helper()} Setting Date for modified directories")
+    with dir_lock:
+        dirSet.update(newSet)
+def setDirectoriesDate():
+    global dirSet
+    log=logging.getLogger("shared")
+    log.info( f" {pid_log_helper()} Setting Date for modified directories")
     output=set()
     rootDir=pathlib.Path(config_.get_save_location(config_.read_config())).resolve()
     for ele in dirSet:
         output.add(ele)
         while ele!=rootDir and ele.parent!=rootDir:
-            split_log.debug(f"{pid_log_helper()} Setting Dates ele:{ele} rootDir:{rootDir}")
+            log.debug(f"{pid_log_helper()} Setting Dates ele:{ele} rootDir:{rootDir}")
             output.add(ele.parent)
             ele=ele.parent
-    split_log.debug(f"{pid_log_helper()} Directories list {rootDir}")
+    log.debug(f"{pid_log_helper()} Directories list {rootDir}")
     for ele in output:
-        with dir_lock:
-            set_time(ele,dates.get_current_time())
+        set_time(ele,dates.get_current_time())
```

### Comparing `ofscraper-3.0.8/ofscraper/utils/encoding.py` & `ofscraper-3.0.9/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/exit.py` & `ofscraper-3.0.9/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/filters.py` & `ofscraper-3.0.9/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/logger.py` & `ofscraper-3.0.9/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/of.py` & `ofscraper-3.0.9/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/paths.py` & `ofscraper-3.0.9/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/profiles.py` & `ofscraper-3.0.9/ofscraper/utils/profiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,16 +121,16 @@
 
 
 def get_profile_names():
     return [profile.name for profile in get_profiles()]
 
     
 def get_current_config_profile():
-    config = config_.read_config()
-    return config[constants.mainProfile]
+    return config_.get_main_profile(config_.read_config())
+    
 
 def get_active_profile():
     if args_.getargs().profile:
         return args_.getargs().profile
     return get_current_config_profile()
 
 def print_current_profile():
```

### Comparing `ofscraper-3.0.8/ofscraper/utils/separate.py` & `ofscraper-3.0.9/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/stdout.py` & `ofscraper-3.0.9/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/ofscraper/utils/userselector.py` & `ofscraper-3.0.9/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.8/pyproject.toml` & `ofscraper-3.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.0.8"
+version = "3.0.9"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-3.0.8/PKG-INFO` & `ofscraper-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.0.8
+Version: 3.0.9
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


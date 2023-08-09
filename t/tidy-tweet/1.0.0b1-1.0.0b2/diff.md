# Comparing `tmp/tidy_tweet-1.0.0b1.tar.gz` & `tmp/tidy_tweet-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0b1.tar", last modified: Thu Aug  3 05:19:06 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0b2.tar", last modified: Wed Aug  9 01:59:19 2023, max compression
```

## Comparing `tidy_tweet-1.0.0b1.tar` & `tidy_tweet-1.0.0b2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.405187 tidy_tweet-1.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.409187 tidy_tweet-1.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.409187 tidy_tweet-1.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.405187 tidy_tweet-1.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.409187 tidy_tweet-1.0.0b1/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 05:19:06.000000 tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:19:06.413187 tidy_tweet-1.0.0b1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 05:18:45.000000 tidy_tweet-1.0.0b1/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.009925 tidy_tweet-1.0.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.001925 tidy_tweet-1.0.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.005925 tidy_tweet-1.0.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-09 01:59:19.009925 tidy_tweet-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.005925 tidy_tweet-1.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-09 01:59:19.009925 tidy_tweet-1.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.001925 tidy_tweet-1.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.005925 tidy_tweet-1.0.0b2/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.005925 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-09 01:59:18.000000 tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.005925 tidy_tweet-1.0.0b2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:59:19.005925 tidy_tweet-1.0.0b2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-09 01:58:59.000000 tidy_tweet-1.0.0b2/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0b1/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0b2/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/.github/workflows/tests.yml` & `tidy_tweet-1.0.0b2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/LICENSE` & `tidy_tweet-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/PKG-INFO` & `tidy_tweet-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0b1/README.md` & `tidy_tweet-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/contributing.md` & `tidy_tweet-1.0.0b2/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/docs/data_model.drawio` & `tidy_tweet-1.0.0b2/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/docs/data_model.svg` & `tidy_tweet-1.0.0b2/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/docs/schema.md` & `tidy_tweet-1.0.0b2/docs/schema.md`

 * *Files 12% similar despite different names*

```diff
@@ -59,20 +59,20 @@
         text protected
         text description
         text location
         text pinned_tweet_id
         integer verified
         text url
         text username
-        integer page_id PK, FK
-        text source_file FK
+        integer source_page PK, FK
+        text source_file PK, FK
     }
     "tweet_by_page" {
         text id PK
-        integer page_id PK, FK
+        integer source_page PK, FK
         text reply_settings
         text conversation_id
         text created_at
         text retweeted_tweet_id FK
         text quoted_tweet_id FK
         text replied_to_tweet_id FK
         text in_reply_to_user_id FK
@@ -81,20 +81,20 @@
         text lang
         text source
         integer possibly_sensitive
         integer like_count
         integer quote_count
         integer reply_count
         integer retweet_count
-        text source_file FK
+        text source_file PK, FK
         integer directly_collected
     }
     "results_page" {
-        integer id PK
-        text file_name
+        integer page PK
+        text file_name PK
         text oldest_id
         text newest_id
         integer result_count
         text inserted_at
         text twarc_version
         text tidy_tweet_version
         text retrieved_at
@@ -103,17 +103,17 @@
     }
     tweet_url |o--o{ tweet : "tweet"
     user_url |o--o{ user : "user"
     tweet_hashtag |o--o{ tweet : "tweet"
     user_hashtag |o--o{ user : "user"
     tweet_mention |o--o{ tweet : "tweet"
     user_mention |o--o{ user : "user"
-    user_by_page |o--o{ results_page : "page"
+    user_by_page |o--o{ results_page : "source page"
     user_by_page |o--o{ results_page : "source file"
-    tweet_by_page |o--o{ results_page : "page"
+    tweet_by_page |o--o{ results_page : "source page"
     tweet_by_page |o--o{ tweet : "retweeted tweet"
     tweet_by_page |o--o{ tweet : "quoted tweet"
     tweet_by_page |o--o{ tweet : "replied to tweet"
     tweet_by_page |o--o{ user : "in reply to user"
     tweet_by_page |o--o{ user : "author"
     tweet_by_page |o--o{ results_page : "source file"
 ```
@@ -200,24 +200,24 @@
 - **protected** (text)
 - **description** (text)
 - **location** (text)
 - **pinned_tweet_id** (text)
 - **verified** (integer): boolean
 - **url** (text)
 - **username** (text)
-- **page_id** (integer primary key references results_page (id))
-- **source_file** (text references results_page (file_name))
+- **source_page** (integer primary key references results_page (page))
+- **source_file** (text primary key references results_page (file_name))
 
 primary key 
 
 
 Table **tweet_by_page**:
 
 - **id** (text primary key )
-- **page_id** (integer primary key references results_page (id))
+- **source_page** (integer primary key references results_page (page))
 - **reply_settings** (text)
 - **conversation_id** (text)
 - **created_at** (text)
 - **retweeted_tweet_id** (text references tweet (id))
 - **quoted_tweet_id** (text references tweet (id))
 - **replied_to_tweet_id** (text references tweet (id))
 - **in_reply_to_user_id** (text references user (id))
@@ -226,28 +226,30 @@
 - **lang** (text)
 - **source** (text)
 - **possibly_sensitive** (integer): boolean
 - **like_count** (integer)
 - **quote_count** (integer)
 - **reply_count** (integer)
 - **retweet_count** (integer)
-- **source_file** (text references results_page (file_name))
+- **source_file** (text primary key references results_page (file_name))
 - **directly_collected** (integer): boolean
 
 primary key 
 
 
 Table **results_page**:
 
-- **id** (integer primary key)
-- **file_name** (text)
+- **page** (integer primary key ): page number within the file
+- **file_name** (text primary key )
 - **oldest_id** (text): oldest tweet id in page
 - **newest_id** (text): newest tweet id in page
 - **result_count** (integer): count given in API response
 - **inserted_at** (text default current_timestamp)
 - **twarc_version** (text)
 - **tidy_tweet_version** (text)
 - **retrieved_at** (text): time response from twitter was recorded
 - **request_url** (text)
 - **additional_metadata** (text): extra metadata from twarc and twitter
 
+primary key 
+
```

### Comparing `tidy_tweet-1.0.0b1/generate_schema_diagram.py` & `tidy_tweet-1.0.0b2/generate_schema_diagram.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-from tidy_tweet.tweet_mapping import create_table_statements
+from tidy_tweet import database_schema
 from typing import NamedTuple, List, Tuple, TextIO
 
 
 class Column(NamedTuple):
     name: str
     type: str
     constraints: str = ""
@@ -117,15 +117,15 @@
         output.write("\n")
 
     if len(table_comment) > 0:
         output.write(table_comment + "\n\n")
 
 
 def write_schema_as_lists(output: TextIO):
-    for statement in create_table_statements:
+    for statement in database_schema:
         parsed_name, parsed_columns, table_comment = parse_table(statement)
 
         write_table_as_list(output, parsed_name, parsed_columns, table_comment)
         output.write("\n")
 
 
 def write_schema_as_mermaid_er(output: TextIO, with_comments=True):
@@ -137,15 +137,15 @@
     output.write("erDiagram\n")
 
     indent = "    "
 
     foreign_keys: List[ForeignKey] = []
 
     # Table definitions
-    for statement in create_table_statements:
+    for statement in database_schema:
         table_name, columns, _ = parse_table(statement)
 
         output.write(indent + f'"{table_name}"' + " {\n")
 
         for col in columns:
             output.write(indent * 2 + col.type + " " + col.name)
```

### Comparing `tidy_tweet-1.0.0b1/setup.cfg` & `tidy_tweet-1.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0b2/src/tidy_tweet/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,24 @@
 @click.argument("json_files", type=click.Path(exists=True), nargs=-1)
 @click.option(
     "--strict/--no_strict",
     default=True,
     help="Should the SQLite tables be created in strict mode (defaults to yes)? "
     "Irrelevant if adding files to an existing database.",
 )
+@click.option(
+    "--json_encoding",
+    type=str,
+    default=None,
+    help="If the json file/s you wish to load are encoded other than UTF-8, specify "
+    "encoding. If you don't know what this means and you're not getting any "
+    "decoding errors using tidy_tweet, you're all good!",
+)
 def tidy_twarc_jsons(
-    database: Path, json_files: Collection[Union[str, PathLike]], strict
+    database: Path, json_files: Collection[Union[str, PathLike]], strict, json_encoding
 ):
     """
     Tidies Twitter json collected with Twarc into relational tables.
 
     Can take one or more JSON_FILES (produced by Twarc) as input, tidies the
     tweet data within those files, and stores the date in DATABASE.
 
@@ -68,15 +76,15 @@
     # Load files into database
     num_files = len(json_files)
     n = 0
     total_pages = 0
     for file in json_files:
         n = n + 1  # Count files for user messaging only
         click.echo(f"Loading {file} (file {n} of {num_files}) into {database}")
-        p = load_twarc_json_to_sqlite(file, database)
+        p = load_twarc_json_to_sqlite(file, database, json_encoding=json_encoding)
         total_pages = total_pages + p
         click.echo(f"{p} pages of Twitter results loaded from {file}")
 
     click.echo(
         f"All done! {total_pages} pages of tweets loaded into {database} from {n} "
         f"files."
     )
```

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0b2/src/tidy_tweet/database.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0b2/src/tidy_tweet/processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,29 +77,33 @@
         else:
             db.executemany(mapping.sql_by_table[table]["insert"], table_mappings)
 
     logger.debug("Finished writing page to database.")
 
 
 def load_twarc_json_to_sqlite(
-    filename: Union[str, PathLike], db_name: Union[str, PathLike]
+    filename: Union[str, PathLike],
+    db_name: Union[str, PathLike],
+    json_encoding: str = None,
 ) -> int:
     """
     Parses a json/jsonl file produced by a Twarc search and loads the Twitter data into
     a tidied, relational format in an sqlite database.
 
     Before calling this function, the database should already have been initialised with
     the `tidy_tweet.initialise_sqlite()` function.
 
     :param filename: The path to a json/jsonl file of Twitter data. The file is expected
     to be in the format of the results of a Twarc search.
     :param db_name: The path to an existing sqlite database to load the data into
     :return: The number of pages of Twitter results loaded in this file
     """
-    with open(filename, "r") as json_fh, sqlite3.connect(db_name) as connection:
+    with open(filename, "r", encoding=json_encoding) as json_fh, sqlite3.connect(
+        db_name
+    ) as connection:
         logger.info(f"Loading {filename} into {db_name}")
 
         page_num = 0
         for page in json_fh:
             page_num = page_num + 1
             logger.info(f"Processing page {page_num} of {filename}")
             page_json = json.loads(page)
```

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0b2/src/tidy_tweet/tweet_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
 
 def map_user(user_json, source_file, page_num) -> Dict[str, List[Dict]]:
     user_map = {
         "id": user_json["id"],
         "username": user_json["username"],
         "name": user_json["name"],
-        "url": user_json["url"],
+        "url": user_json.get("url", None),
         "profile_image_url": user_json["profile_image_url"],
         "description": user_json.get("description", None),
         "created_at": user_json["created_at"],
         "protected": user_json["protected"],
         "verified": user_json["verified"],
         "location": user_json.get("location", None),
         "pinned_tweet_id": user_json.get("pinned_tweet_id", None),
```

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0b2/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0b1/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0b2/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0b2/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/tests/test_cli.py` & `tidy_tweet-1.0.0b2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0b1/tests/test_overall.py` & `tidy_tweet-1.0.0b2/tests/test_overall.py`

 * *Files identical despite different names*


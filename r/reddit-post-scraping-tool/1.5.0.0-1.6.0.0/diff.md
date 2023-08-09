# Comparing `tmp/reddit-post-scraping-tool-1.5.0.0.tar.gz` & `tmp/reddit-post-scraping-tool-1.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-post-scraping-tool-1.5.0.0.tar", last modified: Tue Aug  8 05:25:31 2023, max compression
+gzip compressed data, was "reddit-post-scraping-tool-1.6.0.0.tar", last modified: Wed Aug  9 03:03:41 2023, max compression
```

## Comparing `reddit-post-scraping-tool-1.5.0.0.tar` & `reddit-post-scraping-tool-1.6.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.154493 reddit-post-scraping-tool-1.5.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.154493 reddit-post-scraping-tool-1.5.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.154493 reddit-post-scraping-tool-1.5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.154493 reddit-post-scraping-tool-1.5.0.0/RPST GUI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/AboutBox.Designer.vb
--rw-r--r--   0 runner    (1001) docker     (123)    62772 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/AboutBox.resx
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/AboutBox.vb
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ApiHandler.vb
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ApplicationEvents.vb
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DataGridViewHandler.vb
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DeveloperBox.Designer.vb
--rw-r--r--   0 runner    (1001) docker     (123)    74791 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DeveloperBox.resx
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DeveloperBox.vb
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Application.Designer.vb
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Application.myapp
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Resources.Designer.vb
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Resources.resx
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/PostsProcessor.vb
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/RPST.vbproj
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/RPST.vbproj.user
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ResultsForm.Designer.vb
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ResultsForm.resx
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ResultsForm.vb
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/Settings.vb
--rw-r--r--   0 runner    (1001) docker     (123)    14679 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/StartForm.Designer.vb
--rw-r--r--   0 runner    (1001) docker     (123)   225546 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/StartForm.resx
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/StartForm.vb
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/Utilities.vb
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST.sln
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-08 05:25:31.000000 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-08 05:25:31.000000 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:25:31.000000 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 05:25:31.000000 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 05:25:31.000000 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 05:25:31.000000 reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/rpst/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/rpst/__main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-08 05:25:20.000000 reddit-post-scraping-tool-1.5.0.0/rpst/__rpst_.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 05:25:31.158493 reddit-post-scraping-tool-1.5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.260901 reddit-post-scraping-tool-1.6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.260901 reddit-post-scraping-tool-1.6.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.260901 reddit-post-scraping-tool-1.6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.260901 reddit-post-scraping-tool-1.6.0.0/RPST GUI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/AboutBox.Designer.vb
+-rw-r--r--   0 runner    (1001) docker     (123)    62772 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/AboutBox.resx
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/AboutBox.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/ApiHandler.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/ApplicationEvents.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DataGridViewHandler.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DeveloperBox.Designer.vb
+-rw-r--r--   0 runner    (1001) docker     (123)    74791 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DeveloperBox.resx
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DeveloperBox.vb
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormMain.Designer.vb
+-rw-r--r--   0 runner    (1001) docker     (123)   193128 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormMain.resx
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormMain.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormPosts.Designer.vb
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormPosts.resx
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormPosts.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Application.Designer.vb
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Application.myapp
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Resources.Designer.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Resources.resx
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/PostsProcessor.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/RPST.vbproj
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/RPST.vbproj.user
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/Settings.vb
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/Utilities.vb
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST.sln
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-09 03:03:41.000000 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-09 03:03:41.000000 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:03:41.000000 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-09 03:03:41.000000 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-09 03:03:41.000000 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-09 03:03:41.000000 reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/rpst/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/rpst/__main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-09 03:03:31.000000 reddit-post-scraping-tool-1.6.0.0/rpst/__rpst_.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:03:41.268901 reddit-post-scraping-tool-1.6.0.0/setup.cfg
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `reddit-post-scraping-tool-1.6.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `reddit-post-scraping-tool-1.6.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/.github/dependabot.yml` & `reddit-post-scraping-tool-1.6.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/.github/workflows/codeql.yml` & `reddit-post-scraping-tool-1.6.0.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/.github/workflows/python-publish.yml` & `reddit-post-scraping-tool-1.6.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/.gitignore` & `reddit-post-scraping-tool-1.6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/LICENSE` & `reddit-post-scraping-tool-1.6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/PKG-INFO` & `reddit-post-scraping-tool-1.6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-post-scraping-tool
-Version: 1.5.0.0
+Version: 1.6.0.0
 Summary: Given a subreddit name and a keyword, RPST returns all top (by default) posts that contain the specified keyword.
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Richard Mwewa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,17 +40,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPST (Reddit Post Scraping Tool)
 Given a subreddit name and a keyword, RPST will return all posts from a specified listing (default is 'top') that contain the provided keyword.
 
 [![Upload Python Package](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
-![2023-08-08_07-04](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/10d91093-7b24-4de9-9f02-454b842d6b8e)
-![2023-08-08_07-04_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/268a4c0e-d849-49a3-94ba-296d193774e1)
-
+![2023-08-09_04-05](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d8917a35-3eac-44ce-aa96-1f9685095254)
+![2023-08-09_04-05_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d2fe7269-91d4-49ad-87fb-44282c5637a7)
+***
 
 # ✅ Features
 ## GUI
 - [x] Dark mode (Right-click)
 - [x] Saves results to a JSON (Right-click)
 - [x] Logs errors to a file
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reddit-post-scraping-tool Version: 1.5.0.0 Summary:
+Metadata-Version: 2.1 Name: reddit-post-scraping-tool Version: 1.6.0.0 Summary:
 Given a subreddit name and a keyword, RPST returns all top (by default) posts
 that contain the specified keyword. Author-email: Richard Mwewa
 duck.com> License: MIT License Copyright (c) 2023 Richard Mwewa Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -31,18 +31,18 @@
 tool/actions/workflows/python-publish.yml/badge.svg)](https://github.com/
 rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml) [!
 [CodeQL](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/
 workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-
 scraping-tool/actions/workflows/codeql.yml) ![.Net](https://img.shields.io/
 badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white) ![Python](https://
 img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54) !
-[2023-08-08_07-04](https://github.com/bellingcat/reddit-post-scraping-tool/
-assets/74001397/10d91093-7b24-4de9-9f02-454b842d6b8e) ![2023-08-08_07-04_1]
+[2023-08-09_04-05](https://github.com/bellingcat/reddit-post-scraping-tool/
+assets/74001397/d8917a35-3eac-44ce-aa96-1f9685095254) ![2023-08-09_04-05_1]
 (https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/
-268a4c0e-d849-49a3-94ba-296d193774e1) # â Features ## GUI - [x] Dark mode
+d2fe7269-91d4-49ad-87fb-44282c5637a7) *** # â Features ## GUI - [x] Dark mode
 (Right-click) - [x] Saves results to a JSON (Right-click) - [x] Logs errors to
 a file ## CLI - [x] Saves results to a JSON (-j/--json) - [x] Automatically
 checks for new updates. Notifies user if update were found. # ð TODO ## GUI
 - [ ] Make it installable with a setup.exe/setup.msi file. - [x] Add manual
 dark mode option, that will be persistent in all sessions - [ ] Make it save
 results to a CSV file # ð Wiki [Refer to the Wiki](https://github.com/
 rly0nheart/reddit-post-scraping-tool/wiki) for installation instructions, in
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/README.md` & `reddit-post-scraping-tool-1.6.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # RPST (Reddit Post Scraping Tool)
 Given a subreddit name and a keyword, RPST will return all posts from a specified listing (default is 'top') that contain the provided keyword.
 
 [![Upload Python Package](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
-![2023-08-08_07-04](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/10d91093-7b24-4de9-9f02-454b842d6b8e)
-![2023-08-08_07-04_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/268a4c0e-d849-49a3-94ba-296d193774e1)
-
+![2023-08-09_04-05](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d8917a35-3eac-44ce-aa96-1f9685095254)
+![2023-08-09_04-05_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d2fe7269-91d4-49ad-87fb-44282c5637a7)
+***
 
 # ✅ Features
 ## GUI
 - [x] Dark mode (Right-click)
 - [x] Saves results to a JSON (Right-click)
 - [x] Logs errors to a file
```

#### html2text {}

```diff
@@ -4,21 +4,21 @@
 reddit-post-scraping-tool/actions/workflows/python-publish.yml/badge.svg)]
 (https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/
 python-publish.yml) [![CodeQL](https://github.com/rly0nheart/reddit-post-
 scraping-tool/actions/workflows/codeql.yml/badge.svg)](https://github.com/
 rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml) ![.Net]
 (https://img.shields.io/badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white)
 ![Python](https://img.shields.io/badge/python-
-3670A0?style=flat&logo=python&logoColor=ffdd54) ![2023-08-08_07-04](https://
-github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/10d91093-7b24-
-4de9-9f02-454b842d6b8e) ![2023-08-08_07-04_1](https://github.com/bellingcat/
-reddit-post-scraping-tool/assets/74001397/268a4c0e-d849-49a3-94ba-296d193774e1)
-# â Features ## GUI - [x] Dark mode (Right-click) - [x] Saves results to a
-JSON (Right-click) - [x] Logs errors to a file ## CLI - [x] Saves results to a
-JSON (-j/--json) - [x] Automatically checks for new updates. Notifies user if
+3670A0?style=flat&logo=python&logoColor=ffdd54) ![2023-08-09_04-05](https://
+github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d8917a35-3eac-
+44ce-aa96-1f9685095254) ![2023-08-09_04-05_1](https://github.com/bellingcat/
+reddit-post-scraping-tool/assets/74001397/d2fe7269-91d4-49ad-87fb-44282c5637a7)
+*** # â Features ## GUI - [x] Dark mode (Right-click) - [x] Saves results to
+a JSON (Right-click) - [x] Logs errors to a file ## CLI - [x] Saves results to
+a JSON (-j/--json) - [x] Automatically checks for new updates. Notifies user if
 update were found. # ð TODO ## GUI - [ ] Make it installable with a
 setup.exe/setup.msi file. - [x] Add manual dark mode option, that will be
 persistent in all sessions - [ ] Make it save results to a CSV file # ð Wiki
 [Refer to the Wiki](https://github.com/rly0nheart/reddit-post-scraping-tool/
 wiki) for installation instructions, in addition to all other documentation. #
 ð Donations If you like `RPST` and would like to show support, you can Buy A
 Coffee for the developer using the button below [Buy_Me_A_Coffee] Your support
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/AboutBox.Designer.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/AboutBox.Designer.vb`

 * *Files 4% similar despite different names*

```diff
@@ -36,91 +36,91 @@
         ' 
         ' PictureBoxLogo
         ' 
         PictureBoxLogo.BackColor = Color.Transparent
         PictureBoxLogo.Image = CType(resources.GetObject("PictureBoxLogo.Image"), Image)
         PictureBoxLogo.Location = New Point(12, 12)
         PictureBoxLogo.Name = "PictureBoxLogo"
-        PictureBoxLogo.Size = New Size(99, 111)
+        PictureBoxLogo.Size = New Size(88, 93)
         PictureBoxLogo.SizeMode = PictureBoxSizeMode.StretchImage
         PictureBoxLogo.TabIndex = 0
         PictureBoxLogo.TabStop = False
         ' 
         ' LabelProgramName
         ' 
         LabelProgramName.AutoSize = True
-        LabelProgramName.Font = New Font("Ink Free", 14.25F, FontStyle.Bold, GraphicsUnit.Point)
+        LabelProgramName.Font = New Font("Segoe Script", 9.75F, FontStyle.Bold, GraphicsUnit.Point)
         LabelProgramName.ForeColor = SystemColors.ControlText
-        LabelProgramName.Location = New Point(4, 11)
+        LabelProgramName.Location = New Point(3, 15)
         LabelProgramName.Name = "LabelProgramName"
-        LabelProgramName.Size = New Size(60, 23)
+        LabelProgramName.Size = New Size(48, 20)
         LabelProgramName.TabIndex = 3
         LabelProgramName.Text = "Name"
         ' 
         ' LabelProgramDescription
         ' 
         LabelProgramDescription.AutoSize = True
         LabelProgramDescription.Font = New Font("Segoe UI Semibold", 9F, FontStyle.Bold, GraphicsUnit.Point)
         LabelProgramDescription.ForeColor = SystemColors.ControlText
-        LabelProgramDescription.Location = New Point(4, 54)
+        LabelProgramDescription.Location = New Point(3, 43)
         LabelProgramDescription.Name = "LabelProgramDescription"
         LabelProgramDescription.Size = New Size(68, 15)
         LabelProgramDescription.TabIndex = 4
         LabelProgramDescription.Text = "Description"
         ' 
         ' LabelVersion
         ' 
         LabelVersion.AutoSize = True
         LabelVersion.Font = New Font("Segoe UI", 9F, FontStyle.Underline, GraphicsUnit.Point)
         LabelVersion.ForeColor = SystemColors.ControlText
-        LabelVersion.Location = New Point(372, 17)
+        LabelVersion.Location = New Point(347, 17)
         LabelVersion.Name = "LabelVersion"
         LabelVersion.Size = New Size(45, 15)
         LabelVersion.TabIndex = 5
         LabelVersion.Text = "Version"
         ' 
         ' LinkLabelReadtheWiki
         ' 
         LinkLabelReadtheWiki.AutoSize = True
         LinkLabelReadtheWiki.Font = New Font("Segoe UI", 9F, FontStyle.Regular, GraphicsUnit.Point)
-        LinkLabelReadtheWiki.Location = New Point(337, 54)
+        LinkLabelReadtheWiki.Location = New Point(313, 43)
         LinkLabelReadtheWiki.Name = "LinkLabelReadtheWiki"
         LinkLabelReadtheWiki.Size = New Size(79, 15)
         LinkLabelReadtheWiki.TabIndex = 6
         LinkLabelReadtheWiki.TabStop = True
         LinkLabelReadtheWiki.Text = "Read the Wiki"
         ' 
         ' Panel1
         ' 
         Panel1.BackColor = SystemColors.Control
         Panel1.Controls.Add(LabelProgramDescription)
         Panel1.Controls.Add(LabelProgramName)
         Panel1.Controls.Add(LinkLabelReadtheWiki)
         Panel1.Controls.Add(LabelVersion)
-        Panel1.Location = New Point(117, 12)
+        Panel1.Location = New Point(106, 12)
         Panel1.Name = "Panel1"
-        Panel1.Size = New Size(440, 111)
+        Panel1.Size = New Size(409, 93)
         Panel1.TabIndex = 7
         ' 
         ' LicenseRichTextBox
         ' 
         LicenseRichTextBox.Font = New Font("Cambria", 9.75F, FontStyle.Regular, GraphicsUnit.Point)
-        LicenseRichTextBox.Location = New Point(12, 135)
+        LicenseRichTextBox.Location = New Point(12, 113)
         LicenseRichTextBox.Name = "LicenseRichTextBox"
         LicenseRichTextBox.ReadOnly = True
-        LicenseRichTextBox.Size = New Size(545, 305)
+        LicenseRichTextBox.Size = New Size(503, 329)
         LicenseRichTextBox.TabIndex = 1
         LicenseRichTextBox.Text = "License notice"
         ' 
         ' AboutBox
         ' 
         AutoScaleDimensions = New SizeF(7F, 15F)
         AutoScaleMode = AutoScaleMode.Font
         BackColor = Color.Gainsboro
-        ClientSize = New Size(569, 454)
+        ClientSize = New Size(526, 453)
         Controls.Add(LicenseRichTextBox)
         Controls.Add(Panel1)
         Controls.Add(PictureBoxLogo)
         FormBorderStyle = FormBorderStyle.FixedSingle
         Icon = CType(resources.GetObject("$this.Icon"), Icon)
         MaximizeBox = False
         MinimizeBox = False
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/AboutBox.resx` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/AboutBox.resx`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/AboutBox.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/AboutBox.vb`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     ''' <param name="e">The event data.</param>
     Private Sub AboutBox_Load(sender As Object, e As EventArgs) Handles MyBase.Load
         settings.LoadSettings()
         settings.ToggleDarkMode(settings.DarkMode)
 
         LabelProgramName.Text = My.Application.Info.ProductName
         LabelProgramDescription.Text = "Given a subreddit name and a keyword,
-RPST returns all top posts
-(by default) that contain the specified keyword."
+RPST returns all top posts (by default)
+that contain the specified keyword."
         LabelVersion.Text = $"v{My.Application.Info.Version}"
         LicenseRichTextBox.Text = LicenseText
     End Sub
 
     ''' <summary>
     ''' Handles the LinkClicked event for the LinkLabelReadtheWiki control. 
     ''' Opens the Wiki URL in the default browser.
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ApiHandler.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/ApiHandler.vb`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/ApplicationEvents.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/ApplicationEvents.vb`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DataGridViewHandler.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DataGridViewHandler.vb`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,36 @@
     ''' </summary>
     ''' <param name="dataGridView">The DataGridView to be initialized.</param>
     Public Shared Sub AddColumn(dataGridView As DataGridView)
         ' Clear the Columns and Rows before adding Items to them 
         dataGridView.Rows.Clear()
         dataGridView.Columns.Clear()
 
-        dataGridView.Columns.Add("PostCount", "Index")
-        dataGridView.Columns.Add("PostAuthor", "Author")
-        dataGridView.Columns.Add("PostID", "Post ID")
-        dataGridView.Columns.Add("PostText", "Post Text")
-        dataGridView.Columns.Add("PostSubreddit", "Subreddit")
-        dataGridView.Columns.Add("SubredditVisibility", "Subreddit Visibility")
-        dataGridView.Columns.Add("PostThumbnail", "Thumbnail")
+        dataGridView.Columns.Add("PostCount", "INDEX")
+        dataGridView.Columns.Add("PostAuthor", "AUTHOR")
+        dataGridView.Columns.Add("PostID", "ID")
+        dataGridView.Columns.Add("PostText", "TEXT")
+        dataGridView.Columns.Add("PostSubreddit", "SUBREDDIT")
+        dataGridView.Columns.Add("SubredditVisibility", "VISIBILITY")
+        dataGridView.Columns.Add("PostThumbnail", "THUMBNAIL")
         dataGridView.Columns.Add("PostIsNSFW", "NSFW")
-        dataGridView.Columns.Add("PostIsGilded", "Gilded")
-        dataGridView.Columns.Add("PostUpvotes", "Upvotes")
-        dataGridView.Columns.Add("PostUpvoteRatio", "Upvote Ratio")
-        dataGridView.Columns.Add("PostDownvotes", "Downvotes")
-        dataGridView.Columns.Add("PostAwards", "Awards")
-        dataGridView.Columns.Add("PostTopAward", "Top Award")
-        dataGridView.Columns.Add("PostIsCrosspostable", "Is Crosspostable?")
-        dataGridView.Columns.Add("PostScore", "Score")
-        dataGridView.Columns.Add("PostCategory", "Category")
-        dataGridView.Columns.Add("PostDomain", "Domain")
-        dataGridView.Columns.Add("PostPermalink", "Permalink")
-        dataGridView.Columns.Add("PostCreatedAt", "Created At")
-        dataGridView.Columns.Add("PostApprovedAt", "Approved At")
-        dataGridView.Columns.Add("PostApprovedBy", "Approved By")
+        dataGridView.Columns.Add("PostIsGilded", "GILDED")
+        dataGridView.Columns.Add("PostUpvotes", "UPVOTES")
+        dataGridView.Columns.Add("PostUpvoteRatio", "UPVOTE RATIO")
+        dataGridView.Columns.Add("PostDownvotes", "DOWNVOTES")
+        dataGridView.Columns.Add("PostAwards", "AWARDS")
+        dataGridView.Columns.Add("PostTopAward", "TOP AWARD")
+        dataGridView.Columns.Add("PostIsCrosspostable", "IS CROSS-POSTABLE?")
+        dataGridView.Columns.Add("PostScore", "SCORE")
+        dataGridView.Columns.Add("PostCategory", "CATEGORY")
+        dataGridView.Columns.Add("PostDomain", "DOMAIN")
+        dataGridView.Columns.Add("PostPermalink", "PERMALINK")
+        dataGridView.Columns.Add("PostCreatedAt", "CREATED AT")
+        dataGridView.Columns.Add("PostApprovedAt", "APPROVED ATt")
+        dataGridView.Columns.Add("PostApprovedBy", "APPROVED BY")
     End Sub
 
     Public Shared Sub AddRow(dataGridView As DataGridView, post As JObject, postNumber As Integer)
         ''' <summary>
         ''' Adds a row to the DataGridView based on the data from a Reddit post.
         ''' </summary>
         ''' <param name="dataGridView">The DataGridView to which the row will be added.</param>
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DeveloperBox.Designer.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DeveloperBox.Designer.vb`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DeveloperBox.resx` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DeveloperBox.resx`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/DeveloperBox.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/DeveloperBox.vb`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/LICENSE` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Application.Designer.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Application.Designer.vb`

 * *Files 9% similar despite different names*

```diff
@@ -29,11 +29,11 @@
             Me.SaveMySettingsOnExit = true
             Me.ShutDownStyle = Global.Microsoft.VisualBasic.ApplicationServices.ShutdownMode.AfterMainFormCloses
             Me.HighDpiMode = HighDpiMode.DpiUnaware
         End Sub
         
         <Global.System.Diagnostics.DebuggerStepThroughAttribute()>  _
         Protected Overrides Sub OnCreateMainForm()
-            Me.MainForm = Global.RPST.StartForm
+            Me.MainForm = Global.RPST.FormMain
         End Sub
     End Class
 End Namespace
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Resources.Designer.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Resources.Designer.vb`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/My Project/Resources.resx` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/My Project/Resources.resx`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/PostsProcessor.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/PostsProcessor.vb`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/README.md` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # RPST (Reddit Post Scraping Tool)
 Given a subreddit name and a keyword, RPST will return all posts from a specified listing (default is 'top') that contain the provided keyword.
 
 [![Upload Python Package](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
-![2023-08-08_07-04](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/10d91093-7b24-4de9-9f02-454b842d6b8e)
-![2023-08-08_07-04_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/268a4c0e-d849-49a3-94ba-296d193774e1)
-
+![2023-08-09_04-05](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d8917a35-3eac-44ce-aa96-1f9685095254)
+![2023-08-09_04-05_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d2fe7269-91d4-49ad-87fb-44282c5637a7)
+***
 
 # ✅ Features
 ## GUI
 - [x] Dark mode (Right-click)
 - [x] Saves results to a JSON (Right-click)
 - [x] Logs errors to a file
```

#### html2text {}

```diff
@@ -4,21 +4,21 @@
 reddit-post-scraping-tool/actions/workflows/python-publish.yml/badge.svg)]
 (https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/
 python-publish.yml) [![CodeQL](https://github.com/rly0nheart/reddit-post-
 scraping-tool/actions/workflows/codeql.yml/badge.svg)](https://github.com/
 rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml) ![.Net]
 (https://img.shields.io/badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white)
 ![Python](https://img.shields.io/badge/python-
-3670A0?style=flat&logo=python&logoColor=ffdd54) ![2023-08-08_07-04](https://
-github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/10d91093-7b24-
-4de9-9f02-454b842d6b8e) ![2023-08-08_07-04_1](https://github.com/bellingcat/
-reddit-post-scraping-tool/assets/74001397/268a4c0e-d849-49a3-94ba-296d193774e1)
-# â Features ## GUI - [x] Dark mode (Right-click) - [x] Saves results to a
-JSON (Right-click) - [x] Logs errors to a file ## CLI - [x] Saves results to a
-JSON (-j/--json) - [x] Automatically checks for new updates. Notifies user if
+3670A0?style=flat&logo=python&logoColor=ffdd54) ![2023-08-09_04-05](https://
+github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d8917a35-3eac-
+44ce-aa96-1f9685095254) ![2023-08-09_04-05_1](https://github.com/bellingcat/
+reddit-post-scraping-tool/assets/74001397/d2fe7269-91d4-49ad-87fb-44282c5637a7)
+*** # â Features ## GUI - [x] Dark mode (Right-click) - [x] Saves results to
+a JSON (Right-click) - [x] Logs errors to a file ## CLI - [x] Saves results to
+a JSON (-j/--json) - [x] Automatically checks for new updates. Notifies user if
 update were found. # ð TODO ## GUI - [ ] Make it installable with a
 setup.exe/setup.msi file. - [x] Add manual dark mode option, that will be
 persistent in all sessions - [ ] Make it save results to a CSV file # ð Wiki
 [Refer to the Wiki](https://github.com/rly0nheart/reddit-post-scraping-tool/
 wiki) for installation instructions, in addition to all other documentation. #
 ð Donations If you like `RPST` and would like to show support, you can Buy A
 Coffee for the developer using the button below [Buy_Me_A_Coffee] Your support
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/RPST.vbproj` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/RPST.vbproj`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     <TargetFramework>net6.0-windows</TargetFramework>
     <StartupObject>RPST.My.MyApplication</StartupObject>
     <UseWindowsForms>true</UseWindowsForms>
     <MyType>WindowsForms</MyType>
     <ApplicationIcon>icon.ico</ApplicationIcon>
     <Company>Bellingcat</Company>
     <Description>Given a subreddit name and a keyword, RPST (Reddit Post Scraping Tool) returns all top (by default) posts that contain the specified keyword. </Description>
-    <Copyright>Copyright (c) 2023-2024 Richard Mwewa</Copyright>
+    <Copyright>Copyright (c) 2023 Richard Mwewa</Copyright>
     <PackageProjectUrl>https://github.com/bellingcat/reddit-post-scraping-tool</PackageProjectUrl>
     <PackageReadmeFile>README.md</PackageReadmeFile>
     <RepositoryUrl>https://github.com/bellingcat/reddit-post-scraping-tool</RepositoryUrl>
-    <AssemblyVersion>1.5.0.0</AssemblyVersion>
-    <FileVersion>1.5.0.0</FileVersion>
+    <AssemblyVersion>1.6.0.0</AssemblyVersion>
+    <FileVersion>1.6.0.0</FileVersion>
     <PackageLicenseFile>LICENSE</PackageLicenseFile>
     <PackageRequireLicenseAcceptance>True</PackageRequireLicenseAcceptance>
-    <Version>1.5.0</Version>
+    <Version>1.6.0</Version>
     <PackageTags>reddit;scraper;reddit-scraper;osint</PackageTags>
     <PackageReleaseNotes></PackageReleaseNotes>
     <AnalysisLevel>6.0-recommended</AnalysisLevel>
     <PackageId>RPST</PackageId>
     <Authors>Richard Mwewa</Authors>
     <NeutralLanguage>en</NeutralLanguage>
     <Product>$(AssemblyName) (Reddit Post Scraping Tool)</Product>
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/Settings.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/Settings.vb`

 * *Files 22% similar despite different names*

```diff
@@ -21,24 +21,24 @@
         ' Check if the settings.json file exists
         ' and load the configurations from it
         If File.Exists(settingsFilePath) Then
             Dim json As String = File.ReadAllText(settingsFilePath)
             Dim options As New JsonSerializerOptions With {.PropertyNameCaseInsensitive = True}
             Dim settings = Text.Json.JsonSerializer.Deserialize(Of SettingsManager)(json, options)
             Me.DarkMode = settings.DarkMode
-            StartForm.ToolStripMenuItemDarkMode.Checked = settings.DarkMode
+            FormMain.ToolStripMenuItemDarkMode.Checked = settings.DarkMode
         Else
             ' Settings file does not exist
             ' Create a new file with default settings 'False'
             Dim defaultSettings = New SettingsManager With {.DarkMode = False}
             Dim jsonOutput = Text.Json.JsonSerializer.Serialize(defaultSettings)
             File.WriteAllText(settingsFilePath, jsonOutput)
 
             Me.DarkMode = False
-            StartForm.ToolStripMenuItemDarkMode.Checked = False
+            FormMain.ToolStripMenuItemDarkMode.Checked = False
         End If
     End Sub
 
 
     ''' <summary>
     ''' Toggles the Dark Mode setting on or off based on the provided parameter.
     ''' </summary>
@@ -67,56 +67,54 @@
     ''' If Dark Mode is enabled, a dark theme is applied. If it's disabled, a light theme is set.
     ''' </summary>
     Public Sub ApplyTheme()
         Dim DarkMode As Boolean = GetDarkMode()
         If DarkMode Then
             ' Enable dark mode for the Main form
             ' Background colours (I know 'Colours'/'Colors'😆)
-            StartForm.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.SubredditTextBox.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
-            StartForm.KeywordTextBox.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
-            StartForm.LimitNumericUpDown.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
-            StartForm.LimitNumericUpDown.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
-            StartForm.ListingComboBox.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
-            StartForm.TimeframeComboBox.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
-            ' Foreground colours
-            StartForm.KeywordTextBox.ForeColor = SystemColors.Control
-            StartForm.SubredditTextBox.ForeColor = SystemColors.Control
-            StartForm.LimitNumericUpDown.ForeColor = SystemColors.Control
-            StartForm.LimitNumericUpDown.ForeColor = SystemColors.Control
-            StartForm.ListingComboBox.ForeColor = SystemColors.Control
-            StartForm.TimeframeComboBox.ForeColor = SystemColors.Control
-            StartForm.LabelRPST.ForeColor = SystemColors.Control
-            StartForm.LabelKeyword.ForeColor = SystemColors.Control
-            StartForm.LabelSubreddit.ForeColor = SystemColors.Control
-            StartForm.LabelLimit.ForeColor = SystemColors.Control
-            StartForm.LabelListing.ForeColor = SystemColors.Control
-            StartForm.LabelTimeframe.ForeColor = SystemColors.Control
+            FormMain.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.TextBoxSubreddit.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
+            FormMain.TextBoxKeyword.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
+            FormMain.NumericUpDownLimit.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
+            FormMain.NumericUpDownLimit.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
+            FormMain.ComboBoxListing.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
+            FormMain.ComboBoxTimeframe.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
+            ' Foreground colours
+            FormMain.TextBoxKeyword.ForeColor = SystemColors.Control
+            FormMain.TextBoxSubreddit.ForeColor = SystemColors.Control
+            FormMain.NumericUpDownLimit.ForeColor = SystemColors.Control
+            FormMain.NumericUpDownLimit.ForeColor = SystemColors.Control
+            FormMain.ComboBoxListing.ForeColor = SystemColors.Control
+            FormMain.ComboBoxTimeframe.ForeColor = SystemColors.Control
+            FormMain.LabelKeyword.ForeColor = SystemColors.Control
+            FormMain.LabelSubreddit.ForeColor = SystemColors.Control
+            FormMain.LabelLimit.ForeColor = SystemColors.Control
+            FormMain.LabelListing.ForeColor = SystemColors.Control
+            FormMain.LabelTimeframe.ForeColor = SystemColors.Control
 
-            ResultsForm.BackColor = ColorTranslator.FromHtml("#FF121212")
 
             ' Enable dark mode on 'Right Click Menu' items
             ' Background colours
-            StartForm.ToolStripMenuItemDarkMode.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemSavePosts.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemtoJSON.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemtoCSV.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemAbout.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemDeveloper.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemCheckUpdates.BackColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ToolStripMenuItemQuit.BackColor = ColorTranslator.FromHtml("#FF121212")
-            ' Foreground colours
-            StartForm.ToolStripMenuItemDarkMode.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemSavePosts.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemtoJSON.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemtoCSV.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemAbout.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemDeveloper.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemCheckUpdates.ForeColor = SystemColors.Control
-            StartForm.ToolStripMenuItemQuit.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemDarkMode.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemSavePosts.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemtoJSON.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemtoCSV.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemAbout.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemDeveloper.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemCheckUpdates.BackColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ToolStripMenuItemQuit.BackColor = ColorTranslator.FromHtml("#FF121212")
+            ' Foreground colours
+            FormMain.ToolStripMenuItemDarkMode.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemSavePosts.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemtoJSON.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemtoCSV.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemAbout.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemDeveloper.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemCheckUpdates.ForeColor = SystemColors.Control
+            FormMain.ToolStripMenuItemQuit.ForeColor = SystemColors.Control
 
 
             ' Enable dark mode for the About box
             ' Background colours
             AboutBox.BackColor = ColorTranslator.FromHtml("#FF121212")
             AboutBox.LicenseRichTextBox.BackColor = ColorTranslator.FromHtml("#FF2E2E2E")
             AboutBox.Panel1.BackColor = ColorTranslator.FromHtml("#FF121212")
@@ -124,58 +122,57 @@
             AboutBox.ForeColor = SystemColors.Control
             AboutBox.LicenseRichTextBox.ForeColor = SystemColors.Control
             AboutBox.LabelProgramName.ForeColor = SystemColors.Control
             AboutBox.LabelProgramDescription.ForeColor = SystemColors.Control
             AboutBox.LabelVersion.ForeColor = SystemColors.Control
 
             ' If dark mode is enabled, set the 'Dark Mode' text value to 'Light mode'
-            StartForm.ToolStripMenuItemDarkMode.Text = "Light Mode"
+            FormMain.ToolStripMenuItemDarkMode.Text = "Light Mode"
         Else
             ' Disable dark mode for the Main Form
             ' Background colours
-            StartForm.BackColor = Color.Gainsboro
-            StartForm.KeywordTextBox.BackColor = SystemColors.Control
-            StartForm.SubredditTextBox.BackColor = SystemColors.Control
-            StartForm.LimitNumericUpDown.BackColor = SystemColors.Control
-            StartForm.LimitNumericUpDown.BackColor = SystemColors.Control
-            StartForm.TimeframeComboBox.BackColor = SystemColors.Control
-            StartForm.ListingComboBox.BackColor = SystemColors.Control
-            ' Foreground colours
-            StartForm.KeywordTextBox.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.SubredditTextBox.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LimitNumericUpDown.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LimitNumericUpDown.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.ListingComboBox.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.TimeframeComboBox.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LabelRPST.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LabelKeyword.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LabelSubreddit.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LabelLimit.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LabelListing.ForeColor = ColorTranslator.FromHtml("#FF121212")
-            StartForm.LabelTimeframe.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.BackColor = Color.Gainsboro
+            FormMain.TextBoxKeyword.BackColor = SystemColors.Control
+            FormMain.TextBoxSubreddit.BackColor = SystemColors.Control
+            FormMain.NumericUpDownLimit.BackColor = SystemColors.Control
+            FormMain.NumericUpDownLimit.BackColor = SystemColors.Control
+            FormMain.ComboBoxTimeframe.BackColor = SystemColors.Control
+            FormMain.ComboBoxListing.BackColor = SystemColors.Control
+            ' Foreground colours
+            FormMain.TextBoxKeyword.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.TextBoxSubreddit.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.NumericUpDownLimit.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.NumericUpDownLimit.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ComboBoxListing.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.ComboBoxTimeframe.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.LabelKeyword.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.LabelSubreddit.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.LabelLimit.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.LabelListing.ForeColor = ColorTranslator.FromHtml("#FF121212")
+            FormMain.LabelTimeframe.ForeColor = ColorTranslator.FromHtml("#FF121212")
 
             ' Disable dark mode on 'Right Click Menu' items
             ' Background colours
-            StartForm.ToolStripMenuItemDarkMode.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemSavePosts.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemtoJSON.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemtoCSV.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemAbout.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemDeveloper.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemCheckUpdates.BackColor = Color.Gainsboro
-            StartForm.ToolStripMenuItemQuit.BackColor = Color.Gainsboro
-            ' Foreground colours
-            StartForm.ToolStripMenuItemDarkMode.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemSavePosts.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemtoJSON.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemtoCSV.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemAbout.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemDeveloper.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemCheckUpdates.ForeColor = Color.Black
-            StartForm.ToolStripMenuItemQuit.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemDarkMode.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemSavePosts.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemtoJSON.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemtoCSV.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemAbout.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemDeveloper.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemCheckUpdates.BackColor = Color.Gainsboro
+            FormMain.ToolStripMenuItemQuit.BackColor = Color.Gainsboro
+            ' Foreground colours
+            FormMain.ToolStripMenuItemDarkMode.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemSavePosts.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemtoJSON.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemtoCSV.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemAbout.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemDeveloper.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemCheckUpdates.ForeColor = Color.Black
+            FormMain.ToolStripMenuItemQuit.ForeColor = Color.Black
 
             ' Disable dark mode for the About box
             ' Background colours
             AboutBox.BackColor = Color.Gainsboro
             AboutBox.ForeColor = SystemColors.WindowText
             AboutBox.LicenseRichTextBox.BackColor = SystemColors.Control
             AboutBox.LicenseRichTextBox.ForeColor = SystemColors.WindowText
@@ -183,15 +180,15 @@
             ' Foreground colours
             AboutBox.Panel1.ForeColor = SystemColors.WindowText
             AboutBox.LabelProgramName.ForeColor = SystemColors.WindowText
             AboutBox.LabelProgramDescription.ForeColor = SystemColors.WindowText
             AboutBox.LabelVersion.ForeColor = SystemColors.WindowText
 
             ' If dark mode is disabled, set the 'Light Mode' text value to 'Dark Mode'
-            StartForm.ToolStripMenuItemDarkMode.Text = "Dark Mode"
+            FormMain.ToolStripMenuItemDarkMode.Text = "Dark Mode"
         End If
     End Sub
 
 
     ''' <summary>
     ''' Retrieves the Dark Mode setting value from 'settings.json'. 
     ''' If the settings file doesn't exist, defaults to returning 'False' (Dark Mode off).
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/StartForm.Designer.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormMain.Designer.vb`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ﻿<Global.Microsoft.VisualBasic.CompilerServices.DesignerGenerated()>
-Partial Class StartForm
+Partial Class FormMain
     Inherits System.Windows.Forms.Form
 
     'Form overrides dispose to clean up the component list.
     <System.Diagnostics.DebuggerNonUserCode()>
     Protected Overrides Sub Dispose(ByVal disposing As Boolean)
         Try
             If disposing AndAlso components IsNot Nothing Then
@@ -19,139 +19,148 @@
 
     'NOTE: The following procedure is required by the Windows Form Designer
     'It can be modified using the Windows Form Designer.  
     'Do not modify it using the code editor.
     <System.Diagnostics.DebuggerStepThrough()>
     Private Sub InitializeComponent()
         components = New ComponentModel.Container()
-        Dim resources As ComponentModel.ComponentResourceManager = New ComponentModel.ComponentResourceManager(GetType(StartForm))
-        KeywordTextBox = New TextBox()
-        SubredditTextBox = New TextBox()
+        Dim resources As ComponentModel.ComponentResourceManager = New ComponentModel.ComponentResourceManager(GetType(FormMain))
+        TextBoxKeyword = New TextBox()
+        TextBoxSubreddit = New TextBox()
         ButtonScrape = New Button()
-        TimeframeComboBox = New ComboBox()
-        ListingComboBox = New ComboBox()
+        ComboBoxTimeframe = New ComboBox()
+        ComboBoxListing = New ComboBox()
         LabelKeyword = New Label()
         LabelSubreddit = New Label()
         LabelLimit = New Label()
         LabelListing = New Label()
         LabelTimeframe = New Label()
         ContextMenuStripRightClick = New ContextMenuStrip(components)
         ToolStripMenuItemDarkMode = New ToolStripMenuItem()
         ToolStripMenuItemSavePosts = New ToolStripMenuItem()
         ToolStripMenuItemtoJSON = New ToolStripMenuItem()
         ToolStripMenuItemtoCSV = New ToolStripMenuItem()
         ToolStripMenuItemAbout = New ToolStripMenuItem()
         ToolStripMenuItemDeveloper = New ToolStripMenuItem()
         ToolStripMenuItemCheckUpdates = New ToolStripMenuItem()
         ToolStripMenuItemQuit = New ToolStripMenuItem()
-        LimitNumericUpDown = New NumericUpDown()
-        PictureBoxLogo = New PictureBox()
-        LabelRPST = New Label()
+        NumericUpDownLimit = New NumericUpDown()
+        ToolTip = New ToolTip(components)
         ContextMenuStripRightClick.SuspendLayout()
-        CType(LimitNumericUpDown, ComponentModel.ISupportInitialize).BeginInit()
-        CType(PictureBoxLogo, ComponentModel.ISupportInitialize).BeginInit()
+        CType(NumericUpDownLimit, ComponentModel.ISupportInitialize).BeginInit()
         SuspendLayout()
         ' 
-        ' KeywordTextBox
+        ' TextBoxKeyword
         ' 
-        KeywordTextBox.BackColor = SystemColors.Window
-        KeywordTextBox.ForeColor = SystemColors.WindowText
-        KeywordTextBox.Location = New Point(159, 75)
-        KeywordTextBox.Name = "KeywordTextBox"
-        KeywordTextBox.PlaceholderText = "Keyword"
-        KeywordTextBox.Size = New Size(100, 23)
-        KeywordTextBox.TabIndex = 0
-        ' 
-        ' SubredditTextBox
-        ' 
-        SubredditTextBox.Location = New Point(159, 106)
-        SubredditTextBox.Name = "SubredditTextBox"
-        SubredditTextBox.PlaceholderText = "Subreddit"
-        SubredditTextBox.Size = New Size(100, 23)
-        SubredditTextBox.TabIndex = 4
+        TextBoxKeyword.BackColor = SystemColors.Window
+        TextBoxKeyword.ForeColor = SystemColors.WindowText
+        TextBoxKeyword.Location = New Point(118, 20)
+        TextBoxKeyword.Name = "TextBoxKeyword"
+        TextBoxKeyword.PlaceholderText = "Keyword"
+        TextBoxKeyword.Size = New Size(100, 23)
+        TextBoxKeyword.TabIndex = 0
+        ToolTip.SetToolTip(TextBoxKeyword, "Enter the keyword you want to search for.")
+        ' 
+        ' TextBoxSubreddit
+        ' 
+        TextBoxSubreddit.Location = New Point(118, 49)
+        TextBoxSubreddit.Name = "TextBoxSubreddit"
+        TextBoxSubreddit.PlaceholderText = "Subreddit"
+        TextBoxSubreddit.Size = New Size(100, 23)
+        TextBoxSubreddit.TabIndex = 4
+        ToolTip.SetToolTip(TextBoxSubreddit, "Provide the subreddit to search in.")
         ' 
         ' ButtonScrape
         ' 
-        ButtonScrape.Location = New Point(208, 29)
+        ButtonScrape.Location = New Point(167, 174)
         ButtonScrape.Name = "ButtonScrape"
         ButtonScrape.Size = New Size(51, 28)
         ButtonScrape.TabIndex = 6
         ButtonScrape.Text = "Scrape"
+        ToolTip.SetToolTip(ButtonScrape, "You can also just hit ENTER to start scraping.")
         ButtonScrape.UseVisualStyleBackColor = True
         ' 
-        ' TimeframeComboBox
+        ' ComboBoxTimeframe
         ' 
-        TimeframeComboBox.FormattingEnabled = True
-        TimeframeComboBox.Items.AddRange(New Object() {"Hour", "Day", "Week", "Month", "Year"})
-        TimeframeComboBox.Location = New Point(159, 200)
-        TimeframeComboBox.Name = "TimeframeComboBox"
-        TimeframeComboBox.Size = New Size(100, 23)
-        TimeframeComboBox.TabIndex = 8
-        TimeframeComboBox.Text = "All"
-        ' 
-        ' ListingComboBox
-        ' 
-        ListingComboBox.FormattingEnabled = True
-        ListingComboBox.Items.AddRange(New Object() {"Controversial", "Hot", "Best", "New", "Rising"})
-        ListingComboBox.Location = New Point(159, 168)
-        ListingComboBox.Name = "ListingComboBox"
-        ListingComboBox.Size = New Size(100, 23)
-        ListingComboBox.TabIndex = 9
-        ListingComboBox.Text = "Top"
+        ComboBoxTimeframe.AutoCompleteCustomSource.AddRange(New String() {"Hour", "Day", "Week", "Month", "Year"})
+        ComboBoxTimeframe.AutoCompleteMode = AutoCompleteMode.Append
+        ComboBoxTimeframe.AutoCompleteSource = AutoCompleteSource.CustomSource
+        ComboBoxTimeframe.FormattingEnabled = True
+        ComboBoxTimeframe.Items.AddRange(New Object() {"Hour", "Day", "Week", "Month", "Year"})
+        ComboBoxTimeframe.Location = New Point(118, 136)
+        ComboBoxTimeframe.Name = "ComboBoxTimeframe"
+        ComboBoxTimeframe.Size = New Size(100, 23)
+        ComboBoxTimeframe.TabIndex = 8
+        ComboBoxTimeframe.Text = "All"
+        ToolTip.SetToolTip(ComboBoxTimeframe, "Select the time period for the posts. Default value is `All`.")
+        ' 
+        ' ComboBoxListing
+        ' 
+        ComboBoxListing.AutoCompleteCustomSource.AddRange(New String() {"Controversial", "Hot", "Best", "New", "Rising"})
+        ComboBoxListing.AutoCompleteMode = AutoCompleteMode.Append
+        ComboBoxListing.AutoCompleteSource = AutoCompleteSource.CustomSource
+        ComboBoxListing.FormattingEnabled = True
+        ComboBoxListing.Items.AddRange(New Object() {"Controversial", "Hot", "Best", "New", "Rising"})
+        ComboBoxListing.Location = New Point(118, 107)
+        ComboBoxListing.Name = "ComboBoxListing"
+        ComboBoxListing.Size = New Size(100, 23)
+        ComboBoxListing.TabIndex = 9
+        ComboBoxListing.Text = "Top"
+        ToolTip.SetToolTip(ComboBoxListing, "Choose the type of post listings. Default value is `Top`.")
         ' 
         ' LabelKeyword
         ' 
         LabelKeyword.AutoEllipsis = True
         LabelKeyword.Font = New Font("Segoe UI Semibold", 9F, FontStyle.Bold Or FontStyle.Underline, GraphicsUnit.Point)
         LabelKeyword.ForeColor = Color.Black
-        LabelKeyword.Location = New Point(19, 78)
+        LabelKeyword.Location = New Point(19, 23)
         LabelKeyword.Name = "LabelKeyword"
         LabelKeyword.Size = New Size(71, 20)
         LabelKeyword.TabIndex = 10
         LabelKeyword.Text = "Keyword:"
         ' 
         ' LabelSubreddit
         ' 
         LabelSubreddit.AutoEllipsis = True
         LabelSubreddit.Font = New Font("Segoe UI Semibold", 9F, FontStyle.Bold Or FontStyle.Underline, GraphicsUnit.Point)
         LabelSubreddit.ForeColor = Color.Black
-        LabelSubreddit.Location = New Point(19, 109)
+        LabelSubreddit.Location = New Point(19, 52)
         LabelSubreddit.Name = "LabelSubreddit"
         LabelSubreddit.Size = New Size(71, 23)
         LabelSubreddit.TabIndex = 11
         LabelSubreddit.Text = "Subreddit:"
         ' 
         ' LabelLimit
         ' 
         LabelLimit.AutoEllipsis = True
         LabelLimit.Font = New Font("Segoe UI Semibold", 9F, FontStyle.Bold Or FontStyle.Underline, GraphicsUnit.Point)
         LabelLimit.ForeColor = Color.Black
-        LabelLimit.Location = New Point(19, 137)
+        LabelLimit.Location = New Point(19, 75)
         LabelLimit.Name = "LabelLimit"
         LabelLimit.Size = New Size(56, 23)
         LabelLimit.TabIndex = 12
         LabelLimit.Text = "Limit:"
         ' 
         ' LabelListing
         ' 
         LabelListing.AutoEllipsis = True
         LabelListing.Font = New Font("Segoe UI Semibold", 9F, FontStyle.Bold Or FontStyle.Underline, GraphicsUnit.Point)
         LabelListing.ForeColor = Color.Black
-        LabelListing.Location = New Point(19, 168)
+        LabelListing.Location = New Point(19, 107)
         LabelListing.Name = "LabelListing"
         LabelListing.Size = New Size(56, 23)
         LabelListing.TabIndex = 13
         LabelListing.Text = "Listing:"
         ' 
         ' LabelTimeframe
         ' 
         LabelTimeframe.AutoEllipsis = True
         LabelTimeframe.Font = New Font("Segoe UI Semibold", 9F, FontStyle.Bold Or FontStyle.Underline, GraphicsUnit.Point)
         LabelTimeframe.ForeColor = Color.Black
-        LabelTimeframe.Location = New Point(19, 200)
+        LabelTimeframe.Location = New Point(19, 136)
         LabelTimeframe.Name = "LabelTimeframe"
         LabelTimeframe.Size = New Size(81, 23)
         LabelTimeframe.TabIndex = 14
         LabelTimeframe.Text = "Timeframe:"
         ' 
         ' ContextMenuStripRightClick
         ' 
@@ -224,95 +233,79 @@
         ' 
         ToolStripMenuItemQuit.AutoToolTip = True
         ToolStripMenuItemQuit.Image = CType(resources.GetObject("ToolStripMenuItemQuit.Image"), Image)
         ToolStripMenuItemQuit.Name = "ToolStripMenuItemQuit"
         ToolStripMenuItemQuit.Size = New Size(153, 22)
         ToolStripMenuItemQuit.Text = "Quit"
         ' 
-        ' LimitNumericUpDown
+        ' NumericUpDownLimit
         ' 
-        LimitNumericUpDown.Location = New Point(159, 137)
-        LimitNumericUpDown.Minimum = New Decimal(New Integer() {5, 0, 0, 0})
-        LimitNumericUpDown.Name = "LimitNumericUpDown"
-        LimitNumericUpDown.ReadOnly = True
-        LimitNumericUpDown.Size = New Size(100, 23)
-        LimitNumericUpDown.TabIndex = 15
-        LimitNumericUpDown.Value = New Decimal(New Integer() {10, 0, 0, 0})
-        ' 
-        ' PictureBoxLogo
-        ' 
-        PictureBoxLogo.BackColor = Color.Transparent
-        PictureBoxLogo.Image = CType(resources.GetObject("PictureBoxLogo.Image"), Image)
-        PictureBoxLogo.Location = New Point(19, 12)
-        PictureBoxLogo.Name = "PictureBoxLogo"
-        PictureBoxLogo.Size = New Size(41, 45)
-        PictureBoxLogo.SizeMode = PictureBoxSizeMode.StretchImage
-        PictureBoxLogo.TabIndex = 17
-        PictureBoxLogo.TabStop = False
-        ' 
-        ' LabelRPST
-        ' 
-        LabelRPST.AutoSize = True
-        LabelRPST.BackColor = Color.Transparent
-        LabelRPST.Font = New Font("Ink Free", 9F, FontStyle.Regular, GraphicsUnit.Point)
-        LabelRPST.Location = New Point(50, 51)
-        LabelRPST.Name = "LabelRPST"
-        LabelRPST.Size = New Size(36, 15)
-        LabelRPST.TabIndex = 18
-        LabelRPST.Text = "RPST"
+        NumericUpDownLimit.Location = New Point(118, 78)
+        NumericUpDownLimit.Minimum = New Decimal(New Integer() {5, 0, 0, 0})
+        NumericUpDownLimit.Name = "NumericUpDownLimit"
+        NumericUpDownLimit.ReadOnly = True
+        NumericUpDownLimit.Size = New Size(100, 23)
+        NumericUpDownLimit.TabIndex = 15
+        ToolTip.SetToolTip(NumericUpDownLimit, "Set how many posts you want to go through. Default value is `10`.")
+        NumericUpDownLimit.Value = New Decimal(New Integer() {10, 0, 0, 0})
+        ' 
+        ' ToolTip
+        ' 
+        ToolTip.AutoPopDelay = 5000
+        ToolTip.BackColor = Color.Gainsboro
+        ToolTip.InitialDelay = 500
+        ToolTip.ReshowDelay = 100
+        ToolTip.ToolTipIcon = ToolTipIcon.Info
+        ToolTip.ToolTipTitle = "Tip"
         ' 
-        ' StartForm
+        ' FormMain
         ' 
         AutoScaleDimensions = New SizeF(7F, 15F)
         AutoScaleMode = AutoScaleMode.Font
         BackColor = SystemColors.Control
-        ClientSize = New Size(281, 244)
+        ClientSize = New Size(239, 221)
         ContextMenuStrip = ContextMenuStripRightClick
-        Controls.Add(LabelRPST)
-        Controls.Add(PictureBoxLogo)
-        Controls.Add(TimeframeComboBox)
-        Controls.Add(KeywordTextBox)
+        Controls.Add(ComboBoxTimeframe)
+        Controls.Add(TextBoxKeyword)
         Controls.Add(LabelTimeframe)
         Controls.Add(LabelKeyword)
-        Controls.Add(ListingComboBox)
-        Controls.Add(LimitNumericUpDown)
+        Controls.Add(ComboBoxListing)
+        Controls.Add(NumericUpDownLimit)
         Controls.Add(LabelListing)
         Controls.Add(ButtonScrape)
         Controls.Add(LabelLimit)
         Controls.Add(LabelSubreddit)
-        Controls.Add(SubredditTextBox)
+        Controls.Add(TextBoxSubreddit)
         FormBorderStyle = FormBorderStyle.FixedSingle
         Icon = CType(resources.GetObject("$this.Icon"), Icon)
         MaximizeBox = False
-        Name = "StartForm"
+        Name = "FormMain"
         StartPosition = FormStartPosition.CenterScreen
-        Text = "ProgramName ProgramVersion"
+        Text = "RPST"
         ContextMenuStripRightClick.ResumeLayout(False)
-        CType(LimitNumericUpDown, ComponentModel.ISupportInitialize).EndInit()
-        CType(PictureBoxLogo, ComponentModel.ISupportInitialize).EndInit()
+        CType(NumericUpDownLimit, ComponentModel.ISupportInitialize).EndInit()
         ResumeLayout(False)
         PerformLayout()
     End Sub
 
-    Friend WithEvents KeywordTextBox As TextBox
-    Friend WithEvents SubredditTextBox As TextBox
+    Friend WithEvents TextBoxKeyword As TextBox
+    Friend WithEvents TextBoxSubreddit As TextBox
     Friend WithEvents ButtonScrape As Button
-    Friend WithEvents TimeframeComboBox As ComboBox
-    Friend WithEvents ListingComboBox As ComboBox
+    Friend WithEvents ComboBoxTimeframe As ComboBox
+    Friend WithEvents ComboBoxListing As ComboBox
     Friend WithEvents LabelKeyword As Label
     Friend WithEvents LabelSubreddit As Label
     Friend WithEvents LabelLimit As Label
     Friend WithEvents LabelListing As Label
     Friend WithEvents LabelTimeframe As Label
     Friend WithEvents ContextMenuStripRightClick As ContextMenuStrip
     Friend WithEvents ToolStripMenuItemSavePosts As ToolStripMenuItem
     Friend WithEvents ToolStripMenuItemtoJSON As ToolStripMenuItem
     Friend WithEvents ToolStripMenuItemtoCSV As ToolStripMenuItem
-    Friend WithEvents LimitNumericUpDown As NumericUpDown
+    Friend WithEvents NumericUpDownLimit As NumericUpDown
     Friend WithEvents ToolStripMenuItemDarkMode As ToolStripMenuItem
     Friend WithEvents ToolStripMenuItemAbout As ToolStripMenuItem
     Friend WithEvents ToolStripMenuItemDeveloper As ToolStripMenuItem
     Friend WithEvents ToolStripMenuItemCheckUpdates As ToolStripMenuItem
     Friend WithEvents ToolStripMenuItemQuit As ToolStripMenuItem
-    Friend WithEvents PictureBoxLogo As PictureBox
-    Friend WithEvents LabelRPST As Label
+    Friend WithEvents ToolTip As ToolTip
 End Class
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/StartForm.resx` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormMain.resx`

 * *Files 6% similar despite different names*

#### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/StartForm.resx` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/FormMain.resx`

```diff
@@ -113,14 +113,17 @@
   </resheader>
   <resheader name="reader">
     <value>System.Resources.ResXResourceReader, System.Windows.Forms, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089</value>
   </resheader>
   <resheader name="writer">
     <value>System.Resources.ResXResourceWriter, System.Windows.Forms, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089</value>
   </resheader>
+  <metadata name="ToolTip.TrayLocation" type="System.Drawing.Point, System.Drawing, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a">
+    <value>243, 22</value>
+  </metadata>
   <metadata name="ContextMenuStripRightClick.TrayLocation" type="System.Drawing.Point, System.Drawing, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a">
     <value>38, 22</value>
   </metadata>
   <assembly alias="System.Drawing" name="System.Drawing, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a"/>
   <data name="ToolStripMenuItemDarkMode.Image" type="System.Drawing.Bitmap, System.Drawing" mimetype="application/x-microsoft.net.object.bytearray.base64">
     <value>iVBORw0KGgoAAAANSUhEUgAAAgAAAAIACAYAAAD0eNT6AAAABGdBTUEAALGPC/xhBQAAAAlwSFlzAAAO
         vAAADrwBlbxySQAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAADvXSURBVHhe7Z0J
@@ -1926,377 +1929,14 @@
         vAAADrwBlbxySQAAAR9JREFUOE+Nkj1uwkAQRn0JcpSkDCJBLkKkeEXNBWjsg4WSDjrEGaBwkBDESmmS
         Kgqbeasde1k5CsXn8czOm5n9SdJ81Oj4kt0cjSlEK9HpkJkfrPcL1sP8FjTmjiQHZJmNRXz3kC7K+8fb
         C9iDW02KQdX+6dmW/eFGC+ioK014H4+dQkhjHrZugv6wR9dCu5FQv87s53xuq8nEgVh84gp75cAXXUm0
         57P9Wi7tx3TqLD7xCF4DnxTWTgp8V1VTiPjbIA3hOuk6IDoqiMWPujpd3ZkmEVxfvWcOLBrb7fnP02ZU
         1oh1wHLacs/cG4mIItgwkf/Qb+6Zl8KLEWeji/+ofWF8tICv2AU4db7tpoCMIspFa1EN4C0+8V6bP0p+
         AY7pF0Fg9EWkAAAAAElFTkSuQmCC</value>
   </data>
-  <data name="PictureBoxLogo.Image" type="System.Drawing.Bitmap, System.Drawing" mimetype="application/x-microsoft.net.object.bytearray.base64">
-    <value>iVBORw0KGgoAAAANSUhEUgAAAgAAAAIACAYAAAD0eNT6AAAABGdBTUEAALGPC/xhBQAAAAlwSFlzAAAN
-        0AAADdABEGw9BwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAFPuSURBVHhe7d0J
-        nBxVvTZ+ExbZVPTPX0Svonjd5b0qV0UEARXR60Xvq2yyi4DsskR2QfZNEEE2gbAIAgEEAgQIS4BAQEh6
-        uqfXmUkySaYHbyCsCXuSep9fJyOdzjMz3dW1nKp++Hy+H+AH6e4659T5nao6dc57PM8TERGRDkODIiIi
-        km40KCIiIulGgyIiIpJuNCgiIiLpRoMiIiKSbjQoIiIi6UaDIiIikm40KCIiIulGgyIiIpJuNCgiIiLp
-        RoMiIiKSbjQoIiIi6UaDIiIikm40KCIiIulGgyIiIpJuNCgiIiLpRoMiIiKSbjQoIiIi6UaDIiIikm40
-        KCIiIulGgyIiIpJuNCgiIiLpRoMiIiKSbjQoIiIi6UaDIiIikm40KCIiIulGgyIiIpJuNCgiIiLpRoMi
-        IiKtGhwcXA0+Bz+B38Jf4Ba4Dx6HHMyG5+B/oQ+64DG4B26GP8Mh8APYEMaw75L20aCIiMhILDHDf8Dh
-        cDv0wDvgBex1sIHD9fAr+BT7PdI6GhQREWmE5LsR7A8T4HlgCTsK/XAV7AofZr9VRkeDIiIiBgl2PTgI
-        ngKWjOO2GCbBzrAmOwbhaFBERDoXEul7YXu4E94Glnhd9AqMh61AcwdGQYMiItJ5kDTXhiPgWWAJNkls
-        3oDdFRjLjlU0ABAR6XhIkuvC72ABsGSaZL2wN6zGjr2T0aCIiKQfkqJd8Z8GduucJc80mQf7gu4ILEeD
-        IiKSbkiEP1ueFFmyTLOnYRNWJp2GBkVEJJ2Q/D4N9y5Php1qCVwM67Iy6hQ0KCIi6YJkt8rMmTMvx9/f
-        AJYUO9F82JmVVyegQRERSQ8k/s/n8/nn+/v7WRKUwcEroOPWEKBBERFJh56enoO7uroWFwoFlvjkXd3w
-        eVaGaUWDIiKSbEhmq5RKpftnzJjhmXnz5rGkJytaCLux8kwjGhQRkeTCVf9H8vn8/OnTp3umUqmwZCfD
-        Ox9Sv5IgDYqISDL19vZ+JpfLLRpK/plMxqtWqyzJychugFQvHkSDIiKSPH19fZtks9k3h5K/QYwlN2nO
-        /bA2K+s0oEEREUkWJPrvI/m/U5/88e8sqUlrbOGg9ViZJx0NiohIcvT29v6oq6trSX3yN7r6D0wRPsTK
-        PsloUEREkqFcLn/XXvNrTP4281/P/gP1JKzF6iCpaFBERNxXqVQ+j+S/wm3/IaVSiSUxaY8toZyaiYE0
-        KCIibps9e/YHc7ncQpb8jVb9C831kIpXBGlQRETchQQ0tlAoDLDEbzT5L3TnsnpJGhoUERF3lUqlSSzx
-        D+nt7WVJS4L1U1Y3SUKDIiLipnK5PI4l/XoDAwMsYUmwXoRPsDpKChoUERH3FIvFr2cymZVe96unTX8i
-        9QSsyuoqCWhQRERGtt9++60C68LH4UuwKWwDP4O94BAYBwfCnrAD/BdsCf8JX4BPwDrs8xsh0YzN5XIv
-        sKRfb+bMmSxRSXjOYPWVBDQoItLpkJhXhc/CdmCJ/Ap4DAbhNfAC9Dw8A7fAuXAQ/BhsYFFbirZcLt/E
-        En4j7foXuaWwRWP7SQIaFBHpFEiwY+ArsA9Y8p0IPfAOsGQduRNPPHHANvVhCb+e/T8NyUmikYfEPQqg
-        QRGRNENS/TzYrflbYYElWZdNmzaNJvxGev4fq3GsrbmMBkVE0gRJdEP4JfwV7BY+TbQuuuKKK2iyZ/T6
-        X6wWwr+x9ucqGhQRSTokT5todyHMGkqmSXPwwQfX1vRnyZ7R6n+xu4W1RVfRoIhIEiFp2oz8Y6E0lEST
-        bNKkSTTRM9r8xxlbs7bpIhoUEUkKJMp1wF6zewiWWOJMg0MPPbSlq//u7m6WjCR6j7B26iIaFBFxGRKk
-        zdy3d+7tmX7Qr+Q5YeLEiTTRD6dcLrNkJPFIxGuBNCgi4iIkRlt8Z1coDiXKNDrwwANrr/SxRD+cvr4+
-        logkHpNZ+3UNDYqIuARJcXXYF2YOJck0u/XWW2mSH8msWbNYIpL4fJO1ZZfQoIiIC5AM14RDYWAoOabd
-        /vvv3/LVv9EbAM65m7Vpl9CgiEickAjfB8fA/KHE2CnGjx9PE/xo5s6dy5KQxGcJOL0uAA2KiMQBCXA1
-        OApeHEqInabZVf8aaQtgJx3N2rkraFBEJGpIfrZLXqon943miCOOaOnVv3paA8BJBdbWXUGDIiJRQeJb
-        H+x1PpoUO8mECRNoch+NDRpI8hE3fJW1exfQoIhI2JDwxoJte/vSUALsdM888wxN8KPp6upiiUfccD5r
-        /y6gQRGRMCHZfR2m1ye/TnfMMcf4vv2fy+VY4hE3PMvOARfQoIhIGJDobNneSyHJS/ba9sFPwA1gx3IO
-        nAC/gb1he9gWNoNNYAv4IfwMdof94Ug4Cf4Ck6H35ptvXsySezO0DLDzvszOh7jRoIhI0JDk/gN6gCVV
-        17wDFbgTLMFbYv82rMeOLQhI4nNYcm+G7gA471BW53GjQRGRICFx/hreAJZsXWAJ/0k4Db4La7DjCAuS
-        +JgZM2YsaUzszdIcAOfdweo9bjQoIhIEJFJb0OcmYEk3TkshC+fDj+F97PdHpVwuf58l9mbZyoEk6Yg7
-        XoKxrO7jRIMiIu1CUv0q9AFLwHGwpP8Y7AOh3cr3AwOAy1lib5ZeA0yE/2R1HycaFBFpBxLsgfAmsEQc
-        tV74HXyS/VYXFIvFPEvsrSAJR9xyOKv7ONGgiIgfSLJ2y/8WYIk4Si/AxbAp+52u6e7ufpkl9VZoKWDn
-        /YXVfZxoUESkVUi2H4a43+0vwx6wOvuNrspkMktZUm/FnDlzWNIRdzzG6j5ONCgi0gok3E9BnM/7bULf
-        DuDcRKvRVCqVr7CE3qqZM2eypCPumM/qP040KCLSLCRde7//n8ASc9j+Adux35UUxWLxGJbQW4WBBEs6
-        4pZ1WRuICw2KiDQDydd28Ht5eTKO0qOwDftNSYMBwN9YQm9VoVBgCUfc8k3WBuJCgyIio0ECtqVto57p
-        PwDbs9+TVBgATGUJvVXZbJYlHHHLrqwNxIUGRURGgiRsf0W5nv/bYEvyrs1+T5Lhyr3tVwCN1gJIhINZ
-        G4gLDYqIDAdJ+NjlSTkqU+CL7LekQT6f72cJ3Q+9CeC8Y1gbiAsNiogwSMS2fz9L0mGwiYW7sN+RJt3d
-        3fNZMvejp6eHJR1xx+msDcSFBkVEGiEZ22t2Ud32vxbez35H2uRyuVdYMvcjn8+zpCPuuJC1gbjQoIhI
-        PSRj2yHvreXJOUyvwS/Zb0irbDb7Bkvmftg8gGq1yhKPuGE8awNxoUERkSFIyF+DV5cn6DAVIbXP+ofT
-        1dW1mCVzv/r7+1niETfcwtpAXGhQRMQgIf87zF+eoMN0NazFfkPaYQDwDkvkfmlBIKfdyNpAXGhQRAQJ
-        +SMwa3mCDssi2IN9f6fIZrOvs0TuFwYULPGIG65gbSAuNCginQ1J+f3QtTxJh6UfvsC+v5Pkcrm2dwJs
-        pMcAzjqftYG40KCIdC4k5TFwz/IkHZYcbMC+v9N0d3c/x5J4O0qlEks+Er+TWRuICw2KSOdCYj6qLlGH
-        4TFwalOUOGEAMJcl8XbobQBnjWNtIC40KCKdCYl5M3hneaIOwx2wBvvuTpXP50ssibdL2wM7aX/WBuJC
-        gyLSeZCYPwTzlifqMFwJq7Dv7mSFQuExlsDb1d3dzRKQxOtnrA3EhQZFpLMgMdtz/7uWJ+ownMG+V7z3
-        lEqlS1gCD4ImAzrnS6wNxIUGRaSzIEGPa0jYQXJq4pNryuXy7ix5B0FLAztlCbyXtYG40KCIdA4k6E3B
-        tttlybtdl7HvlHdVKpWPseQdFO0Q6IxZrP7jRIMi0hmQoD8Ic+oSdpBuhbHse2VFmUxmCUveQSgUCiwZ
-        SfQmsbqPEw2KSGdAgr6pLmEHyfbwd+p2p8tyudxLLHkHZe7cuSwhSbT+yOo+TjQoIumHBL1NXcIOkq0g
-        2BFb+QYln89nWeIOiuYCOGFvVvdxokERSTck6NWhZ3nCDtJMWJ99pwyvVCqdwxJ3kGbNmsWSkkTnU6zu
-        40SDIpJuSNIn1CXtoLwM/86+T0ZWqVQ+w5J2kGyTIK0OGJvZrN7jRoMikl5I0p+C15cn7SD9nH2fNCfo
-        XQGZcrnMkpOE70pW53GjQRFJLyTqMBb8uYh9lzSvUChkWNIOml4LjMUurM7jRoMikk5I1D9pSNxBmA6r
-        s++T5pVKpdNYwg5aNpvVo4DofYTVedxoUETSB0l6TQj6nf9X4NPs+6Q1lUplA9vFjyXtoBWLRZakJBwz
-        WH27gAZFJH2QqE+vS9xB2YF9l/gTxtbAw9FugZE5nNW1C2hQRNIFiXoDeLMucQfhYvZd4l+pVPodS9Zh
-        sLsNWiAodIvB2ddiaVBE0gXJ+ryG5N2uPtBKfwGrVCqrh7kscCPNBwjdvayeXUGDIpIeSNTrwaLliTso
-        27LvkvYVCoVnWLIOS3d3twYB4XFy9v8QGhSR9ECyPq0hebfrVvY9Eoxyubw9S9Rh0oZBoVgIa7E6dgUN
-        ikg6IFl/AGyFPpbI/bA7CR9n3yXBCXtzIEaLBAXufFa3LqFBEUkHJOugl/w9mn2PBAvJ+CiWpMPW09PD
-        Epm07k3YgNWtS2hQRJIPyXptWFCXvNtVgtXYd0nwstnsIpakw1apVFhCk9Yk4g0ZGhSR5EOyPrIueQdh
-        a/Y9Eo6oVgZk8N0sqUlz3oZPsDp1DQ2KSLIhWa8B/6xL3u26hX2PhAdX4mOz2ewbLEFHwSYG6u0AX5zc
-        +IehQRFJNiTsXzUk8HYshY3Z90i4cCV+FkvOUbFXBAcGBliSE+4NcG7f/+HQoIgkGxL2Y3UJvF23s++Q
-        aCAJP8+Sc1S6urq0g2DzTmJ16CoaFJHkQsK2/f7tqp0lcz82Yd8j0ahUKltHtUnQSHp7e1nCk3f1QaJW
-        x6RBEUkuJOwTGxJ4Oyax75BoFQqFR1hSjprNC9AjgWH9kNWdy2hQRJILSdvW6WfJ3I/N2HdItCqVyrpd
-        XV1vs6QcNXsk0N/fzxJgx6pWq7exenMdDYpIMiFhf6shgbfjIfYdEo+4FgcaTrFY7Pi7AfPmzbN1E97o
-        7e1N5CRZGhSRZELSvrQhibdD7/07plAoTGPJOC42N6ET5wbY65G2aqIdPwYAx7O6SgIaFJHkQcJ+L7xY
-        l8DbkWXfIfFCslk9l8u9zJJxnPCbvNmzZ9NkmTYzZ86sPQax4y4Wi9NYPSUFDYpI8iBp/7whibfjcPYd
-        Ej8MAjbJZDJLGpOwC2wgMGvWLJo4k87mPdjxDR1rd3f3K4itweooKWhQRJIHSfvOhiTu12JYn32HuKFU
-        Kh1Xn3hdk81ma1fKLJEmid3qt+PI5/MrHB8GYEv7+vq+weomSWhQRJIFCduW/n1zeQJvl179S4BisTip
-        Pim5yG6VVyoVb+7cuTTBusoWPrLtkZHo6XHhmFKxKyYNikiyIGl/ryGJt2Nn9h3inkKhkGEJykW2rDCu
-        mp19c8B+l/2++tv8TKlUuoTVRRLRoIgkC5L26Q1J3K9XYE32HeIeXImORWKdwxKVq2zmvN1St7cH4l5i
-        2L7ffoctcNTMaotI/jezekgqGhSRZEHSfrIuibcjMTuZyTIYBKyFq9YFLGElgd1mtwRsV9+WkMPagdCu
-        8G2Coj2SsLsRrS6vXC6XH2Dln2Q0KCLJgaT9PninLom34zvsO8RtSGrrYxDwKktcSWRzByxJ44q7doVu
-        idteM7QBgs0nsAV4hgYKltgtZv/N/h+btGd/xhK9/XkbXNikRPY9zcLnPMXKPeloUESSA0n7xw1J3K9/
-        whj2HeI+JLz1kDTnswQm/hWLxamsvNOABkUkOZC0z69L4u34G/t8SQ4MAtbI5/MzWSKT1hUKhYmsnNOC
-        BkUkOZC4sw2J3K992edLsmAQMBaJ6ymW0KQ5Nj+gXC6fy8o3TWhQRJIBSXs9CGrv/39n3yHJVCwWb2PJ
-        TUbW1dW1pLe3dx9WpmlDgyKSDEja2zckcb/msc+XZMNV7K+R0BazRCcry+Vyr/T19f0HK8s0okERSQYk
-        7vMaErlf17LPl+SrVCqf0eTA0eXz+Syu/DtqDQwaFJFkQOK+uyGR+7UX+3xJB5sXUCwW72GJr9PZxkql
-        Uul0Vm5pR4MikgxI3H0NidyvDdnnS7qUy+VdstnsIpYIO1GhUOibOXPmZ1lZdQIaFBH3IWmvBrZzH0vo
-        rehnny/pVKlUVi0Wi9fbjnYsKXYCDILeRDkcwsqnk9CgiLgPifvzDYncrzvZ50u6IQF+Np/P97IEmVb2
-        eh8GP/f39fWtxcqk09CgiLgPifunDYncr7PZ50tnKJfLe3Z3d/8vS5hpYYm/UChke3p6Er+Hf5BoUETc
-        h8R9VEMi92tv9vnSWTAQ2B4DgbksgSaVPebAFf+03t7eL7Bj7nQ0KCLuQ+K+qiGR+/Vt9vnSmSqVyjb5
-        fL6n1d3yXLJ8Zv/kvr6+T7BjlGVoUETch8T9eEMi92s99vnS2TAQ+Biunq/N5XIvsyTrGhuwdHd3D+I3
-        n1cul9dmxyQrokERcR8S9/MNidyPBeyzRephMPCdQqHwcFdX11ss+cbFkn4+n38RCX/8zJkzP85+uwyP
-        BkXEbUjc6zYkcr+eYJ8vMhwMBjYrlUpX2q6DGBC8wxJzmGwQgiv9Cn7DuUr67aFBEXEbEvenGxK5X+PZ
-        54s0CwOCrZGMr7AdCJGY/xnUXQK7us9ms69joDEbnz+pp6fnBCT8T7HfIP7QoIi4DYn7Kw2J3K/j2OeL
-        tAODgjVgGyTuk+DSYrF4E9yHQcI0JPRumAW9+PcZiE/B//P3crl8Jf7M2XAw/v07GEi8l322BIcGRcRt
-        SNxbNCRyvw5kny8i6UeDIuI2JO4fNyRyv3Zjny8i6UeDIuI2JO6dGxK5Xz9lny8i6UeDIuI2JO59GxK5
-        X99lny8i6UeDIuI2JO4jGxL5iPbff3/vkEMO8Q4//HDvqKOO8o4//njvpJNO8m699dbdBwcHvwifhPXh
-        /bAa+04RSRcaFJH4IAGvDZ+D74El6P3hCDgeToPzHn/88WcmTZrkTZ482ZsyZYo3depU76mnnqq9OpXL
-        5bxSqeT19vZ6/f39XrVa9fBnWrUYXoX5MAfKkIHH4QGYCDfDNXAJnAf22+w32m+132y/3Y7BjkUrs4k4
-        hgZFJBxIhB+CjeFHsC+cDFfCfVCAl4El5DSwY7NjtGO1Y7ZjtzKwsrAy+RArMxEJBw2KSGuQvMbCR+A/
-        4X/gIDgT/gpToBdeB5YY5V1WRlZWVmZWdlaGVpZWpla2VsZjWR2ISGtoUEQ4JJ8xsBFYQjoJboM+eBtY
-        QpPgWVlbmVvZWx1YXVidjGF1JiIcDYpILdmvA98Ce55tz7mfAHsuzpKSxM/qxurI6srqzOpuHVa3IqIB
-        gMhwV/UzYSmwRCPJYXVodam7BSINaFAkrdDx66pejO4WSMejQZG0QKdus+5/BhdDCXRVL8OxtmFtxNqK
-        tRm9lSCpRoMiSYVO267w7bWyc2EGLAHW2YuMxtqOtSFrS9amdIdAUoUGRZICnfJ7YUs4BWyRGs3Gl7BY
-        27I2Zm3N2py2q5VEo0ERV6HTXQW+AcfAZNC79RIXa3vWBq0tWptchbVZEVfRoIgr0KnaDP0vw2/gTkjz
-        SnmSbNY2rY1aW7U2qzcNxGk0KBIndJwfhF/CTWBr0bPOVsR11nZvBGvLH2RtXSRONCgSNXSQ74Pd4C54
-        C1iHKpJU1qatbVsbfx87B0SiRoMiUUBHuBbsCLZIyxvAOk6RtLG2bm3e2v5a7NwQiQINioQFHZ7N2rfV
-        2OzW6CJgHaRIp7BzwM4FOyf0VoFEigZFgoSObTX4L7gWXgHWEYp0Ojs37Byxc2U1di6JBIkGRdqFDsxe
-        1/s+XAEvAOvwRISzc8bOHTuH9HqhhIIGRfxAR2V74n8HbClVzd4XCYadS3ZO2bk1lp17In7QoEgr0Cl9
-        Cmy5VPuLdWAiEgz7y861T7FzUaQVNCjSDHRC34U7QOvti0TLzjk7977Lzk2RZtBgJ8CJsyp8AD4GnwNb
-        ueuTsB6syf6M1MptTdgX8sA6JhGJlp2Ldk6q3xrG9OnT14T14JPwZfgcfAw+AKuyP9MJaDDpcCKsAV8C
-        e7VmHFwOD8FsWABvAjuR6i0Gm5Vrf00HW5XuVNgTvg0fZt+dVjjej8NZoAl9Im6yc9PO0Y+zczitkMA/
-        DN+GPeFUuAnsr0F4BRaDN4o3YQHMhofgchgH/wNfgjXYdycdDSYNGvynYS+4Enogqj3fX4J74TiwCTqp
-        ayQ4pi3gFrABESsDEXGLnat2zm7Bzukks0QM34Hj4F54CVhCD9pS6IErYS/4NPt9SUODrkPD3gAOhAnw
-        LLCTIA623OcTYKPwzSGRm4Hgd9tiPTagygA7ThFJBjuH7VxO5CJDSLRjYHM4C56At4Al6Dg8CxPgQNiA
-        /X7X0aCL0IA/DAfAFEjKpLMBOB++yY7JNfidHwV7zPEcsOMRkWSyc9rO7Y+yc981SKjfhPNhAFjydc0S
-        mAIHQGIeD9OgK9BYbcLZ3vAgJP0WdD/YnYHPsGONE37TpvA3eBvYbxeRdLBz3M71TVlfECckzs+AXen3
-        A0uySWFzDh6EvcHpiZk0GDc0TrvFfxrYhD3WiJPM5idMhK3YsUcF32/77O8A/wD2O0Uk3ezctz4g1keV
-        SJJbwUSw5+wsoSaZTSw8DZx8RECDcUFD/ArYWtidsh1sF+wOq7PyCAu+74eg5/siYqwv+CHrK8KChLg6
-        7A5dwBJn2tjchWvhK6w84kKDUUPj2xhsNj1rnJ3A/toHQl3mE5+/GTwC7DeISGezvmEz1ncEBQlwLOwD
-        9ooeS5SdwN5e2JiVT9RoMCpobB+Bv4BeMVumG7ZhZdUOfKYNsOyxA/tOEZF61lcEnqCQ9LaB7uVJsNPZ
-        PIG/wEdYWUWFBsOGxmWT+06AhcAaYKebBF9kZdcKfMZG8FfQUr0i0grrM6zv2Ij1La1AkvsiTAKWCDvd
-        QjgBYpksSINhQoPaFuYBa3TyLrsrch60vLgQ/ozdWbHdwzSrX0TaYX2I9SUtX6kiqdmiPedBMyvxdbp5
-        sC0rxzDRYBjQgNaGS4E1MhleCTZhZdoI/9+6cCa8BuyzRET8sD7F+pZ1Wd/TCMlsEygtT27SvEthbVam
-        YaDBoKHR2OSzPmANS0b3DpwIdNMKxNeCY+BFYH9eRCQI1sdYX7MW64uQvFaFE+EdYAlORtcHoU7GHEKD
-        QUEjsR33bNSoSX7BeBo+W1e+q4EtiezScsgikn7W51jfs9pQf4Sk9Vl4enkSk/bYY5MzIdSdCmkwCGgY
-        ttXuZGCNR/yzDYi2gV1h1vKYiEgcrA/aFYnKZvhHtTFPJ5kMH2A5Ngg02C40CJt9bs+uWYOR9kW126GI
-        yKj6+/uXZrNZlsCkfTaXou23MRgabAcag+2C93x94xARkXSrVqtepVJhCUza9zxsznJuO2jQLzSCXeDN
-        +kYhIiKdY86cOV4ul2NJTNrzJuzCcq9fNOgHKn5P0IIzIiLi9fb2ejNmzGCJTPyzbYf3ZDnYDxpsFSp7
-        N1DyFxGRf5k3b57X3d3NEpn4Z4OA3VgubhUNtgKVvDPoNT8REaH6+vq8TCbDkpn4Y68J7sxycitosFmo
-        WNtLWslfRERGNDAw4BUKBZbMxB8bBOzAcnOzaLAZqNAtwVaoo5UtIiLSaNasWbobEBxbcXFLlqObQYOj
-        QSVuCHrVT0REWmZ3A0qlEkto0jp7RXBDlqtHQ4MjQeXZuvPZ+soUERFpVX9/v9fV1cWSmrQmC3R/hpHQ
-        4EhQaRMaK1FERMQPW0BIdwMCMYHl7JHQ4HBQWcc1Vp40zxq63fpi/01EpJPNnDlT6wa07ziWu4dDgwwq
-        6GugSX8+zZ07tzb5hf03ERFZ1k9qT4G22KTAr7EcztBgI1SMbTubq68oaZ6NbG2NbPbfRETkXXanVK8L
-        tiUH/9qmeSQ02AiVclJjJUlzyuVyrTGz/yYiIlxPTw9LbtKck1gub0SD9VARG8Pb9RUjo7Nn/bYEprER
-        Lft/RERkeLNnz9aaAf68DRuznF6PBoegAlaB6fUVIqOz3bDs1RZ7lqVJfyIi/tl+Atpd0Bf7axWW24fQ
-        4BAU/l6NlSEjszWvbSarjVqt4bL/R0REmqdXBX3bi+X2ITRoUOirw5z6SpDh1TdQGwDYXQD2/4mIiD9D
-        F1gNSU6GNwdWZzne0KBBYR/aWPjCNd6isudW7P8TEZH2DD1iHepvZVSHshxvaBCFvDbMry904Wwpy/pJ
-        KjZCZf+fiIgEw+ZW5fP5+iQnw5sPa7Ncv1LAoICPbyxwWVlvb+8KBW2v/LH/T0REgmfrq9T3wTKs41mu
-        XymAQl0DXqgvZFmRPe8vFosrFLC97sf+XxERCY8ttFbfFwv1AqzRmO9X+BeDAt2lsYDlXZb8LdnXF65m
-        /IuIxMeWWdfkwFHt0pjvV/gXg8Kc0li4sgxL/kaT/kRE4mX9sAYBI5rSmO9X+BcU4mcaC1WWsUknbDEK
-        rfEvIuIGm5StQcCIPlOf8xsHAGc3FqgsS/5shyo99xcRcYu9Jqjlg4d1dn3Or0/+q4Je/Wtgz/ZZ8tdz
-        fxERN9m2wlorgLJXAldlA4AtGgux01mCH64R6bm/iIi7Ruq/O9wWbABwWmMBdrKRRpB67i8i4r7h7uB2
-        uNPYAOCZxsLrVCM9Q9JzfxGR5BhuAncHe2aFAQAKaT1YWl9onWqk5K/n/iIiyTPcK9wdaimsVz8A0OI/
-        MNorJLbiFPtzIiLiNhsEaP+Af6ktCjQ0ABjfWFidZrRFJHTrX0Qk2WwQUCgUaB/fYcbXDwAyjQXVSUZb
-        RtL+m00KZH9WRESSRYOA6ZnaAACFMRZery+cTmJX/qRwVqBZ/yIi6aE5AdNfh7E2ANiosXA6hV3Vj7Zs
-        pL1CYo2F/XkREUkmezugw9cJ2MgGAP/dWDCdoNnK14I/IiLpZBeBHbxs8H/bAODoxkJJu2Zv/9ie/+zP
-        i4hIOtjbX6z/7wBH2wDg6sYCSTtL7KQwVmCjQrtLwP68iIikh73izfJAyl1tA4C7GgsjzXp6elhBrKSv
-        r4/+eRERSR+b7M1yQYrdZQOARxsLIq2aHeXZspHsz4uISHo1c3c4RR61AUC2sRDSaLRV/urZcsDsM0RE
-        JL067PXArA0AZjcWQtrY+v3NzvTUxD8Rkc7VQa8HzrYBwILGAkgTG9G1sh2kVvwTEelsHfJ64AIbALzd
-        ePBp0srmD7r6FxER08pj44R62wYAbzQeeFqUSiV20MPS1b+IiAxJ+euBb9gAYH7jQadBb28vO+Bh6epf
-        REQapfj1wPk2AOhrPOCka2aDn0a6+hcREaaVR8kJ0mcDgBmNB5tkfmZw6upfRESGY3klhZMCZ9gAYErj
-        wSaZn4UcdPUvIiIj8XNn2XFTbABwZ+OBJtWsWbPYQY5IV/8iItKMcrlM80hC3WkDgMsbDzKJ/N6i0dW/
-        iIg0w9aVsaXiWS5JoMttAPCbxoNMIj+3/nX1LyIirbCLxpSsD/AbGwBs03iASePn1r/Rmv8iItIq2y2W
-        5ZSE2cYGAB9tPLgk8XvrXzv+iYiIXyl4NfCj7/E8zwYBLzceXFIUCgV2YKPSfv8iIuKXbTKX4EcBL1vu
-        HxoATGs8uCTwu0yjVZrdOWCfKSIi0oxWV5x1yLT6AcBFjQfmunYWZtDkPxERCUJC3wq4qH4AsF3jQbnO
-        761/Yws6sM8URxW7vcGpD3nVu2/xqjdc7lUvPcurnnWUVz12H2/gkB296jF7e9Uzx3nVi8/wqtdf6lXv
-        utkbfOwBbzDfxT9PpFnWhtCWrE3V2pa1MWtraHO1toc2WGuL1iatbaKNWluttVn2eZI6Npmc5RnHbVc/
-        AFgHErMtcDs7NNkywewzxSHVqjf45KNe9fJzvIGDfu4N/Pwb/v36J171z6ctGxDY57LvExlibcQSPtqM
-        tR3appqFtmtt2Nqy2l66JWyBoLdhnX8NAJYPAhKxJLBNvGhnTeaenh76uRIz1Gv1oXu86h9P9Ab2/hHv
-        UNu15/e96rnHetX7bvcG9QqoDEFbsDZhbcPaCG077UKbtrZtbdzaOv0dkli2QFCre9DEaMpQ3q8fABzT
-        eFAuavfVCxtAsM+VmODEqU68yRvYbzvecYbll9t61QnjvcEBtYeOhbq3NmBtgbaRsKCtV++8UXcFUsbv
-        ejQxOIYNAL7WeECuaXczBhs8sM+VeFQfnuQNHLYz7ySjcsD/9ar33kZ/n6SX1bnVPW0TUUHbt3OA/T5J
-        pu7ubpp7HPM1NgAYA7PqD8Y17c62tBEa+1yJ2D+metXj9+OdYlzG7e4NTn2Q/15JD9Sx1TVtAzGxc8HO
-        Cfp7JVESMCFwFoxZaQCwfBBwXOMBuaKdiX/G5g3Ycxr22RKRgQGvevHp3sD236QdoQuq5xzjDc7V/IDU
-        QZ1a3bI6dwLOCTs37Byhv18Sw8++NBE6tj7nNw4ANoB36g/GBUFMsLDXBtlnS0Rm9nnVE37NOz/XHLGb
-        N1hWe0kN1KXVKa1rx9g5YucKPQ5JBIdXCHwHNqjP+SsMAAwO4I7GA4qbzdxvOJCWaenfGGWnewMHxvy8
-        tVV7/2jZ61vseCQ5UIehvVUSFpwrds7Q45FEqFQqNA/F7I7GfL/Cvxj8+B83HkycbMW/IEZTmv0fj+qU
-        e72B3b/LOzrX7bx57Q0FdlzivtrbJahDWreuwzlj5w47LnGf3bVu53X1kPy4Md+v8C8GP34szK0/mDgF
-        scCCFv+JR/X2672BHb7FO7gEqY6/gB6fuMvqjNVlouDcsXOIHZ+4z7Etg+fC2MZ8v8K/DMGP36/xYOIQ
-        1LOUUqlEP1/CU33kfm9gx+Qn/yHVO/5Gj1PcY3XF6jCRcA7ZucSOU9zm2OJA+7Fcv1LA4MevCr31BxOH
-        oJZX1Ot/EevOeAN7fI93aEm187e9wWlT+PGKO1BHVle0DpMK55KdU/R4xWmO7BbYC6uyXL9SYAh+/E6N
-        BxOloJ79G239G6HZM72Bg7fnHVmbqj//pve/O23mPf+Lb3sv7rKF98puW3oL99iy9nf7d4vP3wlXTGG9
-        ZvjLbb3BkjZ5cRbqJqxV/axNWdsaqe1Z27Q2yv5823BO2blFj1uc5chcgJ1Yjjc0aPDjbWGgTP3BRCmo
-        WZS2eBD7fAkBGnv1pAN5B+bTIDreF3bZ3Ht9r629pfv+wPP223ZU9v+9vtd30TFv7g3uEHCHfNgvvME5
-        /fz4JT6oE6sbWmc+WduxNmRtqbW2t3WtzVrbZZ/rl51bWj44eYJ4i60NGfjXwj+NaHAIfvy2jQcThSBH
-        TTaQYN8hwatedjbtuPx4dodNvUV7IumTTrY1ywYD/7vjpvR7/KiecSQ9fomP1QmrKz+srVibsbbD21Rz
-        rO1aG7a2zL7HDzvH2PGLu4K8m+0DGiPP74YG6+EA7mw8oLAF+dykv19Xa5HIPO0NBNDR2VXTq7tvGUDi
-        X9miPbdCZxzMVZnWcHdHbU8JUketsrZhbYS1nXZYW7Y2HcgdAZxjdq6xchB3xbRd8J0sp9ejwXr48R+F
-        l+oPJkxBXv3bqIt9hwSvevKhvMNqwXM7f9tbsk97V12jsVu0dnuWfX9LDttZt2NdgDoIYkMpaxPN3ub3
-        y9q2tXH2/a2wc42WhTgrhrsAL8FHWU6vR4ONcAB7Nx5QWIJ8d1K7/0Xk8YdoR9WKl3bdwvP25R1nGF7Z
-        /Tv0d7RCiwTFr7bYD6mbVlhbYG0kFGjj1tbZ72iFnXOsPMRdEe8RsDfL5Y1okMEBTG48oDC0u+NfPT3/
-        j8bAb/eknVRTtv+Gt2iP4G+7NuP1Pb/b3hsD+23nDc6bS8tEIoCytzqgddMEq3trA6xthM3avLV99rua
-        gnOOlok4yx5HszwVgskshzM0yOAANoSF9QcUtKC3UrQdBNn3SHCq993OO6gmLYwp+Q+xBMB+V7OqN1xO
-        y0XCZ2XP6qRZcSX/Idb22e9qlp17rFzEXdlsluaqAC2EDVkOZ2hwODiAXRsPKEi2Yl/DwbTFBhTseyQg
-        9vz1wJ/RzqkZL9ptf9IxRq2txwF7fN8b7NdCU5FDmVvZ0zppQqS3/Udg5wD7fU3Buad5KMkSwcJAu7Lc
-        PRwaHAkO4tzGgwqCTf4LepKEfSb7LgnItEd4x9SE53beLJSZ/n4t2MX/5Kzq3RN4+UhorMxZXTTD6pq1
-        gTjYOWDnAvudzbBzkJWPuCmMPFfnXJazR0KDI8FB2GZB99UfVBCC3jhBGwCFr3r5ObRTGo2tlrZ4n21o
-        hxiXpftu6/sVweqZ42j5SHiszFldjMbq2OqatYG42LngdwVBOwdZ+Yi7gr7Tvdx9sNJmP6OhwdHgINaF
-        QPcK6O7uZgflm94ACN/AQT+nndJoXtnNjduvjXw/k91tK29Q201HB2VtZU7rYhRxzzkZjp0T7PeOCucg
-        LSNxVtBz3cDW+l+X5erR0GAzcCBfgJfrD8yvuXPnsoNqiy28wL5LApKdzjukUdjyqq5dgf0Lftc/fe5g
-        WH1ICwNFxcqa1cForG6jfNW0FXZO+F222s5FVk7irgAnA74MX2A5uhk02CwcyKbwav2B+RHUuv/17JEC
-        +y4JRvW6i2lnNBpXr8CG+H0roHrBSbScJHhW1qwORhP3rP/R+L0DZeciKydxV0D7A7wKm7Lc3CwabAUO
-        ZjNo6/XAMPZM1hsA4Rr47R60MxqJPecMe7W19v3AG9zex5LGv/oRLScJnpU1rYMRWJ22u7Z/2Ozc8DUX
-        AOciKydxVwB3ve11v81YTm4FDbYKB7QFLKo/wGaF8DykRm8AhMhewfKxgI5tmco6Ptf4fTVLa7RHwPac
-        IGU/GldeOR2NnSPs948I56JeRU2eNh4DLAI0aJ6PW0GDfuCAtoLX6g+wGWHc/tcbACHz+fw/rhX/WvXG
-        Xj4fA2geQOj8Pv+3OmV17ZraCoHk949G8wCSx+djgNcAHSnPw62iQb9wUPY44Ln6gxxNGCsj6Q2AkD06
-        mXZCo3Ht1b/h1G7F+limtXr79by8JDBWxqzsR2J16f6jp2XsHGHHMBo7J1l5ibt8PAZ4Dtq+7V+PBtuB
-        A/skFOoPdDhhzP43tukC+z4Jhp8NWGxPdNbhuWq+j8VZqtdcSMtLgmNlzMp+JFaXrI5dZecKO46RaGOq
-        ZGrhArgAn2Q5tx002C4c2PthUv2BMgHNhFyJXgEMV/Wvl9BOaCTzd/oW7excteAXrW8ZXP3T72l5SXCs
-        jFnZj8TqktWxq+xcYccxEjsnWXmJ25p8BD4J3s9ybbtoMAg4uFXggvqDbRTkzn/1tAtguKp/Po12QiNJ
-        Wif80q6tL8xSPUX7tIfNypiV/UisLlkdu8rX4BPnJCsvcVsTk+AvgFVYjg0CDQYJB7kTvFh/0GZgYIAd
-        bCDszkLj90lwqmccSTuhkby0WzJmYQ95dfct6XGMaNzutLwkOFbGtOxHYHXJ6thVdq6w4xiJnZOsvMR9
-        mUyG5bEXYSeWU4NEg0HDQX4M7q8/aNuqt+GAA6NFgMJVPX4/2gmN5JWEdcKL9tiaHseIDvgfWl4SHCtj
-        WvYjsLpkdewqO1fYcYzEzklWXuK+QqHQmMPuh4+xXBo0GgwDDnQMHAyv20GHtCFCjQ0u7DskHH42Ynkp
-        Ie9hD/F3B0ALsoTNypiW/QgSdwfAxzoU2pAqueo2wnsdDoYxLIeGgQbDhAP+HEwN4/W/IbNnz6YFLcGo
-        XnwG7YRGkrw5AD464VMPo+UlwbEyZmU/kqQNPn3NAcA5ycpL3Lf8bbip8DmWM8NEg2GrVCpfqk/YQevv
-        76cFLcGoXn8p7YRGMn+nZL2KtcDHimzVC0+m5SXBsTJmZT8Sq0tWx66yc4Udx0jsnGTlJYmxPsuVYaPB
-        sJVKpT+yxB0U7QMQrupdN9NOaCS2Dzvr7FzlqxO+9iJaXhIcK2NW9iNJ2uDTzhV2HCOxc5KVlyRG6BP+
-        GBoMWwF/scQdlHnamz1cj3XCSoA+OmGtBBg6fysBJmETqmV8rwSIc5KVlyTGZSxXho0Gw5bNZt9kiTso
-        9oohKWAJis+9ABbunoy9AF7fy+deAA9rL4CwWRmzsh+N1Smra9fYOcJ+/2i0F0DiVViuDBsNhqm3t3c9
-        lrSDpJ0AQzan3xvwsVzpczsn41nsC7u0PgnLqBOOgM/Bp9Upq2vX2DnCfv+IcC7aOUnLS5JiKazNcmaY
-        aDBM5XJ5L5a0g9RQsBKC6jF7885oJNt/w1vi+q3Yfbf1Bn3c/h/Y979pOUnwrKxpHYzA6tTqlta5I+zc
-        sHOE/f6R2LnIykkSB42U582w0GCYSqXSNSxpB4kUrASsesNltDMazauObwn82p7+bsFWLzqFlpMEz8qa
-        1cForG5ZnbvCzg32u0dj5yIrJ0mcfVnODBMNhqlQKGRZ0g6SHgFEIN9FO6PR2JWYq3cBbKKYn53YTPWR
-        +3k5SeCsrFkdjMbq1tXJgHZO+LrzBHYusnKSxPkzy5lhosEw5XK5l1jSDpImAUZj4NAdaYc0mpd3c3Nz
-        loU+r8AG9vieN6g2Fx2UtZU5rYtRWB2zuo+bnRPs944K5yAtI0mix1jODBMNhimTySxlSTtIGgBEo3rl
-        ebxTGkUVXHslsHYF5uP9a1M9+2haPhIeK3NWF6OxOnbtDpSdC3ZOsN87GjsHWflIIr3EcmaYaDAsPT09
-        m7CEHTStAxCRf0ylnVIzbHGWpaQzjMcPvOf9zL5ernrvbbx8JDRW5qwummF1bXXO20K07Bzws+jUEDsH
-        WflIYn2C5c6w0GBYyuXyCSxhB83WViYFKyEYOHQn2jE14wVH9gfwffvV/HJbvYIVB3sVFWVP66QJrjyG
-        snOA/b6m4NyjZSNJ9mOWO8NCg2EplUo3sYQdNC0FHJ3qQ/fwzqlJce/UtmhPH9v+1qnecjUtFwmflT2r
-        k2ZZ3bM2ERVfO07WsXOPlYsk2sEsd4aFBsNSKBSeYAk7aNoMKFrV4/alHVSz4hoELNpjK9/PXmsO/L+a
-        /BcnmwyIOqB10wSre2sDrG2Ere3kj3OOlokk3Zksd4aFBsOSz+dnsoQdtFmzZrGClbA8NdUb8PkK0xC7
-        FRrdnIAftHfbfzk9+49fO3MBhix7HBDNnABr423d9jc41+ycY+UhiXcdy51hocGw5HK5F1jCDlpfXx8r
-        WAlR9YwjeWfVgvk7fSv0twNsBvjzPrb6Xcm4PWg5SPSsLmgdtcDaRNhvB1jbtjbOvr8Vdq6xcpBUeIjl
-        zrDQYFi6urreYgk7aJVKhRWshKk74w3s6H828xDbuc2uyILujO3Ky1Za87vYSqPBqQ/ycpDooS5YHbXK
-        2oa1kaDvRFlbtjbtZ4fJleAcs3ONloOkQaSbAtFgWGbMmBH6GgCmWCyygpWQVa/+E++0fLD3tW3RlnZX
-        brPOfNGeW3nP7uhvhT+met7x9PglPlYnrK78sLZibabdgYC1XWvDfteXYOwcY8cvqbGI5c6w0GAYenp6
-        PsaSdRi6u7tZwUoEqqcfQTsuv+yqyd7bXrTH1k0/Hliyzw+81/bc2lvwi8296s+D63xrjtrLG5yn10yd
-        gzqxuqF15pO1HWtD1pasTbG21sjaqLVVa7OBXPHXsXOLHrukzQdYDg0DDYahUqn8mCXrMHR1aW3s2Nj7
-        2YfvQjuwIPxzh029+Ttv5i3Y5dveS7tt4b2y+5a1v9t2r8/ttFntv7M/Fwjb8a+nzI9b4oe68bNTYLOs
-        bVkbs7ZW3/asLVqbDLXt4ZzSehMd44ssh4aBBsNQLpcPZMk6DDNmzGCFKlEpdbe1SIuTdvmON/jME/x4
-        xR2oI6srWodJZYtN4ZyixytptDnLoWGgwTBgAHAMS9Zh0X4AMZv2iDfQxvK6Ttn+m1713r/z4xTnWF21
-        +1qqM3AO2bnEjlNS6wcsh4aBBsNQKpXOYIk6LFoNMH7Ve271BnZK+CDAkv+Nf6HHJ+6yOkv8IADnjp1D
-        7Pgk1X7KcmgYaDAMGABcxBJ1WLQWgCOmTfEGfvkD3sG5btetvOrkify4xHlWd1aHtG5dh3PGzh12XJJ6
-        v2A5NAw0GAYMAMazRB2WclmTtZxR7PYGDvsF7+hctf9PvcHMP/jxSHKgDq0uaR27CueKnTP0eKQT7M1y
-        aBhoMAzFYnECS9Rh0auAjpnT71VPO5x3eI6prbPe18OPQ5IHddnufhVRsXNEs/07XmQbAtFgGDAAuIcl
-        6rBkMloty0XV8Rd4Azu2vxxqKOx5/0WnaoOfNEKdWt06Oy8A54SdG/S3S6c5iuXQMNBgGAqFwhSWqMM0
-        b948VrgSt+x0XOkc5lRnXP3d/nrNrxOgjq2uWRuIhQ06cS7YOUF/r3Sik1gODQMNhiGqrYDrzZ49mxWu
-        uOLJR73qMXvzjjEqh+/iVR+5j/8+SS2r8zAXrGqGtX07B9jvk452OsuhYaDBMGAA8BBL0mHq6dFz3CSo
-        PjDRGzhkB9pJhubXP/Gqd0/wBqtV+pukA6Duq3fdXGsLtI2EBW29+sBd/DeJDA7+juXQMNBgGIrF4kSW
-        pMOEQQcrXHGRJeJpj3jVy872Bg78Ge8427Xfdl71z6d5g49N1nN+eZe1BbQJaxvWRmjbaRfatLXt2qI+
-        GnTKyI5kOTQMNBgGDABuYkk6TJoImGA2T+C6i5ft9d7OXIHDfuFVr/qjN/jMNP49Io3QVqzNtPXqqrVZ
-        tF1rw3q+Ly06kOXQMNBgGEql0pUsSYdt7lzt3JZ4s/q8welPetWHJnnV26/3qtdc5FX/dLJXPfU33sBR
-        v/SqJx/iVS84qbZVavW267zqg3cvS/h6lU/aZW3IBgRoU7W2ZW3M2hraXK3toQ3W2qK1SWubaKPWVmtt
-        ln2eyOj2Yjk0DDQYBgwALmAJOmxaEVBERBJkR5ZDw0CDYcAA4FSWoMOmeQAiIpIg27EcGgYaDEO5XB7H
-        EnTYNA9AREQS5Hssh4aBBsOAAcC+LEFHQfMAREQkIb7FcmgYaDAMGABsxZJzFDQPQEREEmIjlkPDQINh
-        qFQq67LkHAXNAxARkYRYg+XQMNBgWDKZzFKWoMM2Y8YMr6rFN0RExG0LWO4MCw2GJZvNvsESdBRmzZrF
-        CltERMQVOZY7w0KDYcnlcs+x5ByFYrHICltERMQVk1juDAsNhiWfz1dYco6CHgOIiIjjrmC5Myw0GJZC
-        ofAIS85R0WMAERFx2O9Z7gwLDYalWCxexxJzVPQYQEREHLYvy51hocGwlMvlw1hijooeA4iIiMO2Yrkz
-        LDQYlkql8mmWmKOkxwAiIuKoD7HcGRYaDFMmk1nMEnNU8vk8K3QREZE4VVnODBMNhqm7uzu2VwGHzJs3
-        jxW+iIhIXCJ9BdDQYJgKhcKTLClHqVKpsMIXERGJy5ksZ4aJBsNUKpUuYkk5StoiWEREHPMLljPDRINh
-        KpfLP2VJOWqaDCgiIg75EsuZYaLBMFUqlTXsdTyWlKOkyYAiIuKIN2FVljPDRINhy+VyC1lSjpomA4qI
-        iAOeZLkybDQYtkKhMI0l5KiVy2VWESIiIlE6g+XKsNFg2JB4j2YJOWr2KGJgYIBVhoiISFS2YbkybDQY
-        tkqlsh5LyHHQK4EiIhKjt2EtlivDRoNRyOVyr7CEHDXtDyAiIjGaynJkFGgwCoVC4TGWkOPQ09PDKkVE
-        RCRsp7AcGQUajEK5XD6cJeM42MJAugsgIiIx2JrlyCjQYBQqlcq6LqwHMKS3t5dVjIiISFjs/f81WI6M
-        Ag1GJZfLPc+ScRy6urp0F0BERKJ0H8uNUaHBqBSLxetYMo6L5gKIiEiE9mW5MSo0GJVKpfJ5lojjonUB
-        REQkIovh/2e5MSo0GKVcLvciS8ZxKZVKrKJERESC9DDLiVGiwSgVi8WbWSKO09y5c1lliYiIBOUglhOj
-        RINRqlQqX2VJOE6FQoFVloiISBCWwkdZTowSDUbNlVUB6/X397NKExERadfjLBdGjQajViwW72BJOE4Y
-        lLBKExERadfhLBdGjQajVqlUvsKScNz6+vpYxYmIiPj1DmzAcmHUaDAO3d3dgywJx8leC5w3bx6rQPHh
-        ySef9C688ELv8MMP9w477DDvN7/5jTdu3Djv2muv1bwLEekUf2c5MA40GIdSqXQcS8JxU2Jqnw2kjj/+
-        eG+//fYb0dlnn13bl4F9hohISmzLcmAcaDAOlUplbFdX1zssCcdt1qxZrBKlCZbQ7UqfJXzm17/+tTd+
-        /HhNwhSRNJoNY1gOjAMNxqVYLE5mCThu2i3QH9tfwW71s0Q/miOPPNKbPHky/VwRkYQ6juW+uNBgXCqV
-        yv9hCdgFWiGwdXZLnyX3Vpx11lled3c3/XwRkQSxyX8fYbkvLjQYJxcnAw7RbenmFYtFmtD9OOCAA7zr
-        r79eKzRKIsyZM8d74IEHapNbb7rpJu/OO+/0Hn74Ye0zIrexnBcnGoxTuVw+miVfF2SzWT0KaNJ1111H
-        k3k7jjrqKO+RRx6h3ycStyeeeML705/+5B100EG0/R599NHe3XffrYFA59qG5bw40WDckGhfZwnYBXZl
-        SypWGpxyyim0EwzCeeedp3oQZ9gcoXPOOYe2VeZ3v/udJhZ3ni6W6+JGg3ErlUoXsOTripkzZ7IKljqn
-        nnoq7fyCsv/++3uXX365Vy6X6feLhM0GoRdddBFtn6M5/fTTtcZIZ9mR5bq40WDcKpXKql1dXW+x5OsC
-        LRA0utNOO412fEGz+QFXXnml19PTQ3+HSNBshdCrrrqq1vZYm2yWDR7Y50vq9MBYluviRoMuwOj6apZ8
-        XaG9Akb2hz/8gXZ6YTnwwAO9q6++Wss3S2hsct/f/vY37+CDD6Zt0A+94dIR9mY5zgU06IJyubx2JpNZ
-        zJKvKyqVCqtsAXuHn3V4YbMJWDYBUY9pJCh2t++OO+6oLWHN2lw7brzxRvqdkhrzYDWW41xAg64oFou3
-        scTrEr0ayNlM5zA6zGYdcsgh3g033ODNnj2b/j6R0djdJEvQYbZjWyKbfbekxiEst7mCBl1RLpfXy2Qy
-        S1jidYXNANZ8AM7egWadXpQOPfTQ2hoCulsjzbLb8n/5y19qj5VYmwqaXi1OrfmwJsttrqBBlxSLxbtZ
-        4nWJ1gcY3hVXXEE7vajZWwMXXHBBbUdC9jtFrG3YK6a2HwVrQ2GwO1Xst0gqHMlymkto0CXlcvkDrm4S
-        VC+fz7MGIGAzplnnFxd7D/uuu+7SyoJSG7jbfJXf//73tK2E7be//S39XZJ4tunPe1lOcwkNuqZUKl3I
-        kq5rtF/A8O655x7fGwOFxXYpvOaaa7SoUAeyc9Vm9FsCZm0jKrYeAPt9kng7sVzmGhp0DZLrmGw2u7Ax
-        4bpI76MPz2bm2+I9Ud5ibYb9Hrv1O3XqVPq7JR3sNb57773XO/PMM2k7iIPtEcB+qyTakyyPuYgGXVQu
-        l/dnCddFWuZzZE8//bR30kkn0Q4xbrZeu71GaJM72W+X5Jk2bZp3ySWXBPr+fhDsURT7vZJ4m7Ec5iIa
-        dFV3d3eVJVzX2EqBdrVBGoYsZ89eb7/99tokKNY5uuDYY4+tvUpokzzZMYi7hm7x24CO1W3cbFLqY489
-        Rn+7JNotLHe5igZdValUtrbkypKua/R6YHPskYnf9dSjdMIJJ9TeCddkT3fZQG3ChAmh70PRLhv06nFT
-        Kr0Fn2a5y1U06LJCoYD8ypOua/R6YPNsK9XjjjuOdpiuOfHEE2uJRpMH42WLTVm7GT9+vHfMMcfQunLN
-        uHHj9Hgpvc5jOctlNOiySqWyfhJeCxyiK8bmWYd+8803D7ufuovsMYGtdfDggw9q+eEI2MqO9tqe3TWy
-        RZ5YnbjIrvptYSw9GkytubAOy1kuo0HXlUqlk1iydZVeD2yNbfF72WWX1Z6Tss7UVfY2gU1utFcLH330
-        UXX2AbAyfPzxx2vP8232frs78EVtaJMqDQ5T779YrnIdDSZBd3f3HJZsXaXXA1tXKBS8iy++2LnXBptl
-        AxjbFtkmEtpMdM0JGZ0t2WxX+LZ4lA2mklr39rvtzQMbzLLjlFT5G8tRSUCDSYCO4ouZTGYpS7au0uuB
-        /tjWy3/6059oR5skdjVoSe3SSy/1/v73v9cGBZ3cJmwlRjsv7rzzztot/aOOOoqWW9LYmhJ6c6RjvAAf
-        ZjkqCWgwKUql0hWNSdZl9gaDdg/0r6uryzv//PNpp5tkNjHsD3/4g/fXv/7Ve+CBB2qb0aRp8qglemv7
-        tgiPrbFgx2qv5yX16n44drfnH//4By0DSa09WW5KChpMElwdvsCSrausI9QWte2xcjz33HNpJ5wWNhHS
-        1qf/4x//WLsdfsstt3j33Xdf7a6BPRpxaR8DG6zYIy6rl0ceeaS2z4IlersSTmOib3TyySfXjpuVjaTa
-        AywnJQkNJkmlUtkyKWsDDLHfq8cB7bOrLZeWdY2a7a1gq8nZYMiWWLaJcrfddps3ceLE2tW2vZlgkxFt
-        0PDMM8/Ubkvb4MGStQ1C7a0LY3elbO97m6xqdx/sNTUrW3vFzv68fY4NPu64447aXQp7hHHOOefUXoc8
-        4ogjUp/gh2N3MqxsWduU1HsNNmI5KUloMGmKxeL1LNG6TjODg2GdsD0a6NREJNGxeRz2hooNlFhblI6x
-        H8tFSUODSYQTcpAlWdf19vayxiU+2BXstddeW9vlj3XeIn5Zm7r++ut1voq5jeWgJKLBJKpUKhtlMpnF
-        LMm6Tq8IBsuej9v2w65uOCTJYSsM2qMPrekgy82DD7IclEQ0mFTlcvlQlmCTwN5/bmhoEoCnnnrKu/DC
-        CxO3qJDEy+aW2NwHLeUtdRbDd1juSSoaTLJCoTCVJdgk0IqB4bG7LLYgj01aYx2+iF3t24ZPOg9lGCez
-        nJNkNJhk5XL5vdls9lWWYJNAG8yEy2a933///d5ZZ52lSYPiHXzwwbW3Gp588knaXkSWewJWYTknyWgw
-        6TAI2GLGjBmJWiWwnr2qpVuP4bNX32wVujPOOEODgQ5idW23+O1VST3blya8BBuyXJN0NJgGpVLpOJZc
-        k8J2EdQgIDr2iOD22293fi958c92btQtfmnRO/B9lmPSgAbTolgs3sCSa1KkbUnYpLANXGxBHVvhjSUS
-        SQa70rcB3YQJE/Tevvi1D8staUGDaYIr6WdYck0K2wjHnluThikRsDkZlkD0SmEy2BLKtiiUvQZqj3hY
-        nYo06SyWU9KEBtOkUCisktRFgobYJjh6Vhk/Syi2Va0tu2szxlkCkujZmx1WJ7Yev0t7JEii3QJjWE5J
-        ExpMm3K5vF42m13EkmtS2P4BWjrYLfaowK40//znP3tHHnkkTU4SPFuVz/Y/uPnmm2t7HLC6EWnDU7Am
-        yyVpQ4NphM56Y1xJv8OSa5LYBCbNC3CTPWe2VeNsBz8tRxwcu9tyySWX1HYZtEdirOxFAtIPid3fv1U0
-        mFYYBPxPkl8PHGKd4Lx581jjFYfYXRtLWldeeWVtr/hDDjmEJjh51wEHHOCdcsop3jXXXOM99NBDWntf
-        ovQyfJHljrSiwTTDFfSxLKkmjW3Zalu6NjRgcZxNKrTEZlv32mQ12y+fJcK0sxn6dmV/3nnn1bYYtu2G
-        bcCkga3E5G34HssZaUaDaYdO+K8sqSaRNhJKPtuP3/YssMcHNpnNFiay5Ghbz7LkmST1if666677V6LX
-        ZD1xzK9Yrkg7GuwE+Xz+aZZQk0grB6aXTfy0uz02w33ixIm1LWntebgtZXzcccfVlrJliTcKNs/hhBNO
-        qP2Wiy++uLYV89///nfvgQceqC2ta+1SiV4S4EyWIzoBDXaCNLweWC+bzaqz7VD2KMgmIFo7sDsJU6dO
-        9R5++OHaK4v2loLdWbjllltqq+DZVfhVV11Vu9Ngby+Yyy67rDZPwZ6724ZJNrveFkKyZZInTZpU+xz7
-        PPvcp59+ujYRVbfqJSUmQOpf9xsODXaKcrn8oaS/HlhPrwqKiDTtSViD5YZOQYOdJC2vB9az99MbGrqI
-        iLxrNnTM637DocFOg4T540wms5gl06SyW8JaQlhEZCVV+CzLBZ2GBjsRBgFbpu1OgF4VFBF516xZs57t
-        6en5BssBnYgGOxUGAf+JQcBbLJkmmb17rrsBItKpbNIq+sGXYAvW93cqGuxkGAR8IZvNvs4SaZLZ3QCM
-        funJISKSVraJFy7s3igUCl9nfX4no8FOh0HAhhgEvMoSadLZu9l6hUtE0s5ei7a5ULj4eTOfz/8f1td3
-        OhoU7z2VSuXDuVzuRZZEk85eF9Re6SKSVrZCqvVzuPJ/HYOAz7M+XjQAGFG5XP4AGs8/WRJNAxsda/Eg
-        EUkL689sszTr35D8F+KfP8X6dlmGBuVdGASsiUQ5pzF5poWNkrWfgIgkmS2FXqlU/tWvIfm/Av/G+nR5
-        Fw3KitCwVs3n8+X6xJk2NmqeM2cOPblERFxl/ZYthT7UlyHxL8hkMh9hfbmsiAZlZWhYYwqFwoyhRpZW
-        5XJZGwuJiPOsn7L+qr7/wkCgH39/H+vDZWU0KMPDIOCR+gaXRhhB17aoZSediEjcrH+qv+o33d3d+Nv0
-        VVi/LRwNysiKxeLE+oaXVrbrmxYQEhFXWH9k/VJjX4U++S7WV8vIaFBGhwb318ZGmEa2gFBvb68eC4hI
-        bIYm+dmk5fr+yf69XC5fxvpoGR0NSnPQ8A5HglxS3yDTyh4LaO0AEYmSJX67ALELkcY+yfpeDAoOYn2z
-        NIcGpXlogJvkcrlUrhrI2HM3LSksImFbvoQv7YcQf71UKn2L9cnSPBqU1mAQsFY+n7cZKLSxppG9Nqid
-        BkUkaHaB0TjBrx7+WxX9T8fv5R8EGhR/MCK9pPEZVdph4KP1A0SkbTaz31YnZf3MECT+yfj76qz/ldbR
-        oPhXLpd/1tXV9XZjw00722RIywqLSKvsAsIuJFi/MgQXVkswOPgt63PFPxqU9lQqlY+jsaZ2D4GR2Cs6
-        2m1QREazfI9+2o/UwwXVq+hPtZVvCGhQ2odBwFg07vtYg0675a/maA0BEVmJ9QvWPzTzuDSXy3VlMpl1
-        WB8r7aNBCQ4a+rhOeVWwkZ3gGAhpDQERqfUDQ9v0sv6iHv6fpfl8/gLWp0pwaFCChST49Ww2u5A19E5g
-        7/Daia87AiKdx271N3vFb7q6ut4sFAr/xfpSCRYNSvAwCFgHI9o8a/CdwjoAmyOgtwZE0s9m9dvkYNYX
-        DCeXy/V3d3evz/pQCR4NSniQAC9rdiScZva6jxYUEkkXu80/c+bM2joh7LwfjvWJGCzcgH8ew/pNCQcN
-        SrjsVcFsNvta40nQiWylLz0eEEk2O3/tPGZL9o7G+sJKpfJT1ldKuGhQwocGv3qxWLxHdwOWGXo8oLUE
-        RJLDHufZq3x++zFc9U/GBdF7WR8p4aNBiQ4GAt/L5XIvsZOjU+nxgIjb7Py085Sdv83o6upahIHDT1if
-        KNGhQYkWBgG2ZsB1GEUvZSdLp7LHA9qKWMQNQzvz2XnJztdmYeBwLz5jDdYXSrRoUOKBgcBXcXI8y06a
-        TqbHAyLxsfOuldf4hoOkvzCfz2/H+j6JBw1KvJDs/tCpiweNxtYMt9uPuisgEh6b1Gfb8dr5xs7DVuVy
-        uXvx97VYfyfxoUGJX6VS+RROvt7GE0mWsasRm3ykwYBIMIZe4bN399u92h+Cq/4XkPy3ZX2cxI8GxR3l
-        cvkonETvsJNLlhkaDMyePZt2bCLCWdK3QXQ7M/kZfNYSXMBchH9ehfVr4gYaFLdUKpX1MCqf0XiSycrs
-        PWSbL2CrkLEOT0QGa4PloJP+kO7u7iKS/4asLxO30KC4qVwu/zKbzb7BTjpZmQ0GbPKSBgMiy5bmtcGx
-        n8V6mmF9Ez5/H9Z3iZtoUNxVqVTWKhQKD4Uxck8ze3XJBgPah0A6ibV3a/fW/tl5EQQMKJYi8d89c+ZM
-        vdqXMDQo7sNA4Ov5fL7CTkgZmXWGKD8NBiSV7LU9a99hJv0hNlG5p6fnK6yPEvfRoCQHRvc/7O7uHmAn
-        p4wum83WOkt7Jqq3CSSJ7JU9m8hnV/rWnlk7Dxq+5/lisbgT65MkOWhQkgcn/265XG4BO1mlOfZYxZY3
-        tU1NNG9AXGUDVRuw2sC11V332tXV1bWwUCgczvogSR4alOTCQOBwjM4XspNXWmMDgnw+X1v+VI8LJE42
-        ILWBqQ1Q45j/k8lk3kLiPwv/PJb1O5JMNCjJVyqVzsJA4M3GE1n8s9nTtkiKrZCmZYklTDbgtIGnDUDj
-        nPCLNr8Yv2E8/lk79qUQDUo6VCqV1TEQuLJLCwmFwgYE9i61DQjmzZtHO3KRZtiA0tqRDTCtXbH2FiUM
-        OpZ2d3dPxEXEB1nfIulAg5IuGAi8H4nqdnQs2l8gRDbr2t6ztuVUNSCQkVjCt3ZiA8goZuu3Aon/8Vwu
-        9wnWl0i60KCkEwYCG+AKY4qN7tmJL8GyKzl7Zmuzs62zt9u6etOgs1h92/N7u51vg0ObtBfnLf3h2G9C
-        W50OG7O+Q9KJBiXdMBD4LAYCOOe1mFAc7FUtu/KzSV02m1t3C9LB6tFex7PZ+XYr37Ure8b6APzWZzA4
-        +RLrKyTdaFA6Azqqr+PkfwpXqrojEDPdLUgOqxerH3tmb1f1Vm9JG0zbOY9B6GNoa19kfYN0BhqUzoKB
-        wIfQGVyHK1PtM+AYdrdAA4NoWDnbs3ordyt/qwerD1ZPSYHE/zaO40Y751lfIJ2FBqVz2ToCuKJ5lnUe
-        4g67Y2DPk+1Ws12FWoKyOwf2vNmSlgYJI6tP7nYlb+Vn5Wiv3VmSt/Jl5Z5UXV1dr6KtnIl/XpWd99KZ
-        aFAEVwibo8N42m4VNnYmkgyWxCyZWVKz5GbPpi3ZWdKz5GdLyLLkmHR2XHaLfii523Hb1ftQcu+kuS84
-        3gEMFPfFP49h57l0NhoUGYLOcz10ntejI9GiQilkydCSoj3HtrsJlihtsGBzESxx2pWxsVnslkztLoNN
-        dLPkancbLNEaG1DY4wlLvs3efbD/z/5/+3P25+1z7DPts+07jH2ffa99v/0O+0322+w32m819rvt99uk
-        O01srdXpEpTHFNTrJuycFhlCgyIMOt5x6Fj+yTodEcYSst2JsORsf1eCDg/K+OV8Pn8+/nltdv6KNKJB
-        kZHgKmxLXHVNR2euxwMiMbJzEIPyIs7Hn7NzVWQkNCjSDAwEPlwsFm/ElYceD4hECOecbc5zG86/j7Nz
-        U6QZNCjSKns8kM/n+3RXQCQcy6/2Z5dKpaPx75rUJ22jQRG/KpXKOuigTsVgoF+DAZH25XK5Z3Gl/0dc
-        8f9/7JwT8YsGRYKAwcCHMBg4F1ctAxgM0M5NRFaWzWZfxCD6apw7n2TnlkgQaFAkaBgMrI/BwEX2FoEG
-        AyIry2Qyi3B+3IYr/q+wc0gkaDQoEiYMBj6OwcAV6OyeZx2hSKdA0n8LCf8BXPF/j50rImGiQZGoYDDw
-        mWKxeB06wRdZBymSNl1dXYvy+fy9aPM/xL+PZeeFSBRoUCQOGAx8GYOBm9ExvtLYaYokGdr0S2jbt8I3
-        WNsXiQMNisQNg4GvlkqlK3GlNCuTySxmnaqIq2YsW463H2340r6+vs+zNi4SNxoUcU25XP4hrp5uRKc6
-        gAGBXi8U53R1db2K9vlQoVDYA/+uXffEeTQo4rJKpTIWA4KdMCC4Ex3uc1pvQOKAhP8a2t9TcCza4EdZ
-        WxVxGQ2KJAkGBGtgQPBrXHk9aJMJ9ZqhhCGTybyBZD8jn8+fguSv9/Ml8WhQJMkwIFjXlibGgOCJbDa7
-        kHXmIqOxV/SQ8JHv8+eiHX2OtTWRJKNBkTTBgOBjpVLpVAwIZtgbBnpkII2sTaBtvIw2Mr1YLJ6NpL8x
-        a0siaUKDImlXLpe3wKDgdHT4D+Eqr9rV1fU2SwySPpbscUW/AEn+SST7P6IdfA9xvY8vHYcGRToRBgXr
-        wz5ICtcjORSQJF7V3YJkQ/0tweDuOVzdP4qB3umo028hrhn6IkCDIrIMksUYDAq2xFXiWYVCYQqSyCAS
-        yjv1SUbiZ2tF2FU96mc6Bm/j8fe9Ed8IdGUvMgwaFJGRYUDwUdjf1iZAwiniCvN5DAze1B2DcKGMbWLe
-        cxiMdaHsr0Md2NsfG7I6EpGR0aCI+IfE9GEkpm3hSPzz5UhQ92OQkEfi+ieuUl/D1eoSltw6HQZPi5Hg
-        X8Fgag7K6h8oslvgTNgd5bYx/p81WHmLiD80KCLhwuBgrXK5/C3YH/98PgYKd2CgMB2Jb569qZCWxwxI
-        6rXb8zie15DEn8exzQRbPGcCEvsZ+Puu+O9fxv/7PlZOIhIeGhSR+NmKh/B52BwDhe1gNzgQjsag4TS4
-        EK7C4OEmmIgBxIMwDTJIrkWYiQQ7APORdF+EV5GEX7fb6LDY7kTAUkvQ8A5ib4L994X4/16GBfC/UMWf
-        7YdeKEAGnsTnPgC34nuuwHeeg99gv+tX9lt7enq+MXv27H8bHBwcw45NROJHgyIiIpJuNCgiIiLpRoMi
-        IiKSbjQoIiIi6UaDIiIikm40KCIiIulGgyIiIpJuNCgiIiLpRoMiIiKSbjQoIiIi6UaDIiIikm40KCIi
-        IulGgyIiIpJuNCgiIiLpRoMiIiKSbjQoIiIi6UaDIiIikm40KCIiIulGgyIiIpJuNCgiIiLpRoMiIiKS
-        bjQoIiIi6UaDIiIikm40KCIiIulGgyIiIpJuNCgiIiLpRoMiIiKSbjQoIiIi6UaDIiIikmbee/4fFi8j
-        zX+PctYAAAAASUVORK5CYII=</value>
-  </data>
   <data name="$this.Icon" type="System.Drawing.Icon, System.Drawing" mimetype="application/x-microsoft.net.object.bytearray.base64">
     <value>AAABAAEAAAAAAAEAIACvPgAAFgAAAIlQTkcNChoKAAAADUlIRFIAAAEAAAABAAgGAAAAXHKoZgAAPnZJ
         REFUeNrtvXmcXNdZ5/09595be/Wi1i5LsoVsq1urHdtxHBLiYIgJIQkhbxLIggNDhoSwBHgnwzDMDDMv
         fCYMLwGGMG8y4ElIwJCQkIWQhRBnc4ITO7a2lixLlqy9W1JvtVfde877x6nbKrWq1d3V1d21nO/nU5+2
         S1W37nKe33nOc57zHLBYLBaLxWKxWCwWi8VisVgsFovFYrFYLBaLxWKxWCwWi8VisVgsFovFYrFYLG2B
         sLfAYrmec+fONe1YmzZtsgJgsbSp0XtAL9APbAY2AEkgAUSAEpAHssB54AwwAUwBfquLgRUAizX66+kF
         dgB3VV+7aww/BriAU/N5v/oqVoXgHHAAeKL6ehbItKIYWAGwWMM3uMAg8KPAg8A+YBUgF/EzPnClKgJf
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/Utilities.vb` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/Utilities.vb`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,30 @@
     ''' </remarks>
     Public Shared Sub ProcessRedditPosts(JSONToolStripMenuItem As ToolStripMenuItem)
         ' Collect inputs from the user
         Dim inputs = CollectInputs()
 
         If inputs.HasValue Then
             ' Initialize the DataGridView
-            DataGridViewHandler.AddColumn(ResultsForm.DataGridViewResults)
+            DataGridViewHandler.AddColumn(FormPosts.DataGridViewPosts)
 
             ' Fetch Reddit posts based on the inputs
             Dim processor As New PostsProcessor()
             Dim posts As JObject = processor.FetchPosts(inputs.Value.Subreddit, inputs.Value.Listing, inputs.Value.Limit, inputs.Value.Timeframe)
             Dim totalPosts As Integer = 0
             Dim keywordFound As Boolean = False
 
             ' Iterate over each post
             For Each post In posts("data")("children")
                 totalPosts += 1
                 ' Check if the post contains the keyword
                 If PostsProcessor.PostContainsKeyword(post, inputs.Value.Keyword.ToLower(Globalization.CultureInfo.InvariantCulture)) Then
                     ' Add the post to the DataGridView
-                    DataGridViewHandler.AddRow(ResultsForm.DataGridViewResults, post, totalPosts)
-                    ResultsForm.Show()
+                    DataGridViewHandler.AddRow(FormPosts.DataGridViewPosts, post, totalPosts)
+                    FormPosts.Show()
                     keywordFound = True
                 End If
             Next
 
             ' Check if the keyword was found in any posts
             If Not keywordFound Then
                 MessageBox.Show($"Keyword `{inputs.Value.Keyword}` was not found in any of the " + posts("data")("children").Count.ToString(Globalization.CultureInfo.InvariantCulture) _
@@ -71,30 +71,30 @@
 
 
     ''' <summary>
     ''' Collects and validates user inputs from StartForm and returns them as a Tuple.
     ''' </summary>
     ''' <returns>
     ''' Tuple containing:
-    ''' Keyword (String) - Keyword entered by user in the StartForm.
-    ''' Subreddit (String) - Subreddit entered by user in the StartForm.
+    ''' Keyword (String) - Keyword entered by user in theFormMain.
+    ''' Subreddit (String) - Subreddit entered by user in theFormMain.
     ''' Listing (String) - Listing chosen by user in the StartForm, defaults to 'top' if none is selected.
     ''' Limit (Integer) - Limit entered by user in the StartForm, defaults to 10 if the entered value is over 100.
     ''' Timeframe (String) - Timeframe chosen by user in the StartForm, defaults to 'all' if none is selected.
     ''' </returns>
     ''' <remarks>
     ''' If keyword or subreddit are empty, Displays a warning and returns nothing.
     ''' </remarks>
     Public Shared Function CollectInputs() As (Keyword As String, Subreddit As String, Listing As String, Limit As Integer, Timeframe As String)?
-        Dim keyword As String = StartForm.KeywordTextBox.Text.Trim()
-        Dim subreddit As String = StartForm.SubredditTextBox.Text.Trim()
+        Dim keyword As String = FormMain.TextBoxKeyword.Text.Trim()
+        Dim subreddit As String = FormMain.TextBoxSubreddit.Text.Trim()
         ' Convert the Listing and Subreddit to lowercase using InvariantCulture
-        Dim listing As String = If(String.IsNullOrEmpty(StartForm.ListingComboBox.Text), "top", StartForm.ListingComboBox.Text.ToLower(Globalization.CultureInfo.InvariantCulture).Trim())
-        Dim timeframe As String = If(String.IsNullOrEmpty(StartForm.TimeframeComboBox.Text), "all", StartForm.TimeframeComboBox.Text.ToLower(Globalization.CultureInfo.InvariantCulture).Trim())
-        Dim limit As Integer = StartForm.LimitNumericUpDown.Value
+        Dim listing As String = If(String.IsNullOrEmpty(FormMain.ComboBoxListing.Text), "top", FormMain.ComboBoxListing.Text.ToLower(Globalization.CultureInfo.InvariantCulture).Trim())
+        Dim timeframe As String = If(String.IsNullOrEmpty(FormMain.ComboBoxTimeframe.Text), "all", FormMain.ComboBoxTimeframe.Text.ToLower(Globalization.CultureInfo.InvariantCulture).Trim())
+        Dim limit As Integer = FormMain.NumericUpDownLimit.Value
 
         ' Validate inputs
         If String.IsNullOrEmpty(keyword) AndAlso String.IsNullOrEmpty(subreddit) Then
             MessageBox.Show("Keyword and Subreddit fields should not be empty.", "Invalid Inputs", MessageBoxButtons.OK, MessageBoxIcon.Warning)
             Return Nothing
         ElseIf String.IsNullOrEmpty(keyword) Then
             MessageBox.Show("Keyword field should not be empty.", "Invalid Input", MessageBoxButtons.OK, MessageBoxIcon.Warning)
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST/icon.ico` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST/icon.ico`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/RPST GUI/RPST.sln` & `reddit-post-scraping-tool-1.6.0.0/RPST GUI/RPST.sln`

 * *Files identical despite different names*

### Comparing `reddit-post-scraping-tool-1.5.0.0/pyproject.toml` & `reddit-post-scraping-tool-1.6.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["rpst"]
 
 [project]
 name = "reddit-post-scraping-tool"
-version = "1.5.0.0"
+version = "1.6.0.0"
 description = "Given a subreddit name and a keyword, RPST returns all top (by default) posts that contain the specified keyword."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["osint", "reddit-crawler", "reddit-scraping", "reddit"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/reddit_post_scraping_tool.egg-info/PKG-INFO` & `reddit-post-scraping-tool-1.6.0.0/reddit_post_scraping_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-post-scraping-tool
-Version: 1.5.0.0
+Version: 1.6.0.0
 Summary: Given a subreddit name and a keyword, RPST returns all top (by default) posts that contain the specified keyword.
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Richard Mwewa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,17 +40,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPST (Reddit Post Scraping Tool)
 Given a subreddit name and a keyword, RPST will return all posts from a specified listing (default is 'top') that contain the provided keyword.
 
 [![Upload Python Package](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/workflows/codeql.yml) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
-![2023-08-08_07-04](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/10d91093-7b24-4de9-9f02-454b842d6b8e)
-![2023-08-08_07-04_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/268a4c0e-d849-49a3-94ba-296d193774e1)
-
+![2023-08-09_04-05](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d8917a35-3eac-44ce-aa96-1f9685095254)
+![2023-08-09_04-05_1](https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/d2fe7269-91d4-49ad-87fb-44282c5637a7)
+***
 
 # ✅ Features
 ## GUI
 - [x] Dark mode (Right-click)
 - [x] Saves results to a JSON (Right-click)
 - [x] Logs errors to a file
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reddit-post-scraping-tool Version: 1.5.0.0 Summary:
+Metadata-Version: 2.1 Name: reddit-post-scraping-tool Version: 1.6.0.0 Summary:
 Given a subreddit name and a keyword, RPST returns all top (by default) posts
 that contain the specified keyword. Author-email: Richard Mwewa
 duck.com> License: MIT License Copyright (c) 2023 Richard Mwewa Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -31,18 +31,18 @@
 tool/actions/workflows/python-publish.yml/badge.svg)](https://github.com/
 rly0nheart/reddit-post-scraping-tool/actions/workflows/python-publish.yml) [!
 [CodeQL](https://github.com/rly0nheart/reddit-post-scraping-tool/actions/
 workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/reddit-post-
 scraping-tool/actions/workflows/codeql.yml) ![.Net](https://img.shields.io/
 badge/.NET-5C2D91?style=flat&logo=.net&logoColor=white) ![Python](https://
 img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54) !
-[2023-08-08_07-04](https://github.com/bellingcat/reddit-post-scraping-tool/
-assets/74001397/10d91093-7b24-4de9-9f02-454b842d6b8e) ![2023-08-08_07-04_1]
+[2023-08-09_04-05](https://github.com/bellingcat/reddit-post-scraping-tool/
+assets/74001397/d8917a35-3eac-44ce-aa96-1f9685095254) ![2023-08-09_04-05_1]
 (https://github.com/bellingcat/reddit-post-scraping-tool/assets/74001397/
-268a4c0e-d849-49a3-94ba-296d193774e1) # â Features ## GUI - [x] Dark mode
+d2fe7269-91d4-49ad-87fb-44282c5637a7) *** # â Features ## GUI - [x] Dark mode
 (Right-click) - [x] Saves results to a JSON (Right-click) - [x] Logs errors to
 a file ## CLI - [x] Saves results to a JSON (-j/--json) - [x] Automatically
 checks for new updates. Notifies user if update were found. # ð TODO ## GUI
 - [ ] Make it installable with a setup.exe/setup.msi file. - [x] Add manual
 dark mode option, that will be persistent in all sessions - [ ] Make it save
 results to a CSV file # ð Wiki [Refer to the Wiki](https://github.com/
 rly0nheart/reddit-post-scraping-tool/wiki) for installation instructions, in
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/rpst/__main.py` & `reddit-post-scraping-tool-1.6.0.0/rpst/__main.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     arguments = parser.parse_args()
 
     # Record the start time
     start_time = datetime.now()
 
     try:
         # Check for updates
-        check_updates(version_tag="1.5.0.0")
+        check_updates(version_tag="1.6.0.0")
 
         # Get posts with the provided/parsed arguments
         get_posts(arguments=arguments)
     except KeyboardInterrupt:
         log.warning("User interruption detected.")
     except Exception as e:
         log.error(f"An error occurred: {e}")
```

### Comparing `reddit-post-scraping-tool-1.5.0.0/rpst/__rpst_.py` & `reddit-post-scraping-tool-1.6.0.0/rpst/__rpst_.py`

 * *Files identical despite different names*


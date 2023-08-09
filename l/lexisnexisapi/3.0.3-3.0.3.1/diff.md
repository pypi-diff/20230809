# Comparing `tmp/lexisnexisapi-3.0.3.tar.gz` & `tmp/lexisnexisapi-3.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-3.0.3.tar", last modified: Mon Aug  7 17:36:24 2023, max compression
+gzip compressed data, was "lexisnexisapi-3.0.3.1.tar", last modified: Wed Aug  9 02:37:38 2023, max compression
```

## Comparing `lexisnexisapi-3.0.3.tar` & `lexisnexisapi-3.0.3.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:36:24.499274 lexisnexisapi-3.0.3/
--rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.3/LICENSE.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-07 17:36:24.499023 lexisnexisapi-3.0.3/PKG-INFO
--rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0.3/README.md
--rw-r--r--   0 rwcuffney   (501) staff       (20)      618 2023-08-07 17:35:29.000000 lexisnexisapi-3.0.3/pyproject.toml
--rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-07 17:36:24.499350 lexisnexisapi-3.0.3/setup.cfg
--rw-r--r--   0 rwcuffney   (501) staff       (20)      767 2023-08-07 17:35:43.000000 lexisnexisapi-3.0.3/setup.py
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:36:24.494887 lexisnexisapi-3.0.3/src/
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:36:24.497190 lexisnexisapi-3.0.3/src/lexisnexisapi/
--rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.3/src/lexisnexisapi/__init__.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0.3/src/lexisnexisapi/credentials.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     9672 2023-08-07 17:30:26.000000 lexisnexisapi-3.0.3/src/lexisnexisapi/metabase.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     3015 2023-08-07 17:28:58.000000 lexisnexisapi-3.0.3/src/lexisnexisapi/webservices.py
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:36:24.498664 lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6148 2023-08-04 20:10:21.000000 lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/.DS_Store
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-07 17:36:24.000000 lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/PKG-INFO
--rw-r--r--   0 rwcuffney   (501) staff       (20)      372 2023-08-07 17:36:24.000000 lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-07 17:36:24.000000 lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-07 17:36:24.000000 lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/top_level.txt
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-09 02:37:38.475015 lexisnexisapi-3.0.3.1/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.3.1/LICENSE.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      542 2023-08-09 02:37:38.474625 lexisnexisapi-3.0.3.1/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0.3.1/README.md
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-09 02:37:38.475146 lexisnexisapi-3.0.3.1/setup.cfg
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      789 2023-08-09 02:37:24.000000 lexisnexisapi-3.0.3.1/setup.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-09 02:37:38.468289 lexisnexisapi-3.0.3.1/src/
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-09 02:37:38.471693 lexisnexisapi-3.0.3.1/src/lexisnexisapi/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi/__init__.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi/credentials.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     9672 2023-08-07 17:30:26.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi/metabase.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     3015 2023-08-07 17:28:58.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi/webservices.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-09 02:37:38.474050 lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6148 2023-08-04 20:10:21.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/.DS_Store
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      542 2023-08-09 02:37:38.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      357 2023-08-09 02:37:38.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-09 02:37:38.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-09 02:37:38.000000 lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-3.0.3/PKG-INFO` & `lexisnexisapi-3.0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,180 +1,164 @@
-Metadata-Version: 2.1
-Name: lexisnexisapi
-Version: 3.0.3
-Summary: A module to support the lexisnexis metabase search api
-Home-page: 
-Author: Robert Cuffney
-Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
-License: MIT
-Keywords: example project
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Metabase.py Documentation
-
-## 1. Introduction
-
-### Overview
-
-The `metabase.py` module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.
-
-### Authors
-
-- Robert Cuffney
-- Ozgur Aycan
-- CS Integration Consultants @ LexisNexis
-
-### Version
-
-Current version: 3.0
-## 2. Installation
-
-### Dependencies
-
-To use the `metabase.py` module, you need the following dependencies:
-
-- requests
-- json
-- pandas
-- datetime
-- lexisnexisapi
-
-### Installation
-
-You can install the required dependencies using pip:
-
-```bash
-pip install requests pandas lexisnexisapi
-```
-
-## 3. Usage
-
-### Importing the Module
-
-To use the `metabase.py` module in your Python script, import it as follows:
-
-```python
-from lexisnexisapi import metabase
-```
-
-### Search Class
-
-The `Search` class is the main interface to perform searches and retrieve articles from Metabase. It has the following attributes and methods:
-
-#### Attributes:
-
-- `parameters`: A dictionary of Metabase search parameters.
-- `articles`: A list containing the articles retrieved from the Metabase API response.
-- `totalResults`: The total number of articles available in the search results.
-
-#### Methods:
-
-- `__init__(self, full_dataset=False, **kwargs)`: Initializes the Search object and performs the API request. If `full_dataset` is set to `True`, it retrieves all available articles by making multiple API calls.
-- `articles_dataframe(self, *args)`: Returns a Pandas DataFrame containing the articles' data. You can pass a list of desired fields (`*args`) to filter the DataFrame.
-- `create_file(self, file='articles.json')`: Creates a JSON file with the articles retrieved from the search.
-- `set_parameters(self, p)`: Sets the Metabase search parameters based on the input dictionary `p`.
-
-### Streamline Class
-
-The `Streamline` class helps maximize Metabase search calls without exceeding the rate limit. It keeps track of the remaining API calls per minute and waits for a new minute if needed.
-
-#### Attributes:
-
-- `key`: Metabase API key.
-- `start_minute`: The starting minute when the Streamline object is instantiated.
-- `minute_limit`: The maximum number of API calls allowed per minute based on the rate limit.
-- `calls_remaining`: The remaining API calls within the current minute.
-
-#### Methods:
-
-- `__init__(self, key)`: Initializes the Streamline object with the Metabase API key and fetches the rate limit information.
-- `track_calls(self)`: Updates the remaining API calls and waits for a new minute if the limit is reached.
-- `restart(self)`: Restarts the Streamline object.
-- `wait_for_new_min(self)`: Pauses execution until a new minute starts.
-- `get_current_minute(self)`: Returns the current minute as an integer.
-
-### Article Class
-
-The `Article` class represents an instance of a single article retrieved from Metabase. It sets each key from the article dictionary as an attribute of the class.
-
-### Helper Functions
-
-The module also provides some helper functions:
-
-- `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
-- `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
-- `set_Metabase_Search_Key(v)`: Sets the Metabase search key in the credentials.
-- `get_time()`: Returns the current minute as an integer.
-
-## 4. Examples
-
-### Basic Search Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a basic search
-search = metabase.Search(query="your_query_here", limit=100)
-
-# Get the DataFrame of articles
-df = search.articles_dataframe("title", "author", "published_date")
-print(df.head())
-```
-
-### Full Dataset Search Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a full dataset search
-search = metabase.Search(full_dataset=True, query="your_query_here")
-
-# Create a JSON file with all the articles
-search.create_file("articles_full.json")
-```
-
-### Article Instance Example
-
-```python
-from lexisnexisapi  import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a search and get an article instance
-search = metabase.Search(query="your_query_here", limit=1)
-article_instance = metabase.Article(search.articles[0])
-
-# Access attributes of the article instance
-print(article_instance.title)
-print(article_instance.author)
-print(article_instance.published_date)
-```
-
-### Index Terms Example
-
-```python
-from lexisnexisapi import metabase
-
-# Set the Metabase search key (optional, you can set it in the parameters directly)
-metabase.set_mb_search_key("your_metabase_key")
-
-# Perform a search
-search = metabase.Search(query="your_query_here", limit=100)
-
-# Get the DataFrame of index terms
-index_terms_df = metabase.indexTerms(search, "economy", "politics", "technology")
-print(index_terms_df.head())
-```
-
-Please note that you should replace `your_metabase_key` and `your_query_here` with your actual Metabase API key and desired search query, respectively, in the examples.
+# Metabase.py Documentation
+
+## 1. Introduction
+
+### Overview
+
+The `metabase.py` module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.
+
+### Authors
+
+- Robert Cuffney
+- Ozgur Aycan
+- CS Integration Consultants @ LexisNexis
+
+### Version
+
+Current version: 3.0
+## 2. Installation
+
+### Dependencies
+
+To use the `metabase.py` module, you need the following dependencies:
+
+- requests
+- json
+- pandas
+- datetime
+- lexisnexisapi
+
+### Installation
+
+You can install the required dependencies using pip:
+
+```bash
+pip install requests pandas lexisnexisapi
+```
+
+## 3. Usage
+
+### Importing the Module
+
+To use the `metabase.py` module in your Python script, import it as follows:
+
+```python
+from lexisnexisapi import metabase
+```
+
+### Search Class
+
+The `Search` class is the main interface to perform searches and retrieve articles from Metabase. It has the following attributes and methods:
+
+#### Attributes:
+
+- `parameters`: A dictionary of Metabase search parameters.
+- `articles`: A list containing the articles retrieved from the Metabase API response.
+- `totalResults`: The total number of articles available in the search results.
+
+#### Methods:
+
+- `__init__(self, full_dataset=False, **kwargs)`: Initializes the Search object and performs the API request. If `full_dataset` is set to `True`, it retrieves all available articles by making multiple API calls.
+- `articles_dataframe(self, *args)`: Returns a Pandas DataFrame containing the articles' data. You can pass a list of desired fields (`*args`) to filter the DataFrame.
+- `create_file(self, file='articles.json')`: Creates a JSON file with the articles retrieved from the search.
+- `set_parameters(self, p)`: Sets the Metabase search parameters based on the input dictionary `p`.
+
+### Streamline Class
+
+The `Streamline` class helps maximize Metabase search calls without exceeding the rate limit. It keeps track of the remaining API calls per minute and waits for a new minute if needed.
+
+#### Attributes:
+
+- `key`: Metabase API key.
+- `start_minute`: The starting minute when the Streamline object is instantiated.
+- `minute_limit`: The maximum number of API calls allowed per minute based on the rate limit.
+- `calls_remaining`: The remaining API calls within the current minute.
+
+#### Methods:
+
+- `__init__(self, key)`: Initializes the Streamline object with the Metabase API key and fetches the rate limit information.
+- `track_calls(self)`: Updates the remaining API calls and waits for a new minute if the limit is reached.
+- `restart(self)`: Restarts the Streamline object.
+- `wait_for_new_min(self)`: Pauses execution until a new minute starts.
+- `get_current_minute(self)`: Returns the current minute as an integer.
+
+### Article Class
+
+The `Article` class represents an instance of a single article retrieved from Metabase. It sets each key from the article dictionary as an attribute of the class.
+
+### Helper Functions
+
+The module also provides some helper functions:
+
+- `http_request(p)`: Performs an HTTP request to the Metabase API with the given parameters `p` and returns the API response as a dictionary.
+- `rate_check(mbkey)`: Calls the Metabase rate limit API and returns the results as a list of dictionaries.
+- `set_Metabase_Search_Key(v)`: Sets the Metabase search key in the credentials.
+- `get_time()`: Returns the current minute as an integer.
+
+## 4. Examples
+
+### Basic Search Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a basic search
+search = metabase.Search(query="your_query_here", limit=100)
+
+# Get the DataFrame of articles
+df = search.articles_dataframe("title", "author", "published_date")
+print(df.head())
+```
+
+### Full Dataset Search Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a full dataset search
+search = metabase.Search(full_dataset=True, query="your_query_here")
+
+# Create a JSON file with all the articles
+search.create_file("articles_full.json")
+```
+
+### Article Instance Example
+
+```python
+from lexisnexisapi  import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a search and get an article instance
+search = metabase.Search(query="your_query_here", limit=1)
+article_instance = metabase.Article(search.articles[0])
+
+# Access attributes of the article instance
+print(article_instance.title)
+print(article_instance.author)
+print(article_instance.published_date)
+```
+
+### Index Terms Example
+
+```python
+from lexisnexisapi import metabase
+
+# Set the Metabase search key (optional, you can set it in the parameters directly)
+metabase.set_mb_search_key("your_metabase_key")
+
+# Perform a search
+search = metabase.Search(query="your_query_here", limit=100)
+
+# Get the DataFrame of index terms
+index_terms_df = metabase.indexTerms(search, "economy", "politics", "technology")
+print(index_terms_df.head())
+```
+
+Please note that you should replace `your_metabase_key` and `your_query_here` with your actual Metabase API key and desired search query, respectively, in the examples.
```

### Comparing `lexisnexisapi-3.0.3/setup.py` & `lexisnexisapi-3.0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
+VERSION = '3.0.3.1'
 
 setup(
     name="lexisnexisapi",
-    version='3.0.3',
+    version= VERSION,
     license='MIT',
     author="Robert Cuffney",
     author_email='robert.cuffney@lexisnexis.com',
     description = 'a module to support the lexisnexis metabase search api',
     long_description = ' module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `lexisnexisapi-3.0.3/src/lexisnexisapi/credentials.py` & `lexisnexisapi-3.0.3.1/src/lexisnexisapi/credentials.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0.3/src/lexisnexisapi/metabase.py` & `lexisnexisapi-3.0.3.1/src/lexisnexisapi/metabase.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0.3/src/lexisnexisapi/webservices.py` & `lexisnexisapi-3.0.3.1/src/lexisnexisapi/webservices.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0.3/src/lexisnexisapi.egg-info/.DS_Store` & `lexisnexisapi-3.0.3.1/src/lexisnexisapi.egg-info/.DS_Store`

 * *Files identical despite different names*


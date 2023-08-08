# Comparing `tmp/meilisearch_python_async-1.4.8.tar.gz` & `tmp/meilisearch_python_async-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.4.8.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.5.0.tar", max compression
```

## Comparing `meilisearch_python_async-1.4.8.tar` & `meilisearch_python_async-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-07-20 02:40:01.607102 meilisearch_python_async-1.4.8/LICENSE
--rw-r--r--   0        0        0     5759 2023-07-20 02:40:01.607102 meilisearch_python_async-1.4.8/README.md
--rw-r--r--   0        0        0      151 2023-07-20 02:40:01.607102 meilisearch_python_async-1.4.8/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-07-20 02:40:01.607102 meilisearch_python_async-1.4.8/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0     1486 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/_utils.py
--rw-r--r--   0        0        0       18 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22970 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     2085 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89322 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0     1847 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1334 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0     3311 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11906 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2243 2023-07-20 02:40:01.611102 meilisearch_python_async-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 10:32:22.019360 meilisearch_python_async-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6058 2023-07-31 10:32:22.019360 meilisearch_python_async-1.5.0/README.md
+-rw-r--r--   0        0        0      151 2023-07-31 10:32:22.019360 meilisearch_python_async-1.5.0/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0     1486 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/_utils.py
+-rw-r--r--   0        0        0       18 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22970 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    99499 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0     1847 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1734 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     2234 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0     3326 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11906 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2243 2023-07-31 10:32:22.023360 meilisearch_python_async-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7217 1970-01-01 00:00:00.000000 meilisearch_python_async-1.5.0/PKG-INFO
```

### Comparing `meilisearch_python_async-1.4.8/LICENSE` & `meilisearch_python_async-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/README.md` & `meilisearch_python_async-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,20 @@
 
 ### Muiltiple Searches
 
 This test compares how long it takes to complete 1000 searches (lower is better)
 
 ![Multiple Searches](https://raw.githubusercontent.com/sanders41/meilisearch-python-async/main/assets/searches.png)
 
+### Independent testing
+
+[Prashanth Rao](https://github.com/prrao87) did some independent testing and found this async client
+to be ~30 faster than the sync client. You can find a good write-up of how he tested and the results
+in his [blog post](https://thedataquarry.com/posts/meilisearch-async/).
+
 ## Documentation
 
 See our [docs](https://meilisearch-python-async.paulsanders.dev) for the full documentation.
 
 ## Contributing
 
-Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
+Contributions to this project are welcome. If you are interested in contributing please see our [contributing guide](CONTRIBUTING.md)
```

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/_utils.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/_utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/client.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/index.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from httpx import AsyncClient
 
 from meilisearch_python_async._http_requests import HttpRequests
 from meilisearch_python_async._utils import is_pydantic_2, iso_to_date_time
 from meilisearch_python_async.errors import InvalidDocumentError, MeilisearchError
 from meilisearch_python_async.models.documents import DocumentsInfo
 from meilisearch_python_async.models.index import IndexStats
-from meilisearch_python_async.models.search import SearchResults
+from meilisearch_python_async.models.search import FacetSearchResults, SearchResults
 from meilisearch_python_async.models.settings import (
     Faceting,
     MeilisearchSettings,
     Pagination,
     TypoTolerance,
 )
 from meilisearch_python_async.models.task import TaskInfo
@@ -86,15 +86,15 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.delete()
         """
-        url = f"{self._base_url_with_uid}"
+        url = self._base_url_with_uid
         response = await self._http_requests.delete(url)
         return TaskInfo(**response.json())
 
     async def delete_if_exists(self) -> bool:
         """Delete the index if it already exists.
 
         Returns:
@@ -140,15 +140,15 @@
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     updated_index = await index.update()
         """
         payload = {"primaryKey": primary_key}
-        url = f"{self._base_url_with_uid}"
+        url = self._base_url_with_uid
         response = await self._http_requests.patch(url, payload)
         await wait_for_task(self.http_client, response.json()["taskUid"], timeout_in_ms=100000)
         index_response = await self._http_requests.get(f"{url}")
         self.primary_key = index_response.json()["primaryKey"]
         return self
 
     async def fetch_info(self) -> Index:
@@ -166,15 +166,15 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     index_info = await index.fetch_info()
         """
-        url = f"{self._base_url_with_uid}"
+        url = self._base_url_with_uid
         response = await self._http_requests.get(url)
         index_dict = response.json()
         self.primary_key = index_dict["primaryKey"]
         loop = get_running_loop()
         self.created_at = await loop.run_in_executor(
             None, partial(iso_to_date_time, index_dict["createdAt"])
         )
@@ -270,15 +270,15 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     stats = await index.get_stats()
         """
-        url = f"{self._stats_url}"
+        url = self._stats_url
         response = await self._http_requests.get(url)
 
         return IndexStats(**response.json())
 
     async def search(
         self,
         query: str | None = None,
@@ -295,14 +295,18 @@
         show_matches_position: bool = False,
         highlight_pre_tag: str = "<em>",
         highlight_post_tag: str = "</em>",
         crop_marker: str = "...",
         matching_strategy: str = "all",
         hits_per_page: int | None = None,
         page: int | None = None,
+        attributes_to_search_on: list[str] | None = None,
+        show_ranking_score: bool = False,
+        show_ranking_score_details: bool = False,
+        vector: list[float] | None = None,
     ) -> SearchResults:
         """Search the index.
 
         Args:
 
             query: String containing the word(s) to search
             offset: Number of documents to skip. Defaults to 0.
@@ -321,14 +325,32 @@
             highlight_pre_tag: The opening tag for highlighting text. Defaults to <em>.
             highlight_post_tag: The closing tag for highlighting text. Defaults to </em>
             crop_marker: Marker to display when the number of words excedes the `crop_length`.
                 Defaults to ...
             matching_strategy: Specifies the matching strategy Meilisearch should use. Defaults to `all`.
             hits_per_page: Sets the number of results returned per page.
             page: Sets the specific results page to fetch.
+            attributes_to_search_on: List of field names. Allow search over a subset of searchable
+                attributes without modifying the index settings. Defaults to None.
+            show_ranking_score: If set to True the ranking score will be returned with each document
+                in the search. Defaults to False.
+            show_ranking_score_details: If set to True the ranking details will be returned with
+                each document in the search. Defaults to False. Note: This parameter can only be
+                used with Meilisearch >= v1.3.0, and is experimental in Meilisearch v1.3.0. In order
+                to use this feature in Meilisearch v1.3.0 you first need to enable the feature by
+                sending a PATCH request to /experimental-features with { "scoreDetails": true }.
+                Because this feature is experimental it may be removed or updated causing breaking
+                changes in this library without a major version bump so use with caution.
+            vector: List of vectors for vector search. Defaults to None. Note: This parameter can
+                only be used with Meilisearch >= v1.3.0, and is experimental in Meilisearch v1.3.0.
+                In order to use this feature in Meilisearch v1.3.0 you first need to enable the
+                feature by sending a PATCH request to /experimental-features with
+                { "vectorStore": true }. Because this feature is experimental it may be removed or
+                updated causing breaking changes in this library without a major version bump so use
+                with caution.
 
         Returns:
 
             Results of the search
 
         Raises:
 
@@ -338,38 +360,167 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     search_results = await index.search("Tron")
         """
-        body = {
-            "q": query,
-            "offset": offset,
-            "limit": limit,
-            "filter": filter,
-            "facets": facets,
-            "attributesToRetrieve": attributes_to_retrieve,
-            "attributesToCrop": attributes_to_crop,
-            "cropLength": crop_length,
-            "attributesToHighlight": attributes_to_highlight,
-            "sort": sort,
-            "showMatchesPosition": show_matches_position,
-            "highlightPreTag": highlight_pre_tag,
-            "highlightPostTag": highlight_post_tag,
-            "cropMarker": crop_marker,
-            "matchingStrategy": matching_strategy,
-            "hitsPerPage": hits_per_page,
-            "page": page,
-        }
+        body = _process_search_parameters(
+            q=query,
+            offset=offset,
+            limit=limit,
+            filter=filter,
+            facets=facets,
+            attributes_to_retrieve=attributes_to_retrieve,
+            attributes_to_crop=attributes_to_crop,
+            crop_length=crop_length,
+            attributes_to_highlight=attributes_to_highlight,
+            sort=sort,
+            show_matches_position=show_matches_position,
+            highlight_pre_tag=highlight_pre_tag,
+            highlight_post_tag=highlight_post_tag,
+            crop_marker=crop_marker,
+            matching_strategy=matching_strategy,
+            hits_per_page=hits_per_page,
+            page=page,
+            attributes_to_search_on=attributes_to_search_on,
+            show_ranking_score=show_ranking_score,
+            show_ranking_score_details=show_ranking_score_details,
+            vector=vector,
+        )
+
         url = f"{self._base_url_with_uid}/search"
         response = await self._http_requests.post(url, body=body)
 
         return SearchResults(**response.json())
 
+    async def facet_search(
+        self,
+        query: str | None = None,
+        *,
+        facet_name: str,
+        facet_query: str,
+        offset: int = 0,
+        limit: int = 20,
+        filter: str | list[str | list[str]] | None = None,
+        facets: list[str] | None = None,
+        attributes_to_retrieve: list[str] = ["*"],
+        attributes_to_crop: list[str] | None = None,
+        crop_length: int = 200,
+        attributes_to_highlight: list[str] | None = None,
+        sort: list[str] | None = None,
+        show_matches_position: bool = False,
+        highlight_pre_tag: str = "<em>",
+        highlight_post_tag: str = "</em>",
+        crop_marker: str = "...",
+        matching_strategy: str = "all",
+        hits_per_page: int | None = None,
+        page: int | None = None,
+        attributes_to_search_on: list[str] | None = None,
+        show_ranking_score: bool = False,
+        show_ranking_score_details: bool = False,
+        vector: list[float] | None = None,
+    ) -> FacetSearchResults:
+        """Search the index.
+
+        Args:
+
+            query: String containing the word(s) to search
+            facet_name: The name of the facet to search
+            facet_query: The facet search value
+            offset: Number of documents to skip. Defaults to 0.
+            limit: Maximum number of documents returned. Defaults to 20.
+            filter: Filter queries by an attribute value. Defaults to None.
+            facets: Facets for which to retrieve the matching count. Defaults to None.
+            attributes_to_retrieve: Attributes to display in the returned documents.
+                Defaults to ["*"].
+            attributes_to_crop: Attributes whose values have to be cropped. Defaults to None.
+            crop_length: The maximun number of words to display. Defaults to 200.
+            attributes_to_highlight: Attributes whose values will contain highlighted matching terms.
+                Defaults to None.
+            sort: Attributes by which to sort the results. Defaults to None.
+            show_matches_position: Defines whether an object that contains information about the matches should be
+                returned or not. Defaults to False.
+            highlight_pre_tag: The opening tag for highlighting text. Defaults to <em>.
+            highlight_post_tag: The closing tag for highlighting text. Defaults to </em>
+            crop_marker: Marker to display when the number of words excedes the `crop_length`.
+                Defaults to ...
+            matching_strategy: Specifies the matching strategy Meilisearch should use. Defaults to `all`.
+            hits_per_page: Sets the number of results returned per page.
+            page: Sets the specific results page to fetch.
+            attributes_to_search_on: List of field names. Allow search over a subset of searchable
+                attributes without modifying the index settings. Defaults to None.
+            show_ranking_score: If set to True the ranking score will be returned with each document
+                in the search. Defaults to False.
+            show_ranking_score_details: If set to True the ranking details will be returned with
+                each document in the search. Defaults to False. Note: This parameter can only be
+                used with Meilisearch >= v1.3.0, and is experimental in Meilisearch v1.3.0. In order
+                to use this feature in Meilisearch v1.3.0 you first need to enable the feature by
+                sending a PATCH request to /experimental-features with { "scoreDetails": true }.
+                Because this feature is experimental it may be removed or updated causing breaking
+                changes in this library without a major version bump so use with caution.
+            vector: List of vectors for vector search. Defaults to None. Note: This parameter can
+                only be used with Meilisearch >= v1.3.0, and is experimental in Meilisearch v1.3.0.
+                In order to use this feature in Meilisearch v1.3.0 you first need to enable the
+                feature by sending a PATCH request to /experimental-features with
+                { "vectorStore": true }. Because this feature is experimental it may be removed or
+                updated causing breaking changes in this library without a major version bump so use
+                with caution.
+
+        Returns:
+
+            Results of the search
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_python_async import Client
+            >>> async with Client("http://localhost.com", "masterKey") as client:
+            >>>     index = client.index("movies")
+            >>>     search_results = await index.search(
+            >>>         "Tron",
+            >>>         facet_name="genre",
+            >>>         facet_query="Sci-fi"
+            >>>     )
+        """
+        body = _process_search_parameters(
+            q=query,
+            facet_name=facet_name,
+            facet_query=facet_query,
+            offset=offset,
+            limit=limit,
+            filter=filter,
+            facets=facets,
+            attributes_to_retrieve=attributes_to_retrieve,
+            attributes_to_crop=attributes_to_crop,
+            crop_length=crop_length,
+            attributes_to_highlight=attributes_to_highlight,
+            sort=sort,
+            show_matches_position=show_matches_position,
+            highlight_pre_tag=highlight_pre_tag,
+            highlight_post_tag=highlight_post_tag,
+            crop_marker=crop_marker,
+            matching_strategy=matching_strategy,
+            hits_per_page=hits_per_page,
+            page=page,
+            attributes_to_search_on=attributes_to_search_on,
+            show_ranking_score=show_ranking_score,
+            show_ranking_score_details=show_ranking_score_details,
+            vector=vector,
+        )
+
+        url = f"{self._base_url_with_uid}/facet-search"
+        response = await self._http_requests.post(url, body=body)
+
+        return FacetSearchResults(**response.json())
+
     async def get_document(self, document_id: str) -> dict[str, Any]:
         """Get one document with given document identifier.
 
         Args:
 
             document_id: Unique identifier of the document.
 
@@ -481,15 +632,15 @@
             >>>     {"id": 1, "title": "Movie 1", "genre": "comedy"},
             >>>     {"id": 2, "title": "Movie 2", "genre": "drama"},
             >>> ]
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.add_documents(documents)
         """
-        url = f"{self._documents_url}"
+        url = self._documents_url
         if primary_key:
             formatted_primary_key = urlencode({"primaryKey": primary_key})
             url = f"{url}?{formatted_primary_key}"
 
         response = await self._http_requests.post(url, documents)
 
         return TaskInfo(**response.json())
@@ -892,15 +1043,15 @@
             >>>     {"id": 1, "title": "Movie 1", "genre": "comedy"},
             >>>     {"id": 2, "title": "Movie 2", "genre": "drama"},
             >>> ]
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.update_documents(documents)
         """
-        url = f"{self._documents_url}"
+        url = self._documents_url
         if primary_key:
             formatted_primary_key = urlencode({"primaryKey": primary_key})
             url = f"{url}?{formatted_primary_key}"
 
         response = await self._http_requests.put(url, documents)
 
         return TaskInfo(**response.json())
@@ -1402,15 +1553,15 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.delete_all_document()
         """
-        url = f"{self._documents_url}"
+        url = self._documents_url
         response = await self._http_requests.delete(url)
 
         return TaskInfo(**response.json())
 
     async def get_settings(self) -> MeilisearchSettings:
         """Get settings of the index.
 
@@ -1426,15 +1577,15 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     settings = await index.get_settings()
         """
-        url = f"{self._settings_url}"
+        url = self._settings_url
         response = await self._http_requests.get(url)
 
         return MeilisearchSettings(**response.json())
 
     async def update_settings(self, body: MeilisearchSettings) -> TaskInfo:
         """Update settings of the index.
 
@@ -1479,15 +1630,15 @@
             >>>     await index.update_settings(new_settings)
         """
         if is_pydantic_2():
             body_dict = {k: v for k, v in body.model_dump(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
         else:  # pragma: no cover
             body_dict = {k: v for k, v in body.dict(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
 
-        url = f"{self._settings_url}"
+        url = self._settings_url
         response = await self._http_requests.patch(url, body_dict)
 
         return TaskInfo(**response.json())
 
     async def reset_settings(self) -> TaskInfo:
         """Reset settings of the index to default values.
 
@@ -1503,15 +1654,15 @@
         Examples:
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.reset_settings()
         """
-        url = f"{self._settings_url}"
+        url = self._settings_url
         response = await self._http_requests.delete(url)
 
         return TaskInfo(**response.json())
 
     async def get_ranking_rules(self) -> list[str]:
         """Get ranking rules of the index.
 
@@ -2428,10 +2579,73 @@
 
         if not isinstance(documents, list):
             raise InvalidDocumentError("Meilisearch requires documents to be in a list")
 
         return documents
 
 
+def _process_search_parameters(
+    *,
+    q: str | None = None,
+    facet_name: str | None = None,
+    facet_query: str | None = None,
+    offset: int = 0,
+    limit: int = 20,
+    filter: str | list[str | list[str]] | None = None,
+    facets: list[str] | None = None,
+    attributes_to_retrieve: list[str] = ["*"],
+    attributes_to_crop: list[str] | None = None,
+    crop_length: int = 200,
+    attributes_to_highlight: list[str] | None = None,
+    sort: list[str] | None = None,
+    show_matches_position: bool = False,
+    highlight_pre_tag: str = "<em>",
+    highlight_post_tag: str = "</em>",
+    crop_marker: str = "...",
+    matching_strategy: str = "all",
+    hits_per_page: int | None = None,
+    page: int | None = None,
+    attributes_to_search_on: list[str] | None = None,
+    show_ranking_score: bool = False,
+    show_ranking_score_details: bool = False,
+    vector: list[float] | None = None,
+) -> dict[str, Any]:
+    body: dict[str, Any] = {
+        "q": q,
+        "offset": offset,
+        "limit": limit,
+        "filter": filter,
+        "facets": facets,
+        "attributesToRetrieve": attributes_to_retrieve,
+        "attributesToCrop": attributes_to_crop,
+        "cropLength": crop_length,
+        "attributesToHighlight": attributes_to_highlight,
+        "sort": sort,
+        "showMatchesPosition": show_matches_position,
+        "highlightPreTag": highlight_pre_tag,
+        "highlightPostTag": highlight_post_tag,
+        "cropMarker": crop_marker,
+        "matchingStrategy": matching_strategy,
+        "hitsPerPage": hits_per_page,
+        "page": page,
+        "attributesToSearchOn": attributes_to_search_on,
+        "showRankingScore": show_ranking_score,
+    }
+
+    if facet_name:
+        body["facetName"] = facet_name
+
+    if facet_query:
+        body["facetQuery"] = facet_query
+
+    if show_ranking_score_details:
+        body["showRankingScoreDetails"] = show_ranking_score_details
+
+    if vector:
+        body["vector"] = vector
+
+    return body
+
+
 def _validate_file_type(file_path: Path) -> None:
     if file_path.suffix not in (".json", ".csv", ".ndjson"):
         raise MeilisearchError("File must be a json, ndjson, or csv file")
```

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/models/index.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/models/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/models/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from typing import Any, Dict, List, Optional, Union
 
 from camel_converter.pydantic_base import CamelBase
 from pydantic import Field
 
 
+class FacetHits(CamelBase):
+    value: str
+    count: int
+
+
+class FacetSearchResults(CamelBase):
+    facet_hits: List[FacetHits]
+    facet_query: str
+    processing_time_ms: int
+
+
 class SearchParams(CamelBase):
     index_uid: str
     query: Optional[str] = Field(None, alias="q")
     offset: int = 0
     limit: int = 20
     filter: Optional[Union[str, List[Union[str, List[str]]]]] = None
     facets: Optional[List[str]] = None
@@ -19,25 +30,30 @@
     show_matches_position: bool = False
     highlight_pre_tag: str = "<em>"
     highlight_post_tag: str = "</em>"
     crop_marker: str = "..."
     matching_strategy: str = "all"
     hits_per_page: Optional[int] = None
     page: Optional[int] = None
+    attributes_to_search_on: Optional[List[str]] = None
+    show_ranking_score: bool = False
+    show_ranking_score_details: bool = False
+    vector: Optional[List[float]] = None
 
 
 class SearchResults(CamelBase):
     hits: List[Dict[str, Any]]
     offset: Optional[int] = None
     limit: Optional[int] = None
     estimated_total_hits: Optional[int] = None
     processing_time_ms: int
     query: str
     facet_distribution: Optional[Dict[str, Any]] = None
     total_pages: Optional[int] = None
     total_hits: Optional[int] = None
     page: Optional[int] = None
     hits_per_page: Optional[int] = None
+    vector: Optional[List[float]] = None
 
 
 class SearchResultsWithUID(SearchResults):
     index_uid: str
```

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/models/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         @classmethod
         def validate_finished_at(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
 
 class TaskStatus(CamelBase):
     results: List[TaskResult]
+    total: int
     limit: int
     from_: int = Field(..., alias="from")
     next: Optional[int] = None
 
 
 class TaskInfo(CamelBase):
     task_uid: int
```

### Comparing `meilisearch_python_async-1.4.8/meilisearch_python_async/task.py` & `meilisearch_python_async-1.5.0/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.8/pyproject.toml` & `meilisearch_python_async-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.4.8"
+version = "1.5.0"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.4.8/PKG-INFO` & `meilisearch_python_async-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.4.8
+Version: 1.5.0
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -168,15 +168,21 @@
 
 ### Muiltiple Searches
 
 This test compares how long it takes to complete 1000 searches (lower is better)
 
 ![Multiple Searches](https://raw.githubusercontent.com/sanders41/meilisearch-python-async/main/assets/searches.png)
 
+### Independent testing
+
+[Prashanth Rao](https://github.com/prrao87) did some independent testing and found this async client
+to be ~30 faster than the sync client. You can find a good write-up of how he tested and the results
+in his [blog post](https://thedataquarry.com/posts/meilisearch-async/).
+
 ## Documentation
 
 See our [docs](https://meilisearch-python-async.paulsanders.dev) for the full documentation.
 
 ## Contributing
 
-Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
+Contributions to this project are welcome. If you are interested in contributing please see our [contributing guide](CONTRIBUTING.md)
```


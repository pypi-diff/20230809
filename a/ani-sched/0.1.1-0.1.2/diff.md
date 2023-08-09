# Comparing `tmp/ani-sched-0.1.1.tar.gz` & `tmp/ani-sched-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ani-sched-0.1.1.tar", last modified: Tue Aug  8 20:39:12 2023, max compression
+gzip compressed data, was "ani-sched-0.1.2.tar", last modified: Wed Aug  9 02:57:02 2023, max compression
```

## Comparing `ani-sched-0.1.1.tar` & `ani-sched-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 20:39:12.458883 ani-sched-0.1.1/
--rw-rw-rw-   0        0        0     1085 2023-08-07 00:22:17.000000 ani-sched-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1304 2023-08-08 20:39:12.457884 ani-sched-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-08-08 20:37:46.000000 ani-sched-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 20:39:12.407913 ani-sched-0.1.1/ani_sched/
--rw-rw-rw-   0        0        0      228 2023-08-08 19:08:22.000000 ani-sched-0.1.1/ani_sched/__init__.py
--rw-rw-rw-   0        0        0    12102 2023-08-08 19:36:11.000000 ani-sched-0.1.1/ani_sched/_ani_sched.py
--rw-rw-rw-   0        0        0     8417 2023-08-08 18:39:32.000000 ani-sched-0.1.1/ani_sched/_ani_sched_livechart.py
--rw-rw-rw-   0        0        0     2065 2023-08-08 05:14:55.000000 ani-sched-0.1.1/ani_sched/_base.py
--rw-rw-rw-   0        0        0      768 2023-08-06 04:59:48.000000 ani-sched-0.1.1/ani_sched/_news.py
--rw-rw-rw-   0        0        0      192 2023-08-06 04:59:48.000000 ani-sched-0.1.1/ani_sched/_recently_aired.py
--rw-rw-rw-   0        0        0      645 2023-08-08 05:09:01.000000 ani-sched-0.1.1/ani_sched/config.py
-drwxrwxrwx   0        0        0        0 2023-08-08 20:39:12.454886 ani-sched-0.1.1/ani_sched.egg-info/
--rw-rw-rw-   0        0        0     1304 2023-08-08 20:39:12.000000 ani-sched-0.1.1/ani_sched.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-08-08 20:39:12.000000 ani-sched-0.1.1/ani_sched.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 20:39:12.000000 ani-sched-0.1.1/ani_sched.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-08-08 20:39:12.000000 ani-sched-0.1.1/ani_sched.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-08 20:39:12.000000 ani-sched-0.1.1/ani_sched.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 20:39:12.458883 ani-sched-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-08-08 20:36:02.000000 ani-sched-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 02:57:02.067186 ani-sched-0.1.2/
+-rw-rw-rw-   0        0        0     1085 2023-08-07 00:22:17.000000 ani-sched-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1379 2023-08-09 02:57:02.066187 ani-sched-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-08-09 02:55:20.000000 ani-sched-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 02:57:02.026210 ani-sched-0.1.2/ani_sched/
+-rw-rw-rw-   0        0        0       76 2023-08-09 02:21:41.000000 ani-sched-0.1.2/ani_sched/__init__.py
+-rw-rw-rw-   0        0        0     9645 2023-08-09 02:46:50.000000 ani-sched-0.1.2/ani_sched/_ani_sched.py
+-rw-rw-rw-   0        0        0     1859 2023-08-09 02:39:44.000000 ani-sched-0.1.2/ani_sched/_base.py
+-rw-rw-rw-   0        0        0      645 2023-08-08 05:09:01.000000 ani-sched-0.1.2/ani_sched/config.py
+drwxrwxrwx   0        0        0        0 2023-08-09 02:57:02.063191 ani-sched-0.1.2/ani_sched.egg-info/
+-rw-rw-rw-   0        0        0     1379 2023-08-09 02:57:01.000000 ani-sched-0.1.2/ani_sched.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-08-09 02:57:01.000000 ani-sched-0.1.2/ani_sched.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 02:57:01.000000 ani-sched-0.1.2/ani_sched.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-08-09 02:57:01.000000 ani-sched-0.1.2/ani_sched.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-09 02:57:01.000000 ani-sched-0.1.2/ani_sched.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 02:57:02.067186 ani-sched-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-08-09 02:52:52.000000 ani-sched-0.1.2/setup.py
```

### Comparing `ani-sched-0.1.1/LICENSE` & `ani-sched-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ani-sched-0.1.1/PKG-INFO` & `ani-sched-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: ani-sched
-Version: 0.1.1
+Version: 0.1.2
 Summary: A local MAL API for anime schedules and news (using livechart.me)
 Home-page: https://github.com/lkaijie/ani-sched-api
 Author: lkaijie
 Author-email: 
 License: MIT
 Keywords: api,myanimelist,anime,schedule,news,livechart
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ani-Sched API
+# Python Anime Schedule API
 
 
-[![pypi Version](https://img.shields.io/pypi/v/mal-api.svg?color=informational)](https://pypi.org/project/mal-api/)
+[![pypi Version](https://img.shields.io/pypi/v/ani-sched.svg?color=informational)](https://pypi.org/project/ani-sched/)
 
-An unofficial lightweight API for gathering anime schedules from [MyAnimeList](https://myanimelist.net).
+A lightweight API for gathering anime schedules from [MyAnimeList](https://myanimelist.net) or anime news and announcements from [LiveChart](https://livechart.me).
 
 
 ## Installation and Usage
 
 To install the library:
 
 ```
```

### Comparing `ani-sched-0.1.1/ani_sched/_ani_sched_livechart.py` & `ani-sched-0.1.2/ani_sched/_ani_sched.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,161 @@
 import datetime
 from ani_sched import _base
 from ani_sched._base import _Base
 import ani_sched.config as config
 from typing import List, Dict
+import re
 
+class AniSched(_Base):
+    """AniSched class, used to get anime schedules from MyAnimeList
 
-class AniSched_livechart(_Base):
+    Methods:
+        get_sched(season=None, year=None)
+        
+        get_news()
+        
+        get_recently_aired()
+    Args:
+        timeout (int, optional): Timeout for the requests. Defaults to config.TIMEOUT.
+    """
     def __init__(self, timeout: int = config.TIMEOUT) -> None:
         super().__init__(timeout)
         self.headline_url = config.HEADLINE_ENDPOINT
         self.recently_aired_url = config.RECENTLY_AIRED_ENDPOINT
-        self.lc_url = config.LC_ENDPOINT
-        self.get_redirect(self.lc_url)
-        self.search_url = config.SEARCH_ENDPOINT
-        # self.endpoint = config.LC_ENDPOINT
-        #unused
-    def get_redirect(self, url: str) -> str:
-        # prob can be removed at some point
-        url = self._get_redirect(url)
-        self.lc_url2 = url+config.QUERY
 
-    def get_sched(self, season=None, year=None):
-        """Returns a dict of dicts containing the seasonal anime schedule
-        """
-        def _get_current_season(self) -> str:
-            """example output: winter-2021"""
-            current_month = datetime.datetime.now().month
-            current_year = datetime.datetime.now().year
+        self.mal_url = config.MAL_SCHEDULE_ENDPOINT
+        self.search_url = config.MAL_SEARCH_ENDPOINT
+
+
+    def get_sched(self, season=None, year=None)-> Dict[str, List[Dict]]:
+        """Extracts and returns the schedule from MyAnimeList
+
+        Args:
+            season (str, optional): season of anime. Defaults to None.
+            year (int, optional): year of season. Defaults to None.
+
+        Returns:
+            Dict[str, List[Dict]]: Dict of lists of dicts containing the schedule
             
-            if 1 <= current_month <= 3:
-                return f"winter-{current_year}"
-            elif 4 <= current_month <= 6:
-                return f"spring-{current_year}"
-            elif 7 <= current_month <= 9:
-                return f"summer-{current_year}"
-            elif 10 <= current_month <= 12:
-                return f"fall-{current_year}"
-            else:
-                return "Unknown"
-        
-        def _extract(self, soup):
-            """Returns a dict of dicts containing the seasonal anime schedule
+        Example:
+            {"TV (New)": [{"title": "Bocchi the Rock!",...}]}
+        """
+
+        def _extract_schedule(soup) -> List[Dict]:
+            """Extracts the schedule from the soup object
 
             Args:
-                soup (Beautiful Soup object): Of the anime section of the website
+                soup (BeautifulSoup4 Object): BeautifulSoup4 object of the schedule page ex. https://myanimelist.net/anime/season
 
             Returns:
-                dict: returns a dict containing the anime schedule
+                list: List of dicts containing animes in the schedule
             """
             animes = {}
-            for x in soup.find_all("div", class_="anime-card"):
-                print("type of x",type(x))
-                print("type of soup", type(soup))
-                title = x.find("a", attrs={"data-anime-card-target":"mainTitle"}).text
-                tags = []
-                for y in x.find_all("ol", class_="anime-tags"):
-                    for a in y.find_all("a"):
-                        tags.append(a.text)      
-                img_url = x.find("img", attrs={"data-anime-card-target":"poster"})["src"]
-                try:
-                    rating = x.find("div", class_="anime-avg-user-rating").text
-                except:
-                    rating = "Unknown"
-                studio = []
-                for y in x.find_all("ul", class_="anime-studios"):
-                    for a in y.find_all("a"):
-                        studio.append(a.text)
-                date = x.find("div", class_="anime-date").text
-                
-                source = "Unknown"
-                episodes = "Unknown"
-                for y in x.find("div", class_="anime-metadata"):
-                    if y.get("class") == ["anime-source"]:
-                        source = y.text
-                    elif y.get("class") == ["anime-episodes"]:
-                        episodes = y.text
             
-                summary = x.find("div", class_="anime-synopsis").text
-                # remove or add note section
-                links = []
-                for y in x.find_all("ul", class_="related-links"):
-                    for a in y.find_all("a"):
-                        links.append(a["href"])
-                        
-                info = {
-                    "title": title,
-                    "tags": tags,
-                    "img_url": img_url,
-                    "rating": rating,
-                    "studio": studio,
-                    "date": date,
-                    "source": source,
-                    "episodes": episodes,
-                    "summary": summary,
-                    "links": links
-                }
-                animes[title] = info
-            return animes  
-        
-        if not season:
-            season = _get_current_season(self)
-            # example url: https://www.livechart.me/winter-2021/tv
-            url = f"{self.lc_url}{season}/tv?titles=english"
-            entries = self._parse_url(url,type="selenium")
-            print(url)
-            return _extract(self, entries)
+            def extract_anime_type(soup):
+                animes = []
+                # js-anime-category-producer seasonal-anime
+                for x in soup.find_all("div", class_=re.compile(r'\bjs-anime-category-producer\b.*\bseasonal-anime\b')):
+                    title = x.find("a", class_="link-title").text
+                    try:
+                        title_eng = x.find("a", class_="link-title-english").text
+                    except:
+                        title_eng = title
+                    rating = x.find("div", attrs={"title":"Score"}).text.replace("\n", "").strip()
+                    try:
+                        img_url = x.find("img")["data-src"]
+                    except:
+                        img_url = x.find("img")["src"]
+
+                    members = x.find("div", attrs={"title":"Members"}).text.replace("\n", "").strip()
+                    tags = []
+                    for y in x.find_all("span", class_ = "genre"):
+                        tags.append(y.text.replace("\n", ""))
+                    studio = []
+                    properties = x.find("div", class_ = "properties")
+                    properties = properties.find_all("div")
+                    for u in properties[0].find_all("span", class_ = "item"):
+                        studio.append(u.text)
+                    source = properties[1].find("span", class_ = "item").text
+                    summary = x.find("p", class_ = "preline").text.replace("\n", "").replace("\r", "").strip()
+                    link = x.find("a", class_ = "link-title")["href"]
+                    date_and_episode = x.find("div", class_ = "prodsrc")
+                    date_and_episode = date_and_episode.find("div",class_="info")
+                    date_and_episode = date_and_episode.find_all("span", class_="item")
+                    start_date = date_and_episode[0].text.replace("\n", "").strip()
+                    episodes = date_and_episode[1].text.replace("\n", "").replace("         ", "").strip()
+                    
+                    anime_info = {
+                        "title": title,
+                        "title_eng": title_eng,
+                        "rating": rating,
+                        "img_url": img_url,
+                        "members": members,
+                        "tags": tags,
+                        "studio": studio,
+                        "source": source,
+                        "summary": summary,
+                        "episodes": episodes,
+                        "start_date": start_date,
+                        "link": link
+                    }
+                    animes.append(anime_info)
+                return animes
+            
+            new_soup = soup.find("div", class_="js-categories-seasonal")
+            for type_of_anime in new_soup.find_all("div", class_=re.compile(r'\bseasonal-anime-list\b.*\bjs-seasonal-anime-list\b')):
+                anime_type = type_of_anime.find("div", class_="anime-header").text
+                match anime_type:
+                    case "TV (New)":
+                        animes["TV (New)"] = extract_anime_type(type_of_anime)
+                        continue
+                    case "TV (Continuing)":
+                        animes["TV (Continuing)"] = extract_anime_type(type_of_anime)
+                        continue
+                    case "ONA":
+                        animes["ONA"] = extract_anime_type(type_of_anime)
+                        continue
+                    case "OVA":
+                        animes["OVA"] = extract_anime_type(type_of_anime)
+                        continue
+                    case "Movie":
+                        animes["Movie"] = extract_anime_type(type_of_anime)
+                        continue
+                    case "Special":
+                        animes["Special"] = extract_anime_type(type_of_anime)
+                        continue
+                    case _:
+                        continue
+            return animes
+   
+        if not season: # if no season is provided, get the current season
+            entries = self._parse_url(self.mal_url)
+            return _extract_schedule(entries)
         else:
             if not season and not year:
                 raise ValueError("Must provide season and year")
             elif season not in ["winter", "spring", "summer", "fall"]:
                 raise ValueError("Season must be one of the following: winter, spring, summer, fall")
             else:
-                # example url: https://www.livechart.me/summer-2021/tv
-                endpoint = f"{self.lc_url}{season}-{year}/tv?titles=english"
-                print(endpoint)
-                entries = self._parse_url(endpoint, type="selenium")
-                return _extract(self, entries)
-    
+                endpoint = f"{self.mal_url}/{year}/{season}"
+                return _extract_schedule(self._parse_url(endpoint))
+                
     def get_news(self) -> None:
         """Returns a list of dicts containing the news entries of the feed
         """
-        # print("Getting news...")
         entries = self._parse_feed(self.headline_url)
         return entries
     
     def get_recently_aired(self) -> None:
         """Returns a list of dicts containing the recently aired anime
         """
-        # print("Getting recently aired...")
         entries = self._parse_feed(self.recently_aired_url)
         return entries
         
-    def search_anime(self, query: str) -> List:
+    # def search_anime(self, query: str) -> List:
         """Returns a list of the first 5 search results
 
         Args:
             query (str): The search query
 
         Returns:
             List: returns a list in the format of [title, url]
@@ -149,15 +169,15 @@
                 url_list.append([title, url])
             return url_list
         
         url = f"{self.lc_url}search?q={query}"
         entries = self._parse_url(url, type="selenium")
         return _extract_search_results(entries)
         
-    def extract_link(self, url: str) -> Dict:
+    # def extract_link(self, url: str) -> Dict:
         """Returns a dict containing the anime info
 
         Args:
             url (str): The url of the anime
 
         Returns:
             dict: returns a dict containing the anime info
@@ -195,10 +215,7 @@
             "source": source,
             "episodes": episodes,
             "summary": summary,
             "links": links
         }
         return info
 
-if __name__ == "__main__":
-    anisched = AniSched()
-    anisched.get_sched("summer", 2021)
```

### Comparing `ani-sched-0.1.1/ani_sched/_base.py` & `ani-sched-0.1.2/ani_sched/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import feedparser
 import json
 import requests
-from selenium import webdriver
+# from selenium import webdriver
 from bs4 import BeautifulSoup
 
 
 
 class _Base:
     def __init__(self, timeout: int) -> None:
         self.timeout = timeout
@@ -17,44 +17,41 @@
             url (str): Url to parse
             type (str, optional): "selenium" allows for browsers that require JS, leave empty for requests instead. Defaults to None.
 
         Returns:
             soup: BeautifulSoup object of the url
         """
         if type == "normal" or type == None:
-            # use requests
             response = requests.get(url, timeout=self.timeout)
-            # soup = BeautifulSoup(response.text, "html.parser", from_encoding="utf-8")
             soup = BeautifulSoup(response.text, "html.parser")
             return soup
         
         elif type == "selenium":
-            # use selenium
-            options = webdriver.ChromeOptions()
-            options.add_argument('--ignore-certificate-errors')
-            options.add_argument('--headless=new')    
-            response = webdriver.Chrome(options=options)
-            response.get(url)
-            # soup = BeautifulSoup(response.page_source, "html.parser", from_encoding="utf-8")
-            soup = BeautifulSoup(response.page_source, "html.parser")
-            return soup
+            # options = webdriver.ChromeOptions()
+            # options.add_argument('--ignore-certificate-errors')
+            # options.add_argument('--headless=new')    
+            # response = webdriver.Chrome(options=options)
+            # response.get(url)
+            # soup = BeautifulSoup(response.page_source, "html.parser")
+            # return soup
+            pass
         
     
     def _parse_feed(self, url: str) -> None:
         """Returns a list of dicts containing the entries of the feed
 
         Args:
             url (str): url of rss feed
         """
         feed = feedparser.parse(url)
         entries = feed.entries
         return entries
         
     def _get_redirect(self, url: str) -> str:
-        """Returns the redirected url
+        """Returns the red irected url
 
         Args:
             url (str): url to redirect
 
         Returns:
             str: redirected url
         """
```

### Comparing `ani-sched-0.1.1/ani_sched/config.py` & `ani-sched-0.1.2/ani_sched/config.py`

 * *Files identical despite different names*

### Comparing `ani-sched-0.1.1/ani_sched.egg-info/PKG-INFO` & `ani-sched-0.1.2/ani_sched.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: ani-sched
-Version: 0.1.1
+Version: 0.1.2
 Summary: A local MAL API for anime schedules and news (using livechart.me)
 Home-page: https://github.com/lkaijie/ani-sched-api
 Author: lkaijie
 Author-email: 
 License: MIT
 Keywords: api,myanimelist,anime,schedule,news,livechart
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Ani-Sched API
+# Python Anime Schedule API
 
 
-[![pypi Version](https://img.shields.io/pypi/v/mal-api.svg?color=informational)](https://pypi.org/project/mal-api/)
+[![pypi Version](https://img.shields.io/pypi/v/ani-sched.svg?color=informational)](https://pypi.org/project/ani-sched/)
 
-An unofficial lightweight API for gathering anime schedules from [MyAnimeList](https://myanimelist.net).
+A lightweight API for gathering anime schedules from [MyAnimeList](https://myanimelist.net) or anime news and announcements from [LiveChart](https://livechart.me).
 
 
 ## Installation and Usage
 
 To install the library:
 
 ```
```

### Comparing `ani-sched-0.1.1/setup.py` & `ani-sched-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ani-sched",
-    version="0.1.1",
+    version="0.1.2",
     description="A local MAL API for anime schedules and news (using livechart.me)",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="lkaijie",
     author_email="",
     url="https://github.com/lkaijie/ani-sched-api",
     packages=setuptools.find_packages(),
-    install_requires=["requests", "beautifulsoup4","selenium","feedparser"],
+    install_requires=["requests", "beautifulsoup4","feedparser"],
     keywords=["api", "myanimelist", "anime", "schedule", "news", "livechart"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```


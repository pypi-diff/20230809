# Comparing `tmp/DeepLScrapper-1.6.0.tar.gz` & `tmp/DeepLScrapper-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLScrapper-1.6.0.tar", last modified: Thu Jul 27 22:34:57 2023, max compression
+gzip compressed data, was "DeepLScrapper-1.7.0.tar", last modified: Wed Aug  9 02:38:01 2023, max compression
```

## Comparing `DeepLScrapper-1.6.0.tar` & `DeepLScrapper-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:34:57.126063 DeepLScrapper-1.6.0/DeepLScrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/DeepLScrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/DeepLScrapper/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:38:01.351400 DeepLScrapper-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:38:01.351400 DeepLScrapper-1.7.0/DeepLScrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-09 02:37:51.000000 DeepLScrapper-1.7.0/DeepLScrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-09 02:37:51.000000 DeepLScrapper-1.7.0/DeepLScrapper/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:38:01.351400 DeepLScrapper-1.7.0/DeepLScrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-09 02:38:01.000000 DeepLScrapper-1.7.0/DeepLScrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-09 02:38:01.000000 DeepLScrapper-1.7.0/DeepLScrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 02:38:01.000000 DeepLScrapper-1.7.0/DeepLScrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-09 02:38:01.000000 DeepLScrapper-1.7.0/DeepLScrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-09 02:38:01.000000 DeepLScrapper-1.7.0/DeepLScrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-09 02:37:51.000000 DeepLScrapper-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-09 02:38:01.351400 DeepLScrapper-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-09 02:37:51.000000 DeepLScrapper-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 02:38:01.351400 DeepLScrapper-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-09 02:37:51.000000 DeepLScrapper-1.7.0/setup.py
```

### Comparing `DeepLScrapper-1.6.0/DeepLScrapper/translator.py` & `DeepLScrapper-1.7.0/DeepLScrapper/translator.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,69 +4,91 @@
 from fake_useragent import UserAgent
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from bs4 import BeautifulSoup
+import concurrent.futures
 
 
 class DeepLScrapper:
     """
-        A web scrapper for the DeepL translation service using Selenium.
+    A web scrapper for the DeepL translation service using Selenium.
 
-        This class allows you to translate texts from one language to another using the DeepL translation service.
-        It utilizes the Selenium WebDriver with a headless Chrome browser to interact with the DeepL website.
+    This class allows you to translate texts from one language to another using the DeepL translation service.
+    It utilizes the Selenium WebDriver with a headless Chrome browser to interact with the DeepL website.
 
-        Args:
-            rate_limit_delay (int, optional): The delay in seconds between retries when rate-limited by DeepL. Default is 10.
-
-        Attributes:
-            RATE_LIMIT_DELAY (int): The delay in seconds between retries when rate-limited by DeepL.
-
-        Note:
-            - Language detection (auto-detection) is not supported in this version. Please provide the source language.
-            - The 'fake_useragent' library is used to generate a random User-Agent for browser emulation.
+    Args:
+        rate_limit_delay (int, optional): The delay in seconds between retries when rate-limited by DeepL. Default is 10.
+        enable_caching (bool, optional): Enable or disable caching of translations. Default is True.
+        max_cache_size (int, optional): Maximum number of cached translations to keep. Default is 1000.
+        multi_threading (bool, optional): Enable or disable multi-threading for parallel translation. Default is False.
+        database_path (str, optional): Path to the SQLite database for translation memory. Default is 'translation_memory.db'.
+
+    Note:
+        - Language detection (auto-detection) is not supported in this version. Please provide the source language.
+        - The 'fake_useragent' library is used to generate a random User-Agent for browser emulation.
+        - If multi-threading is enabled, translations will be processed concurrently for improved efficiency.
     """
 
-    def __init__(self, rate_limit_delay=10):
+    def __init__(self, rate_limit_delay=10, enable_caching=True, max_cache_size=1000, multi_threading=False,
+                 database_path='translation_memory.db'):
+        self.ENABLE_CACHING = enable_caching
+        self.MAX_CACHE_SIZE = max_cache_size
         self.RATE_LIMIT_DELAY = rate_limit_delay
+        self.MULTI_THREADING = multi_threading
+        self.DATABASE_PATH = database_path
         self._initialize_driver()
         self._create_translation_table()
 
     def _initialize_driver(self):
         ua = UserAgent()
         user_agent = ua.random
         options = Options()
         options.add_argument(f"user-agent={user_agent}")
         options.add_argument("--headless")
         self.driver = webdriver.Chrome(options=options)
 
     def _create_translation_table(self):
-        conn = sqlite3.connect('translation_memory.db')
+        conn = sqlite3.connect(self.DATABASE_PATH)
         c = conn.cursor()
         c.execute('''CREATE TABLE IF NOT EXISTS translations 
                      (source_text TEXT, source_lang TEXT, target_lang TEXT, translation TEXT)''')
         conn.commit()
         conn.close()
 
     def _get_translation_from_memory(self, text, source_lang, target_lang):
-        conn = sqlite3.connect('translation_memory.db')
+        if not self.ENABLE_CACHING:
+            return None
+
+        conn = sqlite3.connect(self.DATABASE_PATH)
         c = conn.cursor()
         c.execute('''SELECT translation FROM translations 
                      WHERE source_text=? AND source_lang=? AND target_lang=?''', (text, source_lang, target_lang))
         result = c.fetchone()
         conn.close()
-        if result:
+        if result is not None:
             return result[0]
         return None
 
     def _store_translation_in_memory(self, text, source_lang, target_lang, translation):
-        conn = sqlite3.connect('translation_memory.db')
+        if not self.ENABLE_CACHING:
+            return
+
+        conn = sqlite3.connect(self.DATABASE_PATH)
         c = conn.cursor()
+
+        c.execute('SELECT COUNT(*) FROM translations')
+        cache_size = c.fetchone()[0]
+        if cache_size >= self.MAX_CACHE_SIZE:
+            c.execute(
+                'DELETE FROM translations WHERE rowid IN (SELECT rowid FROM translations ORDER BY rowid ASC LIMIT ?)',
+                (cache_size - self.MAX_CACHE_SIZE + 1,))
+
         c.execute('''INSERT INTO translations (source_text, source_lang, target_lang, translation) 
                      VALUES (?, ?, ?, ?)''', (text, source_lang, target_lang, translation))
         conn.commit()
         conn.close()
 
     def _translate_single_text(self, text, source_lang, target_lang, max_retries, retry_delay):
         cached_translation = self._get_translation_from_memory(text, source_lang, target_lang)
@@ -77,15 +99,16 @@
         retries = 0
         while retries < max_retries:
             try:
                 url = f'https://www.deepl.com/translator#{source_lang}/{target_lang}/{text}'
                 self.driver.get(url)
 
                 wait = WebDriverWait(self.driver, 10)
-                translation_element = wait.until(EC.visibility_of_element_located((By.CLASS_NAME, 'sentence_highlight')))
+                translation_element = wait.until(
+                    EC.visibility_of_element_located((By.CLASS_NAME, 'sentence_highlight')))
 
                 soup = BeautifulSoup(self.driver.page_source, 'html.parser')
                 translation = self._extract_translation(soup)
 
                 self._store_translation_in_memory(text, source_lang, target_lang, translation)
 
                 return translation
@@ -112,29 +135,44 @@
         elif isinstance(text, list):
             return self._translate_multiple_texts(text, source_lang, target_lang, max_retries, retry_delay)
         else:
             raise ValueError("Invalid 'text' parameter. It should be a string or a list of strings.")
 
     def _translate_multiple_texts(self, texts, source_lang, target_lang, max_retries, retry_delay):
         translations = []
-        for text in texts:
-            translation = self._translate_single_text(text, source_lang, target_lang, max_retries, retry_delay)
-            translations.append(translation)
+
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            future_to_text = {
+                executor.submit(self._translate_single_text, text, source_lang, target_lang, max_retries,
+                                retry_delay): text
+                for text in texts
+            }
+
+            for future in concurrent.futures.as_completed(future_to_text):
+                text = future_to_text[future]
+                try:
+                    translation = future.result()
+                    translations.append(translation)
+                except Exception as e:
+                    error_message = f"Translation failed for text '{text}': {e}"
+                    logging.error(error_message)
+                    translations.append(error_message)
+
         return translations
 
     def _extract_translation(self, soup):
         translation_element = soup.find('span', {'class': 'sentence_highlight'})
         if translation_element:
             translation = translation_element.text.strip()
             return translation
         else:
             raise ValueError("Translation not found on the page.")
 
     def clear_translation_memory(self):
-        conn = sqlite3.connect('translation_memory.db')
+        conn = sqlite3.connect(self.DATABASE_PATH)
         c = conn.cursor()
         c.execute('DELETE FROM translations')
         conn.commit()
         conn.close()
 
     def close(self):
         self.driver.quit()
```

### Comparing `DeepLScrapper-1.6.0/DeepLScrapper.egg-info/PKG-INFO` & `DeepLScrapper-1.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: DeepLScrapper
-Version: 1.6.0
-Summary: An unofficial Python library for translating text using DeepL
-Author: Olger Chotza
-Author-email: olgerdev@icloud.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DeepLScrapper
 
 An unofficial Python library for translating text using DeepL.
 
 ## Introduction
 
 ### Summary
@@ -29,23 +12,35 @@
 
 The idea behind the project is to create an unofficial Python library called "DeepLScrapper" that provides a workaround for the limitations of the official DeepL API. DeepL offers a powerful and accurate translation service, but it comes with certain usage restrictions and rate limits when accessing the service through their API.
 
 The goal of DeepLScrapper is to leverage web scraping techniques using Selenium WebDriver to interact with the DeepL translation website directly, allowing users to perform text translations without being bound by the API's usage limitations. By bypassing the API, the library can offer more flexibility in terms of translation volume and frequency, making it suitable for applications that require large-scale or frequent text translations.
 
 ### Key features
 
-- No API Limits: DeepLScrapper does not rely on the official DeepL API, enabling users to perform unlimited text translations without encountering rate limits or usage restrictions.
+- Unlimited Translations: DeepLScrapper offers unlimited text translations without relying on the official DeepL API, avoiding rate limits or usage restrictions.
+
+- Translation Versatility: This library accommodates both single text and bulk translation needs, catering to a wide range of use cases and applications.
+
+- Efficient Caching: DeepLScrapper employs an intelligent caching mechanism that stores past translations, reducing redundant requests and enhancing overall translation efficiency.
+
+- Custom Rate Limiting: Users have the freedom to set their preferred rate limit delay between retry attempts, providing flexibility in handling rate-limiting errors from the DeepL website.
+
+- Diverse User-Agent: The library generates a random User-Agent using the "fake_useragent" library, ensuring a diverse and realistic browser identity for seamless interaction with the DeepL website.
+
+- Multi-Threading Support: DeepLScrapper supports multi-threading, enabling parallel translation of multiple texts for faster and more efficient processing.
+
+- Comprehensive Error Handling: The library offers robust error handling, managing rate-limiting errors and providing informative error messages for easy troubleshooting.
 
-- Translation Flexibility: The library supports both single text translation and bulk translation of multiple texts, making it suitable for various use cases and applications.
+- Database Integration: The integrated SQLite database facilitates efficient storage and retrieval of translations, enhancing performance and data management.
 
-- Caching Mechanism: DeepLScrapper incorporates a caching mechanism to store previously translated texts, reducing redundant requests and improving translation efficiency.
+- Headless Browser Automation: Utilizing a headless Chrome browser via Selenium WebDriver, DeepLScrapper ensures a seamless and automated translation process.
 
-- Customizable Rate Limiting: Users can customize the rate limit delay between retry attempts in case of rate-limiting errors from the DeepL website.
+- Customizable Configuration: Users can customize caching settings, database paths, and more to tailor the library to their specific requirements.
 
-- User-Agent Randomization: The library generates a random User-Agent for browser emulation using the "fake_useragent" library, ensuring a diverse and realistic browser footprint.
+- Language Support: DeepLScrapper supports translation between various languages, providing a comprehensive language repertoire for diverse translation needs.
 
 By offering a versatile and unrestricted translation solution, DeepLScrapper provides developers with a powerful tool to integrate high-volume and frequent text translations into their applications without the limitations of the official DeepL API. However, it's important to keep in mind that the library should be used responsibly and in compliance with the DeepL website's terms of service and policies.
 
 ## Installation
 
 You can install DeepLScrapper using pip:
 
@@ -55,15 +50,15 @@
 
 ## Usage
 
 ```python
 from DeepLScrapper import DeepLScrapper
 
 # Initialize the translator with a custom rate limit delay of 5 seconds
-translator = DeepLScrapper(rate_limit_delay=5)
+translator = DeepLScrapper(rate_limit_delay=5, enable_caching=True, max_cache_size=100, multi_threading=True)
 
 try:
     # Translate text from English to German
     translation = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 1:", translation)
 
     # Translate the same text again to test caching
@@ -101,14 +96,17 @@
 - Selenium
 - BeautifulSoup4
 - fake_useragent
 - sqlite3
 
 ## Version History
 
+- 1.7.0
+    - Added a multi-threading feature. The class now supports multiple threads for faster translations.
+    - Added caching enabled/disabled option and a maximum cache size option.
 - 1.6.0
     - Added a translation memory feature. The class now stores previously translated texts in the database, reducing redundant requests to DeepL and speeding up translations for repeated texts.
 - 1.5.[0-2]
     - Restructured the project
     - Fixed the issue to using the library
     - Updated the documentation regarding the changes
 - 1.[1-4].0
@@ -125,8 +123,8 @@
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Support
 
-If you like this project, please consider giving it a ⭐. And check out my other projects on GitHub. If you would like to support me, donations are welcome.
+If you like this project, please consider giving it a ⭐. And check out my other projects on GitHub. If you would like to support me, donations are welcome.
```

### Comparing `DeepLScrapper-1.6.0/LICENSE` & `DeepLScrapper-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.6.0/PKG-INFO` & `DeepLScrapper-1.7.0/DeepLScrapper.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.6.0
+Version: 1.7.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -29,23 +29,35 @@
 
 The idea behind the project is to create an unofficial Python library called "DeepLScrapper" that provides a workaround for the limitations of the official DeepL API. DeepL offers a powerful and accurate translation service, but it comes with certain usage restrictions and rate limits when accessing the service through their API.
 
 The goal of DeepLScrapper is to leverage web scraping techniques using Selenium WebDriver to interact with the DeepL translation website directly, allowing users to perform text translations without being bound by the API's usage limitations. By bypassing the API, the library can offer more flexibility in terms of translation volume and frequency, making it suitable for applications that require large-scale or frequent text translations.
 
 ### Key features
 
-- No API Limits: DeepLScrapper does not rely on the official DeepL API, enabling users to perform unlimited text translations without encountering rate limits or usage restrictions.
+- Unlimited Translations: DeepLScrapper offers unlimited text translations without relying on the official DeepL API, avoiding rate limits or usage restrictions.
 
-- Translation Flexibility: The library supports both single text translation and bulk translation of multiple texts, making it suitable for various use cases and applications.
+- Translation Versatility: This library accommodates both single text and bulk translation needs, catering to a wide range of use cases and applications.
 
-- Caching Mechanism: DeepLScrapper incorporates a caching mechanism to store previously translated texts, reducing redundant requests and improving translation efficiency.
+- Efficient Caching: DeepLScrapper employs an intelligent caching mechanism that stores past translations, reducing redundant requests and enhancing overall translation efficiency.
 
-- Customizable Rate Limiting: Users can customize the rate limit delay between retry attempts in case of rate-limiting errors from the DeepL website.
+- Custom Rate Limiting: Users have the freedom to set their preferred rate limit delay between retry attempts, providing flexibility in handling rate-limiting errors from the DeepL website.
 
-- User-Agent Randomization: The library generates a random User-Agent for browser emulation using the "fake_useragent" library, ensuring a diverse and realistic browser footprint.
+- Diverse User-Agent: The library generates a random User-Agent using the "fake_useragent" library, ensuring a diverse and realistic browser identity for seamless interaction with the DeepL website.
+
+- Multi-Threading Support: DeepLScrapper supports multi-threading, enabling parallel translation of multiple texts for faster and more efficient processing.
+
+- Comprehensive Error Handling: The library offers robust error handling, managing rate-limiting errors and providing informative error messages for easy troubleshooting.
+
+- Database Integration: The integrated SQLite database facilitates efficient storage and retrieval of translations, enhancing performance and data management.
+
+- Headless Browser Automation: Utilizing a headless Chrome browser via Selenium WebDriver, DeepLScrapper ensures a seamless and automated translation process.
+
+- Customizable Configuration: Users can customize caching settings, database paths, and more to tailor the library to their specific requirements.
+
+- Language Support: DeepLScrapper supports translation between various languages, providing a comprehensive language repertoire for diverse translation needs.
 
 By offering a versatile and unrestricted translation solution, DeepLScrapper provides developers with a powerful tool to integrate high-volume and frequent text translations into their applications without the limitations of the official DeepL API. However, it's important to keep in mind that the library should be used responsibly and in compliance with the DeepL website's terms of service and policies.
 
 ## Installation
 
 You can install DeepLScrapper using pip:
 
@@ -55,15 +67,15 @@
 
 ## Usage
 
 ```python
 from DeepLScrapper import DeepLScrapper
 
 # Initialize the translator with a custom rate limit delay of 5 seconds
-translator = DeepLScrapper(rate_limit_delay=5)
+translator = DeepLScrapper(rate_limit_delay=5, enable_caching=True, max_cache_size=100, multi_threading=True)
 
 try:
     # Translate text from English to German
     translation = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 1:", translation)
 
     # Translate the same text again to test caching
@@ -101,14 +113,17 @@
 - Selenium
 - BeautifulSoup4
 - fake_useragent
 - sqlite3
 
 ## Version History
 
+- 1.7.0
+    - Added a multi-threading feature. The class now supports multiple threads for faster translations.
+    - Added caching enabled/disabled option and a maximum cache size option.
 - 1.6.0
     - Added a translation memory feature. The class now stores previously translated texts in the database, reducing redundant requests to DeepL and speeding up translations for repeated texts.
 - 1.5.[0-2]
     - Restructured the project
     - Fixed the issue to using the library
     - Updated the documentation regarding the changes
 - 1.[1-4].0
```

### Comparing `DeepLScrapper-1.6.0/setup.py` & `DeepLScrapper-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DeepLScrapper',
-    version='1.6.0',
+    version='1.7.0',
     description='An unofficial Python library for translating text using DeepL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Olger Chotza',
     author_email='olgerdev@icloud.com',
     packages=find_packages(),
     install_requires=[
```


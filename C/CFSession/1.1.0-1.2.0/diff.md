# Comparing `tmp/CFSession-1.1.0.tar.gz` & `tmp/CFSession-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CFSession-1.1.0.tar", last modified: Sun Aug  6 12:32:59 2023, max compression
+gzip compressed data, was "dist\CFSession-1.2.0.tar", last modified: Wed Aug  9 04:15:01 2023, max compression
```

## Comparing `CFSession-1.1.0.tar` & `CFSession-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 12:32:59.000000 CFSession-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-08-06 12:32:59.000000 CFSession-1.1.0/CFSession/
--rw-rw-rw-   0        0        0      515 2023-08-06 11:58:53.000000 CFSession-1.1.0/CFSession/__init__.py
--rw-rw-rw-   0        0        0     8180 2023-08-06 12:03:13.000000 CFSession-1.1.0/CFSession/cf.py
--rw-rw-rw-   0        0        0    12753 2023-08-06 12:08:31.000000 CFSession-1.1.0/CFSession/cfbrowser.py
--rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-1.1.0/CFSession/cfcookie.py
--rw-rw-rw-   0        0        0     1958 2023-08-06 11:56:03.000000 CFSession-1.1.0/CFSession/cfdefaults.py
--rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-1.1.0/CFSession/cfdirmodel.py
--rw-rw-rw-   0        0        0     2882 2023-04-09 04:00:18.000000 CFSession-1.1.0/CFSession/cfexception.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:32:59.000000 CFSession-1.1.0/CFSession.egg-info/
--rw-rw-rw-   0        0        0     3664 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3664 2023-08-06 12:32:59.000000 CFSession-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2023-07-20 10:13:27.000000 CFSession-1.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-08-06 12:32:59.000000 CFSession-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-08-05 19:24:50.000000 CFSession-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 04:15:01.000000 CFSession-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-08-09 04:15:01.000000 CFSession-1.2.0/CFSession/
+-rw-rw-rw-   0        0        0      515 2023-08-06 11:58:53.000000 CFSession-1.2.0/CFSession/__init__.py
+-rw-rw-rw-   0        0        0     9457 2023-08-09 02:50:13.000000 CFSession-1.2.0/CFSession/cf.py
+-rw-rw-rw-   0        0        0    13325 2023-08-09 03:06:24.000000 CFSession-1.2.0/CFSession/cfbrowser.py
+-rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-1.2.0/CFSession/cfcookie.py
+-rw-rw-rw-   0        0        0     1958 2023-08-06 11:56:03.000000 CFSession-1.2.0/CFSession/cfdefaults.py
+-rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-1.2.0/CFSession/cfdirmodel.py
+-rw-rw-rw-   0        0        0     2944 2023-08-09 03:03:30.000000 CFSession-1.2.0/CFSession/cfexception.py
+drwxrwxrwx   0        0        0        0 2023-08-09 04:15:01.000000 CFSession-1.2.0/CFSession.egg-info/
+-rw-rw-rw-   0        0        0     5965 2023-08-09 04:15:00.000000 CFSession-1.2.0/CFSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-08-09 04:15:00.000000 CFSession-1.2.0/CFSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 04:15:00.000000 CFSession-1.2.0/CFSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-08-09 04:15:00.000000 CFSession-1.2.0/CFSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-09 04:15:00.000000 CFSession-1.2.0/CFSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5965 2023-08-09 04:15:01.000000 CFSession-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4956 2023-08-09 02:15:39.000000 CFSession-1.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-09 04:15:01.000000 CFSession-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-08-08 22:59:31.000000 CFSession-1.2.0/setup.py
```

### Comparing `CFSession-1.1.0/CFSession/__init__.py` & `CFSession-1.2.0/CFSession/__init__.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.1.0/CFSession/cf.py` & `CFSession-1.2.0/CFSession/cf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #UC
 import undetected_chromedriver as uc
 #Sel
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
-from selenium.common.exceptions import StaleElementReferenceException
+from selenium.common.exceptions import StaleElementReferenceException, TimeoutException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 #Modules
 from .cfdefaults import Required_defaults
+from .cfdirmodel import cfDirectory
 from pathlib import Path
 import typing
 import time
 import sys
 import json
+import threading
 
 #Not a constant. CAPITAL for more readable syntax
 #If constant is ever declared we will use CONST_VARIABLE_NAME
 IGNORE_WARN = True
 STDOUT = False
 DEBUG = False
 DUMMY = False
@@ -60,14 +62,15 @@
     def __init__(self, driver: uc.Chrome, directory, target = ["Just a moment...","Please Wait..."], timeout: int = 40, bypass_mode: bool = True) -> None:
         self.TARGET_NAME = target
         self.driver = driver
         self.website = driver.current_url
         self.directory = directory
         self.timeout = timeout
         self.bypass_mode = bypass_mode
+        self.children = []
     
     def start(self):
         return self._main_process()
     
     def find_element(self, element, max_attempts=3, target: uc.Chrome =False):
         attempt = 1
         while True:
@@ -79,34 +82,56 @@
             except StaleElementReferenceException as e:
                 de_print(f"Error element stale {attempt}/{max_attempts} {e}")
                 if attempt == max_attempts:
                     raise
                 time.sleep(1)
                 attempt += 1
 
-    def init_bypass(self):
-        WaitFor = lambda i: WebDriverWait(self.driver, 10).until(
+    def WaitForElement(self, i):
+        WebDriverWait(self.driver, 10).until(
             EC.visibility_of(
             self.find_element(
             (By.TAG_NAME, 'body'),
-            ))) and time.sleep(i)
+        )))
+        time.sleep(i)
+
+    def init_bypass(self):
         self.driver.execute_script(f'window.open("{self.website}","_blank");')
-        WaitFor(5)
-        self.driver.switch_to.window(window_name=self.driver.window_handles[0])
-        self.driver.close() # close first tab
+        self.WaitForElement(10)
         self.driver.switch_to.window(window_name=self.driver.window_handles[0]) 
-        WaitFor(2)
-        
+        self.WaitForElement(5)
+        self.driver.close()
+        self.driver.switch_to.window(window_name=self.driver.window_handles[0])
+    
+    def click_bypass(self):
+        #https://stackoverflow.com/questions/76575298/how-to-click-on-verify-you-are-human-checkbox-challenge-by-cloudflare-using-se
+        try:
+            self.driver.execute_script(f'window.open("{self.website}","_blank");')
+            self.WaitForElement(5)
+            WebDriverWait(self.driver, 5).until(EC.frame_to_be_available_and_switch_to_it((By.CSS_SELECTOR,"iframe[title='Widget containing a Cloudflare security challenge']")))
+            WebDriverWait(self.driver, 5).until(EC.element_to_be_clickable((By.CSS_SELECTOR, "label.ctp-checkbox-label"))).click()
+            de_print("Clicked on verify")
+        except TimeoutException:
+            de_print("Click bypass Timeout")
+            self.driver.close()
+            self.driver.switch_to.window(window_name=self.driver.window_handles[0])
+        except Exception:
+            warn_print("An error occured on click_bypass")
+
+    def main_bypass(self):
+        self.click_bypass()
+
     def _main_process(self):
         timeout = 0
         if self.bypass_mode: self.init_bypass()
         while any(ext in self.driver.title for ext in self.TARGET_NAME):
             timeout += 1
             if timeout >= self.timeout:
                 break
+            if self.bypass_mode: self.main_bypass()
             norm_print("Waiting for cloudflare...")
             de_print(f"cur: {self.driver.title}")
             time.sleep(1)
         else:
             de_print(self.driver.title)
             de_print("Done")
             self.save_cookie_verified()
@@ -114,28 +139,31 @@
         de_print("Failed to bypass, return failure")
         return False
 
     def save_cookie(self, driver, file):
         """Cookie save, requires driver and file"""
         json.dump(driver, file)
 
-
     def save_cookie_verified(self):
         de_print('saving cookie')
         json.dump(self.driver.execute_script("return navigator.userAgent;"), open(self.directory.session_path(),"w"))
         if DEBUG and DUMMY:
             de_print("DUMMY COOKIE")
             dummy = [{"domain": ".nowsecure.nl", "expiry": 1690714605, "httpOnly": True, "name": "cf_clearance", "path": "/", "sameSite": "None", "secure": True, "value": "IOt5_jFk89BojBTV0NWAPj8zh4xq_zSxxt.2scnbY.4-1659175005-0-150"}]
             self.save_cookie(dummy , open(self.directory.cookie_path(),"w"))
         else:
             self.save_cookie(self.driver.get_cookies(), open(self.directory.cookie_path(),"w"))
             de_print("Cookies Saved")
+    
+    def clear_children(self):
+        for child in self.children:
+            child.join()
 
 class SiteBrowserProcess:
-    def __init__(self, destination: str, directory: str, headless_mode: bool = False, ignore_defaults: bool = False, defaults: typing.Union[Required_defaults, bool] = Required_defaults(), process_timeout: int = 40, bypass_mode: bool = True, *args, **kwargs) -> None:
+    def __init__(self, destination: str, directory: cfDirectory, headless_mode: bool = False, ignore_defaults: bool = False, defaults: typing.Union[Required_defaults, bool] = Required_defaults(), process_timeout: int = 10, bypass_mode: bool = True, *args, **kwargs) -> None:
         self.args = args
         self.kwargs = kwargs
         self.defaults = defaults
         self.ignore_defaults = ignore_defaults
         self.destination = destination
         self.directory = directory
         self.process_done = False
```

### Comparing `CFSession-1.1.0/CFSession/cfbrowser.py` & `CFSession-1.2.0/CFSession/cfbrowser.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,24 @@
         :param \*\*kwargs: Optional arguments that ``request`` takes.
         :return: :class:`Response <Response>` object
         :rtype: requests.Response
         """
         self.url = url
         return self.request("DELETE", url, **kwargs)
 
+    def options(self, url, **kwargs) -> requests.Response:
+        r"""Sends an OPTIONS request.
+        :param url: URL for the new :class:`Request` object.
+        :param \*\*kwargs: Optional arguments that ``request`` takes.
+        :return: :class:`Response <Response>` object
+        :rtype: requests.Response
+        """
+        self.url = url
+        return self.request("OPTIONS", url, **kwargs)
+
     def reload_token(self,site_requested,reset=False):
         cookieStatus =  self.cookieChecker.cookie_available()
         if not cookieStatus[0] or reset:
             self.cf_proccache = self._class_initialize(site_requested,directory=self.directory,*self.arg,**self.kwarg)
             if reset:
                 self.cookieChecker.delete_cookies()
             self.cf_proccache.start()
@@ -162,18 +172,21 @@
                     content = self.session.post(url, **kwargs)
                 elif method == "PATCH":
                     content = self.session.patch(url, **kwargs)
                 elif method == "PUT":
                     content = self.session.put(url, **kwargs)
                 elif method == "DELETE":
                     content = self.session.delete(url, **kwargs)
+                elif method == "OPTIONS":
+                    content = self.session.options(url, **kwargs)
                 content.raise_for_status()
                 return content
             except requests.exceptions.HTTPError as e:
                 http_code = e.response.status_code
+                http_content = e.response.content
                 caught_exception = e
                 if http_code == 404:
                     self.exception = NotFound(response=e.response)
                     break
                 elif http_code == 503:
                     #CF blocked us, update the token
                     #Recheck token
@@ -194,15 +207,15 @@
             except requests.exceptions.TooManyRedirects as e:
                 self.exception = TooManyRedirects(response=e.response)
                 break
             except requests.exceptions.Timeout as e:
                 self.exception = Timeout(response=e.response)
                 break
             except requests.exceptions.RequestException as e: #When an arbitrary error occurs
-                self.exception = CFException(response=e.response)
+                self.exception = CFException(message=repr(e))
                 break
         else:
             caught_code = caught_exception.response.status_code
             if caught_code == 503:
                 self.exception = CloudflareBlocked(response=caught_exception.response)
             self.exception = HTTPError(response=caught_exception.response)
         try:
```

### Comparing `CFSession-1.1.0/CFSession/cfcookie.py` & `CFSession-1.2.0/CFSession/cfcookie.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.1.0/CFSession/cfdefaults.py` & `CFSession-1.2.0/CFSession/cfdefaults.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.1.0/CFSession/cfdirmodel.py` & `CFSession-1.2.0/CFSession/cfdirmodel.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.1.0/CFSession/cfexception.py` & `CFSession-1.2.0/CFSession/cfexception.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 This module contains the exceptions for CFSession
 """
 
 class CFException(Exception): #Parent class
     def __init__(self,message=None,response=None,request=None, *args, **kwargs):
         """There was an ambiguous exception that occurred while handling your
     request."""
-        super().__init__(message,*args, **kwargs)
         self.response = response
+        message = repr(response) if not message else message
+        super().__init__(message,*args, **kwargs)
 
 
 
 class NetworkError(CFException): #Main class
     def __init__(self, response=None,*args,**kwargs):
         default_message = repr(response)
         super().__init__(default_message,response=response, *args, **kwargs)
```

### Comparing `CFSession-1.1.0/LICENSE` & `CFSession-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CFSession-1.1.0/setup.py` & `CFSession-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setup(
     name='CFSession',
-    version='1.1.0',
+    version='1.2.0',
     author='Kinuseka',
     author_email='realkingseeker1089@gmail.com',
     description='A Cloudflare IUAM session grabber',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Kinuseka/CFSession',
     classifiers=[
@@ -26,12 +26,12 @@
         'Operating System :: MacOS',
         'Intended Audience :: Developers',
         'Topic :: Internet',
         'Typing :: Typed'
     ],
     install_requires=[
         'requests>=2.25.0',
-        'undetected-chromedriver>=3.1.6'
+        'undetected-chromedriver>=3.1.6,!=3.5.1'
     ],
     packages=['CFSession'],
     python_requires=">=3.6",
 )
```


# Comparing `tmp/liveramp_automation-0.2.3.tar.gz` & `tmp/liveramp_automation-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.2.3.tar", last modified: Fri Aug  4 07:07:09 2023, max compression
+gzip compressed data, was "liveramp_automation-0.2.4.tar", last modified: Wed Aug  9 01:22:47 2023, max compression
```

## Comparing `liveramp_automation-0.2.3.tar` & `liveramp_automation-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:09.029425 liveramp_automation-0.2.3/
--rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.2.3/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-04 07:07:09.028629 liveramp_automation-0.2.3/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.2.3/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:08.986971 liveramp_automation-0.2.3/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      116 2023-08-03 08:05:33.000000 liveramp_automation-0.2.3/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-04 07:06:12.000000 liveramp_automation-0.2.3/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:09.000259 liveramp_automation-0.2.3/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.2.3/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.2.3/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     4054 2023-08-04 07:05:09.000000 liveramp_automation-0.2.3/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3921 2023-08-04 06:07:09.000000 liveramp_automation-0.2.3/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.2.3/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:09.015761 liveramp_automation-0.2.3/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.2.3/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1369 2023-08-02 08:00:32.000000 liveramp_automation-0.2.3/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.2.3/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      993 2023-08-02 08:00:32.000000 liveramp_automation-0.2.3/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1285 2023-08-02 08:22:54.000000 liveramp_automation-0.2.3/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     8485 2023-08-03 08:57:37.000000 liveramp_automation-0.2.3/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1282 2023-08-02 08:22:54.000000 liveramp_automation-0.2.3/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1091 2023-08-02 08:02:29.000000 liveramp_automation-0.2.3/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:08.992806 liveramp_automation-0.2.3/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-04 07:07:08.000000 liveramp_automation-0.2.3/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-04 07:07:08.000000 liveramp_automation-0.2.3/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-04 07:07:08.000000 liveramp_automation-0.2.3/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-04 07:07:08.000000 liveramp_automation-0.2.3/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-04 07:07:08.000000 liveramp_automation-0.2.3/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-04 07:07:09.029663 liveramp_automation-0.2.3/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1335 2023-08-02 08:44:39.000000 liveramp_automation-0.2.3/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:09.017648 liveramp_automation-0.2.3/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.2.3/tests/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:09.021172 liveramp_automation-0.2.3/tests/test_helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.2.3/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      498 2023-08-04 07:01:30.000000 liveramp_automation-0.2.3/tests/test_helpers/test_file.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-04 07:07:09.026631 liveramp_automation-0.2.3/tests/test_utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.2.3/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.2.3/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.2.3/tests/test_utils/test_request.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.147847 liveramp_automation-0.2.4/
+-rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.2.4/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-09 01:22:47.147052 liveramp_automation-0.2.4/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.2.4/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.085118 liveramp_automation-0.2.4/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-07 01:16:12.000000 liveramp_automation-0.2.4/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-09 01:22:25.000000 liveramp_automation-0.2.4/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.106219 liveramp_automation-0.2.4/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.2.4/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1731 2023-08-08 06:47:43.000000 liveramp_automation-0.2.4/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     4800 2023-08-08 05:44:22.000000 liveramp_automation-0.2.4/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3845 2023-08-08 05:44:22.000000 liveramp_automation-0.2.4/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.2.4/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.127633 liveramp_automation-0.2.4/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.2.4/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1369 2023-08-02 08:00:32.000000 liveramp_automation-0.2.4/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.2.4/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      993 2023-08-02 08:00:32.000000 liveramp_automation-0.2.4/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1285 2023-08-02 08:22:54.000000 liveramp_automation-0.2.4/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     8485 2023-08-03 08:57:37.000000 liveramp_automation-0.2.4/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)    24466 2023-08-09 00:44:35.000000 liveramp_automation-0.2.4/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1091 2023-08-02 08:02:29.000000 liveramp_automation-0.2.4/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.093315 liveramp_automation-0.2.4/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-09 01:22:46.000000 liveramp_automation-0.2.4/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1037 2023-08-09 01:22:46.000000 liveramp_automation-0.2.4/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-09 01:22:46.000000 liveramp_automation-0.2.4/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-09 01:22:46.000000 liveramp_automation-0.2.4/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-09 01:22:46.000000 liveramp_automation-0.2.4/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-09 01:22:47.148253 liveramp_automation-0.2.4/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     2333 2023-08-07 03:24:17.000000 liveramp_automation-0.2.4/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.130579 liveramp_automation-0.2.4/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.2.4/tests/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.135788 liveramp_automation-0.2.4/tests/test_helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.2.4/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      555 2023-08-07 03:16:53.000000 liveramp_automation-0.2.4/tests/test_helpers/test_file.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-09 01:22:47.145432 liveramp_automation-0.2.4/tests/test_utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.2.4/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.2.4/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       64 2023-08-04 08:01:46.000000 liveramp_automation-0.2.4/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.2.4/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       64 2023-08-08 08:12:12.000000 liveramp_automation-0.2.4/tests/test_utils/test_selenium.py
```

### Comparing `liveramp_automation-0.2.3/LICENSE` & `liveramp_automation-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/PKG-INFO` & `liveramp_automation-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 0.2.3
+Version: 0.2.4
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.2.3/README.md` & `liveramp_automation-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation/helpers/bucket.py` & `liveramp_automation-0.2.4/liveramp_automation/helpers/bucket.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 
 class BucketHelper:
     def __init__(self, project_id):
         self.project_id = project_id
         self.client = storage.Client(project=self.project_id)
 
-    def upload_to_bucket(self, src_path, dest_bucket_name, dest_path):
+    def upload_all_files_to_bucket(self, src_path, dest_bucket_name, dest_path):
         bucket_upload = self.client.bucket(dest_bucket_name)
         if os.path.isfile(src_path):
             blob = bucket_upload.blob(os.path.join(dest_path, os.path.basename(src_path)))
             blob.upload_from_filename(src_path)
             return
         for item in glob.glob(src_path + '/*'):
             if os.path.isfile(item):
                 if item == ".keep":
                     continue
                 blob = bucket_upload.blob(os.path.join(dest_path, os.path.basename(item)))
                 blob.upload_from_filename(item)
             else:
                 self.upload_to_bucket(item, dest_bucket_name, os.path.join(dest_path, os.path.basename(item)))
 
-    def download_from_bucket(self, src_bucket_name, src_path, dest_path):
+    def download_all_files_from_bucket(self, src_bucket_name, src_path, dest_path):
         bucket_download = self.client.bucket(src_bucket_name)
         blobs = bucket_download.list_blobs(prefix=src_path)
         for blob in blobs:
             if blob.name.endswith("/"):
                 continue
             file_name = os.path.join(dest_path, os.path.basename(blob.name))
             blob.download_to_filename(file_name)
```

### Comparing `liveramp_automation-0.2.3/liveramp_automation/helpers/file.py` & `liveramp_automation-0.2.4/liveramp_automation/helpers/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 class FileHelper:
 
     @staticmethod
     def read_json_report(path) -> dict:
         """Read all the content of the json file
 
         :param path:
-        :return:
+        :return: dict
         """
         with open(path, 'r') as file:
             json_string = file.read()
             data = json.loads(json_string)
         return data
 
     @staticmethod
     def read_init_file(file_path, file_name, file_mode="r") -> dict:
         """Read all the content of the init file
 
         :param file_path:
         :param file_name:
         :param file_mode:
-        :return: data_dict
+        :return: dict
         """
         try:
             full_path = os.path.join(file_path, file_name)
             with open(full_path, mode=file_mode) as file:
                 data_dict = {}
                 current_module = None
                 for line in file:
@@ -117,7 +117,28 @@
         result_dict = {
             "Cases": test_cases,
             "Failures": failures,
             "Errors": errors,
             "Skipped": skipped
         }
         return result_dict
+
+    @staticmethod
+    def files_under_folder_with_suffix_xlsx(path_string):
+        default_directory = os.path.join(os.getcwd(), path_string)
+        files = os.listdir(default_directory)
+        new_files = []
+        for file in files:
+            if ".xlsx" in file:
+                new_files.append(file)
+        return new_files
+
+    def files_under_folder_with_suffix_csv(default_directory):
+        files = os.listdir(default_directory)
+        new_files = []
+        for file in files:
+            if ".csv" in file:
+                new_files.append(file)
+        return new_files
+
+    def files_under_folder_with_suffix(file_suffix, folder_path):
+        return [file for file in os.listdir(folder_path) if file.endswith(file_suffix)]
```

### Comparing `liveramp_automation-0.2.3/liveramp_automation/helpers/login.py` & `liveramp_automation-0.2.4/liveramp_automation/helpers/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 from liveramp_automation.utils.log import Logger
 from liveramp_automation.utils.time import fixed_wait
 
 
 class LoginHepler:
 
     @staticmethod
-    def liveramp_okta_login_page(page, config, username, password):
+    def liveramp_okta_login_page(page, url, username, password):
         """
         This function, "liveramp_okta_login_page," facilitates Okta login using Playwright.
         Both the username and password are mandatory.
         Please invoke this API with the username and password provided in os.environ[].
         :param page:
-        :param config:
+        :param url:
         :param username:
         :param password:
         :return:
         """
         Logger.info("Going to login to OKTA...")
-        url = config['login_url']
         Logger.info("The login url is {}".format(url))
         page.goto(url)
         fixed_wait()
         url_new = page.url
         Logger.info("The current url is {}.".format(url_new))
         if url_new.__contains__(url):
             Logger.info("Login to OKTA succefully.")
@@ -35,27 +34,26 @@
             page.get_by_role("button", name="Sign In").click()
             Logger.info("We could login to OKTA successfully.")
             # wait for the login process to complete
             fixed_wait(20)
 
     #
     @staticmethod
-    def liveramp_okta_login_driver(driver, config, username, password):
+    def liveramp_okta_login_driver(driver, url, username, password):
         """
          "liveramp_okta_login_driver," is to facilitate Okta login using Selenium.
          Both the username and password are mandatory.
          Please utilize this API by providing the username and password from os.environ[].
         :param driver:
-        :param config:
+        :param url:
         :param username:
         :param password:
         :return:
         """
         Logger.info("Going to login to OKTA...")
-        url = config['login_url']
         Logger.info("The login url is {}.".format(url))
         driver.get(url)
         fixed_wait()
         if driver.current_url.__contains__(url):
             Logger.info("Login to OKTA succefully.")
         else:
             username_box = driver.find_element(by=By.ID, value='idp-discovery-username')
@@ -74,15 +72,15 @@
     def call_oauth2_get_token(username, password) -> str:
         """
         The purpose of the method `call_oauth2_get_token` is to initiate an OAuth2 login.
         Both the API username and password (sensitive) are mandatory for this process.
         Please ensure that you provide the required username and password from os.environ[] when calling this API.
         :param username:
         :param password:
-        :return:
+        :return: str
         """
         data = {
             "grant_type": "password",
             "scope": "openid",
             "client_id": "liveramp-api"
         }
         Logger.info("The default params are the {}".format(data))
```

### Comparing `liveramp_automation-0.2.3/liveramp_automation/utils/allure.py` & `liveramp_automation-0.2.4/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation/utils/log.py` & `liveramp_automation-0.2.4/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation/utils/parsers.py` & `liveramp_automation-0.2.4/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation/utils/playwright.py` & `liveramp_automation-0.2.4/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation/utils/request.py` & `liveramp_automation-0.2.4/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation/utils/time.py` & `liveramp_automation-0.2.4/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.2.3/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.2.4/liveramp_automation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.2.3
+Version: 0.2.4
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.2.3/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-0.2.4/liveramp_automation.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 liveramp_automation/utils/selenium.py
 liveramp_automation/utils/time.py
 tests/__init__.py
 tests/test_helpers/__init__.py
 tests/test_helpers/test_file.py
 tests/test_utils/__init__.py
 tests/test_utils/test_log.py
-tests/test_utils/test_request.py
+tests/test_utils/test_playwright.py
+tests/test_utils/test_request.py
+tests/test_utils/test_selenium.py
```


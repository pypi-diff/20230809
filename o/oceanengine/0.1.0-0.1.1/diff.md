# Comparing `tmp/oceanengine-0.1.0.tar.gz` & `tmp/oceanengine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanengine-0.1.0.tar", last modified: Fri Mar  3 09:44:55 2023, max compression
+gzip compressed data, was "oceanengine-0.1.1.tar", last modified: Tue Aug  8 04:28:25 2023, max compression
```

## Comparing `oceanengine-0.1.0.tar` & `oceanengine-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-03-03 09:44:55.119665 oceanengine-0.1.0/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2416 2023-03-03 09:44:55.119542 oceanengine-0.1.0/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2025 2023-03-03 09:33:30.000000 oceanengine-0.1.0/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-03-03 09:44:55.118679 oceanengine-0.1.0/oceanengine/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      372 2023-03-03 09:40:32.000000 oceanengine-0.1.0/oceanengine/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    17328 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/ad.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8962 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/ad_postback.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    19161 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/business.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3185 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/cc.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3709 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/e.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2337 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/m_toutiao.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    22055 2023-03-03 09:33:30.000000 oceanengine-0.1.0/oceanengine/open.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-03-03 09:44:55.119357 oceanengine-0.1.0/oceanengine.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2416 2023-03-03 09:44:55.000000 oceanengine-0.1.0/oceanengine.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      365 2023-03-03 09:44:55.000000 oceanengine-0.1.0/oceanengine.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-03-03 09:44:55.000000 oceanengine-0.1.0/oceanengine.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       47 2023-03-03 09:44:55.000000 oceanengine-0.1.0/oceanengine.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       12 2023-03-03 09:44:55.000000 oceanengine-0.1.0/oceanengine.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-03-03 09:44:55.119728 oceanengine-0.1.0/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      932 2023-03-03 09:44:27.000000 oceanengine-0.1.0/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-08 04:28:25.967849 oceanengine-0.1.1/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2416 2023-08-08 04:28:25.967741 oceanengine-0.1.1/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2025 2023-03-03 09:33:30.000000 oceanengine-0.1.1/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-08 04:28:25.966785 oceanengine-0.1.1/oceanengine/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      372 2023-03-03 09:40:32.000000 oceanengine-0.1.1/oceanengine/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    17328 2023-03-03 09:33:30.000000 oceanengine-0.1.1/oceanengine/ad.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8962 2023-03-03 09:33:30.000000 oceanengine-0.1.1/oceanengine/ad_postback.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    22928 2023-08-08 04:26:52.000000 oceanengine-0.1.1/oceanengine/business.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3185 2023-03-03 09:33:30.000000 oceanengine-0.1.1/oceanengine/cc.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3709 2023-03-03 09:33:30.000000 oceanengine-0.1.1/oceanengine/e.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2337 2023-03-03 09:33:30.000000 oceanengine-0.1.1/oceanengine/m_toutiao.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    22055 2023-03-03 09:33:30.000000 oceanengine-0.1.1/oceanengine/open.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-08 04:28:25.967546 oceanengine-0.1.1/oceanengine.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2416 2023-08-08 04:28:25.000000 oceanengine-0.1.1/oceanengine.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      365 2023-08-08 04:28:25.000000 oceanengine-0.1.1/oceanengine.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-08-08 04:28:25.000000 oceanengine-0.1.1/oceanengine.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       47 2023-08-08 04:28:25.000000 oceanengine-0.1.1/oceanengine.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       12 2023-08-08 04:28:25.000000 oceanengine-0.1.1/oceanengine.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-08-08 04:28:25.967889 oceanengine-0.1.1/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      932 2023-08-08 04:27:51.000000 oceanengine-0.1.1/setup.py
```

### Comparing `oceanengine-0.1.0/PKG-INFO` & `oceanengine-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanengine
-Version: 0.1.0
+Version: 0.1.1
 Summary: make it easy to use oceanengine
 Home-page: https://gitee.com/ZeroSeeker/oceanengine
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanengine-0.1.0/README.md` & `oceanengine-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine/ad.py` & `oceanengine-0.1.1/oceanengine/ad.py`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine/ad_postback.py` & `oceanengine-0.1.1/oceanengine/ad_postback.py`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine/business.py` & `oceanengine-0.1.1/oceanengine/business.py`

 * *Files 10% similar despite different names*

```diff
@@ -154,16 +154,14 @@
         headers=headers,
         timeout=timeout,
         return_json=True
     )
     return response
 
 
-
-
 def business_bm_user_id(
         cookie: str,
         csrf_token: str,
         timeout: int = 5
 ):
     """
     直接获取user_id
@@ -590,10 +588,136 @@
     }
     response = lazyrequests.lazy_requests(
         method='POST',
         url=url,
         headers=headers,
         json=data,
         timeout=timeout,
+        return_json=True
+    )
+    return response
+
+
+def bp_promotion_ad_get_account_list(
+        cookie: str,
+        csrf_token: str,
+        page: int = 1,
+        page_size: int = 10,
+        timeout: int = 5,
+        start_date: str = None,
+        end_date: str = None,
+        order_field: str = 'stat_cost',
+        order_type: int = 1
+):
+    """
+    主账号
+    【推广】-【巨量广告】-【账户】
+    :param cookie:
+    :param csrf_token:
+    :param page: 页码，默认为1
+    :param page_size: 每页数量，默认为10，可选10，20，50，100
+    :param timeout: 超时时间，单位为秒，默认为5
+    :param start_date: 开始日期，默认为当日0点，例如：2022-03-21
+    :param end_date: 结束日期，默认为次日0点，例如：2022-03-22
+    :param order_field: 排序列，默认为stat_cost，默认按照消耗排序
+    :param order_type: 排序方式：0:升序，1:降序；默认为1，降序
+    """
+
+    if start_date:
+        start_time = lazytime.get_date2timestamp(date=start_date)
+    else:
+        start_time = lazytime.get_date2timestamp(date=lazytime.get_date_string(-1))
+
+    if end_date:
+        end_time = lazytime.get_date2timestamp(date=end_date) + 86400
+    else:
+        end_time = lazytime.get_date2timestamp(date=lazytime.get_date_string(0))
+
+    url = "https://business.oceanengine.com/nbs/api/bm/promotion/ad/get_account_list"
+    headers = {
+        "Accept": "application/json, text/plain, */*",
+        "Accept-Encoding": "gzip, deflate",
+        "Accept-Language": "zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2",
+        "Connection": "keep-alive",
+        "Content-Type": "application/json",
+        "Cookie": cookie,
+        "Host": "business.oceanengine.com",
+        "Origin": "https://business.oceanengine.com",
+        "Referer": "https://business.oceanengine.com/site/promotion/ad/superior/account",
+        "Sec-Fetch-Dest": "empty",
+        "Sec-Fetch-Mode": "cors",
+        "Sec-Fetch-Site": "same-origin",
+        "TE": "trailers",
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/115.0",
+        "x-csrf-token": csrf_token,
+    }
+    data = {
+        "offset": page,
+        "limit": page_size,
+        "order_type": order_type,
+        "order_field": order_field,
+        "fields": [
+            "convert_cnt",
+            "conversion_cost",
+            "conversion_rate",
+            "deep_convert_cnt",
+            "deep_convert_cost",
+            "deep_convert_rate",
+            "stat_cost",
+            "show_cnt",
+            "cpm_platform",
+            "click_cnt",
+            "ctr",
+            "cpc_platform"
+        ],
+        "cascade_metrics": [
+            "advertiser_followed",
+            "advertiser_name",
+            "advertiser_id",
+            "advertiser_status",
+            "advertiser_budget",
+            "advertiser_remark",
+            "advertiser_balance",
+            "advertiser_valid_balance"
+        ],
+        "filter": {
+            "group": {
+
+            },
+            "advertiser": {
+
+            },
+            "campaign": {
+
+            },
+            "ad": {
+
+            },
+            "project": {
+
+            },
+            "promotion": {
+
+            },
+            "search": {
+                "keyword": "",
+                "searchType": 0,
+                "queryType": "phrase"
+            },
+            "pricingCategory": [
+                2
+            ]
+        },
+        "account_type": 0,
+        "platform_version": "2.0",
+        "start_time": start_time,
+        "end_time": end_time
+    }
+    response = lazyrequests.lazy_requests(
+        method='POST',
+        url=url,
+        headers=headers,
+        json=data,
+        timeout=timeout,
         return_json=True
     )
     return response
```

### Comparing `oceanengine-0.1.0/oceanengine/cc.py` & `oceanengine-0.1.1/oceanengine/cc.py`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine/e.py` & `oceanengine-0.1.1/oceanengine/e.py`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine/m_toutiao.py` & `oceanengine-0.1.1/oceanengine/m_toutiao.py`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine/open.py` & `oceanengine-0.1.1/oceanengine/open.py`

 * *Files identical despite different names*

### Comparing `oceanengine-0.1.0/oceanengine.egg-info/PKG-INFO` & `oceanengine-0.1.1/oceanengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanengine
-Version: 0.1.0
+Version: 0.1.1
 Summary: make it easy to use oceanengine
 Home-page: https://gitee.com/ZeroSeeker/oceanengine
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanengine-0.1.0/setup.py` & `oceanengine-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oceanengine",
-    version="0.1.0",
+    version="0.1.1",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use oceanengine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/oceanengine",
     packages=setuptools.find_packages(),
```


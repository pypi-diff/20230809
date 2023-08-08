# Comparing `tmp/pkscreener-0.4.20230805.17.tar.gz` & `tmp/pkscreener-0.4.20230808.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.4.20230805.17.tar", last modified: Sat Aug  5 07:40:29 2023, max compression
+gzip compressed data, was "pkscreener-0.4.20230808.18.tar", last modified: Tue Aug  8 22:06:32 2023, max compression
```

## Comparing `pkscreener-0.4.20230805.17.tar` & `pkscreener-0.4.20230808.18.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 07:40:29.536005 pkscreener-0.4.20230805.17/
--rw-rw-rw-   0        0        0     1086 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/LICENSE
--rw-rw-rw-   0        0        0     1091 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/LICENSE-Screenipy
--rw-rw-rw-   0        0        0    69449 2023-08-05 07:40:29.536005 pkscreener-0.4.20230805.17/PKG-INFO
--rw-rw-rw-   0        0        0    68347 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 07:40:29.520380 pkscreener-0.4.20230805.17/pkscreener/
--rw-rw-rw-   0        0        0     8992 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/Telegram.py
--rw-rw-rw-   0        0        0      404 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:40:29.536005 pkscreener-0.4.20230805.17/pkscreener/classes/
--rw-rw-rw-   0        0        0     1014 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Archiver.py
--rw-rw-rw-   0        0        0     3470 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    10065 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0      473 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0      391 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/ColorText.py
--rw-rw-rw-   0        0        0    11723 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9348 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    14101 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     6368 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23216 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/ParallelProcessing.py
--rw-rw-rw-   0        0        0    11684 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0     4796 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/PortfolioTracker.py
--rw-rw-rw-   0        0        0    49373 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Screener.py
--rw-rw-rw-   0        0        0      947 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0      649 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/UserChoice.py
--rw-rw-rw-   0        0        0    30737 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0       26 2023-08-05 07:40:22.000000 pkscreener-0.4.20230805.17/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0    11228 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/log.py
--rw-rw-rw-   0        0        0     4038 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0    45776 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/globals.py
--rw-rw-rw-   0        0        0    27552 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0     7755 2023-08-05 07:36:45.000000 pkscreener-0.4.20230805.17/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:40:29.520380 pkscreener-0.4.20230805.17/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    69449 2023-08-05 07:40:29.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-08-05 07:40:29.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 07:40:29.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-08-05 07:40:29.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-05 07:40:24.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      585 2023-08-05 07:40:29.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-05 07:40:29.000000 pkscreener-0.4.20230805.17/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-05 07:40:29.536005 pkscreener-0.4.20230805.17/setup.cfg
--rw-rw-rw-   0        0        0     2583 2023-08-05 07:36:46.000000 pkscreener-0.4.20230805.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:06:32.337116 pkscreener-0.4.20230808.18/
+-rw-rw-rw-   0        0        0     1086 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/LICENSE
+-rw-rw-rw-   0        0        0     1091 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/LICENSE-Screenipy
+-rw-rw-rw-   0        0        0    21931 2023-08-08 22:06:32.337116 pkscreener-0.4.20230808.18/PKG-INFO
+-rw-rw-rw-   0        0        0    21030 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 22:06:32.321561 pkscreener-0.4.20230808.18/pkscreener/
+-rw-rw-rw-   0        0        0     9061 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/Telegram.py
+-rw-rw-rw-   0        0        0      404 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:06:32.337116 pkscreener-0.4.20230808.18/pkscreener/classes/
+-rw-rw-rw-   0        0        0     1014 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Archiver.py
+-rw-rw-rw-   0        0        0     3470 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    10065 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0      473 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0      391 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/ColorText.py
+-rw-rw-rw-   0        0        0    11723 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9348 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    14101 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     6368 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23216 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/ParallelProcessing.py
+-rw-rw-rw-   0        0        0    11684 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0     4796 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/PortfolioTracker.py
+-rw-rw-rw-   0        0        0    49372 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Screener.py
+-rw-rw-rw-   0        0        0      947 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0      649 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/UserChoice.py
+-rw-rw-rw-   0        0        0    31133 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0       26 2023-08-08 22:06:26.000000 pkscreener-0.4.20230808.18/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0    11228 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/log.py
+-rw-rw-rw-   0        0        0     4038 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0    45807 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/globals.py
+-rw-rw-rw-   0        0        0    28110 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0     7786 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:06:32.321561 pkscreener-0.4.20230808.18/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    21931 2023-08-08 22:06:32.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-08-08 22:06:32.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 22:06:32.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-08-08 22:06:32.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-08 22:06:27.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      585 2023-08-08 22:06:32.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 22:06:32.000000 pkscreener-0.4.20230808.18/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-08 22:06:32.337116 pkscreener-0.4.20230808.18/setup.cfg
+-rw-rw-rw-   0        0        0     2583 2023-08-08 22:02:51.000000 pkscreener-0.4.20230808.18/setup.py
```

### Comparing `pkscreener-0.4.20230805.17/LICENSE` & `pkscreener-0.4.20230808.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/LICENSE-Screenipy` & `pkscreener-0.4.20230808.18/LICENSE-Screenipy`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/Telegram.py` & `pkscreener-0.4.20230808.18/pkscreener/Telegram.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 # if TOKEN == "00000000xxxxxxx":
 #     raise ValueError("There is no value for the telegram TOKEN, telegram is required to telegram one, see tutorial: https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token")
 def is_token_telegram_configured():
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     initTelegram()
     if TOKEN == "00000000xxxxxxx":
-        print("There is not value for the telegram TOKEN, telegram is required to telegram one, see tutorial: https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token")
+        print("[+] There is no value for the telegram TOKEN. It is required to telegram someone.\n[+] see tutorial: https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token")
         return False
     return  True
 
 def send_exception(ex, extra_mes = ""):
     message_aler = extra_mes + "   ** Exception **" + str(ex)
     if not is_token_telegram_configured():
         return
@@ -81,14 +81,15 @@
 
 
 def send_message(message, parse_type = ParseMode.HTML, list_png = None,userID=None):
     initTelegram()
     # botsUrl = f"https://api.telegram.org/bot{TOKEN}"  # + "/sendMessage?chat_id={}&text={}".format(chat_idLUISL, message_aler, parse_mode=ParseMode.HTML)
     # url = botsUrl + "/sendMessage?chat_id={}&text={}&parse_mode={parse_mode}".format(chat_idLUISL, message_aler,parse_mode=ParseMode.MARKDOWN_V2)
     if not is_token_telegram_configured():
+        print('No ')
         return
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     if userID is not None:
         LIST_PEOPLE_IDS_CHAT = [userID]
     if list_png is None or any(elem is None for elem in list_png):
         resp = None
         for people_id in LIST_PEOPLE_IDS_CHAT:
@@ -110,14 +111,15 @@
     #     # print(telegram_msg)
     #     # print(telegram_msg.content)
 
 def send_photo(photoFilePath, message = "", message_id = None,userID=None):
     initTelegram()
     if not is_token_telegram_configured():
         return
+    print(f'Sending message:{message}')
     method = "/sendPhoto"
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     photo = open(photoFilePath, "rb")
     if message_id is not None:
         params = {'chat_id': (userID if userID is not None else Channel_Id), 'caption' : message,'parse_mode':ParseMode.HTML, 'reply_to_message_id':message_id}
     else:
         params = {'chat_id': (userID if userID is not None else Channel_Id), 'caption': message, 'parse_mode': ParseMode.HTML}
```

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/Archiver.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/Backtest.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/ConfigManager.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/Fetcher.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/MenuOptions.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/ParallelProcessing.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/ParallelProcessing.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/Pktalib.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/PortfolioTracker.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/PortfolioTracker.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/Screener.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/Screener.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,15 +789,15 @@
                     endDate = tops.iloc[i]['Date']
                     startDate = tops.iloc[i+1]['Date']
                     lowPoints.append(data[(data.Date >= startDate) & (data.Date <= endDate)].describe()['Low']['min'])
                 lowPointsOrg = lowPoints
                 lowPoints.sort(reverse=True)
                 lowPointsSorted = lowPoints
                 ltp = data.head(1)['Close'][0]
-                if lowPointsOrg == lowPointsSorted and  ltp < highestTop and ltp > lowPoints[0]:
+                if lowPointsOrg == lowPointsSorted and ltp < highestTop and ltp > lowPoints[0]:
                     screenDict['Pattern'] = colorText.BOLD + colorText.GREEN + f'VCP (BO: {highestTop})' + colorText.END
                     saveDict['Pattern'] = f'VCP (BO: {highestTop})'
                     return True
         except Exception as e:
             self.default_logger.debug(e, exc_info=True)
         return False
```

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/SuppressOutput.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/UserChoice.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/UserChoice.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/Utility.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,22 @@
                   '[+] Failed to load recently screened result table from disk! Skipping..' + colorText.END)
 
     def formatRatio(ratio, volumeRatio):
         if(ratio >= volumeRatio and ratio != np.nan and (not math.isinf(ratio)) and (ratio != 20)):
             return colorText.BOLD + colorText.GREEN + str(ratio) + "x" + colorText.END
         return colorText.BOLD + colorText.FAIL + str(ratio) + "x" + colorText.END
     
+    def removeAllColorStyles(styledText):
+        styles = [colorText.HEAD, colorText.END, colorText.BOLD, colorText.UNDR,
+                  colorText.BLUE, colorText.GREEN, colorText.WARN, colorText.FAIL]
+        cleanedUpStyledValue = styledText
+        for style in styles:
+            cleanedUpStyledValue = cleanedUpStyledValue.replace(style,'')
+        return cleanedUpStyledValue
+
     def getCellColor(cellStyledValue=''):
         otherStyles = [colorText.HEAD, colorText.END, colorText.BOLD, colorText.UNDR]
         mainStyles = [colorText.BLUE, colorText.GREEN, colorText.WARN, colorText.FAIL]
         colorsDict = {colorText.BLUE:'blue', colorText.GREEN:'green',colorText.WARN:'yellow',colorText.FAIL:'red'}
         cleanedUpStyledValue = cellStyledValue
         cellFillColor = 'white'
         for style in otherStyles:
```

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/log.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/log.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/classes/multiprocessing_logging.py` & `pkscreener-0.4.20230808.18/pkscreener/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener/globals.py` & `pkscreener-0.4.20230808.18/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,31 +210,27 @@
             configManager.deleteFileWithPattern()
     return 'X', 12, 2, {'0':'X','1':'12','2':'2'}
     
 def handleSecondaryMenuChoices(menuOption, testing=False,defaultAnswer=None,user=None):
     if menuOption == 'H':
         helpData = Utility.tools.showDevInfo(defaultAnswer=defaultAnswer)
         if user is not None:
-            sendMessageToTelegramChannel(messaage=helpData.replace('\n','|'),user=user)
+            sendMessageToTelegramChannel(message=Utility.tools.removeAllColorStyles(helpData),user=user)
             return
-        else:
-            print('Not sending DevInfo to telegram as User is empty or none.')
     elif menuOption == 'U':
         OTAUpdater.checkForUpdate(getProxyServer(), VERSION, skipDownload=testing)
     elif menuOption == 'T':
         toggleUserConfig()
     elif menuOption == 'E':
         configManager.setConfig(ConfigManager.parser)
     elif menuOption == 'Y':
         configData = configManager.showConfigFile(defaultAnswer=defaultAnswer)
         if user is not None:
-            sendMessageToTelegramChannel(messaage=configData.replace('\n','|'),user=user)
+            sendMessageToTelegramChannel(message=Utility.tools.removeAllColorStyles(configData),user=user)
             return
-        else:
-            print('Not sending Config to telegram as User is empty or none.')
     # main()
     return
 
 def getTopLevelMenuChoices(startupoptions, testBuild, downloadOnly):
     global selectedChoice
     executeOption = None
     menuOption = None
@@ -257,15 +253,15 @@
     menuOption = menuOption
     tickerOption = tickerOption
     try:
         if menuOption is None:
             selectedMenu = initExecution(menuOption=menuOption)
             menuOption = selectedMenu.menuKey
         if menuOption in ['H','U','T','E','Y']:
-            return handleSecondaryMenuChoices(menuOption, testBuild,defaultAnswer=defaultAnswer,user=user)
+            handleSecondaryMenuChoices(menuOption, testBuild,defaultAnswer=defaultAnswer,user=user)
         elif menuOption == 'X':
             tickerOption, executeOption = initPostLevel0Execution(menuOption=menuOption,tickerOption=tickerOption, executeOption=executeOption)
             tickerOption, executeOption = initPostLevel1Execution(tickerOption=tickerOption, executeOption=executeOption)
     except KeyboardInterrupt:
         input(colorText.BOLD + colorText.FAIL +
             "[+] Press any key to Exit!" + colorText.END)
         sys.exit(0)
@@ -318,14 +314,16 @@
     selectedMenu = initExecution(menuOption=menuOption)
     menuOption = selectedMenu.menuKey
     if menuOption in ['X','T','E','Y','U','H']:
         # Print Level 2 menu options
         menuOption, tickerOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,downloadOnly,startupoptions, menuOption=menuOption, 
             tickerOption=tickerOption, executeOption=executeOption,defaultAnswer=defaultAnswer,user=user)
+        if menuOption in ['H','U','T','E','Y']:
+            return
     elif menuOption == 'B':
         # Backtests
         tickerOption, executeOption, backtestPeriod = takeBacktestInputs(menuOption,tickerOption, executeOption)
     else:
         print('Work in progress! Try selecting a different option.')
         sleep(3)
         main(testing=testing, testBuild=testBuild, downloadOnly=downloadOnly,
@@ -341,14 +339,16 @@
     if tickerOption == 0:
         if len(options) >= 4:
             listStockCodes = str(options[3]).split(',')
     if executeOption == 'Z':
         input(colorText.BOLD + colorText.FAIL +
               "[+] Press any key to Exit!" + colorText.END)
         sys.exit(0)
+    if executeOption is None:
+        executeOption = 0
     executeOption = int(executeOption)
     volumeRatio = configManager.volumeRatio
     if executeOption == 4:
         daysForLowestVolume = handleScannerExecuteOption4(executeOption, options)
     if executeOption == 5:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 5:
@@ -698,16 +698,16 @@
 def takeBacktestInputs(menuOption=None,tickerOption=None,executeOption=None,backtestPeriod=0):
     print(colorText.BOLD + colorText.GREEN +
                                       "[+] For backtesting, you can choose from (1,2,3,4,5,10,15,22,30) periods.")
     backtestPeriod = 0
     try:
         backtestPeriod = int(input(colorText.BOLD + colorText.FAIL +
                                     "[+] Enter backtesting period (Default is 30 [days]): "))
-    except:
-        pass
+    except Exception as e:
+         default_logger().debug(e, exc_info=True)
     if backtestPeriod == 0:
         backtestPeriod = 30
     tickerOption, executeOption = initPostLevel0Execution(menuOption=menuOption,
                                                             tickerOption=tickerOption,
                                                             executeOption=executeOption,
                                                             skip=['N', 'E'])
     tickerOption, executeOption = initPostLevel1Execution(tickerOption=tickerOption,
@@ -767,15 +767,16 @@
     # Exit all processes. Without this, it threw error in next screening session
     for worker in consumers:
         try:
             worker.terminate()
         except OSError as e:
             default_logger().debug(e, exc_info=True)
             if e.winerror == 5:
-                pass
+                 default_logger().debug(e, exc_info=True)
+                 continue
 
     # Flush the queue so depending processes will end
     from queue import Empty
     while True:
         try:
             _ = tasks_queue.get(False)
         except Exception as e:
@@ -811,16 +812,16 @@
             columns={
                 'Trend': f'Trend({configManager.daysToLookback}Prds)',
                 'Breakout': f'Breakout ({configManager.daysToLookback}Prds)',
                 'Consol.': f'Consol.({configManager.daysToLookback}Prds)',
             },
             inplace=True
         )
-    except:
-        pass
+    except Exception as e:
+         default_logger().debug(e, exc_info=True)
     return screenResults, saveResults
 
 def printNotifySaveScreenedResults(screenResults,saveResults,selectedChoice,menuChoiceHierarchy,testing,user=None):
     Utility.tools.clearScreen()
     print(colorText.BOLD + colorText.FAIL + f'[+] You chose: {menuChoiceHierarchy}\n' + colorText.END)
     tabulated_results = tabulate(screenResults, headers='keys', tablefmt='grid')
     print(tabulated_results)
@@ -835,15 +836,14 @@
                 if is_token_telegram_configured():
                     Utility.tools.tableToImage(markdown_results,tabulated_results,pngName,menuChoiceHierarchy)
                     sendMessageToTelegramChannel(message=None, photo_filePath=pngName, caption=caption, user=user)
                     try:
                         os.remove(pngName)
                     except Exception as e:
                         default_logger().debug(e, exc_info=True)
-                        pass
             print(colorText.BOLD + colorText.GREEN +
                     f"[+] Found {len(screenResults)} Stocks." + colorText.END)
             Utility.tools.setLastScreenedResults(screenResults)
     elif user is not None:
         sendMessageToTelegramChannel(message=f'No scan results found for {menuChoiceHierarchy}', user=user)
 
 def saveDownloadedData(downloadOnly, testing, stockDict, configManager, loadCount):
@@ -864,15 +864,14 @@
         print(colorText.BOLD + colorText.WARN +
             "[+] Note: Trend calculation is based on number of days recent to screen as per your configuration." + colorText.END)
         try:
             if filename is not None:
                 os.remove(filename)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
-            pass
     print(colorText.BOLD + colorText.GREEN +
         "[+] Screening Completed! Press Enter to Continue.." + colorText.END)
     if defaultAnswer is None:
         input('')
 
 def sendTestStatus(screenResults, label,user=None):
     msg = '<b>SUCCESS</b>' if len(screenResults) >= 1 else '<b>FAIL</b>'
@@ -887,31 +886,28 @@
 
 def sendMessageToTelegramChannel(message=None,photo_filePath=None,document_filePath=None, caption=None, user=None):
     if message is not None:
         try:
             send_message(message,userID=user)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
-            pass
     if photo_filePath is not None:
         try:
             send_document(photo_filePath, caption,userID=user)
             # Breather for the telegram API to be able to send the heavy photo
             sleep(2)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
-            pass
     if document_filePath is not None:
         try:
             send_document(document_filePath, caption,userID=user)
             # Breather for the telegram API to be able to send the document
             sleep(1)
         except Exception as e:
             default_logger().debug(e, exc_info=True)
-            pass
 
 def getProxyServer():
     # Get system wide proxy for networking
     try:
         proxyServer = urllib.request.getproxies()['http']
     except KeyError as e:
         default_logger().debug(e, exc_info=True)
```

### Comparing `pkscreener-0.4.20230805.17/pkscreener/pkscreenerbot.py` & `pkscreener-0.4.20230808.18/pkscreener/pkscreenerbot.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,21 +86,18 @@
         if mnu.menuKey in ['X','B','Z']:
             inlineMenus.append(InlineKeyboardButton(mnu.keyTextLabel().split('(')[0], callback_data='C'+str(mnu.menuKey)))
     keyboard = [
         inlineMenus
     ]
     reply_markup = InlineKeyboardMarkup(keyboard)
     # Send message with text and appended InlineKeyboard
-    await update.message.reply_text(f"Welcome {user.first_name},{(user.username)}! Please choose a menu option by selecting a button from below.\n\nPlease note that this bot restarts every hour starting at 5:30am IST until 10:30pm IST to keep it running on free servers. If it does not respond, please try again in 2-3 minutes to avoid the restart duration!", reply_markup=reply_markup)
-    try:
-        await context.bot.send_message(
-                chat_id=int(f'-{Channel_Id}'), text=f'Name: {user.first_name}, Username:@{user.username} with ID: {str(user.id)} started using the bot!', parse_mode=ParseMode.HTML
-            )
-    except:
-        pass
+    await update.message.reply_text(f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n   /X ", reply_markup=reply_markup)
+    await context.bot.send_message(
+            chat_id=int(f'-{Channel_Id}'), text=f'Name: {user.first_name}, Username:@{user.username} with ID: {str(user.id)} started using the bot!', parse_mode=ParseMode.HTML
+        )
     # Tell ConversationHandler that we're in state `FIRST` now
     return START_ROUTES
 
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace('CX','X').replace('CB','B')
@@ -188,31 +185,31 @@
         options = ':'.join(selection)
         await launchScreener(options=options, user=query.from_user,context=context, optionChoices=optionChoices, update=update)
     try:
         if optionChoices != '':
             await context.bot.send_message(
                 chat_id=int(f'-{Channel_Id}'), text=f'Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> submitted scan request <b>{optionChoices}</b> to the bot!', parse_mode=ParseMode.HTML
             )
-    except Exception as e:
+    except Exception:
         await start(update,context)
     await sendUpdatedMenu(menuText=menuText, update=update, context=context, reply_markup=reply_markup)
     return START_ROUTES
 
 async def sendUpdatedMenu(menuText, update: Update, context, reply_markup):
     try:
         await update.callback_query.edit_message_text(
             text=menuText.replace('     ','').replace('    ','').replace('\t',''), reply_markup=reply_markup
         )
-    except:
+    except Exception:
         await start(update,context)
 
 async def launchScreener(options, user, context,optionChoices, update):
     try:
         Popen(['pkscreener','-a','Y','-e','-p','-o', str(options.upper()), '-u', str(user.id)])
-    except:
+    except Exception:
         await start(update,context)
 
 async def BBacktests(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     await query.answer()
     keyboard = [
@@ -277,21 +274,21 @@
     )
 
     try:
         # Finally, send the message
         await context.bot.send_message(
             chat_id=int(f'-{Channel_Id}'), text=message, parse_mode=ParseMode.HTML
         )
-    except:
+    except Exception:
         try:
             await context.bot.send_message(
                 chat_id=int(f'-{Channel_Id}'), text=tb_string, parse_mode=ParseMode.HTML
             )
-        except:
-            pass
+        except Exception:
+            print(tb_string)
 
 async def command_handler(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if update.message is not None and abs(update.message.from_user.id) in [Channel_Id, GROUP_CHAT_ID]:
         # We want to avoid sending any help message back to channel or group.
         return START_ROUTES
     msg = update.effective_message
     m = re.match('\s*/([0-9a-zA-Z_-]+)\s*(.*)', msg.text)
@@ -313,14 +310,15 @@
     if cmd == 'start':
         await start(update=update, context=context)
         return START_ROUTES
     if cmd == 'help':
         await help_command(update=update, context=context)
         return START_ROUTES
     if cmd == 'x':
+        await shareUpdateWithChannel(update=update,context=context)
         m0.renderForMenu(selectedMenu=None, skip=['S','T','E','U','Z'], renderStyle=MenuRenderStyle.STANDALONE)
         selectedMenu = m0.find(cmd.upper())
         cmdText = ''
         cmds = m1.renderForMenu(selectedMenu=selectedMenu, skip=['W','E','M','Z'],asList=True, renderStyle=MenuRenderStyle.STANDALONE)
         for cmd in cmds:
             cmdText = f'{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}'
         cmdText = f'{cmdText}\n\nFor option 0 <Screen stocks by the stock name>, please type in the command in the following format\n/X_0 SBIN\n or \n/X_0_0 SBIN\nand hit send where SBIN is the NSE stock code.For multiple stocks, you can type in \n/X_0 SBIN,ICICIBANK,OtherStocks\nYou can put in any number of stocks separated by space or comma(,).'
@@ -328,14 +326,15 @@
         await update.message.reply_text(f"Choose an option:\n{cmdText}")
         return START_ROUTES
 
     if update.message is None:
         await help_command(update=update,context=context)
         return START_ROUTES
     if 'x_0' in cmd or 'x_0_0' in cmd:
+        await shareUpdateWithChannel(update=update,context=context)
         shouldScan = False
         if len(args) > 0:
             shouldScan = True
             selection = ['X','0','0',f"{','.join(args)}".replace(' ','')]
         if shouldScan:
             options = ':'.join(selection)
             await launchScreener(options=options, user=update.message.from_user,context=context, optionChoices=cmd.upper(), update=update)
@@ -344,14 +343,15 @@
         else:
             cmdText = f'For option 0 <Screen stocks by the stock name>, please type in the command in the following format\n/X_0 SBIN or /X_0_0 SBIN and hit send where SBIN is the NSE stock code.For multiple stocks, you can type in /X_0 SBIN,ICICIBANK,OtherStocks . You can put in any number of stocks separated by space or comma(,).'
             """Send a message when the command /help is issued."""
             await update.message.reply_text(f"Choose an option:\n{cmdText}")
             return START_ROUTES
 
     if 'x_' in cmd:
+        await shareUpdateWithChannel(update=update,context=context)
         selection = cmd.split('_')
         if len(selection) == 2:
             m0.renderForMenu(selectedMenu=None, skip=['S','T','E','U','Z'], renderStyle=MenuRenderStyle.STANDALONE)
             selectedMenu = m0.find(selection[0].upper())
             m1.renderForMenu(selectedMenu=selectedMenu, skip=['W','E','M','Z'],asList=True, renderStyle=MenuRenderStyle.STANDALONE)
             selectedMenu = m1.find(selection[1].upper())
             if selectedMenu.menuKey == 'N': # Nifty prediction
@@ -397,47 +397,53 @@
                     selection.extend(['',''])
         if len(selection) >= 4:
             options = ':'.join(selection)
             await launchScreener(options=options, user=update.message.from_user,context=context, optionChoices=cmd.upper(), update=update)
             await sendRequestSubmitted(cmd.upper(),update=update,context=context)
             return START_ROUTES
     if cmd == 'y' or cmd == 'h':
+        await shareUpdateWithChannel(update=update,context=context)
         await launchScreener(options=f'{cmd.upper()}:', user=update.message.from_user,context=context, optionChoices=cmd.upper(), update=update)
         await sendRequestSubmitted(cmd.upper(),update=update,context=context)
         return START_ROUTES
     await update.message.reply_text(f"{cmd.upper()} : Not implemented yet!")
     await help_command(update=update,context=context)
     
 async def sendRequestSubmitted(optionChoices,update,context):
     menuText = f'You chose {optionChoices}. You will receive the results soon! \n\nSince it is running on a free server, it might take from a few seconds up to ~12 minutes depending upon how many stocks need to be scanned (1 to 2000+ in Nifty). You will get notified here when the results arrive!'
     await update.message.reply_text(menuText)
     await help_command(update=update, context=context)
-    try:
-        query = update.message
-        message =f'Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> submitted scan request <b>{optionChoices}</b> to the bot!'
-        await context.bot.send_message(
-               chat_id=int(f'-{Channel_Id}'), text=message, parse_mode=ParseMode.HTML
-            )
-    except:
-        pass
+    await shareUpdateWithChannel(update=update,context=context,optionChoices=optionChoices)
+
+async def shareUpdateWithChannel(update,context,optionChoices=''):
+    query = update.message
+    message =f'Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using ({optionChoices}) the bot!'
+    await context.bot.send_message(
+            chat_id=int(f'-{Channel_Id}'), text=message, parse_mode=ParseMode.HTML
+        )
     
 async def help_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if update.callback_query is not None and abs(update.callback_query.from_user.id) in [Channel_Id, GROUP_CHAT_ID]:
         # We want to avoid sending any help message back to channel or group.
         return
     if update.message is not None and abs(update.message.from_user.id) in [Channel_Id, GROUP_CHAT_ID]:
         # We want to avoid sending any help message back to channel or group.
         return
     cmds = m0.renderForMenu(selectedMenu=None, skip=['S','T','E','U','Z','S','B'],asList=True, renderStyle=MenuRenderStyle.STANDALONE)
     cmdText = ''
     for cmd in cmds:
         cmdText = f'{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}'
     """Send a message when the command /help is issued."""
     await update.message.reply_text(f"You can begin by typing in /start and hit send!\n\nOR\n\nChoose an option:\n{cmdText}") #  \n\nThis bot restarts every hour starting at 5:30am IST until 10:30pm IST to keep it running on free servers. If it does not respond, please try again in a minutes to avoid the restart duration!
-
+    query = update.message
+    message =f'Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using the bot!'
+    await context.bot.send_message(
+            chat_id=int(f'-{Channel_Id}'), text=message, parse_mode=ParseMode.HTML
+        )
+    
 def addCommandsForMenuItems(application):
     cmds0 = m0.renderForMenu(selectedMenu=None, skip=['S','T','E','U','Z'], asList=True,renderStyle=MenuRenderStyle.STANDALONE)
     for mnu0 in cmds0:
         p0=mnu0.menuKey.upper()
         application.add_handler(CommandHandler(p0, command_handler))
         selectedMenu = m0.find(p0)
         cmds1=m1.renderForMenu(selectedMenu=selectedMenu, skip=['W','E','M','Z'],asList=True, renderStyle=MenuRenderStyle.STANDALONE)
```

### Comparing `pkscreener-0.4.20230805.17/pkscreener/pkscreenercli.py` & `pkscreener-0.4.20230808.18/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 def pkscreenercli():
     if sys.platform.startswith('darwin'):
         multiprocessing.set_start_method('fork')
     configManager.getConfig(ConfigManager.parser)
 
     if args.log or configManager.logsEnabled:
         setupLogger(shouldLog=True, trace=args.testbuild)
-        if not args.prodbuild:
+        if not args.prodbuild and args.answerdefault is None:
             input(f'Press any key to continue...')
     from pkscreener.globals import main
     import pkscreener.classes.Utility as Utility
     
     configManager.default_logger = default_logger()
     Utility.tools.clearScreen()
```

### Comparing `pkscreener-0.4.20230805.17/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.4.20230808.18/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/pkscreener.egg-info/requires.txt` & `pkscreener-0.4.20230808.18/pkscreener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.17/setup.py` & `pkscreener-0.4.20230808.18/setup.py`

 * *Files identical despite different names*


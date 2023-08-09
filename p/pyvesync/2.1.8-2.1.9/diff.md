# Comparing `tmp/pyvesync-2.1.8.tar.gz` & `tmp/pyvesync-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvesync-2.1.8.tar", last modified: Mon Jul 17 15:39:51 2023, max compression
+gzip compressed data, was "pyvesync-2.1.9.tar", last modified: Wed Aug  9 01:07:15 2023, max compression
```

## Comparing `pyvesync-2.1.8.tar` & `pyvesync-2.1.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.195637 pyvesync-2.1.8/
--rw-rw-rw-   0        0        0     1089 2023-07-14 00:55:01.000000 pyvesync-2.1.8/LICENSE
--rw-rw-rw-   0        0        0       44 2023-07-14 00:55:01.000000 pyvesync-2.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    34658 2023-07-17 15:39:51.195637 pyvesync-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    33905 2023-07-17 13:14:50.000000 pyvesync-2.1.8/README.md
--rw-rw-rw-   0        0        0       16 2023-07-14 00:55:01.000000 pyvesync-2.1.8/requirements.txt
--rw-rw-rw-   0        0        0      342 2023-07-17 15:39:51.196637 pyvesync-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1357 2023-07-17 13:55:24.000000 pyvesync-2.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.163636 pyvesync-2.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.175637 pyvesync-2.1.8/src/pyvesync/
--rw-rw-rw-   0        0        0      216 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/__init__.py
--rw-rw-rw-   0        0        0    20649 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/helpers.py
--rw-rw-rw-   0        0        0    13951 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesync.py
--rw-rw-rw-   0        0        0     5682 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncbasedevice.py
--rw-rw-rw-   0        0        0    45082 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncbulb.py
--rw-rw-rw-   0        0        0    70455 2023-07-17 13:55:29.000000 pyvesync-2.1.8/src/pyvesync/vesyncfan.py
--rw-rw-rw-   0        0        0    24285 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesynckitchen.py
--rw-rw-rw-   0        0        0    25884 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncoutlet.py
--rw-rw-rw-   0        0        0    13023 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncswitch.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.195637 pyvesync-2.1.8/src/pyvesync.egg-info/
--rw-rw-rw-   0        0        0    34658 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 03:41:33.000000 pyvesync-2.1.8/src/pyvesync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 01:07:15.115244 pyvesync-2.1.9/
+-rw-rw-rw-   0        0        0     1089 2023-07-14 00:55:01.000000 pyvesync-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-07-14 00:55:01.000000 pyvesync-2.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    35684 2023-08-09 01:07:15.115244 pyvesync-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    34931 2023-07-31 02:49:48.000000 pyvesync-2.1.9/README.md
+-rw-rw-rw-   0        0        0       16 2023-07-14 00:55:01.000000 pyvesync-2.1.9/requirements.txt
+-rw-rw-rw-   0        0        0      342 2023-08-09 01:07:15.117250 pyvesync-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1318 2023-08-09 01:03:04.000000 pyvesync-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:07:15.078243 pyvesync-2.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-09 01:07:15.093244 pyvesync-2.1.9/src/pyvesync/
+-rw-rw-rw-   0        0        0      216 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/__init__.py
+-rw-rw-rw-   0        0        0    21171 2023-08-09 00:48:59.000000 pyvesync-2.1.9/src/pyvesync/helpers.py
+-rw-rw-rw-   0        0        0    13951 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/vesync.py
+-rw-rw-rw-   0        0        0     5682 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/vesyncbasedevice.py
+-rw-rw-rw-   0        0        0    45082 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/vesyncbulb.py
+-rw-rw-rw-   0        0        0    71010 2023-08-09 00:44:06.000000 pyvesync-2.1.9/src/pyvesync/vesyncfan.py
+-rw-rw-rw-   0        0        0    24285 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/vesynckitchen.py
+-rw-rw-rw-   0        0        0    25884 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/vesyncoutlet.py
+-rw-rw-rw-   0        0        0    13023 2023-07-14 00:55:01.000000 pyvesync-2.1.9/src/pyvesync/vesyncswitch.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:07:15.113242 pyvesync-2.1.9/src/pyvesync.egg-info/
+-rw-rw-rw-   0        0        0    35684 2023-08-09 01:07:15.000000 pyvesync-2.1.9/src/pyvesync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-08-09 01:07:15.000000 pyvesync-2.1.9/src/pyvesync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 01:07:15.000000 pyvesync-2.1.9/src/pyvesync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 03:41:33.000000 pyvesync-2.1.9/src/pyvesync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-08-09 01:07:15.000000 pyvesync-2.1.9/src/pyvesync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-09 01:07:15.000000 pyvesync-2.1.9/src/pyvesync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 01:07:15.114241 pyvesync-2.1.9/test/
+-rw-rw-rw-   0        0        0     2225 2023-08-09 00:27:38.000000 pyvesync-2.1.9/test/test.py
```

### Comparing `pyvesync-2.1.8/LICENSE` & `pyvesync-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/PKG-INFO` & `pyvesync-2.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvesync
-Version: 2.1.8
+Version: 2.1.9
 Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
 Home-page: https://github.com/webdjoe/pyvesync
 Author: Mark Perdue, Joe Trabulsy
 Author-email: webdjoe@gmail.com
 License: MIT
 Keywords: iot,vesync,levoit,etekcity,cosori,valceno
 Classifier: License :: OSI Approved :: MIT License
@@ -936,47 +936,87 @@
 import logging
 import json
 from pyvesync import VeSync
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
+USERNAME = "YOUR USERNAME"
+PASSWORD = "YOUR PASSWORD"
+
 def test_device():
-  # Instantiate VeSync class and login
-  manager = VeSync(user, password, debug=True)
-  if manager.login() == False
-    logger("Unable to login")
-    return
-
-  # Test specific device
-  # If this were a humidifier and there is only one humidifier/purifier
-  # You can access it with the device index
-  fan = manager.fans[0]
-  # or loop through the fan devices and test for device with "My Device" name
-  # Use lower() to avoid capitalization issues
-  my_device_name = "My Device"
-  fan = None
-  for dev in manager.fans:
-    if dev.name.lower() == my_device_name.lower()
-      fan = dev
-  if fan == None:
-    logger.debug("Device not found")
-    logger.debug("Devices found - \n" + json.dumps(manager._dev_list))
-    return
-
-  # Test all device methods and functionality
-  # Be aware some devices lose internet connectivity if turned off
-  fan.turn_on()
-  fan.turn_off()
-  fan.sleep_mode()
+    # Instantiate VeSync class and login
+    manager = VeSync(USERNAME, PASSWORD, debug=True)
+    if manager.login() == False:
+        logger.debug("Unable to login")
+        return
+
+    # Pull and update devices
+    manager.update()
+
+    fan = None
+    logger.debug(str(manager.fans))
+
+    for dev in manager.fans:
+        # Print all device info
+        logger.debug(dev.device_name + "\n")
+        logger.debug(dev.display())
+
+        # Find correct device
+        if dev.device_name.lower() == DEVICE_NAME.lower():
+            fan = dev
+            break
+
+    if fan == None:
+        logger.debug("Device not found")
+        logger.debug("Devices found - \n %s", str(manager._dev_list))
+        return
+
+
+    logger.debug('--------------%s-----------------' % fan.device_name)
+    logger.debug(dev.display())
+    logger.debug(dev.displayJSON())
+    # Test all device methods and functionality
+    # Test Properties
+    logger.debug("Fan is on - %s", fan.is_on)
+    logger.debug("Modes - %s", fan.modes)
+    logger.debug("Fan Level - %s", fan.fan_level)
+    logger.debug("Fan Air Quality - %s", fan.air_quality)
+    logger.debug("Screen Status - %s", fan.screen_status)
+
+    fan.turn_on()
+    fan.turn_off()
+    fan.sleep_mode()
+    fan.auto_mode()
+    fan.manual_mode()
+    fan.change_fan_speed(3)
+    fan.change_fan_speed(2)
+    fan.child_lock_on()
+    fan.child_lock_off()
+    fan.turn_off_display()
+    fan.turn_on_display()
+
+    fan.set_light_detection_on()
+    logger.debug(fan.light_detection_state)
+    logger.debug(fan.light_detection)
+
+    # Only on Vital 200S
+    fan.pet_mode()
+
+    logger.debug("Set Fan Speed - %s", fan.set_fan_speed)
+    logger.debug("Current Fan Level - %s", fan.fan_level)
+    logger.debug("Current mode - %s", fan.mode)
+
+    # Display all device info
+    logger.debug(dev.display())
+    logger.debug(dev.displayJSON())
 
-# Make script runnable from command line
 if __name__ == "__main__":
-  logger.debug("Testing device")
-  test_device()
+    logger.debug("Testing device")
+    test_device()
 ...
 
 ```
 
 ## Device Requests
 
 SSL pinning makes capturing packets much harder. In order to be able to capture packets, SSL pinning needs to be disabled before running an SSL proxy. Use an Android emulator such as Android Studio, which is available for Windows and Linux for free. Download the APK from APKPure or a similiar site and use [Objection](https://github.com/sensepost/objection) or [Frida](https://frida.re/docs/gadget/). Followed by capturing the packets with Charles Proxy or another SSL proxy application.
```

### Comparing `pyvesync-2.1.8/README.md` & `pyvesync-2.1.9/src/pyvesync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pyvesync
+Version: 2.1.9
+Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
+Home-page: https://github.com/webdjoe/pyvesync
+Author: Mark Perdue, Joe Trabulsy
+Author-email: webdjoe@gmail.com
+License: MIT
+Keywords: iot,vesync,levoit,etekcity,cosori,valceno
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # pyvesync [![build status](https://img.shields.io/pypi/v/pyvesync.svg)](https://pypi.python.org/pypi/pyvesync) [![Build Status](https://dev.azure.com/webdjoe/pyvesync/_apis/build/status/webdjoe.pyvesync?branchName=master)](https://dev.azure.com/webdjoe/pyvesync/_build/latest?definitionId=4&branchName=master) [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) <!-- omit in toc -->
 
 pyvesync is a library to manage VeSync compatible [smart home devices](#supported-devices)
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Installation](#installation)
@@ -917,47 +936,87 @@
 import logging
 import json
 from pyvesync import VeSync
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
+USERNAME = "YOUR USERNAME"
+PASSWORD = "YOUR PASSWORD"
+
 def test_device():
-  # Instantiate VeSync class and login
-  manager = VeSync(user, password, debug=True)
-  if manager.login() == False
-    logger("Unable to login")
-    return
-
-  # Test specific device
-  # If this were a humidifier and there is only one humidifier/purifier
-  # You can access it with the device index
-  fan = manager.fans[0]
-  # or loop through the fan devices and test for device with "My Device" name
-  # Use lower() to avoid capitalization issues
-  my_device_name = "My Device"
-  fan = None
-  for dev in manager.fans:
-    if dev.name.lower() == my_device_name.lower()
-      fan = dev
-  if fan == None:
-    logger.debug("Device not found")
-    logger.debug("Devices found - \n" + json.dumps(manager._dev_list))
-    return
-
-  # Test all device methods and functionality
-  # Be aware some devices lose internet connectivity if turned off
-  fan.turn_on()
-  fan.turn_off()
-  fan.sleep_mode()
+    # Instantiate VeSync class and login
+    manager = VeSync(USERNAME, PASSWORD, debug=True)
+    if manager.login() == False:
+        logger.debug("Unable to login")
+        return
+
+    # Pull and update devices
+    manager.update()
+
+    fan = None
+    logger.debug(str(manager.fans))
+
+    for dev in manager.fans:
+        # Print all device info
+        logger.debug(dev.device_name + "\n")
+        logger.debug(dev.display())
+
+        # Find correct device
+        if dev.device_name.lower() == DEVICE_NAME.lower():
+            fan = dev
+            break
+
+    if fan == None:
+        logger.debug("Device not found")
+        logger.debug("Devices found - \n %s", str(manager._dev_list))
+        return
+
+
+    logger.debug('--------------%s-----------------' % fan.device_name)
+    logger.debug(dev.display())
+    logger.debug(dev.displayJSON())
+    # Test all device methods and functionality
+    # Test Properties
+    logger.debug("Fan is on - %s", fan.is_on)
+    logger.debug("Modes - %s", fan.modes)
+    logger.debug("Fan Level - %s", fan.fan_level)
+    logger.debug("Fan Air Quality - %s", fan.air_quality)
+    logger.debug("Screen Status - %s", fan.screen_status)
+
+    fan.turn_on()
+    fan.turn_off()
+    fan.sleep_mode()
+    fan.auto_mode()
+    fan.manual_mode()
+    fan.change_fan_speed(3)
+    fan.change_fan_speed(2)
+    fan.child_lock_on()
+    fan.child_lock_off()
+    fan.turn_off_display()
+    fan.turn_on_display()
+
+    fan.set_light_detection_on()
+    logger.debug(fan.light_detection_state)
+    logger.debug(fan.light_detection)
+
+    # Only on Vital 200S
+    fan.pet_mode()
+
+    logger.debug("Set Fan Speed - %s", fan.set_fan_speed)
+    logger.debug("Current Fan Level - %s", fan.fan_level)
+    logger.debug("Current mode - %s", fan.mode)
+
+    # Display all device info
+    logger.debug(dev.display())
+    logger.debug(dev.displayJSON())
 
-# Make script runnable from command line
 if __name__ == "__main__":
-  logger.debug("Testing device")
-  test_device()
+    logger.debug("Testing device")
+    test_device()
 ...
 
 ```
 
 ## Device Requests
 
 SSL pinning makes capturing packets much harder. In order to be able to capture packets, SSL pinning needs to be disabled before running an SSL proxy. Use an Android emulator such as Android Studio, which is available for Windows and Linux for free. Download the APK from APKPure or a similiar site and use [Objection](https://github.com/sensepost/objection) or [Frida](https://frida.re/docs/gadget/). Followed by capturing the packets with Charles Proxy or another SSL proxy application.
```

### Comparing `pyvesync-2.1.8/src/pyvesync/helpers.py` & `pyvesync-2.1.9/src/pyvesync/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,28 +191,41 @@
                                           '(?<=cid": "))',
                                           '[^"]+')
                                           ),
                                  '##_REDACTED_##', stringvalue)
         return stringvalue
 
     @staticmethod
+    def nested_code_check(response: dict) -> bool:
+        """Return true if all code values are 0."""
+        if isinstance(response, dict):
+            for key, value in response.items():
+                if key == 'code':
+                    if value != 0:
+                        return False
+                elif isinstance(value, dict):
+                    if not Helpers.nested_code_check(value):
+                        return False
+        return True
+
+    @staticmethod
     def call_api(api: str, method: str, json_object:  Optional[dict] = None,
                  headers: Optional[dict] = None) -> tuple:
         """Make API calls by passing endpoint, header and body."""
         response = None
         status_code = None
 
         try:
             logger.debug("=======call_api=============================")
             logger.debug("[%s] calling '%s' api", method, api)
             logger.debug("API call URL: \n  %s%s", API_BASE_URL, api)
             logger.debug("API call headers: \n  %s",
-                         Helpers.redactor(json.dumps(headers)))
+                         Helpers.redactor(json.dumps(headers, indent=2)))
             logger.debug("API call json: \n  %s",
-                         Helpers.redactor(json.dumps(json_object)))
+                         Helpers.redactor(json.dumps(json_object, indent=2)))
             if method.lower() == 'get':
                 r = requests.get(
                     API_BASE_URL + api, json=json_object, headers=headers,
                     timeout=API_TIMEOUT
                 )
             elif method.lower() == 'post':
                 r = requests.post(
@@ -230,15 +243,15 @@
             logger.debug(e)
         else:
             if r.status_code == 200:
                 status_code = 200
                 if r.content:
                     response = r.json()
                     logger.debug("API response: \n\n  %s \n ",
-                                 Helpers.redactor(json.dumps(response)))
+                                 Helpers.redactor(json.dumps(response, indent=2)))
             else:
                 logger.debug('Unable to fetch %s%s', API_BASE_URL, api)
         return response, status_code
 
     @staticmethod
     def code_check(r: dict) -> bool:
         """Test if code == 0 for successful API call."""
```

### Comparing `pyvesync-2.1.8/src/pyvesync/vesync.py` & `pyvesync-2.1.9/src/pyvesync/vesync.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/src/pyvesync/vesyncbasedevice.py` & `pyvesync-2.1.9/src/pyvesync/vesyncbasedevice.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/src/pyvesync/vesyncbulb.py` & `pyvesync-2.1.9/src/pyvesync/vesyncbulb.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/src/pyvesync/vesyncfan.py` & `pyvesync-2.1.9/src/pyvesync/vesyncfan.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,22 +95,22 @@
         'models': ['LV-PUR131S', 'LV-RH131S'],
         'features': ['air_quality']
     },
     'Vital100S': {
         'module': 'VeSyncVital',
         'models': ['LAP-V102S-AASR', 'LAP-V102S-WUS', 'LAP-V102S-WEU',
                    'LAP-V102S-AUSR', 'LAP-V102S-WJP'],
-        'modes': ['manual', 'auto', 'sleep', 'off'],
+        'modes': ['manual', 'auto', 'sleep', 'off', 'pet'],
         'features': ['air_quality'],
         'levels': list(range(1, 5))
     },
     'Vital200S': {
         'module': 'VeSyncVital',
         'models': ['LAP-V201S-AASR', 'LAP-V201S-WJP', 'LAP-V201S-WEU',
-                   'LAP-V102S-AUSR', 'LAP-V201S-WUS'],
+                   'LAP-V201S-WUS', 'LAP-V201-AUSR'],
         'modes': ['manual', 'auto', 'sleep', 'off', 'pet'],
         'features': ['air_quality'],
         'levels': list(range(1, 5))
     }
 }
 
 
@@ -764,36 +764,28 @@
 
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
-        if not isinstance(r, dict):
-            logger.debug('Error in purifier response')
+        if Helpers.nested_code_check(r) is False or not isinstance(r, dict):
+            logger.debug('Error getting purifier details')
+            self.connection_status = 'offline'
             return
-        if not isinstance(r.get('result'), dict):
-            logger.debug('Error in purifier response')
-            return
-        outer_result = r.get('result', {})
-        inner_result = None
 
-        if outer_result:
-            inner_result = r.get('result', {}).get('result')
-        if inner_result is not None and Helpers.code_check(r):
-            if outer_result.get('code') == 0:
-                self.build_purifier_dict(inner_result)
-            else:
-                logger.debug('error in inner result dict from purifier')
-            if inner_result.get('configuration', {}):
-                self.build_config_dict(inner_result.get('configuration', {}))
-            else:
-                logger.debug('No configuration found in purifier status')
+        inner_result = r.get('result', {}).get('result')
+
+        if inner_result is not None:
+            self.build_purifier_dict(inner_result)
         else:
-            logger.debug('Error in purifier response')
+            self.connection_status = 'offline'
+            logger.debug('error in inner result dict from purifier')
+        if inner_result.get('configuration', {}):
+            self.build_config_dict(inner_result.get('configuration', {}))
 
     def build_api_dict(self, method: str) -> Tuple[Dict, Dict]:
         """Return default body for Levoit Vital 100S/200S API."""
         header = Helpers.bypass_header()
         body = Helpers.bypass_body_v2(self.manager)
         body['cid'] = self.cid
         body['deviceId'] = self.cid
@@ -804,34 +796,31 @@
             'source': 'APP',
             'data': {}
         }
         return header, body
 
     def build_purifier_dict(self, dev_dict: dict) -> None:
         """Build Bypass purifier status dictionary."""
-        power_switch = dev_dict.get('power_switch', 0)
+        self.connection_status = 'online'
+        power_switch = bool(dev_dict.get('powerSwitch', 0))
         self.enabled = power_switch
-        self.device_status = 'on' if power_switch else 'off'
+        self.device_status = 'on' if power_switch is True else 'off'
         self.mode = dev_dict.get('workMode', 'manual')
 
         self.speed = dev_dict.get('fanSpeedLevel', 0)
 
         self.set_speed_level = dev_dict.get('manualSpeedLevel', 1)
 
         self.details['filter_life'] = dev_dict.get('filterLifePercent', 0)
-        self.details['display'] = dev_dict.get('display', False)
         self.details['child_lock'] = bool(dev_dict.get('childLockSwitch', 0))
-        self.details['night_light'] = dev_dict.get('night_light', 'off')
         self.details['display'] = bool(dev_dict.get('screenState', 0))
-        self.details['display_forever'] = dev_dict.get('display_forever', False)
         self.details['light_detection_switch'] = bool(
             dev_dict.get('lightDetectionSwitch', 0))
         self.details['environment_light_state'] = bool(
             dev_dict.get('environmentLightState', 0))
-        self.details['screen_state'] = bool(dev_dict.get('screenState', 0))
         self.details['screen_switch'] = bool(dev_dict.get('screenSwitch', 0))
 
         if self.air_quality_feature is True:
             self.details['air_quality_value'] = dev_dict.get(
                 'PM25', 0)
             self.details['air_quality'] = dev_dict.get('air_quality', 0)
         if dev_dict.get('timerRemain') is not None:
@@ -844,32 +833,29 @@
 
     def pet_mode(self) -> bool:
         """Set Pet Mode for Levoit Vital 200S."""
         return self.mode_toggle('pet')
 
     def set_light_detection(self, toggle: bool) -> bool:
         """Enable/Disable Light Detection Feature."""
-        if toggle is True:
-            toggle_id = 1
-        else:
-            toggle_id = 0
+        toggle_id = int(toggle)
         if self.details['light_detection_switch'] == toggle_id:
             logger.debug("Light Detection is already set to %s", toggle_id)
             return True
 
-        head, body = self.build_api_dict('setLightDetectionSwitch')
+        head, body = self.build_api_dict('setLightDetection')
         body['payload']['data']['lightDetectionSwitch'] = toggle_id
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
 
-        if r is not None and Helpers.code_check(r):
+        if r is not None and Helpers.nested_code_check(r):
             self.details['light_detection'] = toggle
             return True
         logger.debug("Error toggling purifier - %s",
                      self.device_name)
         return False
 
     def set_light_detection_on(self) -> bool:
@@ -899,26 +885,26 @@
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
 
-        if r is not None and Helpers.code_check(r):
+        if r is not None and Helpers.nested_code_check(r):
             if toggle:
                 self.device_status = 'on'
             else:
                 self.device_status = 'off'
             return True
         logger.debug("Error toggling purifier - %s",
                      self.device_name)
         return False
 
     def set_child_lock(self, mode: bool) -> bool:
-        """Levoit 100S set Child Lock."""
+        """Levoit 100S/200S set Child Lock."""
         if mode:
             toggle_id = 1
         else:
             toggle_id = 0
         head, body = self.build_api_dict('setChildLock')
         body['payload']['data'] = {
             'childLockSwitch': toggle_id
@@ -927,15 +913,15 @@
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
 
-        if r is not None and Helpers.code_check(r):
+        if r is not None and Helpers.nested_code_check(r):
             self.details['child_lock'] = mode
             return True
 
         logger.debug("Error toggling purifier child lock - %s", self.device_name)
         return False
 
     def set_display(self, mode: bool) -> bool:
@@ -952,15 +938,15 @@
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
 
-        if r is not None and Helpers.code_check(r):
+        if r is not None and Helpers.nested_code_check(r):
             self.details['screen_switch'] = mode
             return True
 
         logger.debug("Error toggling purifier display - %s", self.device_name)
         return False
 
     def set_timer(self, timer_duration: int, action: str = 'off',
@@ -1002,15 +988,15 @@
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
 
-        if r is not None and Helpers.code_check(r):
+        if r is not None and Helpers.nested_code_check(r):
             self.timer = Timer(timer_duration, action)
             return True
 
         logger.debug("Error setting timer for - %s", self.device_name)
         return False
 
     def clear_timer(self) -> bool:
@@ -1022,15 +1008,15 @@
         r, _ = Helpers.call_api(
             '/cloud/v2/deviceManaged/bypassV2',
             method='post',
             headers=head,
             json_object=body,
         )
 
-        if r is not None and Helpers.code_check(r):
+        if r is not None and Helpers.nested_code_check(r):
             self.timer = None
             return True
 
         logger.debug("Error setting timer for - %s", self.device_name)
         return False
 
     def set_auto_preference(self, preference: str = 'default',
@@ -1162,14 +1148,40 @@
 
         if Helpers.code_check(r):
             self.mode = mode
             return True
         logger.debug('Error setting purifier mode')
         return False
 
+    def displayJSON(self) -> str:
+        """Return air purifier status and properties in JSON output."""
+        sup = super().displayJSON()
+        sup_val = json.loads(sup)
+        sup_val.update(
+            {
+                'Mode': self.mode,
+                'Filter Life': str(self.details['filter_life']),
+                'Fan Level': str(self.speed),
+                'Display On': self.details['display'],
+                'Child Lock': self.details['child_lock'],
+                'Night Light': str(self.details['night_light']),
+                'Display Set On': self.details['screen_switch'],
+                'Light Detection Enabled': self.details['light_detection_switch'],
+                'Environment Light State': self.details['environment_light_state']
+            }
+        )
+        if self.air_quality_feature is True:
+            sup_val.update(
+                {'Air Quality Level': str(self.details.get('air_quality', ''))}
+            )
+            sup_val.update(
+                {'Air Quality Value': str(self.details.get('air_quality_value', ''))}
+            )
+        return json.dumps(sup_val, indent=4)
+
 
 class VeSyncAir131(VeSyncBaseDevice):
     """Levoit Air Purifier Class."""
 
     def __init__(self, details, manager):
         """Initilize air purifier class."""
         super().__init__(details, manager)
```

### Comparing `pyvesync-2.1.8/src/pyvesync/vesynckitchen.py` & `pyvesync-2.1.9/src/pyvesync/vesynckitchen.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/src/pyvesync/vesyncoutlet.py` & `pyvesync-2.1.9/src/pyvesync/vesyncoutlet.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/src/pyvesync/vesyncswitch.py` & `pyvesync-2.1.9/src/pyvesync/vesyncswitch.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.8/src/pyvesync.egg-info/PKG-INFO` & `pyvesync-2.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pyvesync
-Version: 2.1.8
-Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
-Home-page: https://github.com/webdjoe/pyvesync
-Author: Mark Perdue, Joe Trabulsy
-Author-email: webdjoe@gmail.com
-License: MIT
-Keywords: iot,vesync,levoit,etekcity,cosori,valceno
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # pyvesync [![build status](https://img.shields.io/pypi/v/pyvesync.svg)](https://pypi.python.org/pypi/pyvesync) [![Build Status](https://dev.azure.com/webdjoe/pyvesync/_apis/build/status/webdjoe.pyvesync?branchName=master)](https://dev.azure.com/webdjoe/pyvesync/_build/latest?definitionId=4&branchName=master) [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) <!-- omit in toc -->
 
 pyvesync is a library to manage VeSync compatible [smart home devices](#supported-devices)
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Installation](#installation)
@@ -936,47 +917,87 @@
 import logging
 import json
 from pyvesync import VeSync
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
+USERNAME = "YOUR USERNAME"
+PASSWORD = "YOUR PASSWORD"
+
 def test_device():
-  # Instantiate VeSync class and login
-  manager = VeSync(user, password, debug=True)
-  if manager.login() == False
-    logger("Unable to login")
-    return
-
-  # Test specific device
-  # If this were a humidifier and there is only one humidifier/purifier
-  # You can access it with the device index
-  fan = manager.fans[0]
-  # or loop through the fan devices and test for device with "My Device" name
-  # Use lower() to avoid capitalization issues
-  my_device_name = "My Device"
-  fan = None
-  for dev in manager.fans:
-    if dev.name.lower() == my_device_name.lower()
-      fan = dev
-  if fan == None:
-    logger.debug("Device not found")
-    logger.debug("Devices found - \n" + json.dumps(manager._dev_list))
-    return
-
-  # Test all device methods and functionality
-  # Be aware some devices lose internet connectivity if turned off
-  fan.turn_on()
-  fan.turn_off()
-  fan.sleep_mode()
+    # Instantiate VeSync class and login
+    manager = VeSync(USERNAME, PASSWORD, debug=True)
+    if manager.login() == False:
+        logger.debug("Unable to login")
+        return
+
+    # Pull and update devices
+    manager.update()
+
+    fan = None
+    logger.debug(str(manager.fans))
+
+    for dev in manager.fans:
+        # Print all device info
+        logger.debug(dev.device_name + "\n")
+        logger.debug(dev.display())
+
+        # Find correct device
+        if dev.device_name.lower() == DEVICE_NAME.lower():
+            fan = dev
+            break
+
+    if fan == None:
+        logger.debug("Device not found")
+        logger.debug("Devices found - \n %s", str(manager._dev_list))
+        return
+
+
+    logger.debug('--------------%s-----------------' % fan.device_name)
+    logger.debug(dev.display())
+    logger.debug(dev.displayJSON())
+    # Test all device methods and functionality
+    # Test Properties
+    logger.debug("Fan is on - %s", fan.is_on)
+    logger.debug("Modes - %s", fan.modes)
+    logger.debug("Fan Level - %s", fan.fan_level)
+    logger.debug("Fan Air Quality - %s", fan.air_quality)
+    logger.debug("Screen Status - %s", fan.screen_status)
+
+    fan.turn_on()
+    fan.turn_off()
+    fan.sleep_mode()
+    fan.auto_mode()
+    fan.manual_mode()
+    fan.change_fan_speed(3)
+    fan.change_fan_speed(2)
+    fan.child_lock_on()
+    fan.child_lock_off()
+    fan.turn_off_display()
+    fan.turn_on_display()
+
+    fan.set_light_detection_on()
+    logger.debug(fan.light_detection_state)
+    logger.debug(fan.light_detection)
+
+    # Only on Vital 200S
+    fan.pet_mode()
+
+    logger.debug("Set Fan Speed - %s", fan.set_fan_speed)
+    logger.debug("Current Fan Level - %s", fan.fan_level)
+    logger.debug("Current mode - %s", fan.mode)
+
+    # Display all device info
+    logger.debug(dev.display())
+    logger.debug(dev.displayJSON())
 
-# Make script runnable from command line
 if __name__ == "__main__":
-  logger.debug("Testing device")
-  test_device()
+    logger.debug("Testing device")
+    test_device()
 ...
 
 ```
 
 ## Device Requests
 
 SSL pinning makes capturing packets much harder. In order to be able to capture packets, SSL pinning needs to be disabled before running an SSL proxy. Use an Android emulator such as Android Studio, which is available for Windows and Linux for free. Download the APK from APKPure or a similiar site and use [Objection](https://github.com/sensepost/objection) or [Frida](https://frida.re/docs/gadget/). Followed by capturing the packets with Charles Proxy or another SSL proxy application.
```

### Comparing `pyvesync-2.1.8/src/pyvesync.egg-info/SOURCES.txt` & `pyvesync-2.1.9/src/pyvesync.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 src/pyvesync/vesyncoutlet.py
 src/pyvesync/vesyncswitch.py
 src/pyvesync.egg-info/PKG-INFO
 src/pyvesync.egg-info/SOURCES.txt
 src/pyvesync.egg-info/dependency_links.txt
 src/pyvesync.egg-info/not-zip-safe
 src/pyvesync.egg-info/requires.txt
-src/pyvesync.egg-info/top_level.txt
+src/pyvesync.egg-info/top_level.txt
+test/test.py
```


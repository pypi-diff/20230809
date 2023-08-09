# Comparing `tmp/unic-0.1.1.tar.gz` & `tmp/unic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.1.1.tar", max compression
+gzip compressed data, was "unic-0.2.0.tar", max compression
```

## Comparing `unic-0.1.1.tar` & `unic-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.1.1/LICENSE
--rw-r--r--   0        0        0      843 2023-08-06 14:15:38.996439 unic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-08-05 05:54:33.805710 unic-0.1.1/README.md
--rw-r--r--   0        0        0      127 2023-08-06 14:15:30.709679 unic-0.1.1/unic/__init__.py
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.1.1/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.1.1/unic/configs/unit/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.987478 unic-0.1.1/unic/timeobject/__init__.py
--rw-r--r--   0        0        0     2056 2023-08-02 13:34:57.987478 unic-0.1.1/unic/timeobject/timeobject.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.1.1/unic/unit/__init__.py
--rw-r--r--   0        0        0     1982 2023-08-05 06:11:01.782318 unic-0.1.1/unic/unit/timeunit.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.1.1/unic/unixtime/__init__.py
--rw-r--r--   0        0        0      889 2023-08-02 13:34:58.004259 unic-0.1.1/unic/unixtime/unixtime.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.1.1/unic/utils/__init__.py
--rw-r--r--   0        0        0      673 2023-08-02 13:34:58.004259 unic-0.1.1/unic/utils/check_parameter.py
--rw-r--r--   0        0        0      391 2023-08-02 13:34:58.004259 unic-0.1.1/unic/utils/config_parser.py
--rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 unic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.2.0/LICENSE
+-rw-r--r--   0        0        0      843 2023-08-09 04:03:50.419164 unic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1581 2023-08-09 04:01:36.533334 unic-0.2.0/README.md
+-rw-r--r--   0        0        0      167 2023-08-09 04:03:44.077983 unic-0.2.0/unic/__init__.py
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.2.0/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.2.0/unic/configs/unit/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.2.0/unic/time_unit/datetime/__init__.py
+-rw-r--r--   0        0        0     2059 2023-08-09 03:40:52.019505 unic-0.2.0/unic/time_unit/datetime/datetime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.2.0/unic/time_unit/time/__init__.py
+-rw-r--r--   0        0        0     1995 2023-08-09 03:58:03.078903 unic-0.2.0/unic/time_unit/time/time_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.2.0/unic/time_unit/unixtime/__init__.py
+-rw-r--r--   0        0        0      894 2023-08-09 03:52:21.013979 unic-0.2.0/unic/time_unit/unixtime/unixtime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.2.0/unic/utils/__init__.py
+-rw-r--r--   0        0        0      673 2023-08-02 13:34:58.004259 unic-0.2.0/unic/utils/check_parameter.py
+-rw-r--r--   0        0        0      391 2023-08-02 13:34:58.004259 unic-0.2.0/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 unic-0.2.0/PKG-INFO
```

### Comparing `unic-0.1.1/LICENSE` & `unic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.1.1/pyproject.toml` & `unic-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.1.1"
+version = "0.2.0"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'unixtime']
```

### Comparing `unic-0.1.1/README.md` & `unic-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 ![Python minimum version](https://img.shields.io/badge/Python-3.8%2B-brightgreen)
 [![pytest](https://github.com/subretu/unic/actions/workflows/pytest.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/pytest.yml)
 [![black](https://github.com/subretu/unic/actions/workflows/format.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/format.yml)
 
 # unic
-- unic is a Python package that can convert various units.
+unic is a Python package that can convert various units.
+
+## Conversion Targets
 - The current available conversion targets are as follows.
-  - Time Unit
+### Time Unit
+  - Time
     - minute / second / milisecond → hour
     - hour / second / milisecond → minute
     - hour / minute / milisecond → second
     - hour / minute / second → milisecond
-  - Time Object
+  - Datetime
     - unixtime / unixtime+timezone → datetime.datetime
     - unixtime / unixtime+timezone → datetime.date
-  - Unix Time
+  - Unixtime
     - string(yyyy-mm-dd hh:mm:ss) / string(yyyy-mm-dd hh:mm:ss)+timezone → unixtime
 
 ## Installing
 
   ```
   pip install unic
   ```
 
 
 
 ## Example
-
 ### Time Unit
+#### Time
 
 ```python
 import unic
 
 
-converter = unic.TimeUnit()
+converter = unic.TimeModel()
 # Convert hour to minute
-converte_min = converter.convert(2, from_unit="hour", to_unit="min")
+convert_min = converter.convert(2, from_unit="hour", to_unit="min")
 ```
 
-### Time Object
+#### Datetime
 
 ```python
 import unic
 
 
-converter = unic.TimeObject()
+converter = unic.DatetimeModel()
 # Convert to datatime
-converte_datetime = converter.convert(1577841753, target="datetime")
+convert_datetime = converter.convert(1577841753, target="datetime")
 ```
 
-### Unix Time
+#### Unixtime
 
 ```python
 import unic
 
 
-converter = unic.Unixtime()
+converter = unic.UnixtimeModel()
 # Specify time zone
-converte_unixtime = converter.convert("2023-05-12 10:15:20", tz="Asia/Tokyo")
+convert_unixtime = converter.convert("2023-05-12 10:15:20", tz="Asia/Tokyo")
 ```
```

### Comparing `unic-0.1.1/unic/configs/timezone/settings.toml` & `unic-0.2.0/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.1.1/unic/timeobject/timeobject.py` & `unic-0.2.0/unic/time_unit/datetime/datetime_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date, datetime, timezone, timedelta
 from unic.utils import check_parameter, config_parser
 
 
-class TimeObject:
+class DatetimeModel:
     def convert(self, data: int, **kwargs: any) -> date:
         self.check_parameter_name(kwargs)
         tz = kwargs.get("tz", None)
         target = kwargs["target"]
 
         if tz:
             check_parameter.check_value(tz)
```

### Comparing `unic-0.1.1/unic/unit/timeunit.py` & `unic-0.2.0/unic/time_unit/time/time_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     StrictStr,
 )
 from unic.utils import config_parser
 from fractions import Fraction
 from typing import Union
 
 
-class TimeUnitModel(BaseModel):
+class UnitValidationModel(BaseModel):
     # Prevent automatic conversion
     data: Union[StrictInt, StrictFloat]
     from_unit: StrictStr
     to_unit: StrictStr
 
     @field_validator("from_unit")
     def from_unit_check(cls, v):
@@ -32,19 +32,19 @@
         if v not in valid_units:
             raise ValueError(
                 f"Invalid to_unit name: {v}. Allowed values are {valid_units}."
             )
         return v
 
 
-class TimeUnit:
+class TimeModel:
     def convert(self, data: int, *, from_unit: str = None, to_unit: str = None) -> int:
         try:
             self.check_parameter_count(from_unit, to_unit)
-            input_data = TimeUnitModel(data=data, from_unit=from_unit, to_unit=to_unit)
+            input_data = UnitValidationModel(data=data, from_unit=from_unit, to_unit=to_unit)
         except ValidationError as e:
             raise ValueError(e.errors()[0]["msg"])
 
         parameter = config_parser.parse_toml("unit")
         data = float(input_data.data * Fraction(parameter[from_unit][to_unit]))
 
         return data
```

### Comparing `unic-0.1.1/unic/unixtime/unixtime.py` & `unic-0.2.0/unic/time_unit/unixtime/unixtime_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timezone, timedelta
 from unic.utils import check_parameter, config_parser
 
 
-class Unixtime:
+class UnixtimeModel:
     def convert(self, data: str, **kwargs: any) -> int:
         check_parameter.check_number(kwargs)
 
         if len(kwargs) == 1:
             tz = kwargs.get("tz", None)
             check_parameter.check_value(tz)
             parameter = config_parser.parse_toml("timezone")
```

### Comparing `unic-0.1.1/unic/utils/check_parameter.py` & `unic-0.2.0/unic/utils/check_parameter.py`

 * *Files identical despite different names*

### Comparing `unic-0.1.1/PKG-INFO` & `unic-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,unixtime
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
@@ -20,63 +20,66 @@
 Description-Content-Type: text/markdown
 
 ![Python minimum version](https://img.shields.io/badge/Python-3.8%2B-brightgreen)
 [![pytest](https://github.com/subretu/unic/actions/workflows/pytest.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/pytest.yml)
 [![black](https://github.com/subretu/unic/actions/workflows/format.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/format.yml)
 
 # unic
-- unic is a Python package that can convert various units.
+unic is a Python package that can convert various units.
+
+## Conversion Targets
 - The current available conversion targets are as follows.
-  - Time Unit
+### Time Unit
+  - Time
     - minute / second / milisecond → hour
     - hour / second / milisecond → minute
     - hour / minute / milisecond → second
     - hour / minute / second → milisecond
-  - Time Object
+  - Datetime
     - unixtime / unixtime+timezone → datetime.datetime
     - unixtime / unixtime+timezone → datetime.date
-  - Unix Time
+  - Unixtime
     - string(yyyy-mm-dd hh:mm:ss) / string(yyyy-mm-dd hh:mm:ss)+timezone → unixtime
 
 ## Installing
 
   ```
   pip install unic
   ```
 
 
 
 ## Example
-
 ### Time Unit
+#### Time
 
 ```python
 import unic
 
 
-converter = unic.TimeUnit()
+converter = unic.TimeModel()
 # Convert hour to minute
-converte_min = converter.convert(2, from_unit="hour", to_unit="min")
+convert_min = converter.convert(2, from_unit="hour", to_unit="min")
 ```
 
-### Time Object
+#### Datetime
 
 ```python
 import unic
 
 
-converter = unic.TimeObject()
+converter = unic.DatetimeModel()
 # Convert to datatime
-converte_datetime = converter.convert(1577841753, target="datetime")
+convert_datetime = converter.convert(1577841753, target="datetime")
 ```
 
-### Unix Time
+#### Unixtime
 
 ```python
 import unic
 
 
-converter = unic.Unixtime()
+converter = unic.UnixtimeModel()
 # Specify time zone
-converte_unixtime = converter.convert("2023-05-12 10:15:20", tz="Asia/Tokyo")
+convert_unixtime = converter.convert("2023-05-12 10:15:20", tz="Asia/Tokyo")
 ```
```


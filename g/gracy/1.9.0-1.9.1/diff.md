# Comparing `tmp/gracy-1.9.0.tar.gz` & `tmp/gracy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gracy-1.9.0.tar", max compression
+gzip compressed data, was "gracy-1.9.1.tar", max compression
```

## Comparing `gracy-1.9.0.tar` & `gracy-1.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1084 2023-02-21 11:04:32.593677 gracy-1.9.0/LICENSE
--rw-r--r--   0        0        0    24001 2023-02-21 11:04:32.593677 gracy-1.9.0/README.md
--rw-r--r--   0        0        0     2290 2023-02-21 11:05:22.369267 gracy-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1097 2023-02-21 11:05:22.321267 gracy-1.9.0/src/gracy/__init__.py
--rw-r--r--   0        0        0      396 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_configs.py
--rw-r--r--   0        0        0    14670 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_core.py
--rw-r--r--   0        0        0     3338 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_loggers.py
--rw-r--r--   0        0        0    14758 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_models.py
--rw-r--r--   0        0        0      206 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_replay/_models.py
--rw-r--r--   0        0        0      952 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_replay/_sqlite_schema.py
--rw-r--r--   0        0        0     3286 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_replay/_storages.py
--rw-r--r--   0        0        0      878 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_replay/_wrappers.py
--rw-r--r--   0        0        0     3194 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_reports/_builders.py
--rw-r--r--   0        0        0     2410 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_reports/_models.py
--rw-r--r--   0        0        0     8063 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_reports/_printers.py
--rw-r--r--   0        0        0      618 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/_types.py
--rw-r--r--   0        0        0     3793 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-21 11:04:32.597677 gracy-1.9.0/src/gracy/py.typed
--rw-r--r--   0        0        0    25576 1970-01-01 00:00:00.000000 gracy-1.9.0/setup.py
--rw-r--r--   0        0        0    25443 1970-01-01 00:00:00.000000 gracy-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-02-21 12:25:09.161183 gracy-1.9.1/LICENSE
+-rw-r--r--   0        0        0    24001 2023-02-21 12:25:09.161183 gracy-1.9.1/README.md
+-rw-r--r--   0        0        0     2290 2023-02-21 12:26:01.956926 gracy-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1097 2023-02-21 12:26:01.908926 gracy-1.9.1/src/gracy/__init__.py
+-rw-r--r--   0        0        0      396 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_configs.py
+-rw-r--r--   0        0        0    14670 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_core.py
+-rw-r--r--   0        0        0     3338 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_loggers.py
+-rw-r--r--   0        0        0    14758 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_models.py
+-rw-r--r--   0        0        0      206 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_replay/_models.py
+-rw-r--r--   0        0        0      952 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_replay/_sqlite_schema.py
+-rw-r--r--   0        0        0     3286 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_replay/_storages.py
+-rw-r--r--   0        0        0      878 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_replay/_wrappers.py
+-rw-r--r--   0        0        0     3194 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_reports/_builders.py
+-rw-r--r--   0        0        0     2410 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_reports/_models.py
+-rw-r--r--   0        0        0     8063 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_reports/_printers.py
+-rw-r--r--   0        0        0      618 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/_types.py
+-rw-r--r--   0        0        0     3795 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-21 12:25:09.165183 gracy-1.9.1/src/gracy/py.typed
+-rw-r--r--   0        0        0    25576 1970-01-01 00:00:00.000000 gracy-1.9.1/setup.py
+-rw-r--r--   0        0        0    25443 1970-01-01 00:00:00.000000 gracy-1.9.1/PKG-INFO
```

### Comparing `gracy-1.9.0/LICENSE` & `gracy-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/README.md` & `gracy-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/pyproject.toml` & `gracy-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gracy"
-version = "1.9.0"
+version = "1.9.1"
 description = "Gracefully manage your API interactions"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["api", "throttling", "http", "https", "async", "retry"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/gracy"
 repository = "https://github.com/guilatrova/gracy"
```

### Comparing `gracy-1.9.0/src/gracy/__init__.py` & `gracy-1.9.1/src/gracy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 from ._replay._models import GracyRecording
 from ._replay._storages import GracyReplay, GracyReplayStorage, SQLiteReplayStorage
 from ._reports._models import GracyAggregatedRequest, GracyAggregatedTotal, GracyReport
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s %(message)s")
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 __all__ = [
     "exceptions",
     # Core
     "Gracy",
     "graceful",
     # Models
```

### Comparing `gracy-1.9.0/src/gracy/_core.py` & `gracy-1.9.1/src/gracy/_core.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_loggers.py` & `gracy-1.9.1/src/gracy/_loggers.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_models.py` & `gracy-1.9.1/src/gracy/_models.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_replay/_sqlite_schema.py` & `gracy-1.9.1/src/gracy/_replay/_sqlite_schema.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_replay/_storages.py` & `gracy-1.9.1/src/gracy/_replay/_storages.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_replay/_wrappers.py` & `gracy-1.9.1/src/gracy/_replay/_wrappers.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_reports/_builders.py` & `gracy-1.9.1/src/gracy/_reports/_builders.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_reports/_models.py` & `gracy-1.9.1/src/gracy/_reports/_models.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_reports/_printers.py` & `gracy-1.9.1/src/gracy/_reports/_printers.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/_types.py` & `gracy-1.9.1/src/gracy/_types.py`

 * *Files identical despite different names*

### Comparing `gracy-1.9.0/src/gracy/exceptions.py` & `gracy-1.9.1/src/gracy/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         self.url = response.request.url
         self.response = response
 
         super().__init__(msg)
 
     def __reduce__(self):
-        return (GracyParseFailed, (self.response))
+        return (GracyParseFailed, (self.response,))
 
 
 class BadResponse(GracyException):
     def __init__(
         self,
         message: str | None,
         url: str,
@@ -119,8 +119,8 @@
     def __init__(self, request: httpx.Request) -> None:
         self.request = request
 
         msg = f"Gracy was unable to replay {request.method} {request.url} - did you forget to record it?"
         super().__init__(msg)
 
     def __reduce__(self):
-        return (GracyReplayRequestNotFound, (self.request))
+        return (GracyReplayRequestNotFound, (self.request,))
```

### Comparing `gracy-1.9.0/setup.py` & `gracy-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['httpx>=0.23.3,<0.24.0']
 
 extras_require = \
 {'rich': ['rich']}
 
 setup_kwargs = {
     'name': 'gracy',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'Gracefully manage your API interactions',
     'long_description': '<p align="center">\n    <img src="https://raw.githubusercontent.com/guilatrova/gracy/main/img/logo.png">\n</p>\n\n<h2 align="center">Gracefully manage your API interactions</h2>\n\n<p align="center">\n  <!-- CI --><a href="https://github.com/guilatrova/gracy/actions"><img alt="Actions Status" src="https://github.com/guilatrova/gracy/workflows/CI/badge.svg"></a>\n  <!-- PyPI --><a href="https://pypi.org/project/gracy/"><img alt="PyPI" src="https://img.shields.io/pypi/v/gracy"/></a>\n  <!-- Supported Python versions --><img src="https://badgen.net/pypi/python/gracy" />\n  <!-- Alternative Python versioning: <img alt="python version" src="https://img.shields.io/badge/python-3.9%20%7C%203.10-blue"> -->\n  <!-- PyPI downloads --><a href="https://pepy.tech/project/gracy/"><img alt="Downloads" src="https://static.pepy.tech/badge/gracy/week"/></a>\n  <!-- LICENSE --><a href="https://github.com/guilatrova/gracy/blob/main/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/guilatrova/gracy"/></a>\n  <!-- Formatting --><a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>\n  <!-- Tryceratops --><a href="https://github.com/guilatrova/tryceratops"><img alt="try/except style: tryceratops" src="https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black" /></a>\n  <!-- Typing --><a href="https://github.com/python/mypy"><img alt="Types: mypy" src="https://img.shields.io/badge/types-mypy-blue.svg"/></a>\n  <!-- Follow handle --><a href="https://twitter.com/intent/user?screen_name=guilatrova"><img alt="Follow guilatrova" src="https://img.shields.io/twitter/follow/guilatrova?style=social"/></a>\n  <!-- Sponsor --><a href="https://github.com/sponsors/guilatrova"><img alt="Sponsor guilatrova" src="https://img.shields.io/github/sponsors/guilatrova?logo=GitHub%20Sponsors&style=social"/></a>\n</p>\n\nGracy helps you handle failures, logging, retries, throttling, and tracking for all your HTTP interactions. Gracy uses [httpx](https://github.com/encode/httpx) under the hood.\n\n> "Let Gracy do the boring stuff while you focus on your application"\n\n---\n\n**Summary**\n\n- [🧑\u200d💻 Get started](#-get-started)\n  - [Installation](#installation)\n  - [Usage](#usage)\n    - [Simple example](#simple-example)\n    - [More examples](#more-examples)\n- [Settings](#settings)\n  - [Strict/Allowed status code](#strictallowed-status-code)\n  - [Parsing](#parsing)\n  - [Retry](#retry)\n  - [Throttling](#throttling)\n  - [Logging](#logging)\n  - [Custom Exceptions](#custom-exceptions)\n- [Reports](#reports)\n  - [Logger](#logger)\n  - [List](#list)\n  - [Table](#table)\n- [Replay requests](#replay-requests)\n  - [Recording](#recording)\n  - [Replay](#replay)\n- [Advanced Usage](#advanced-usage)\n  - [Customizing/Overriding configs per method](#customizingoverriding-configs-per-method)\n  - [Customizing HTTPx client](#customizing-httpx-client)\n  - [Creating a custom Replay data source](#creating-a-custom-replay-data-source)\n- [📚 Extra Resources](#-extra-resources)\n- [Change log](#change-log)\n- [License](#license)\n- [Credits](#credits)\n\n\n## 🧑\u200d💻 Get started\n\n### Installation\n\n```\npip install gracy\n```\n\nOR\n\n```\npoetry add gracy\n```\n\n### Usage\n\nExamples will be shown using the [PokeAPI](https://pokeapi.co).\n\n#### Simple example\n\n```py\n# 0. Import\nimport asyncio\nfrom typing import Awaitable\nfrom gracy import BaseEndpoint, Gracy, GracyConfig, LogEvent, LogLevel\n\n# 1. Define your endpoints\nclass PokeApiEndpoint(BaseEndpoint):\n    GET_POKEMON = "/pokemon/{NAME}" # 👈 Put placeholders as needed\n\n# 2. Define your Graceful API\nclass GracefulPokeAPI(Gracy[str]):\n    class Config:  # type: ignore\n        BASE_URL = "https://pokeapi.co/api/v2/" # 👈 Optional BASE_URL\n        # 👇 Define settings to apply for every request\n        SETTINGS = GracyConfig(\n          log_request=LogEvent(LogLevel.DEBUG),\n          log_response=LogEvent(LogLevel.INFO, "{URL} took {ELAPSED}"),\n          parser={\n            "default": lambda r: r.json()\n          }\n        )\n\n    async def get_pokemon(self, name: str) -> Awaitable[dict]:\n        return await self.get(PokeApiEndpoint.GET_POKEMON, {"NAME": name})\n\npokeapi = GracefulPokeAPI()\n\nasync def main():\n    try:\n      pokemon = await pokeapi.get_pokemon("pikachu")\n      print(pokemon)\n\n    finally:\n        pokeapi.report_status("rich")\n\n\nasyncio.run(main())\n```\n\n#### More examples\n\n- [PokeAPI with retries, parsers, logs](./examples/pokeapi.py)\n- [PokeAPI with throttling](./examples/pokeapi_throttle.py)\n- [PokeAPI with replay](./examples/pokeapi_replay.py)\n\n## Settings\n\n### Strict/Allowed status code\n\nBy default Gracy considers any successful status code (200-299) as successful.\n\n**Strict**\n\nYou can modify this behavior by defining a strict status code or increase the range of allowed status codes:\n\n```py\nfrom http import HTTPStatus\n\nGracyConfig(\n  strict_status_code=HTTPStatus.CREATED\n)\n```\n\nor a list of values:\n\n```py\nfrom http import HTTPStatus\n\nGracyConfig(\n  strict_status_code={HTTPStatus.OK, HTTPStatus.CREATED}\n)\n```\n\nUsing `strict_status_code` means that any other code not specified will raise an error regardless of being successful or not.\n\n**Allowed**\n\nYou can also keep the behavior, but extend the range of allowed codes.\n\n```py\nfrom http import HTTPStatus\n\nGracyConfig(\n  allowed_status_code=HTTPStatus.NOT_FOUND\n)\n```\n\nor a list of values\n\n\n```py\nfrom http import HTTPStatus\n\nGracyConfig(\n  allowed_status_code={HTTPStatus.NOT_FOUND, HTTPStatus.FORBIDDEN}\n)\n```\n\nUsing `allowed_status_code` means that all successful codes plus your defined codes will be considered successful.\n\nThis is quite useful for parsing as you\'ll see soon.\n\n⚠️ Note that `strict_status_code` takes precedence over `allowed_status_code`, probably you don\'t want to combine those. Prefer one or the other.\n\n### Parsing\n\nParsing allows you to handle the request based on the status code returned.\n\nThe basic example is parsing `json`:\n\n```py\nGracyConfig(\n  parser={\n    "default": lambda r: r.json()\n  }\n)\n```\n\nIn this example all successful requests will automatically return the `json()` result.\n\nYou can also narrow it down to handle specific status codes.\n\n```py\nclass Config:\n  SETTINGS = GracyConfig(\n    ...,\n    allowed_status_code=HTTPStatusCode.NOT_FOUND,\n    parser={\n      "default": lambda r: r.json()\n      HTTPStatusCode.NOT_FOUND: None\n    }\n  )\n\nasync def get_pokemon(self, name: str) -> dict| None:\n  # 👇 Returns either dict or None\n  return await self.get(PokeApiEndpoint.GET_POKEMON, {"NAME": name})\n```\n\nOr even customize [exceptions to improve your code readability](https://guicommits.com/handling-exceptions-in-python-like-a-pro/):\n\n```py\nclass PokemonNotFound(GracyUserDefinedException):\n  ... # More on exceptions below\n\nclass Config:\n  GracyConfig(\n    ...,\n    allowed_status_code=HTTPStatusCode.NOT_FOUND,\n    parser={\n      "default": lambda r: r.json()\n      HTTPStatusCode.NOT_FOUND: PokemonNotFound\n    }\n  )\n\nasync def get_pokemon(self, name: str) -> Awaitable[dict]:\n  # 👇 Returns either dict or raises PokemonNotFound\n  return await self.get(PokeApiEndpoint.GET_POKEMON, {"NAME": name})\n```\n\n### Retry\n\nWho doesn\'t hate flaky APIs? 🙋\n\nYet there\'re many of them.\n\nUsing tenacity, backoff, retry, aiohttp_retry, and any other retry libs is **NOT easy enough**. 🙅\n\nYou still would need to code the implementation for each request which is annoying.\n\nHere\'s how Gracy allows you to implement your retry logic:\n\n```py\nclass Config:\n  GracyConfig(\n    retry=GracefulRetry(\n      delay=1,\n      max_attempts=3,\n      delay_modifier=1.5,\n      retry_on=None,\n      log_before=None,\n      log_after=LogEvent(LogLevel.WARNING),\n      log_exhausted=LogEvent(LogLevel.CRITICAL),\n      behavior="break",\n    )\n  )\n```\n\n| Parameter        | Description                                                                               | Example                                                                                                      |\n| ---------------- | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |\n| `delay`          | How many seconds to wait between retries                                                  | `2` would wait 2 seconds, `1.5` would wait 1.5 seconds, and so on                                            |\n| `max_attempts`   | How many times should Gracy retry the request?                                            | `10` means 1 regular request with additional 10 retries in case they keep failing. `1` should be the minimum |\n| `delay_modifier` | Allows you to specify increasing delay times by multiplying this value to `delay`         | Setting `1` means no delay change. Setting `2` means delay will be doubled every retry                       |\n| `retry_on`       | Should we retry for which status codes? `None` means for any non successful status code   | `HTTPStatus.BAD_REQUEST`, or `{HTTPStatus.BAD_REQUEST, HTTPStatus.FORBIDDEN}`                                |\n| `log_before`     | Specify log level. `None` means don\'t log                                                 | More on logging later                                                                                        |\n| `log_after`      | Specify log level. `None` means don\'t log                                                 | More on logging later                                                                                        |\n| `log_exhausted`  | Specify log level. `None` means don\'t log                                                 | More on logging later                                                                                        |\n| `behavior`       | Allows you to define how to deal if the retry fails. `pass` will accept any retry failure | `pass` or `break` (default)                                                                                  |\n\n\n### Throttling\n\nRate limiting issues? No more.\n\nGracy helps you proactively deal with it before any API throws 429 in your face.\n\n**Creating rules**\n\nYou can define rules per endpoint using regex:\n\n```py\nSIMPLE_RULE = ThrottleRule(\n  url_pattern=r".*",\n  max_requests=2\n)\nprint(SIMPLE_RULE)\n# Output: "2 requests per second for URLs matching re.compile(\'.*\')"\n\nCOMPLEX_RULE = ThrottleRule(\n  url_pattern=r".*\\/pokemon\\/.*",\n  max_requests=10,\n  per_time=timedelta(minutes=1, seconds=30),\n)\nprint(COMPLEX_RULE)\n# Output: 10 requests per 90 seconds for URLs matching re.compile(\'.*\\\\/pokemon\\\\/.*\')\n```\n\n**Setting throttling**\n\nYou can set up logging and assign rules as:\n\n```py\nclass Config:\n  GracyConfig(\n    throttling=GracefulThrottle(\n        rules=ThrottleRule(r".*", 2), # 2 reqs/s for any endpoint\n        log_limit_reached=LogEvent(LogLevel.ERROR),\n        log_wait_over=LogEvent(LogLevel.WARNING),\n    ),\n  )\n```\n\n### Logging\n\nYou can **define and customize logs** for events by using `LogEvent` and `LogLevel`:\n\n```py\nverbose_log = LogEvent(LogLevel.CRITICAL)\ncustom_warn_log = LogEvent(LogLevel.WARNING, custom_message="{METHOD} {URL} is quite slow and flaky")\ncustom_error_log = LogEvent(LogLevel.INFO, custom_message="{URL} returned a bad status code {STATUS}, but that\'s fine")\n```\n\nNote that placeholders are formatted and replaced later on by Gracy based on the event type, like:\n\n**Placeholders per event**\n\n| Placeholder             | Description                                           | Example                                     | Supported Events                   |\n| ----------------------- | ----------------------------------------------------- | ------------------------------------------- | ---------------------------------- |\n| `{URL}`                 | Full url being targetted                              | `https://pokeapi.co/api/v2/pokemon/pikachu` | *All*                              |\n| `{UURL}`                | Full **Unformatted** url being targetted              | `https://pokeapi.co/api/v2/pokemon/{NAME}`  | *All*                              |\n| `{ENDPOINT}`            | Endpoint being targetted                              | `/pokemon/pikachu`                          | *All*                              |\n| `{UENDPOINT}`           | **Unformatted** endpoint being targetted              | `/pokemon/{NAME}`                           | *All*                              |\n| `{METHOD}`              | HTTP Request being used                               | `GET`, `POST`                               | *All*                              |\n| `{STATUS}`              | Status code returned by the response                  | `200`, `404`, `501`                         | *After Request, On request errors* |\n| `{ELAPSED}`             | Amount of seconds taken for the request to complete   | *Numeric*                                   | *After Request, On request errors* |\n| `{RETRY_DELAY}`         | How long Gracy will wait before repeating the request | *Numeric*                                   | *Any Retry event*                  |\n| `{CUR_ATTEMPT}`         | Current attempt count for the current request         | *Numeric*                                   | *Any Retry event*                  |\n| `{MAX_ATTEMPT}`         | Max attempt defined for the current request           | *Numeric*                                   | *Any Retry event*                  |\n| `{THROTTLE_LIMIT}`      | How many reqs/s is defined for the current request    | *Numeric*                                   | *Any Throttle event*               |\n| `{THROTTLE_TIME}`       | How long Gracy will wait before calling the request   | *Numeric*                                   | *Any Throttle event*               |\n| `{THROTTLE_TIME_RANGE}` | Time range defined by the throttling rule             | `second`, `90 seconds`                      | *Any Throttle event*               |\n\nand you can set up the log events as follows:\n\n**Requests**\n\n1. Before request\n2. After response\n3. Response has non successful errors\n\n```py\nGracyConfig(\n  log_request=LogEvent(),\n  log_response=LogEvent(),\n  log_errors=LogEvent(),\n)\n```\n\n**Retry**\n\n1. Before retry\n2. After retry\n3. When retry exhausted\n\n```py\nGracefulRetry(\n  ...,\n  log_before=LogEvent(),\n  log_after=LogEvent(),\n  log_exhausted=LogEvent(),\n)\n```\n\n**Throttling**\n\n1. When reqs/s limit is reached\n2. When limit decreases again\n\n```py\nGracefulThrottle(\n  ...,\n  log_limit_reached=LogEvent()\n  log_wait_over=LogEvent()\n)\n```\n\n**Dynamic Customization**\n\nYou can customize it even further by passing a lambda:\n\n```py\nLogEvent(\n    LogLevel.ERROR,\n    lambda r: "Request failed with {STATUS}" f" and it was {\'redirected\' if r.is_redirect else \'NOT redirected\'}"\n    if r\n    else "",\n)\n```\n\nConsider that:\n\n- Not all log events have the response available, so you need to guard yourself against it\n- Placeholders still works (e.g. `{STATUS}`)\n- You need to watch out for some attrs that might break the formatting logic (e.g. `r.headers`)\n\n### Custom Exceptions\n\nYou can define custom exceptions for more [fine grained control over your exception messages/types](https://guicommits.com/how-to-structure-exception-in-python-like-a-pro/).\n\nThe simplest you can do is:\n\n```py\nfrom gracy import Gracy, GracyConfig\nfrom gracy.exceptions import GracyUserDefinedException\n\nclass MyCustomException(GracyUserDefinedException):\n  pass\n\nclass MyApi(Gracy[str]):\n  class Config:\n    SETTINGS = GracyConfig(\n      ...,\n      parser={\n        HTTPStatus.BAD_REQUEST: MyCustomException\n      }\n    )\n```\n\nThis will raise your custom exception under the conditions defined in your parser.\n\nYou can improve it even further by customizing your message:\n\n```py\nclass PokemonNotFound(GracyUserDefinedException):\n    BASE_MESSAGE = "Unable to find a pokemon with the name [{NAME}] at {URL} due to {STATUS} status"\n\n    def _format_message(self, request_context: GracyRequestContext, response: httpx.Response) -> str:\n        format_args = self._build_default_args()\n        name = request_context.endpoint_args.get("NAME", "Unknown")\n        return self.BASE_MESSAGE.format(NAME=name, **format_args)\n```\n\n## Reports\n\n### Logger\n\nRecommended for production environments.\n\nGracy reports a short summary using `logger.info`.\n\n```python\npokeapi = GracefulPokeAPI()\n# do stuff with your API\npokeapi.report_status("logger")\n\n# OUTPUT\n❯ Gracy tracked that \'https://pokeapi.co/api/v2/pokemon/{NAME}\' was hit 1 time(s) with a success rate of 100.00%, avg latency of 0.45s, and a rate of 1.0 reqs/s.\n❯ Gracy tracked a total of 2 requests with a success rate of 100.00%, avg latency of 0.24s, and a rate of 1.0 reqs/s.\n```\n\n### List\n\nUses `print` to generate a short list with all attributes:\n\n```python\npokeapi = GracefulPokeAPI()\n# do stuff with your API\npokeapi.report_status("list")\n\n# OUTPUT\n   ____\n  / ___|_ __ __ _  ___ _   _\n | |  _| \'__/ _` |/ __| | | |\n | |_| | | | (_| | (__| |_| |\n  \\____|_|  \\__,_|\\___|\\__, |\n                       |___/  Requests Summary Report\n\n\n1. https://pokeapi.co/api/v2/pokemon/{NAME}\n    Total Reqs (#): 1\n       Success (%): 100.00%\n          Fail (%): 0.00%\n   Avg Latency (s): 0.39\n   Max Latency (s): 0.39\n         2xx Resps: 1\n         3xx Resps: 0\n         4xx Resps: 0\n         5xx Resps: 0\n      Avg Reqs/sec: 1.0 reqs/s\n\n\n2. https://pokeapi.co/api/v2/generation/{ID}/\n    Total Reqs (#): 1\n       Success (%): 100.00%\n          Fail (%): 0.00%\n   Avg Latency (s): 0.04\n   Max Latency (s): 0.04\n         2xx Resps: 1\n         3xx Resps: 0\n         4xx Resps: 0\n         5xx Resps: 0\n      Avg Reqs/sec: 1.0 reqs/s\n\n\nTOTAL\n    Total Reqs (#): 2\n       Success (%): 100.00%\n          Fail (%): 0.00%\n   Avg Latency (s): 0.21\n   Max Latency (s): 0.00\n         2xx Resps: 2\n         3xx Resps: 0\n         4xx Resps: 0\n         5xx Resps: 0\n      Avg Reqs/sec: 1.0 reqs/s\n```\n\n### Table\n\nIt requires you to install [Rich](https://github.com/Textualize/rich).\n\n```py\npokeapi = GracefulPokeAPI()\n# do stuff with your API\npokeapi.report_status("rich")\n```\n\nHere\'s an example of how it looks:\n\n![Report](https://raw.githubusercontent.com/guilatrova/gracy/main/img/report-example.png)\n\n\n## Replay requests\n\nGracy allows you to replay requests and responses from previous interactions.\n\nThis is powerful because it allows you to test APIs without latency or consuming your rate limit. Now writing unit tests that relies on third-party APIs is doable.\n\nIt works in two steps:\n\n| **Step**     | **Description**                                                                | **Hits the API?** |\n| ------------ | ------------------------------------------------------------------------------ | ----------------- |\n| 1. Recording | Stores all requests/responses to be later replayed                             | **Yes**           |\n| 2. Replay    | Returns all previously generated responses based on your request as a "replay" | No                |\n\n### Recording\n\nThe effort to record requests/responses is ZERO. You just need to pass a recording config to your Graceful API:\n\n```py\nrecord_mode = GracyReplay("record", SQLiteReplayStorage("pokeapi.sqlite3"))\npokeapi = GracefulPokeAPI(record_mode)\n```\n\n**Every request** will be recorded to the defined data source.\n\n### Replay\n\nOnce you have recorded all your requests you can enable the replay mode:\n\n```py\nreplay_mode = GracyReplay("replay", SQLiteReplayStorage("pokeapi.sqlite3"))\npokeapi = GracefulPokeAPI(replay_mode)\n```\n\n**Every request** will be routed to the defined data source resulting in faster responses.\n\n**⚠️ Note that parsers, retries, throttling, and similar configs will work as usual**.\n\n\n## Advanced Usage\n\n### Customizing/Overriding configs per method\n\nAPIs may return different responses/conditions/payloads based on the endpoint.\n\nYou can override any `GracyConfig` on a per method basis by using the `graceful` decorator.\n\n```python\nfrom gracy import Gracy, GracyConfig, GracefulRetry, graceful\n\nretry = GracefulRetry(...)\n\nclass GracefulPokeAPI(Gracy[PokeApiEndpoint]):\n    class Config:  # type: ignore\n        BASE_URL = "https://pokeapi.co/api/v2/"\n        SETTINGS = GracyConfig(\n            retry=retry,\n            log_errors=LogEvent(\n                LogLevel.ERROR, "How can I become a pokemon master if {URL} keeps failing with {STATUS}"\n            ),\n        )\n\n    @graceful(\n        retry=None, # 👈 Disables retry set in Config\n        log_errors=None, # 👈 Disables log_errors set in Config\n        allowed_status_code=HTTPStatus.NOT_FOUND,\n        parser={\n            "default": lambda r: r.json()["order"],\n            HTTPStatus.NOT_FOUND: None,\n        },\n    )\n    async def maybe_get_pokemon_order(self, name: str):\n        val: str | None = await self.get(PokeApiEndpoint.GET_POKEMON, {"NAME": name})\n        return val\n\n    @graceful( # 👈 Retry and log_errors are still set for this one\n      strict_status_code=HTTPStatus.OK,\n      parser={"default": lambda r: r.json()["order"]},\n    )\n    async def get_pokemon_order(self, name: str):\n      val: str = await self.get(PokeApiEndpoint.GET_POKEMON, {"NAME": name})\n      return val\n```\n\n### Customizing HTTPx client\n\nYou might want to modify the HTTPx client settings, do so by:\n\n```py\nclass YourAPIClient(Gracy[str]):\n    class Config:  # type: ignore\n        ...\n\n    def __init__(self, token: token) -> None:\n        self._token = token\n        super().__init__()\n\n    # 👇 Implement your logic here\n    def _create_client(self) -> httpx.AsyncClient:\n        client = super()._create_client()\n        client.headers = {"Authorization": f"token {self._token}"}  # type: ignore\n        return client\n```\n\n### Creating a custom Replay data source\n\nGracy was built with extensibility in mind.\n\nYou can create your own storage to store/load anywhere (e.g. Mongo Database), here\'s an example:\n\n```py\nimport httpx\nfrom gracy import GracyReplayStorage, GracyRecording\n\nclass MyCustomStorage(GracyReplayStorage):\n  def prepare(self) -> None: # (Optional) Executed upon API instance creation.\n    ...\n\n  async def record(self, response: httpx.Response) -> None:\n    ... # REQUIRED. Your logic to store the response object. Note the httpx.Response has request data.\n\n  async def load(self, request: httpx.Request) -> httpx.Response:\n    ... # REQUIRED. Your logic to load a response object based on the request.\n\n\n# Usage\nrecord_mode = GracyReplay("record", MyCustomStorage())\nreplay_mode = GracyReplay("replay", MyCustomStorage())\n\npokeapi = GracefulPokeAPI(record_mode)\n```\n\n## 📚 Extra Resources\n\nSome good practices I learned over the past years guided Gracy\'s philosophy, you might benefit by reading:\n\n- [How to log](https://guicommits.com/how-to-log-in-python-like-a-pro/)\n- [How to handle exceptions](https://guicommits.com/handling-exceptions-in-python-like-a-pro/)\n  - [How to structure exceptions](https://guicommits.com/how-to-structure-exception-in-python-like-a-pro/)\n- [How to use Async correctly](https://guicommits.com/effective-python-async-like-a-pro/)\n- [Book: Python like a PRO](https://guilatrova.gumroad.com/l/python-like-a-pro)\n- [Book: Effective Python](https://amzn.to/3bEVHpG)\n\n<!-- ## Contributing -->\n<!-- Thank you for considering making Gracy better for everyone! -->\n<!-- Refer to [Contributing docs](docs/CONTRIBUTING.md).-->\n\n## Change log\n\nSee [CHANGELOG](CHANGELOG.md).\n\n## License\n\nMIT\n\n## Credits\n\nThanks to the last three startups I worked which forced me to do the same things and resolve the same problems over and over again. I got sick of it and built this lib.\n\nMost importantly: **Thanks to God**, who allowed me (a random 🇧🇷 guy) to work for many different 🇺🇸 startups. This is ironic since due to God\'s grace, I was able to build Gracy. 🙌\n\nAlso, thanks to the [httpx](https://github.com/encode/httpx) and [rich](https://github.com/Textualize/rich) projects for the beautiful and simple APIs that powers Gracy.\n',
     'author': 'Guilherme Latrova',
     'author_email': 'hello@guilatrova.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/guilatrova/gracy',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['gracy', 'gracy._replay', 'gracy._reports'] package_data =
 \ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0'] extras_require = \
-{'rich': ['rich']} setup_kwargs = { 'name': 'gracy', 'version': '1.9.0',
+{'rich': ['rich']} setup_kwargs = { 'name': 'gracy', 'version': '1.9.1',
 'description': 'Gracefully manage your API interactions', 'long_description': '
   \n [https://raw.githubusercontent.com/guilatrova/gracy/main/img/logo.png]\n
 \n\n
               ***** Gracefully manage your API interactions *****
 \n\n
   \n [Actions_Status]\n [PyPI]\n [https://badgen.net/pypi/python/gracy]\n \n
        [Downloads]\n [GitHub]\n [Code_style:_black]\n [try/except_style:
```

### Comparing `gracy-1.9.0/PKG-INFO` & `gracy-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gracy
-Version: 1.9.0
+Version: 1.9.1
 Summary: Gracefully manage your API interactions
 Home-page: https://github.com/guilatrova/gracy
 License: MIT
 Keywords: api,throttling,http,https,async,retry
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
 Requires-Python: >=3.8.1,<4.0
```


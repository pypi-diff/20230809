# Comparing `tmp/bing_rewards-2.0.0.tar.gz` & `tmp/bing_rewards-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bing_rewards-2.0.0.tar", max compression
+gzip compressed data, was "bing_rewards-2.1.0.tar", max compression
```

## Comparing `bing_rewards-2.0.0.tar` & `bing_rewards-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-03-24 03:16:47.331887 bing_rewards-2.0.0/LICENSE
--rw-r--r--   0        0        0     7019 2023-03-24 03:16:47.331887 bing_rewards-2.0.0/README.md
--rw-r--r--   0        0        0    11412 2023-03-24 03:16:47.331887 bing_rewards-2.0.0/bing_rewards/__init__.py
--rw-r--r--   0        0        0       38 2023-03-24 03:16:47.331887 bing_rewards-2.0.0/bing_rewards/__main__.py
--rw-r--r--   0        0        0   230192 2023-03-24 03:16:47.335887 bing_rewards-2.0.0/bing_rewards/data/keywords.txt
--rw-r--r--   0        0        0     1799 2023-03-24 03:16:47.335887 bing_rewards-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8147 1970-01-01 00:00:00.000000 bing_rewards-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-09 01:00:57.972184 bing_rewards-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7974 2023-08-09 01:00:57.972184 bing_rewards-2.1.0/README.md
+-rw-r--r--   0        0        0    12313 2023-08-09 01:00:57.976184 bing_rewards-2.1.0/bing_rewards/__init__.py
+-rw-r--r--   0        0        0       38 2023-08-09 01:00:57.976184 bing_rewards-2.1.0/bing_rewards/__main__.py
+-rw-r--r--   0        0        0   230192 2023-08-09 01:00:57.976184 bing_rewards-2.1.0/bing_rewards/data/keywords.txt
+-rw-r--r--   0        0        0     1799 2023-08-09 01:00:57.976184 bing_rewards-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 bing_rewards-2.1.0/PKG-INFO
```

### Comparing `bing_rewards-2.0.0/LICENSE` & `bing_rewards-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bing_rewards-2.0.0/README.md` & `bing_rewards-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 ### A CLI app to perform Bing searches
 Please submit an issue or pull-request if you have an idea for a feature
 
 - [Install](#installation)
 - [Requirements](#requirements)
 - [Usage](#usage)
-- [Config](#config)
+- [Config](#configuration)
 
 ## **Features**
 
-* Script types searche queries into the address bar, so must be run in a GUI environment.
+* Script types search queries into the address bar, so must be run in a GUI environment.
 * Use a mobile user agent to get mobile points (`--mobile`)
 * Configurable number of searches with `--count=`
 * All files are local, makes no http(s) requests
 * Only one external dependance (pynput)
 * Fine tune delay and set browser executable with [config](#configuration) at `$XDG_CONFIG_HOME` or `%APPDATA%` on Windows
 * Best Value: gift cards: **1,050 points / $1** (current rate)
 ***
@@ -41,71 +41,77 @@
 pipx install bing-rewards
 ```
 
 **NEW IN 2.0:** Now using the `pynput` backend with significantly less dependencies than the old `PyAutoGUI`. Delete any old virtual enviroment and reinstall to clean up old depdendencies.
 
 ## **Requirements**
 
-- At least Python 3.7
+- At least Python 3.8
 
 - [pynput](https://github.com/moses-palmer/pynput) package is used to control keypresses and type Bing search URLS.
 WARNING: This script *will* take control away from the keyboard while running. **Pynput** performs key presses. i.e., it does not operate headless or in the background.
 
 - `chrome` must be discoverable on the system PATH. [Download Google Chrome](https://www.google.com/intl/en/chrome/).
 If your chromium based browser has a different name use the `--exe` flag with an absolute path to the browser executable to use (e.g. `--exe=$(which brave-browser)`). Also see the `"browser-path"` key in the [config](#configuration) file.
 
-- To earn points from searching, you must also have logged into [bing.com](https://www.bing.com) with your Microsoft account at least once, to save cookies.
+- To earn points from searching, you *must* also have logged into [bing.com](https://www.bing.com) with your Microsoft account at least once, to save cookies.
 
 ## **Usage**
 
-#### `bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-d | -m]`
+#### `bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-d | -m] [--profile "Profile X"]`
 
 Ex:
 Complete mobile and desktop daily points
 
 `$ bing-rewards`
 
 Run 10 searches with mobile user-agent in a new window
 
 `$ bing-rewards -m -c10`
 
 `$ bing-rewards --mobile --count=10`
 
+Complete mobile and desktop daily points using specified chrome profile "Profile 1"
+
+`$ bing-rewards --profile "Profile 1"`
+
 Launches Chrome as a subprocess with special flags. Tested on Windows 10 and Linux (Ubuntu + Arch), however it should work on Mac OS as well.
 
 ⚠️Known Issue: No other instance of chrome.exe can be open when the script runs. Chrome prevents different user agents in each window. The script will run, but Chrome will not appear as Edge
 
 
 ## **Configuration**
 
 Running with no options will complete mobile and desktop daily search quota.
 The following options are available to change the default behavior.
 Options supplied at execution time override any config.
-| Flag                    | Option                                                                              |
-| ----------------------- | ----------------------------------------------------------------------------------- |
-| `-h`, `--help`          | Display help and exit                                                               |
-| `-c`, `--count=N`       | Override the number of searches to complete                                         |
-| `-d`, `--desktop`       | Only use desktop user agent                                                         |
-| `-m`, `--mobile`        | Only use a mobile user agent                                                        |
-| `-n`, `--dryrun`        | Do everything but type the search query                                             |
-| `--open-rewards`   | Open the rewards page at the end of the run                                         |
-| `-X`, `--no-exit`       | Do not close the browser after completing a search                                  |
-| `--load-delay`     | Override the time given to Chrome to load in seconds                                |
-| `--search-delay`   | Override the time between searches in seconds                                       |
-| `--exe EXE`             | The full path of the Chrome compatible browser executable (Brave and Chrome tested) |
-| `--nowindow`            | Don't open a new Chrome window, just type the keys                                  |
+| Flag                    | Option                                                                                |
+| ----------------------- | --------------------------------------------------------------------------------------|
+| `-h`, `--help`          | Display help and exit                                                                 |
+| `-c`, `--count=N`       | Override the number of searches to complete                                           |
+| `-d`, `--desktop`       | Only use desktop user agent                                                           |
+| `-m`, `--mobile`        | Only use a mobile user agent                                                          |
+| `-n`, `--dryrun`        | Do everything but type the search query                                               |
+| `--open-rewards`        | Open the rewards page at the end of the run                                           |
+| `-X`, `--no-exit`       | Do not close the browser after completing a search                                    |
+| `--load-delay`          | Override the time given to Chrome to load in seconds                                  |
+| `--search-delay`        | Override the time between searches in seconds                                         |
+| `--exe EXE`             | The full path of the Chrome compatible browser executable (Brave and Chrome tested)   |
+| `--nowindow`            | Don't open a new Chrome window, just type the keys                                    |
+| `--profile "Profile N"` | Launches chrome using the specified profile. Otherwise use default.                   |
+| `--ime`                 | Triggers Windows IME to switch to English input by pressing "shift"                   |
 
 A config file is also generated in $XDG_CONFIG_HOME or %APPDATA% on Windows
 where precise delay modifications can be made.
 
 Example config `~/.config/bing-rewards/config.json`
 ```json
 {
-    "desktop-count": 34,
-    "mobile-count": 40,
+    "desktop-count": 30,
+    "mobile-count": 20,
     "load-delay": 1.5,
     "search-delay": 2,
     "search-url": "https://www.bing.com/search?q=",
     "desktop-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37",
     "mobile-agent": "Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Mobile Safari/537.36 Edge/18.19041",
     "browser-path": "C:\\Program Files (x86)\\BraveSoftware\\Brave-Browser\\Application\\brave.exe"
 }
@@ -126,7 +132,28 @@
 
 ## Words:
 The [keywords](https://www.myhelpfulguides.com/keywords.txt) included in this repo where taken from this site
 https://www.myhelpfulguides.com/2018/07/19/bing-rewards-auto-searcher-with-python-3/.
 
 This script provided the original inspiration but has since been complelty rewritten and expanded.
 The original author was contacted for the original source of keywords, but declined to respond
+
+## Development
+
+This project uses [Poetry](https://python-poetry.org) for dependency management and packaging.
+
+The easiest way to install python apps is with [pipx](https://pypa.github.io/pipx/)
+
+```
+# Install pipx
+pip install pipx
+# Install poetry
+pipx install poetry
+```
+
+Then, fork the repo, clone and install the dependencies with `poetry install`.
+
+Install the defined pre-commit hooks: `poetry run pre-commit install`
+
+Activate the virtualenv: `poetry shell`
+
+Feel free to open a PR with additional features or fixes
```

#### html2text {}

```diff
@@ -1,76 +1,87 @@
 # Bing-Rewards
               [PyPI - Python Version] [PyPi] [PyPI_-_Downloads]
                          [PyPI - License] [Formatting]
 ### A CLI app to perform Bing searches Please submit an issue or pull-request
 if you have an idea for a feature - [Install](#installation) - [Requirements]
-(#requirements) - [Usage](#usage) - [Config](#config) ## **Features** * Script
-types searche queries into the address bar, so must be run in a GUI
+(#requirements) - [Usage](#usage) - [Config](#configuration) ## **Features** *
+Script types search queries into the address bar, so must be run in a GUI
 environment. * Use a mobile user agent to get mobile points (`--mobile`) *
 Configurable number of searches with `--count=` * All files are local, makes no
 http(s) requests * Only one external dependance (pynput) * Fine tune delay and
 set browser executable with [config](#configuration) at `$XDG_CONFIG_HOME` or
 `%APPDATA%` on Windows * Best Value: gift cards: **1,050 points / $1** (current
 rate) *** ## **Installation** ```bash pip install bing-rewards ``` Will make
 the executable `bing-rewards` available on your PATH. Look below or try the `--
 help` flag to see detailed usage. **Recommended**: Use a virtual environment or
 [`pipx`](https://pypa.github.io/pipx/) to avoid poluting your global package
 path with executable apps. See: [pipx](https://pypa.github.io/pipx/) ```bash
 pipx install bing-rewards ``` **NEW IN 2.0:** Now using the `pynput` backend
 with significantly less dependencies than the old `PyAutoGUI`. Delete any old
 virtual enviroment and reinstall to clean up old depdendencies. ##
-**Requirements** - At least Python 3.7 - [pynput](https://github.com/moses-
+**Requirements** - At least Python 3.8 - [pynput](https://github.com/moses-
 palmer/pynput) package is used to control keypresses and type Bing search URLS.
 WARNING: This script *will* take control away from the keyboard while running.
 **Pynput** performs key presses. i.e., it does not operate headless or in the
 background. - `chrome` must be discoverable on the system PATH. [Download
 Google Chrome](https://www.google.com/intl/en/chrome/). If your chromium based
 browser has a different name use the `--exe` flag with an absolute path to the
 browser executable to use (e.g. `--exe=$(which brave-browser)`). Also see the
 `"browser-path"` key in the [config](#configuration) file. - To earn points
-from searching, you must also have logged into [bing.com](https://www.bing.com)
-with your Microsoft account at least once, to save cookies. ## **Usage** ####
-`bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-d | -m]` Ex:
-Complete mobile and desktop daily points `$ bing-rewards` Run 10 searches with
-mobile user-agent in a new window `$ bing-rewards -m -c10` `$ bing-rewards --
-mobile --count=10` Launches Chrome as a subprocess with special flags. Tested
-on Windows 10 and Linux (Ubuntu + Arch), however it should work on Mac OS as
-well. â ï¸Known Issue: No other instance of chrome.exe can be open when the
-script runs. Chrome prevents different user agents in each window. The script
-will run, but Chrome will not appear as Edge ## **Configuration** Running with
-no options will complete mobile and desktop daily search quota. The following
-options are available to change the default behavior. Options supplied at
-execution time override any config. | Flag | Option | | ----------------------
-- | ---------------------------------------------------------------------------
--------- | | `-h`, `--help` | Display help and exit | | `-c`, `--count=N` |
-Override the number of searches to complete | | `-d`, `--desktop` | Only use
-desktop user agent | | `-m`, `--mobile` | Only use a mobile user agent | | `-
-n`, `--dryrun` | Do everything but type the search query | | `--open-rewards` |
-Open the rewards page at the end of the run | | `-X`, `--no-exit` | Do not
-close the browser after completing a search | | `--load-delay` | Override the
-time given to Chrome to load in seconds | | `--search-delay` | Override the
-time between searches in seconds | | `--exe EXE` | The full path of the Chrome
-compatible browser executable (Brave and Chrome tested) | | `--nowindow` |
-Don't open a new Chrome window, just type the keys | A config file is also
-generated in $XDG_CONFIG_HOME or %APPDATA% on Windows where precise delay
-modifications can be made. Example config `~/.config/bing-rewards/config.json`
-```json { "desktop-count": 34, "mobile-count": 40, "load-delay": 1.5, "search-
-delay": 2, "search-url": "https://www.bing.com/search?q=", "desktop-agent":
-"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37", "mobile-agent":
-"Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1) AppleWebKit/537.36 (KHTML,
-like Gecko) Chrome/70.0.3538.102 Mobile Safari/537.36 Edge/18.19041", "browser-
-path": "C:\\Program Files (x86)\\BraveSoftware\\Brave-
-Browser\\Application\\brave.exe" } ``` Delay timings are in seconds ## User
-agents If interested, the following user agents are passed to Chrome using the
-`--user-agent` argument. These are clearly defined at the top of `bing-
-rewards.py`. Edge Browser on Windows 10 desktop: > Mozilla/5.0 (Windows NT
-10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61
-Safari/537.36 Edg/83.0.478.37 Mobile Edge Browser on Windows 10 phone: >
-Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/70.0.3538.102 Mobile Safari/537.36 Edge/18.19041 *** ## Words:
-The [keywords](https://www.myhelpfulguides.com/keywords.txt) included in this
-repo where taken from this site https://www.myhelpfulguides.com/2018/07/19/
-bing-rewards-auto-searcher-with-python-3/. This script provided the original
-inspiration but has since been complelty rewritten and expanded. The original
-author was contacted for the original source of keywords, but declined to
-respond
+from searching, you *must* also have logged into [bing.com](https://
+www.bing.com) with your Microsoft account at least once, to save cookies. ##
+**Usage** #### `bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-
+d | -m] [--profile "Profile X"]` Ex: Complete mobile and desktop daily points
+`$ bing-rewards` Run 10 searches with mobile user-agent in a new window `$
+bing-rewards -m -c10` `$ bing-rewards --mobile --count=10` Complete mobile and
+desktop daily points using specified chrome profile "Profile 1" `$ bing-rewards
+--profile "Profile 1"` Launches Chrome as a subprocess with special flags.
+Tested on Windows 10 and Linux (Ubuntu + Arch), however it should work on Mac
+OS as well. â ï¸Known Issue: No other instance of chrome.exe can be open when
+the script runs. Chrome prevents different user agents in each window. The
+script will run, but Chrome will not appear as Edge ## **Configuration**
+Running with no options will complete mobile and desktop daily search quota.
+The following options are available to change the default behavior. Options
+supplied at execution time override any config. | Flag | Option | | -----------
+------------ | ----------------------------------------------------------------
+----------------------| | `-h`, `--help` | Display help and exit | | `-c`, `--
+count=N` | Override the number of searches to complete | | `-d`, `--desktop` |
+Only use desktop user agent | | `-m`, `--mobile` | Only use a mobile user agent
+| | `-n`, `--dryrun` | Do everything but type the search query | | `--open-
+rewards` | Open the rewards page at the end of the run | | `-X`, `--no-exit` |
+Do not close the browser after completing a search | | `--load-delay` |
+Override the time given to Chrome to load in seconds | | `--search-delay` |
+Override the time between searches in seconds | | `--exe EXE` | The full path
+of the Chrome compatible browser executable (Brave and Chrome tested) | | `--
+nowindow` | Don't open a new Chrome window, just type the keys | | `--profile
+"Profile N"` | Launches chrome using the specified profile. Otherwise use
+default. | | `--ime` | Triggers Windows IME to switch to English input by
+pressing "shift" | A config file is also generated in $XDG_CONFIG_HOME or
+%APPDATA% on Windows where precise delay modifications can be made. Example
+config `~/.config/bing-rewards/config.json` ```json { "desktop-count": 30,
+"mobile-count": 20, "load-delay": 1.5, "search-delay": 2, "search-url": "https:
+//www.bing.com/search?q=", "desktop-agent": "Mozilla/5.0 (Windows NT 10.0;
+Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/
+537.36 Edg/83.0.478.37", "mobile-agent": "Mozilla/5.0 (Windows Phone 10.0;
+Android 6.0.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102
+Mobile Safari/537.36 Edge/18.19041", "browser-path": "C:\\Program Files
+(x86)\\BraveSoftware\\Brave-Browser\\Application\\brave.exe" } ``` Delay
+timings are in seconds ## User agents If interested, the following user agents
+are passed to Chrome using the `--user-agent` argument. These are clearly
+defined at the top of `bing-rewards.py`. Edge Browser on Windows 10 desktop: >
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like
+Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37 Mobile Edge Browser on
+Windows 10 phone: > Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1)
+AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Mobile Safari/
+537.36 Edge/18.19041 *** ## Words: The [keywords](https://
+www.myhelpfulguides.com/keywords.txt) included in this repo where taken from
+this site https://www.myhelpfulguides.com/2018/07/19/bing-rewards-auto-
+searcher-with-python-3/. This script provided the original inspiration but has
+since been complelty rewritten and expanded. The original author was contacted
+for the original source of keywords, but declined to respond ## Development
+This project uses [Poetry](https://python-poetry.org) for dependency management
+and packaging. The easiest way to install python apps is with [pipx](https://
+pypa.github.io/pipx/) ``` # Install pipx pip install pipx # Install poetry pipx
+install poetry ``` Then, fork the repo, clone and install the dependencies with
+`poetry install`. Install the defined pre-commit hooks: `poetry run pre-commit
+install` Activate the virtualenv: `poetry shell` Feel free to open a PR with
+additional features or fixes
```

### Comparing `bing_rewards-2.0.0/bing_rewards/__init__.py` & `bing_rewards-2.1.0/bing_rewards/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,14 +160,24 @@
     )
     p.add_argument(
         "-X",
         "--no-exit",
         help="Don't close the browser window after searching",
         action="store_true",
     )
+    p.add_argument(
+        "--profile",
+        help="Sets the chrome profile for launch",
+        type=str,
+    )
+    p.add_argument(
+        "--ime",
+        help="Triggers windows IME to switch to english by pressing SHIFT",
+        action="store_true",
+    )
     return p.parse_args()
 
 
 def parse_config(default_config: Dict) -> Dict:
     # Config file in .config or APPDATA on Windows
     config_home = Path(
         os.environ.get("APPDATA")
@@ -203,23 +213,28 @@
     """
     minimum_version = (3, 6)
     assert (
         sys.version_info >= minimum_version
     ), "Only Python {}.{} and above is supported.".format(*minimum_version)
 
 
-def browser_cmd(exe: Path | None, agent: str) -> List[str]:
+def browser_cmd(exe: Path | None, agent: str, profile: str | None = None) -> List[str]:
     """
     Generate command to open Google Chrome with user-agent `agent`
     """
     if exe is not None:
         browser = str(exe)
     else:
         browser = "chrome"
-    return [browser, "--new-window", f'--user-agent="{agent}"']
+    cmd = [browser, "--new-window", f'--user-agent="{agent}"']
+    # Switch to non default profile if supplied with valid string
+    # NO CHECKING IS DONE if the profile exists
+    if profile is not None:
+        cmd.extend(["--profile-directory=" + profile])
+    return cmd
 
 
 def get_words_gen() -> Generator:
     while True:
         # Wrapped in an infinite loop to support circular reading of the file
         with KEYWORDS.open(mode="r", encoding="utf8") as fh:
             fh.seek(0, SEEK_END)
@@ -240,22 +255,30 @@
     """
     try:
         # Open Chrome as a subprocess
         # Only if a new window should be opened
         if not args.no_window and not args.dryrun:
             if os.name == "posix":
                 chrome = subprocess.Popen(
-                    browser_cmd(args.exe or config.get("browser-path") or None, agent),
+                    browser_cmd(
+                        args.exe or config.get("browser-path") or None,
+                        agent,
+                        args.profile,
+                    ),
                     stderr=subprocess.DEVNULL,
                     stdout=subprocess.DEVNULL,
                     preexec_fn=os.setsid,
                 )
             else:
                 chrome = subprocess.Popen(
-                    browser_cmd(args.exe or config.get("browser-path") or None, agent),
+                    browser_cmd(
+                        args.exe or config.get("browser-path") or None,
+                        agent,
+                        args.profile,
+                    ),
                 )
             print(f"Opening browser with pid {chrome.pid}")
     except FileNotFoundError as e:
         print("Unexpected error:", e)
         print(
             "ERROR: Chrome could not be found on system PATH\n"
             "Make sure it is installed and added to PATH,"
@@ -278,14 +301,19 @@
         # Use pynput to trigger keyboard events and type search querys
         if not args.dryrun:
             # Alt + D to focus the address bar in most browsers
             key_controller.press(Key.alt)
             key_controller.press("d")
             key_controller.release("d")
             key_controller.release(Key.alt)
+
+            if args.ime:
+                # Incase users use a Windows IME, change the language to English
+                # Issue #35
+                key_controller.tap(Key.shift)
             time.sleep(0.08)
 
             # Type the url into the address bar
             # This is very fast and hopefully reliable
             key_controller.type(search_url + "\n")
 
         print(f"Search {i+1}: {query}")
@@ -314,15 +342,14 @@
     check_python_version()
     config = parse_config(SETTINGS)
     args = parse_args()
     # Removed. Dry run now respects set delay times
     # if args.dryrun:
     #     config["search-delay"] = 0
     #     config["load-delay"] = 0
-
     words_gen = get_words_gen()
 
     def desktop():
         # Complete search with desktop settings
         count = args.count or config.get("desktop-count") or DESKTOP_COUNT
         print(f"Doing {count} desktop searches")
```

### Comparing `bing_rewards-2.0.0/bing_rewards/data/keywords.txt` & `bing_rewards-2.1.0/bing_rewards/data/keywords.txt`

 * *Files identical despite different names*

### Comparing `bing_rewards-2.0.0/pyproject.toml` & `bing_rewards-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bing-rewards"
-version = "2.0.0"
+version = "2.1.0"
 description = "Perform automated Bing Rewards searches"
 authors = ["jack-mil <62065280+jack-mil@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jack-mil/bing-rewards"
 repository = "https://github.com/jack-mil/bing-rewards"
 keywords = ["automation", "bing", "search", "pyautogui", "points", "xbox"]
```

### Comparing `bing_rewards-2.0.0/PKG-INFO` & `bing_rewards-2.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bing-rewards
-Version: 2.0.0
+Version: 2.1.0
 Summary: Perform automated Bing Rewards searches
 Home-page: https://github.com/jack-mil/bing-rewards
 License: MIT
 Keywords: automation,bing,search,pyautogui,points,xbox
 Author: jack-mil
 Author-email: 62065280+jack-mil@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -39,19 +39,19 @@
 
 ### A CLI app to perform Bing searches
 Please submit an issue or pull-request if you have an idea for a feature
 
 - [Install](#installation)
 - [Requirements](#requirements)
 - [Usage](#usage)
-- [Config](#config)
+- [Config](#configuration)
 
 ## **Features**
 
-* Script types searche queries into the address bar, so must be run in a GUI environment.
+* Script types search queries into the address bar, so must be run in a GUI environment.
 * Use a mobile user agent to get mobile points (`--mobile`)
 * Configurable number of searches with `--count=`
 * All files are local, makes no http(s) requests
 * Only one external dependance (pynput)
 * Fine tune delay and set browser executable with [config](#configuration) at `$XDG_CONFIG_HOME` or `%APPDATA%` on Windows
 * Best Value: gift cards: **1,050 points / $1** (current rate)
 ***
@@ -68,71 +68,77 @@
 pipx install bing-rewards
 ```
 
 **NEW IN 2.0:** Now using the `pynput` backend with significantly less dependencies than the old `PyAutoGUI`. Delete any old virtual enviroment and reinstall to clean up old depdendencies.
 
 ## **Requirements**
 
-- At least Python 3.7
+- At least Python 3.8
 
 - [pynput](https://github.com/moses-palmer/pynput) package is used to control keypresses and type Bing search URLS.
 WARNING: This script *will* take control away from the keyboard while running. **Pynput** performs key presses. i.e., it does not operate headless or in the background.
 
 - `chrome` must be discoverable on the system PATH. [Download Google Chrome](https://www.google.com/intl/en/chrome/).
 If your chromium based browser has a different name use the `--exe` flag with an absolute path to the browser executable to use (e.g. `--exe=$(which brave-browser)`). Also see the `"browser-path"` key in the [config](#configuration) file.
 
-- To earn points from searching, you must also have logged into [bing.com](https://www.bing.com) with your Microsoft account at least once, to save cookies.
+- To earn points from searching, you *must* also have logged into [bing.com](https://www.bing.com) with your Microsoft account at least once, to save cookies.
 
 ## **Usage**
 
-#### `bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-d | -m]`
+#### `bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-d | -m] [--profile "Profile X"]`
 
 Ex:
 Complete mobile and desktop daily points
 
 `$ bing-rewards`
 
 Run 10 searches with mobile user-agent in a new window
 
 `$ bing-rewards -m -c10`
 
 `$ bing-rewards --mobile --count=10`
 
+Complete mobile and desktop daily points using specified chrome profile "Profile 1"
+
+`$ bing-rewards --profile "Profile 1"`
+
 Launches Chrome as a subprocess with special flags. Tested on Windows 10 and Linux (Ubuntu + Arch), however it should work on Mac OS as well.
 
 ⚠️Known Issue: No other instance of chrome.exe can be open when the script runs. Chrome prevents different user agents in each window. The script will run, but Chrome will not appear as Edge
 
 
 ## **Configuration**
 
 Running with no options will complete mobile and desktop daily search quota.
 The following options are available to change the default behavior.
 Options supplied at execution time override any config.
-| Flag                    | Option                                                                              |
-| ----------------------- | ----------------------------------------------------------------------------------- |
-| `-h`, `--help`          | Display help and exit                                                               |
-| `-c`, `--count=N`       | Override the number of searches to complete                                         |
-| `-d`, `--desktop`       | Only use desktop user agent                                                         |
-| `-m`, `--mobile`        | Only use a mobile user agent                                                        |
-| `-n`, `--dryrun`        | Do everything but type the search query                                             |
-| `--open-rewards`   | Open the rewards page at the end of the run                                         |
-| `-X`, `--no-exit`       | Do not close the browser after completing a search                                  |
-| `--load-delay`     | Override the time given to Chrome to load in seconds                                |
-| `--search-delay`   | Override the time between searches in seconds                                       |
-| `--exe EXE`             | The full path of the Chrome compatible browser executable (Brave and Chrome tested) |
-| `--nowindow`            | Don't open a new Chrome window, just type the keys                                  |
+| Flag                    | Option                                                                                |
+| ----------------------- | --------------------------------------------------------------------------------------|
+| `-h`, `--help`          | Display help and exit                                                                 |
+| `-c`, `--count=N`       | Override the number of searches to complete                                           |
+| `-d`, `--desktop`       | Only use desktop user agent                                                           |
+| `-m`, `--mobile`        | Only use a mobile user agent                                                          |
+| `-n`, `--dryrun`        | Do everything but type the search query                                               |
+| `--open-rewards`        | Open the rewards page at the end of the run                                           |
+| `-X`, `--no-exit`       | Do not close the browser after completing a search                                    |
+| `--load-delay`          | Override the time given to Chrome to load in seconds                                  |
+| `--search-delay`        | Override the time between searches in seconds                                         |
+| `--exe EXE`             | The full path of the Chrome compatible browser executable (Brave and Chrome tested)   |
+| `--nowindow`            | Don't open a new Chrome window, just type the keys                                    |
+| `--profile "Profile N"` | Launches chrome using the specified profile. Otherwise use default.                   |
+| `--ime`                 | Triggers Windows IME to switch to English input by pressing "shift"                   |
 
 A config file is also generated in $XDG_CONFIG_HOME or %APPDATA% on Windows
 where precise delay modifications can be made.
 
 Example config `~/.config/bing-rewards/config.json`
 ```json
 {
-    "desktop-count": 34,
-    "mobile-count": 40,
+    "desktop-count": 30,
+    "mobile-count": 20,
     "load-delay": 1.5,
     "search-delay": 2,
     "search-url": "https://www.bing.com/search?q=",
     "desktop-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37",
     "mobile-agent": "Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Mobile Safari/537.36 Edge/18.19041",
     "browser-path": "C:\\Program Files (x86)\\BraveSoftware\\Brave-Browser\\Application\\brave.exe"
 }
@@ -154,7 +160,28 @@
 ## Words:
 The [keywords](https://www.myhelpfulguides.com/keywords.txt) included in this repo where taken from this site
 https://www.myhelpfulguides.com/2018/07/19/bing-rewards-auto-searcher-with-python-3/.
 
 This script provided the original inspiration but has since been complelty rewritten and expanded.
 The original author was contacted for the original source of keywords, but declined to respond
 
+## Development
+
+This project uses [Poetry](https://python-poetry.org) for dependency management and packaging.
+
+The easiest way to install python apps is with [pipx](https://pypa.github.io/pipx/)
+
+```
+# Install pipx
+pip install pipx
+# Install poetry
+pipx install poetry
+```
+
+Then, fork the repo, clone and install the dependencies with `poetry install`.
+
+Install the defined pre-commit hooks: `poetry run pre-commit install`
+
+Activate the virtualenv: `poetry shell`
+
+Feel free to open a PR with additional features or fixes
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bing-rewards Version: 2.0.0 Summary: Perform
+Metadata-Version: 2.1 Name: bing-rewards Version: 2.1.0 Summary: Perform
 automated Bing Rewards searches Home-page: https://github.com/jack-mil/bing-
 rewards License: MIT Keywords: automation,bing,search,pyautogui,points,xbox
 Author: jack-mil Author-email: 62065280+jack-mil@users.noreply.github.com
 Requires-Python: >=3.8,<4.0 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: Microsoft :: Windows Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
@@ -13,78 +13,89 @@
 Requires-Dist: pynput (>=1,<2) Project-URL: Issue Tracker, https://github.com/
 jack-mil/bing-rewards/issues Project-URL: Repository, https://github.com/jack-
 mil/bing-rewards Description-Content-Type: text/markdown # Bing-Rewards
               [PyPI - Python Version] [PyPi] [PyPI_-_Downloads]
                          [PyPI - License] [Formatting]
 ### A CLI app to perform Bing searches Please submit an issue or pull-request
 if you have an idea for a feature - [Install](#installation) - [Requirements]
-(#requirements) - [Usage](#usage) - [Config](#config) ## **Features** * Script
-types searche queries into the address bar, so must be run in a GUI
+(#requirements) - [Usage](#usage) - [Config](#configuration) ## **Features** *
+Script types search queries into the address bar, so must be run in a GUI
 environment. * Use a mobile user agent to get mobile points (`--mobile`) *
 Configurable number of searches with `--count=` * All files are local, makes no
 http(s) requests * Only one external dependance (pynput) * Fine tune delay and
 set browser executable with [config](#configuration) at `$XDG_CONFIG_HOME` or
 `%APPDATA%` on Windows * Best Value: gift cards: **1,050 points / $1** (current
 rate) *** ## **Installation** ```bash pip install bing-rewards ``` Will make
 the executable `bing-rewards` available on your PATH. Look below or try the `--
 help` flag to see detailed usage. **Recommended**: Use a virtual environment or
 [`pipx`](https://pypa.github.io/pipx/) to avoid poluting your global package
 path with executable apps. See: [pipx](https://pypa.github.io/pipx/) ```bash
 pipx install bing-rewards ``` **NEW IN 2.0:** Now using the `pynput` backend
 with significantly less dependencies than the old `PyAutoGUI`. Delete any old
 virtual enviroment and reinstall to clean up old depdendencies. ##
-**Requirements** - At least Python 3.7 - [pynput](https://github.com/moses-
+**Requirements** - At least Python 3.8 - [pynput](https://github.com/moses-
 palmer/pynput) package is used to control keypresses and type Bing search URLS.
 WARNING: This script *will* take control away from the keyboard while running.
 **Pynput** performs key presses. i.e., it does not operate headless or in the
 background. - `chrome` must be discoverable on the system PATH. [Download
 Google Chrome](https://www.google.com/intl/en/chrome/). If your chromium based
 browser has a different name use the `--exe` flag with an absolute path to the
 browser executable to use (e.g. `--exe=$(which brave-browser)`). Also see the
 `"browser-path"` key in the [config](#configuration) file. - To earn points
-from searching, you must also have logged into [bing.com](https://www.bing.com)
-with your Microsoft account at least once, to save cookies. ## **Usage** ####
-`bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-d | -m]` Ex:
-Complete mobile and desktop daily points `$ bing-rewards` Run 10 searches with
-mobile user-agent in a new window `$ bing-rewards -m -c10` `$ bing-rewards --
-mobile --count=10` Launches Chrome as a subprocess with special flags. Tested
-on Windows 10 and Linux (Ubuntu + Arch), however it should work on Mac OS as
-well. â ï¸Known Issue: No other instance of chrome.exe can be open when the
-script runs. Chrome prevents different user agents in each window. The script
-will run, but Chrome will not appear as Edge ## **Configuration** Running with
-no options will complete mobile and desktop daily search quota. The following
-options are available to change the default behavior. Options supplied at
-execution time override any config. | Flag | Option | | ----------------------
-- | ---------------------------------------------------------------------------
--------- | | `-h`, `--help` | Display help and exit | | `-c`, `--count=N` |
-Override the number of searches to complete | | `-d`, `--desktop` | Only use
-desktop user agent | | `-m`, `--mobile` | Only use a mobile user agent | | `-
-n`, `--dryrun` | Do everything but type the search query | | `--open-rewards` |
-Open the rewards page at the end of the run | | `-X`, `--no-exit` | Do not
-close the browser after completing a search | | `--load-delay` | Override the
-time given to Chrome to load in seconds | | `--search-delay` | Override the
-time between searches in seconds | | `--exe EXE` | The full path of the Chrome
-compatible browser executable (Brave and Chrome tested) | | `--nowindow` |
-Don't open a new Chrome window, just type the keys | A config file is also
-generated in $XDG_CONFIG_HOME or %APPDATA% on Windows where precise delay
-modifications can be made. Example config `~/.config/bing-rewards/config.json`
-```json { "desktop-count": 34, "mobile-count": 40, "load-delay": 1.5, "search-
-delay": 2, "search-url": "https://www.bing.com/search?q=", "desktop-agent":
-"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37", "mobile-agent":
-"Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1) AppleWebKit/537.36 (KHTML,
-like Gecko) Chrome/70.0.3538.102 Mobile Safari/537.36 Edge/18.19041", "browser-
-path": "C:\\Program Files (x86)\\BraveSoftware\\Brave-
-Browser\\Application\\brave.exe" } ``` Delay timings are in seconds ## User
-agents If interested, the following user agents are passed to Chrome using the
-`--user-agent` argument. These are clearly defined at the top of `bing-
-rewards.py`. Edge Browser on Windows 10 desktop: > Mozilla/5.0 (Windows NT
-10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61
-Safari/537.36 Edg/83.0.478.37 Mobile Edge Browser on Windows 10 phone: >
-Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/70.0.3538.102 Mobile Safari/537.36 Edge/18.19041 *** ## Words:
-The [keywords](https://www.myhelpfulguides.com/keywords.txt) included in this
-repo where taken from this site https://www.myhelpfulguides.com/2018/07/19/
-bing-rewards-auto-searcher-with-python-3/. This script provided the original
-inspiration but has since been complelty rewritten and expanded. The original
-author was contacted for the original source of keywords, but declined to
-respond
+from searching, you *must* also have logged into [bing.com](https://
+www.bing.com) with your Microsoft account at least once, to save cookies. ##
+**Usage** #### `bing-rewards [-h] [--no-window] [-n] [--exe EXE] [-c COUNT] [-
+d | -m] [--profile "Profile X"]` Ex: Complete mobile and desktop daily points
+`$ bing-rewards` Run 10 searches with mobile user-agent in a new window `$
+bing-rewards -m -c10` `$ bing-rewards --mobile --count=10` Complete mobile and
+desktop daily points using specified chrome profile "Profile 1" `$ bing-rewards
+--profile "Profile 1"` Launches Chrome as a subprocess with special flags.
+Tested on Windows 10 and Linux (Ubuntu + Arch), however it should work on Mac
+OS as well. â ï¸Known Issue: No other instance of chrome.exe can be open when
+the script runs. Chrome prevents different user agents in each window. The
+script will run, but Chrome will not appear as Edge ## **Configuration**
+Running with no options will complete mobile and desktop daily search quota.
+The following options are available to change the default behavior. Options
+supplied at execution time override any config. | Flag | Option | | -----------
+------------ | ----------------------------------------------------------------
+----------------------| | `-h`, `--help` | Display help and exit | | `-c`, `--
+count=N` | Override the number of searches to complete | | `-d`, `--desktop` |
+Only use desktop user agent | | `-m`, `--mobile` | Only use a mobile user agent
+| | `-n`, `--dryrun` | Do everything but type the search query | | `--open-
+rewards` | Open the rewards page at the end of the run | | `-X`, `--no-exit` |
+Do not close the browser after completing a search | | `--load-delay` |
+Override the time given to Chrome to load in seconds | | `--search-delay` |
+Override the time between searches in seconds | | `--exe EXE` | The full path
+of the Chrome compatible browser executable (Brave and Chrome tested) | | `--
+nowindow` | Don't open a new Chrome window, just type the keys | | `--profile
+"Profile N"` | Launches chrome using the specified profile. Otherwise use
+default. | | `--ime` | Triggers Windows IME to switch to English input by
+pressing "shift" | A config file is also generated in $XDG_CONFIG_HOME or
+%APPDATA% on Windows where precise delay modifications can be made. Example
+config `~/.config/bing-rewards/config.json` ```json { "desktop-count": 30,
+"mobile-count": 20, "load-delay": 1.5, "search-delay": 2, "search-url": "https:
+//www.bing.com/search?q=", "desktop-agent": "Mozilla/5.0 (Windows NT 10.0;
+Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.61 Safari/
+537.36 Edg/83.0.478.37", "mobile-agent": "Mozilla/5.0 (Windows Phone 10.0;
+Android 6.0.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102
+Mobile Safari/537.36 Edge/18.19041", "browser-path": "C:\\Program Files
+(x86)\\BraveSoftware\\Brave-Browser\\Application\\brave.exe" } ``` Delay
+timings are in seconds ## User agents If interested, the following user agents
+are passed to Chrome using the `--user-agent` argument. These are clearly
+defined at the top of `bing-rewards.py`. Edge Browser on Windows 10 desktop: >
+Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like
+Gecko) Chrome/83.0.4103.61 Safari/537.36 Edg/83.0.478.37 Mobile Edge Browser on
+Windows 10 phone: > Mozilla/5.0 (Windows Phone 10.0; Android 6.0.1)
+AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Mobile Safari/
+537.36 Edge/18.19041 *** ## Words: The [keywords](https://
+www.myhelpfulguides.com/keywords.txt) included in this repo where taken from
+this site https://www.myhelpfulguides.com/2018/07/19/bing-rewards-auto-
+searcher-with-python-3/. This script provided the original inspiration but has
+since been complelty rewritten and expanded. The original author was contacted
+for the original source of keywords, but declined to respond ## Development
+This project uses [Poetry](https://python-poetry.org) for dependency management
+and packaging. The easiest way to install python apps is with [pipx](https://
+pypa.github.io/pipx/) ``` # Install pipx pip install pipx # Install poetry pipx
+install poetry ``` Then, fork the repo, clone and install the dependencies with
+`poetry install`. Install the defined pre-commit hooks: `poetry run pre-commit
+install` Activate the virtualenv: `poetry shell` Feel free to open a PR with
+additional features or fixes
```


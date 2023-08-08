# Comparing `tmp/i8kgui-0.8.4.tar.gz` & `tmp/i8kgui-0.8.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i8kgui-0.8.4.tar", last modified: Tue Aug  8 21:52:00 2023, max compression
+gzip compressed data, was "i8kgui-0.8.4.dev0.tar", last modified: Fri Jun  9 01:50:00 2023, max compression
```

## Comparing `i8kgui-0.8.4.tar` & `i8kgui-0.8.4.dev0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.294040 i8kgui-0.8.4/
--rw-rw-r--   0 demon     (1000) demon     (1000)    35149 2023-06-07 13:27:26.000000 i8kgui-0.8.4/LICENSE
--rw-rw-r--   0 demon     (1000) demon     (1000)     9347 2023-08-08 21:52:00.294040 i8kgui-0.8.4/PKG-INFO
--rw-rw-r--   0 demon     (1000) demon     (1000)     9026 2023-08-08 20:13:45.000000 i8kgui-0.8.4/README.md
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.294040 i8kgui-0.8.4/i8kgui/
--rw-rw-r--   0 demon     (1000) demon     (1000)        0 2023-06-07 13:27:26.000000 i8kgui-0.8.4/i8kgui/__init__.py
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.294040 i8kgui-0.8.4/i8kgui/desktop/
--rw-rw-r--   0 demon     (1000) demon     (1000)      114 2023-06-07 13:27:26.000000 i8kgui-0.8.4/i8kgui/desktop/i8kgui.desktop
--rwxrwxr-x   0 demon     (1000) demon     (1000)    90241 2023-08-08 18:55:11.000000 i8kgui-0.8.4/i8kgui/i8kgui
--rwxrwxr-x   0 demon     (1000) demon     (1000)     2832 2023-06-08 09:38:16.000000 i8kgui-0.8.4/i8kgui/i8kgui_thermal_control
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.294040 i8kgui-0.8.4/i8kgui/icons/
--rw-rw-r--   0 demon     (1000) demon     (1000)    24084 2023-06-07 13:27:26.000000 i8kgui-0.8.4/i8kgui/icons/i8kgui_icon.png
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.290040 i8kgui-0.8.4/i8kgui/polkit_actions/
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.294040 i8kgui-0.8.4/i8kgui/polkit_actions/ubuntu/
--rw-rw-r--   0 demon     (1000) demon     (1000)      777 2023-08-08 21:10:26.000000 i8kgui-0.8.4/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy
--rw-rw-r--   0 demon     (1000) demon     (1000)      747 2023-06-08 09:38:16.000000 i8kgui-0.8.4/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.smbios-thermal-ctl.policy
-drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-08-08 21:52:00.294040 i8kgui-0.8.4/i8kgui.egg-info/
--rw-rw-r--   0 demon     (1000) demon     (1000)     9347 2023-08-08 21:52:00.000000 i8kgui-0.8.4/i8kgui.egg-info/PKG-INFO
--rw-rw-r--   0 demon     (1000) demon     (1000)      462 2023-08-08 21:52:00.000000 i8kgui-0.8.4/i8kgui.egg-info/SOURCES.txt
--rw-rw-r--   0 demon     (1000) demon     (1000)        1 2023-08-08 21:52:00.000000 i8kgui-0.8.4/i8kgui.egg-info/dependency_links.txt
--rw-rw-r--   0 demon     (1000) demon     (1000)       26 2023-08-08 21:52:00.000000 i8kgui-0.8.4/i8kgui.egg-info/requires.txt
--rw-rw-r--   0 demon     (1000) demon     (1000)        7 2023-08-08 21:52:00.000000 i8kgui-0.8.4/i8kgui.egg-info/top_level.txt
--rw-rw-r--   0 demon     (1000) demon     (1000)       87 2023-06-09 00:12:39.000000 i8kgui-0.8.4/pyproject.toml
--rw-rw-r--   0 demon     (1000) demon     (1000)       38 2023-08-08 21:52:00.294040 i8kgui-0.8.4/setup.cfg
--rw-rw-r--   0 demon     (1000) demon     (1000)     1216 2023-08-08 20:01:15.000000 i8kgui-0.8.4/setup.py
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/
+-rw-rw-r--   0 demon     (1000) demon     (1000)    35149 2023-06-07 13:27:26.000000 i8kgui-0.8.4.dev0/LICENSE
+-rw-rw-r--   0 demon     (1000) demon     (1000)     8698 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/PKG-INFO
+-rw-rw-r--   0 demon     (1000) demon     (1000)     8372 2023-06-09 01:43:10.000000 i8kgui-0.8.4.dev0/README.md
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/i8kgui/
+-rw-rw-r--   0 demon     (1000) demon     (1000)        0 2023-06-07 13:27:26.000000 i8kgui-0.8.4.dev0/i8kgui/__init__.py
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/i8kgui/desktop/
+-rw-rw-r--   0 demon     (1000) demon     (1000)      114 2023-06-07 13:27:26.000000 i8kgui-0.8.4.dev0/i8kgui/desktop/i8kgui.desktop
+-rwxrwxr-x   0 demon     (1000) demon     (1000)    86700 2023-06-08 18:29:04.000000 i8kgui-0.8.4.dev0/i8kgui/i8kgui
+-rwxrwxr-x   0 demon     (1000) demon     (1000)     2832 2023-06-08 09:38:16.000000 i8kgui-0.8.4.dev0/i8kgui/i8kgui_thermal_control
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/i8kgui/icons/
+-rw-rw-r--   0 demon     (1000) demon     (1000)    24084 2023-06-07 13:27:26.000000 i8kgui-0.8.4.dev0/i8kgui/icons/i8kgui_icon.png
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.984336 i8kgui-0.8.4.dev0/i8kgui/polkit_actions/
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/i8kgui/polkit_actions/ubuntu/
+-rw-rw-r--   0 demon     (1000) demon     (1000)      755 2023-06-08 18:23:31.000000 i8kgui-0.8.4.dev0/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy
+-rw-rw-r--   0 demon     (1000) demon     (1000)      747 2023-06-08 09:38:16.000000 i8kgui-0.8.4.dev0/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.smbios-thermal-ctl.policy
+drwxrwxr-x   0 demon     (1000) demon     (1000)        0 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/i8kgui.egg-info/
+-rw-rw-r--   0 demon     (1000) demon     (1000)     8698 2023-06-09 01:50:00.000000 i8kgui-0.8.4.dev0/i8kgui.egg-info/PKG-INFO
+-rw-rw-r--   0 demon     (1000) demon     (1000)      462 2023-06-09 01:50:00.000000 i8kgui-0.8.4.dev0/i8kgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 demon     (1000) demon     (1000)        1 2023-06-09 01:50:00.000000 i8kgui-0.8.4.dev0/i8kgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 demon     (1000) demon     (1000)       26 2023-06-09 01:50:00.000000 i8kgui-0.8.4.dev0/i8kgui.egg-info/requires.txt
+-rw-rw-r--   0 demon     (1000) demon     (1000)        7 2023-06-09 01:50:00.000000 i8kgui-0.8.4.dev0/i8kgui.egg-info/top_level.txt
+-rw-rw-r--   0 demon     (1000) demon     (1000)       87 2023-06-09 00:12:39.000000 i8kgui-0.8.4.dev0/pyproject.toml
+-rw-rw-r--   0 demon     (1000) demon     (1000)       38 2023-06-09 01:50:00.988336 i8kgui-0.8.4.dev0/setup.cfg
+-rw-rw-r--   0 demon     (1000) demon     (1000)     1220 2023-06-09 01:45:03.000000 i8kgui-0.8.4.dev0/setup.py
```

### Comparing `i8kgui-0.8.4/LICENSE` & `i8kgui-0.8.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `i8kgui-0.8.4/PKG-INFO` & `i8kgui-0.8.4.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i8kgui
-Version: 0.8.4
+Version: 0.8.4.dev0
 Summary: A Dell thermal management GUI to control fan speeds and monitor temperatures.
 Home-page: https://github.com/razman786/i8kgui
 Author: Raz
 Author-email: razman786@users.noreply.github.com
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -53,43 +53,43 @@
 * Adds polkit action configurations to allow users to change fan modes without a
   password
 
 ## Installation
 
 ### Automated Installation (Recommended)
 
-This version has only been tested on Ubuntu 20.04/23.04 (it should also work on 22.04)
+This version has only been tested on Ubuntu 20.04 (it should also work on 22.04)
 and with a Dell laptop (XPS 7590). The installation script undertakes a
 system-wide installation with all optional components (i.e. `cpupower-gui` and
-`undervolt`). i8kgui itself is installed within a users `$HOME` directory. Please see below for other install options.
+`undervolt`). Please see below for other install options.
 
 ```
 git clone https://github.com/razman786/i8kgui
 cd i8kgui
 ./install_i8kgui_ubuntu.sh
 ```
 
 #### Automated Installation Options
 
 Install option | i8kutils | Dell BIOS fan control | libsmbios | cpupower-gui | undervolt
-:---:|:---:|:---:|:---:|:---:|:---:|
-`-all` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | 
-`-norm` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | |
-`-min` | :heavy_check_mark: |
-`-fix` | :heavy_check_mark: | :heavy_check_mark: |
-`-smbios` | :heavy_check_mark: | | :heavy_check_mark: |
-`-power` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | 
+:---|:---:|:---:|:---:|:---:|:---:
+`-all` | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:
+`-norm` | :white_check_mark: | :white_check_mark: | :white_check_mark: |  |
+`-min` | :white_check_mark: | | |  |
+`-fix` | :white_check_mark: | :white_check_mark: | |  |
+`-smbios` | :white_check_mark: | | :white_check_mark: |  |
+`-power` | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 
 See `./install_i8kgui_ubuntu.sh -h` for usage information.
 
 ### Manual Installation
 
 #### Prerequisites
 
-This guide has only been tested on Ubuntu 20.04/23.04 and with a Dell XPS laptop.
+This guide has only been tested on Ubuntu 20.04 and with a Dell XPS laptop.
 
 The [dell-smm-hwmon](https://www.kernel.org/doc/html/latest/hwmon/dell-smm-hwmon.html)
 kernel module is required for basic functionality.
 
 ##### i8kutils
 
 Please install and configure i8kutils from
@@ -127,95 +127,79 @@
 sudo cp dell-bios-fan-control.service /etc/systemd/system/
 sudo systemctl enable dell-bios-fan-control.service
 ```
 
 ##### libsmbios (optional)
 
 If supported by your system, libsmbios will allow BIOS thermal modes to be changed, amongst other
-features. On Ubuntu, please install the following package to interface with (SM)BIOS
+features. On Ubuntu 20.04, please install the following package to interface with (SM)BIOS
 information:
 
 ```
 sudo apt install python3-libsmbios
 ```
 
 ##### cpupower-gui (optional)
 
-On Ubuntu, install the following optional package to change the CPU
+On Ubuntu 20.04, install the following optional package to change the CPU
 Governor:
 
 ```
 sudo apt install cpupower-gui
 ```
 
-##### polkit actions (optional)
+#### i8kgui Installation
 
-The polkit action files will allow thermal controls to be changed without
-requiring a user password. If your installation of `i8kgui` is frequently asking
-for a password, please do the following:
+##### System-wide with polkit actions (Recommended)
 
-Using a text editor, change the `I8KGUI_THERMAL_PATH` placeholder in the 
-`i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy` file to the correct location, i.e. `/home/someuser`
+###### Using PyPI
 
-To manually install the polkit action files, do the following:
 ```
-sudo cp i8kgui/polkit_actions/ubuntu/* /usr/share/polkit-1/actions
+sudo pip3 install i8kgui --prefix=/usr
 ```
 
-Please note that, the installation script by default will use the polkit action files for
-Ubuntu. Polkit action files for Manjaro Linux (tested with version 22.1.3) are
-located in `i8kgui/polkit_actions/manjaro`. 
-
-#### i8kgui Installation
-
-###### Using PyPI
+###### Using Git
 
-On Ubuntu 20.04 and 22.04 use the following:
 ```
-pip3 install i8kgui --user
+git clone https://github.com/razman786/i8kgui
+sudo pip3 install . --prefix=/usr
 ```
 
-For Ubuntu 23.04 the command needs to be altered:
-```
-pip3 install i8kgui --user --break-system-packages
-```
+Please note that the default installation will use the polkit action files for
+Ubuntu. Polkit action files for Manjaro Linux (tested with version 22.1.3) are
+located in `i8kgui/polkit_actions/manjaro`. For example, to manually install the
+polkit action files, do the following `sudo cp i8kgui/polkit_actions/ubuntu/* /usr/share/polkit-1/actions`
 
-###### Using Git
+##### Stable
 
 ```
 git clone https://github.com/razman786/i8kgui
-```
-On Ubuntu 20.04 and 22.04 use the following:
-```
 pip3 install . --user
 ```
 
-For Ubuntu 23.04 the command is as follows:
-```
-pip3 install . --user --break-system-packages
-```
-
-##### Development version
+##### Development
 
 ```
 git clone https://github.com/razman786/i8kgui
 git checkout development && git pull
 pip3 install . --user
 ```
 
 #### Uninstall i8kgui
 
-For Ubuntu 20.04 and 22.04 use the following:
+##### System-wide with polkit actions
+
 ```
-pip3 uninstall i8kgui
+sudo PYTHONUSERBASE=/usr pip3 uninstall i8kgui
 ```
 
-For Ubuntu 23.04 use the following:
+##### Stable or Development
+
 ```
-pip3 uninstall i8kgui --break-system-packages
+pip3 uninstall i8kgui
 ```
 
 ## Usage
 
 Please ensure that you have configured i8kutils *before* starting!
 
 Once i8kutils is correctly configured using the `/etc/i8kmon.conf` file, please
```

### Comparing `i8kgui-0.8.4/README.md` & `i8kgui-0.8.4.dev0/i8kgui.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: i8kgui
+Version: 0.8.4.dev0
+Summary: A Dell thermal management GUI to control fan speeds and monitor temperatures.
+Home-page: https://github.com/razman786/i8kgui
+Author: Raz
+Author-email: razman786@users.noreply.github.com
+License: GPL
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # I8KGUI
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/razman786/i8kgui/installation.yml?branch=master)  ![GitHub release (latest by date)](https://img.shields.io/github/v/release/razman786/i8kgui)
 
 ## Introduction
 
 A Dell thermal management GUI to control fan speeds and monitor temperatures.
@@ -42,43 +53,43 @@
 * Adds polkit action configurations to allow users to change fan modes without a
   password
 
 ## Installation
 
 ### Automated Installation (Recommended)
 
-This version has only been tested on Ubuntu 20.04/23.04 (it should also work on 22.04)
+This version has only been tested on Ubuntu 20.04 (it should also work on 22.04)
 and with a Dell laptop (XPS 7590). The installation script undertakes a
 system-wide installation with all optional components (i.e. `cpupower-gui` and
-`undervolt`). i8kgui itself is installed within a users `$HOME` directory. Please see below for other install options.
+`undervolt`). Please see below for other install options.
 
 ```
 git clone https://github.com/razman786/i8kgui
 cd i8kgui
 ./install_i8kgui_ubuntu.sh
 ```
 
 #### Automated Installation Options
 
 Install option | i8kutils | Dell BIOS fan control | libsmbios | cpupower-gui | undervolt
-:---:|:---:|:---:|:---:|:---:|:---:|
-`-all` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | 
-`-norm` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | |
-`-min` | :heavy_check_mark: |
-`-fix` | :heavy_check_mark: | :heavy_check_mark: |
-`-smbios` | :heavy_check_mark: | | :heavy_check_mark: |
-`-power` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | 
+:---|:---:|:---:|:---:|:---:|:---:
+`-all` | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:
+`-norm` | :white_check_mark: | :white_check_mark: | :white_check_mark: |  |
+`-min` | :white_check_mark: | | |  |
+`-fix` | :white_check_mark: | :white_check_mark: | |  |
+`-smbios` | :white_check_mark: | | :white_check_mark: |  |
+`-power` | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 
 See `./install_i8kgui_ubuntu.sh -h` for usage information.
 
 ### Manual Installation
 
 #### Prerequisites
 
-This guide has only been tested on Ubuntu 20.04/23.04 and with a Dell XPS laptop.
+This guide has only been tested on Ubuntu 20.04 and with a Dell XPS laptop.
 
 The [dell-smm-hwmon](https://www.kernel.org/doc/html/latest/hwmon/dell-smm-hwmon.html)
 kernel module is required for basic functionality.
 
 ##### i8kutils
 
 Please install and configure i8kutils from
@@ -116,95 +127,79 @@
 sudo cp dell-bios-fan-control.service /etc/systemd/system/
 sudo systemctl enable dell-bios-fan-control.service
 ```
 
 ##### libsmbios (optional)
 
 If supported by your system, libsmbios will allow BIOS thermal modes to be changed, amongst other
-features. On Ubuntu, please install the following package to interface with (SM)BIOS
+features. On Ubuntu 20.04, please install the following package to interface with (SM)BIOS
 information:
 
 ```
 sudo apt install python3-libsmbios
 ```
 
 ##### cpupower-gui (optional)
 
-On Ubuntu, install the following optional package to change the CPU
+On Ubuntu 20.04, install the following optional package to change the CPU
 Governor:
 
 ```
 sudo apt install cpupower-gui
 ```
 
-##### polkit actions (optional)
+#### i8kgui Installation
 
-The polkit action files will allow thermal controls to be changed without
-requiring a user password. If your installation of `i8kgui` is frequently asking
-for a password, please do the following:
+##### System-wide with polkit actions (Recommended)
 
-Using a text editor, change the `I8KGUI_THERMAL_PATH` placeholder in the 
-`i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy` file to the correct location, i.e. `/home/someuser`
+###### Using PyPI
 
-To manually install the polkit action files, do the following:
 ```
-sudo cp i8kgui/polkit_actions/ubuntu/* /usr/share/polkit-1/actions
+sudo pip3 install i8kgui --prefix=/usr
 ```
 
-Please note that, the installation script by default will use the polkit action files for
-Ubuntu. Polkit action files for Manjaro Linux (tested with version 22.1.3) are
-located in `i8kgui/polkit_actions/manjaro`. 
-
-#### i8kgui Installation
-
-###### Using PyPI
+###### Using Git
 
-On Ubuntu 20.04 and 22.04 use the following:
 ```
-pip3 install i8kgui --user
+git clone https://github.com/razman786/i8kgui
+sudo pip3 install . --prefix=/usr
 ```
 
-For Ubuntu 23.04 the command needs to be altered:
-```
-pip3 install i8kgui --user --break-system-packages
-```
+Please note that the default installation will use the polkit action files for
+Ubuntu. Polkit action files for Manjaro Linux (tested with version 22.1.3) are
+located in `i8kgui/polkit_actions/manjaro`. For example, to manually install the
+polkit action files, do the following `sudo cp i8kgui/polkit_actions/ubuntu/* /usr/share/polkit-1/actions`
 
-###### Using Git
+##### Stable
 
 ```
 git clone https://github.com/razman786/i8kgui
-```
-On Ubuntu 20.04 and 22.04 use the following:
-```
 pip3 install . --user
 ```
 
-For Ubuntu 23.04 the command is as follows:
-```
-pip3 install . --user --break-system-packages
-```
-
-##### Development version
+##### Development
 
 ```
 git clone https://github.com/razman786/i8kgui
 git checkout development && git pull
 pip3 install . --user
 ```
 
 #### Uninstall i8kgui
 
-For Ubuntu 20.04 and 22.04 use the following:
+##### System-wide with polkit actions
+
 ```
-pip3 uninstall i8kgui
+sudo PYTHONUSERBASE=/usr pip3 uninstall i8kgui
 ```
 
-For Ubuntu 23.04 use the following:
+##### Stable or Development
+
 ```
-pip3 uninstall i8kgui --break-system-packages
+pip3 uninstall i8kgui
 ```
 
 ## Usage
 
 Please ensure that you have configured i8kutils *before* starting!
 
 Once i8kutils is correctly configured using the `/etc/i8kmon.conf` file, please
```

### Comparing `i8kgui-0.8.4/i8kgui/i8kgui` & `i8kgui-0.8.4.dev0/i8kgui/i8kgui`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for
 # more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
+from pathlib import Path
+from contextlib import contextmanager
+from contextlib import suppress
 import os
 import glob
 import shutil
 import warnings
 
-import cpuinfo
-import psutil
-
-from pathlib import Path
-from contextlib import contextmanager, suppress
-
 from PySide6 import QtCore
-from PySide6.QtCore import Qt, QProcess, QSettings, QSize, Slot, QTimer
-from PySide6.QtGui import QAction, QActionGroup, QColor, QIcon, QIntValidator, QPalette, QScreen
+from PySide6.QtCore import QProcess, QSettings, QSize, Slot, QTimer
+from PySide6.QtGui import (QAction, QActionGroup, QColor, QIcon, QIntValidator, QPalette, QScreen, Qt)
 from PySide6.QtWidgets import (QApplication, QCheckBox, QDialog, QFormLayout, QLabel, QLineEdit, QMainWindow, QMenu,
                                QMessageBox, QPushButton, QSystemTrayIcon)
-
+import cpuinfo
+import psutil
 
 warnings.filterwarnings("ignore")
 
 
 class I8kGui(QMainWindow):
     """I8kGui."""
 
@@ -54,21 +52,18 @@
         self.scaling_sysfs = None
         self.tdp = None
         self.ht_sysfs = None
         self.num_phy_cores = psutil.cpu_count(logical=False)
         self.coretemps_sysfs = []
         self.is_intel_cpu = True
         self.cpu_num = psutil.cpu_count()
-        self.tray_menu = QMenu(self)
+        self.tray_menu = QMenu()
         self.thermal_menu_group = QActionGroup(self.tray_menu)
         self.thermal_control_menu = QMenu("Thermal Control N/A")
-        self.cpupower = None
         self.p = None
-        self.p_smbios = None
-        self.p_state_smbios = None
         self.is_i8kmon_active = False
         self.is_dell_fan_control_active = False
         self.is_smbios_active = False
         self.degree_sign = u'\N{DEGREE SIGN}'
         self.use_cpu_ave_freq = False
         self.thermal_modes = {}
         self.p_state = None
@@ -81,16 +76,16 @@
         self.always_on = False
         self.bios_thermal_control_on = False
         self.monitor_interval = 1000
         self.always_on_checkbox = QCheckBox()
         self.thermal_checkbox = QCheckBox()
         self.cpu_ave_freq_checkbox = QCheckBox()
         self.interval_input = QLineEdit()
-        self.settings_dialog = QDialog(self)
-        self.info_dialog = QDialog(self)
+        self.settings_dialog = QDialog()
+        self.info_dialog = QDialog()
         self.save_button = QPushButton("Save", self.settings_dialog)
         self.smbios_button = QPushButton("SMBIOS Information",
                                          self.info_dialog)
         self.cpu_model = QLabel(cpuinfo.get_cpu_info()['brand_raw'])
         self.cpu_tdp = QLabel("N/A")
         self.i8k_format_version = QLabel("1")
         self.bios_version = QLabel("1")
@@ -100,23 +95,29 @@
         self.fan_mode_menu_item = QAction("")
         self.fan_mode_menu_item.setCheckable(False)
         self.left_fan_thermal_menu_item = QAction("")
         self.left_fan_thermal_menu_item.setCheckable(False)
         self.right_fan_thermal_menu_item = QAction("")
         self.right_fan_thermal_menu_item.setCheckable(False)
         self.i8k_info = {}
+        # check dependencies
+        self.check_prerequisites()
+        # load settings
+        self.load_settings()
         self.monitorTimer = QTimer(self)
-        self.monitorTimer.timeout.connect(self.refresh_monitor,
-                                          type=Qt.QueuedConnection)
+        self.monitorTimer.timeout.connect(self.refresh_monitor)
         self.monitorTimer.setInterval(self.monitor_interval)
+        self.create_settings_dialog()
+        self.create_info_dialog()
         self.tray = None
         self.first_load = True
         self.cpu_temp_sensors = []
         self.cpu_sysfs_siblings = []
         self.cpu_siblings = {}
+        self.detect_cpu()
         self.cpu_usage = QAction("CPU Usage:\t")
         self.cpu_mhz = QAction("CPU MHz:\t")
         self.cpu_details = QMenu("Per CPU Core\t")
         self.cpu_turbo = QMenu("CPU Turbo Boost\t")
         self.cpu_turbo_enabled = QAction("CPU Turbo Boost:\tN/A")
         self.cpu_turbo_enabled.setCheckable(False)
         self.min_cpu_freq = QAction("CPU Min. Freq:\t0 MHz")
@@ -125,44 +126,29 @@
         self.max_cpu_freq.setCheckable(False)
         self.min_cpu_turbo = QAction("CPU Min. Turbo:\t0%")
         self.min_cpu_turbo.setCheckable(False)
         self.max_cpu_turbo = QAction("CPU Max. Turbo:\t0%")
         self.max_cpu_turbo.setCheckable(False)
         self.cpu_freq_list = []
         self.cpu_curr_freqs = []
+        self.build_cpu_menu()
         self.cpu_governor = QAction("CPU Governor:\t")
         self.cpu_temp = QAction("CPU Temp:\t")
         self.left_fan_rpm = QAction("Left Fan:\t")
         self.right_fan_rpm = QAction("Right Fan:\t")
         self.left_fan_status = QAction("Left Fan Mode:\t")
         self.right_fan_status = QAction("Right Fan Mode:\t")
-        # check dependencies
-        self.check_prerequisites()
-        # load settings
-        self.load_settings()
-        # create settings window
-        self.create_settings_dialog()
-        # create information window
-        self.create_info_dialog()
-        # detect CPU architecture
-        self.detect_cpu()
-        # build CPU sub menu
-        self.build_cpu_menu()
-        # load i8kgui system tray
         self.load_sys_tray()
 
     def close_app(self):
-        """close_app. Save settings, stop monitoring and quit.
+        """close_app. Save settings and quit.
 
         :param self:
         """
         self.save_settings()
-        if self.monitorTimer.isActive():
-            self.monitorTimer.stop()
-        self.kill_process()
         app.quit()
 
     def thermal_error_dialog(
         self,
         cmd='disable',
         msg="Critical Service Error. "
             "Please click 'OK' and enter your password if asked."):
@@ -171,15 +157,15 @@
         :param self:
         :param cmd:
         :param msg:
         """
         # displays an error dialog when services are out of sync
         error_dialog = QMessageBox(QMessageBox.Icon.Critical, "i8kgui", msg)
         error_dialog.setText(msg)
-        button = error_dialog.open()
+        button = error_dialog.exec()
         if button == QMessageBox.Ok:
             # disable bios thermal control (i.e. default is i8kmon)
             if cmd in ['enable', 'disable']:
                 self.bios_thermal_control(op=cmd)
 
     def detect_cpu(self):
         """detect_cpu - find out if HT enabled, create a CPU sibling list and a CPU
@@ -255,17 +241,22 @@
                             else:
                                 # Adding new logical core
                                 self.cpu_siblings[int(pair[1])] = int(pair[0])
         if not self.cpu_siblings:
             self.cpu_siblings[0] = 0
         print(f"Found: CPU siblings: {self.cpu_siblings}")
         # create physical CPU temp sensor list
-        for i in range(len(self.cpu_siblings)):
-            j = i % self.num_phy_cores
+        j = 0
+        once = True
+        for _ in self.cpu_siblings:
+            if j > self.num_phy_cores - 1 and once:
+                j = 0
+                once = False
             self.cpu_temp_sensors.append(j)
+            j += 1
         print(f"Found: CPU temp sensors {self.cpu_temp_sensors}")
 
     def sanitise_thermal_modes(self, modes):
         """sanitise_thermal_modes.
 
         :param modes:
         """
@@ -276,47 +267,44 @@
         if "Supported Thermal Modes: " in modes:
             modes.remove("Supported Thermal Modes: ")
         if "Supported Thermal Modes:" in modes:
             modes.remove("Supported Thermal Modes:")
         if "" in modes:
             modes.remove("")
         modes = [i.strip() for i in modes]
+        # modes = [*set(modes)]
         s_modes = []
         [s_modes.append(x) for x in modes if x not in s_modes]
         return s_modes
 
     def load_settings(self):
         """load_settings.
 
         :param self:
         """
         # load continuous data collection setting
         always_on = str(self.settings.value('always_on'))
         if always_on and always_on.lower() == 'false':
             self.always_on = False
-            self.always_on_checkbox.setChecked(False)
-            self.always_on_checkbox.setCheckState(Qt.CheckState.Unchecked)
+            self.always_on_checkbox.setCheckState(Qt.Unchecked)
         else:
             self.always_on = True
-            self.always_on_checkbox.setChecked(True)
-            self.always_on_checkbox.setCheckState(Qt.CheckState.Checked)
+            self.always_on_checkbox.setCheckState(Qt.Checked)
 
         # load monitoring interval setting
         self.monitor_interval = int(str(self.settings.value('interval', 1000)))
 
         # load average CPU freq. setting
         use_cpu_ave_freq = str(self.settings.value('use_cpu_ave_freq'))
         if use_cpu_ave_freq and use_cpu_ave_freq.lower() == 'true':
             self.use_cpu_ave_freq = True
-            self.cpu_ave_freq_checkbox.setChecked(True)
-            self.cpu_ave_freq_checkbox.setCheckState(Qt.CheckState.Checked)
+            self.cpu_ave_freq_checkbox.setCheckState(Qt.Checked)
         else:
             self.use_cpu_ave_freq = False
-            self.cpu_ave_freq_checkbox.setChecked(False)
-            self.cpu_ave_freq_checkbox.setCheckState(Qt.CheckState.Unchecked)
+            self.cpu_ave_freq_checkbox.setCheckState(Qt.Unchecked)
 
         if info := list(self.settings.value('smbios', [])):
             # reconstruct list back into dict preserving order
             self.smbios_info = {
                 info[i][0]: info[i][1]
                 for i in range(0, len(info))
             }
@@ -402,65 +390,57 @@
         self.settings.setValue('always_on', self.always_on)
         self.settings.setValue('use_cpu_ave_freq', self.use_cpu_ave_freq)
         self.settings.setValue('interval', self.monitor_interval)
         if self.smbios_info:
             # preserve ordering by storing a list
             self.settings.setValue('smbios', list(self.smbios_info.items()))
 
-    def handle_thermal_control(self, checked):
-        """Enable/disable thermal control based on the current state of smbios and i8kmon.
+    def enable_thermal_control(self, checked):
+        """enable_thermal_control.
 
-        :param checked: The state of the thermal checkbox.
+        :param checked:
         """
-        if checked != 0:
+        # DEBUG
+        # print(f"DEBUG: BIOS control checkbox, smbios active {self.is_smbios_active}, "
+        #       f"i8kmon active {self.is_i8kmon_active}, "
+        #       f"is checkbox checked? {checked == Qt.Checked}, "
+        #       f"checkstate {self.thermal_checkbox.checkState()}")
+
+        if checked == Qt.Checked:
             if self.is_smbios_active:
-                self.enable_bios_thermal_control()
+                self.bios_thermal_control(op='enable')
                 self.switch_thermal_menu()
-                print("Switching to bios thermal control")
-            else:
-                self.handle_inactive_controller('i8kmon', 'smbios')
+                print("Info: switching to bios thermal control")
+            elif not self.is_smbios_active and self.is_i8kmon_active:
+                # else:
+                self.bios_thermal_control(op='disable')
+                self.thermal_checkbox.setChecked(False)
+                self.thermal_checkbox.setCheckState(Qt.CheckState.Unchecked)
+                self.switch_thermal_menu()
+                print("Error: smbios is not active, reverting to i8kmon thermal control")
+                self.thermal_error_dialog('error', "libsmbios is not active. Reverting to i8kmon thermal control")
         else:
             if self.is_i8kmon_active:
-                self.disable_bios_thermal_control()
+                self.bios_thermal_control(op='disable')
                 self.switch_thermal_menu()
-                print("Switching to i8kmon thermal control")
-            else:
-                self.handle_inactive_controller('smbios', 'i8kmon')
-
-    def handle_inactive_controller(self, active_controller, inactive_controller):
-        """Handle the case where the active thermal controller is not available.
-
-        :param active_controller: The name of the active controller.
-        :param inactive_controller: The name ofthe inactive controller.
-        """
-        if inactive_controller == 'smbios':
-            self.disable_bios_thermal_control()
-        else:
-            self.enable_bios_thermal_control()
-        self.thermal_checkbox.setChecked(False)
-        self.thermal_checkbox.setCheckState(Qt.CheckState.Unchecked)
-        self.switch_thermal_menu()
-        print(f"{active_controller} is not available, reverting to {inactive_controller} thermal control")
-        self.thermal_error_dialog(
-            'error', f"{active_controller} is not active. Reverting to {inactive_controller} thermal control")
-
-    def enable_bios_thermal_control(self):
-        """Enable thermal control through BIOS."""
-        self.bios_thermal_control(op='enable')
-
-    def disable_bios_thermal_control(self):
-        """Disable thermal control through BIOS."""
-        self.bios_thermal_control(op='disable')
+                print("Info: switching to i8kmon thermal control")
+            elif not self.is_i8kmon_active and self.is_smbios_active:
+                self.bios_thermal_control(op='enable')
+                self.thermal_checkbox.setChecked(True)
+                self.thermal_checkbox.setCheckState(Qt.CheckState.Checked)
+                self.switch_thermal_menu()
+                print("Error: i8kmon is not active, reverting to smbios thermal control")
+                self.thermal_error_dialog('error', "i8kmon is not active. Reverting to libsmbios thermal control")
 
     def always_collect(self, checked):
         """always_collect. Collect metrics continuously at a set time interval.
 
         :param checked:
         """
-        if checked != 0:
+        if checked == Qt.Checked:
             self.monitor_interval = int(self.interval_input.text())
             self.monitorTimer.setInterval(self.monitor_interval)
             self.always_on = True
             if self.monitorTimer.isActive():
                 self.monitorTimer.stop()
             self.monitorTimer.start()
         else:
@@ -469,15 +449,15 @@
                 self.monitorTimer.stop()
 
     def enable_ave_cpu_freq(self, checked):
         """enable_ave_cpu_freq. Enable average CPU frequency over all all cores.
 
         :param checked:
         """
-        self.use_cpu_ave_freq = checked != 0
+        self.use_cpu_ave_freq = checked == Qt.Checked
 
     def save_dialog_settings(self):
         """save_dialog_settings."""
         if self.monitor_interval != int(self.interval_input.text()):
             self.monitor_interval = int(self.interval_input.text())
             self.monitorTimer.setInterval(self.monitor_interval)
             if self.monitorTimer.isActive():
@@ -506,14 +486,17 @@
                 self.smbios_data.append(part_item.strip())
 
     def check_thermal_control(self):
         """check_thermal_control. Check systemd services.
 
         :param self:
         """
+        if self.p is not None:
+            return
+
         active_services = []
         self._is_systemd_service_active(
             'i8kmon.service',
             active_services,
             "Warn: systemctl i8kmon.service not found",
         )
         self._is_systemd_service_active(
@@ -533,23 +516,22 @@
         :param service:
         :param active_services:
         :param err_msg:
         """
         # check which system services are active.
         # keep a reference to the QProcess (e.g. on self)
         # while it's running.
-        subproc = QProcess()
-        subproc.start("systemctl", ['is-enabled', service])
-        subproc.waitForFinished(1000)
-        result_systemd = subproc.readLine()
+        self.p = QProcess()
+        self.p.start("systemctl", ['is-enabled', service])
+        self.p.waitForFinished()
+        result_systemd = self.p.readLine()
         output_systemd = bytes(result_systemd).decode("utf8")
         is_service_active = output_systemd.strip('\n')
-        if subproc.state != 0:
-            self.kill_process(subproc)
-        subproc = None
+        self.p.close()
+        self.p = None
         # check if systemd service is enabled,
         if is_service_active == 'enabled':
             active_services.append(service)
         else:
             print(f"Error: systemd service check {err_msg}")
 
     def check_prerequisites(self):
@@ -567,59 +549,67 @@
         else:
             print(f"Error: CPU vendor not supported {cpu_vendor}")
 
         #
         # check Sysfs interfaces
         #
 
-        def check_sysfs(path, found_str, not_found_str):
-            if Path(path).is_file():
-                print(f"Found: {found_str}")
-                return True
-            else:
-                print(f"Error: {not_found_str} not found")
-                return False
-
-        # Check AC power supply
+        # check power
+        # Intel Dell 7950 power supply
         self.power_sysfs = "/sys/class/power_supply/AC/online"
-        if check_sysfs(self.power_sysfs, "Sysfs AC power supply", "Sysfs AC power supply"):
+        if Path(self.power_sysfs).is_file():
             self.power_enabled = True
+            print("Found: Sysfs AC power")
         else:
+            # AMD Dell 5575 power supply
             self.power_sysfs = "/sys/class/power_supply/ACAD/online"
-            if check_sysfs(self.power_sysfs, "Sysfs ACAD power supply", "Sysfs AC power supply"):
+            if Path(self.power_sysfs).is_file():
+                print("Found: Sysfs ACAD power ")
                 self.power_enabled = True
             else:
                 self.power_enabled = False
+                print("Error: Sysfs AC power not found")
 
-        # Check Scaling Governor
+        # check scaling governor
         self.scaling_sysfs = "/sys/devices/system/cpu/cpu0/cpufreq/scaling_governor"
-        if check_sysfs(self.scaling_sysfs, "Sysfs scaling governor", "Sysfs scaling governor not found"):
+        if Path(self.scaling_sysfs).is_file():
             self.scaling_enabled = True
+            print("Found: Sysfs scaling governor")
         else:
             self.scaling_enabled = False
+            print("Error: Sysfs scaling governor not found")
 
-        # Check RAPL TDP
+        # check RAPL TDP
         # not available on AMD Dell 5575
         self.tdp = "/sys/devices/virtual/powercap/intel-rapl/intel-rapl:0/constraint_0_max_power_uw"
-        if check_sysfs(self.tdp, "Sysfs RAPL TDP", "Sysfs RAPL TDP not found"):
-            self.tdp_enabled = True
-        elif check_sysfs(self.tdp, "Sysfs RAPL TDP alternative", "Sysfs RAPL TDP not found"):
+        if Path(self.tdp).is_file():
             self.tdp_enabled = True
+            print("Found: Sysfs RAPL TDP")
         else:
-            self.tdp_enabled = False
+            self.tdp = "/sys/devices/virtual/powercap/intel-rapl/intel-rapl0:0/constraint_0_max_power_uw"
+            if Path(self.tdp).is_file():
+                self.tdp_enabled = True
+                print("Found: Sysfs RAPL TDP alternative")
+            else:
+                self.tdp_enabled = False
+                print("Error: Sysfs RAPL TDP not found")
 
-        # Check SMT
+        # check SMT
         self.ht_sysfs = "/sys/devices/system/cpu/smt/active"
-        if check_sysfs(self.ht_sysfs, "Sysfs SMT status", "Sysfs SMT status not found"):
-            pass
+        if Path(self.ht_sysfs).is_file():
+            print("Found: Sysfs SMT status")
+        else:
+            print("Error: Sysfs SMT status not found")
 
-        # Check CPU siblings
+        # check CPU siblings
         cpu_siblings_sysfs = "/sys/devices/system/cpu/cpu0/topology/thread_siblings_list"
-        if check_sysfs(cpu_siblings_sysfs, "Sysfs CPU siblings", "Sysfs CPU siblings not found"):
-            pass
+        if Path(cpu_siblings_sysfs).is_file():
+            print("Found: Sysfs CPU siblings")
+        else:
+            print("Error: Sysfs CPU siblings not found")
 
         #
         # check CPU coretemps and turbo settings
         #
 
         # check cpu coretemp or k10temp sysfs interface
         use_hwmon_temp = False
@@ -889,21 +879,20 @@
         if not thermal_file.is_file():
             thermal_file = Path("i8kgui_thermal_control")
         # check for smbios-thermal-ctl
         self.smbois_ctl = Path(str(shutil.which("smbios-thermal-ctl"))).resolve()
         # check that smbios is working
         if self.smbois_ctl.is_file():
             print(f"Found: (SM)BIOS Thermal Control {self.smbois_ctl}")
-            subproc = QProcess()
-            subproc.start("pkexec", [str(thermal_file.resolve()), '--status'])
-            subproc.waitForFinished(1000)
-            smbios_stdout = subproc.readAllStandardOutput()
-            if subproc.state() != 0:
-                self.kill_process(subproc)
-            subproc = None
+            self.p = QProcess()
+            self.p.start("pkexec", [str(thermal_file.resolve()), '--status'])
+            self.p.waitForFinished()
+            smbios_stdout = self.p.readAllStandardOutput()
+            self.p.close()
+            self.p = None
             smbios_stdout = bytes(smbios_stdout).decode("utf8")
             if smbios_stdout.startswith('Status Current Thermal Modes'):
                 split_stdout = smbios_stdout.split('\n')
                 split_stdout = self.sanitise_thermal_modes(split_stdout)
                 for item in split_stdout[1:]:
                     print(f"Found: libsmbios current thermal mode '{item}'")
                     self.current_thermal_mode_data.append(item)
@@ -921,15 +910,15 @@
         # check i8kmon prerequisites
         # minimum 1 fan and CPU temp
         i8kmon_passed = bool(
             (
                 (Path(self.i8kmon_fan1).is_file()
                     or Path(self.i8kmon_fan2).is_file())
                 and (Path(self.i8kmon_fan1_target).is_file()
-                     or Path(self.i8kmon_fan2_target).is_file())
+                    or Path(self.i8kmon_fan2_target).is_file())
                 and Path(self.i8kmon_temp).is_file()
             )
         )
         # check sysfs prerequisites
         # minimum scaling, SMT and CPU core siblings
         sysfs_passed = bool(
             (Path(self.scaling_sysfs).is_file()
@@ -963,44 +952,44 @@
         thermal_file = Path(str(shutil.which("i8kgui_thermal_control")))
         if not thermal_file.is_file():
             thermal_file = Path("i8kgui_thermal_control")
         # enable bios control and disable i8kmon
         if op == 'enable':
             self.p = QProcess()
             self.p.readyReadStandardOutput.connect(
-                self.handle_thermal_stdout, type=Qt.QueuedConnection)
+                self.handle_thermal_stdout)
             self.p.readyReadStandardError.connect(
-                self.handle_thermal_stderr, type=Qt.QueuedConnection)
-            self.p.stateChanged.connect(self.handle_process_state, type=Qt.QueuedConnection)
+                self.handle_thermal_stderr)
+            self.p.stateChanged.connect(self.handle_process_state)
             # clean up once complete
-            self.p.finished.connect(self.thermal_process_finished, type=Qt.QueuedConnection)
+            self.p.finished.connect(self.thermal_process_finished)
             self.p.start("pkexec",
                          [str(thermal_file.resolve()), '--enable'])
         # disable bios control and enable i8kmon
         elif op == 'disable':
             self.p = QProcess()
             self.p.readyReadStandardOutput.connect(
-                self.handle_thermal_stdout, type=Qt.QueuedConnection)
+                self.handle_thermal_stdout)
             self.p.readyReadStandardError.connect(
-                self.handle_thermal_stderr, type=Qt.QueuedConnection)
-            self.p.stateChanged.connect(self.handle_process_state, type=Qt.QueuedConnection)
+                self.handle_thermal_stderr)
+            self.p.stateChanged.connect(self.handle_process_state)
             # clean up once complete
-            self.p.finished.connect(self.thermal_process_disable_finished, type=Qt.QueuedConnection)
+            self.p.finished.connect(self.thermal_process_disable_finished)
             self.p.start("pkexec",
                          [str(thermal_file.resolve()), '--disable'])
         # get BIOS controlled thermal mode
         elif op == 'status':
             self.p = QProcess()
             self.p.readyReadStandardOutput.connect(
-                self.handle_thermal_stdout, type=Qt.QueuedConnection)
+                self.handle_thermal_stdout)
             self.p.readyReadStandardError.connect(
-                self.handle_thermal_stderr, type=Qt.QueuedConnection)
-            self.p.stateChanged.connect(self.handle_process_state, type=Qt.QueuedConnection)
+                self.handle_thermal_stderr)
+            self.p.stateChanged.connect(self.handle_process_state)
             # clean up once complete
-            self.p.finished.connect(self.thermal_process_finished, type=Qt.QueuedConnection)
+            self.p.finished.connect(self.thermal_process_finished)
             self.p.start("pkexec",
                          [str(thermal_file.resolve()), '--status'])
 
     def handle_thermal_stderr(self):
         """handle_thermal_stderr.
 
         :param self:
@@ -1045,51 +1034,34 @@
         elif stdout.startswith('Status Current Thermal Modes'):
             print(f"stdout {stdout}")
             split_stdout = stdout.split('\n')
             split_stdout = self.sanitise_thermal_modes(split_stdout)
             for item in split_stdout:
                 self.current_thermal_mode_data.append(item)
 
-    def close_process(self, proc=None):
+    def close_process(self):
         """close_process.
 
         :param self:
         """
-        if proc is None and self.p:
-            if self.p.state() != 0:
-                with suppress(Exception):
-                    self.p.terminate()
-                    self.p.waitForFinished(1000)
-                    self.p.kill()
-            self.p = None
-        elif proc:
-            if proc.state() != 0:
-                with suppress(Exception):
-                    proc.terminate()
-                    proc.waitForFinished(1000)
-                    proc.kill()
-            proc = None
+        if self.p and self.p.state() != 0:
+            self.p.close()
+        self.p = None
 
-    def kill_process(self, proc=None):
+    def kill_process(self):
         """kill_process.
 
         :param self:
         """
-        if proc is None and self.p:
-            with suppress(Exception):
+        with suppress(Exception):
+            if self.p:
                 self.p.terminate()
                 self.p.waitForFinished(1000)
                 self.p.kill()
-            self.p = None
-        elif proc:
-            with suppress(Exception):
-                proc.terminate()
-                proc.waitForFinished(1000)
-                proc.kill()
-            proc = None
+        self.p = None
 
     def thermal_selection_finished(self):
         """thermal_selection_finished.
 
         :param self:
         """
         # bios mode change
@@ -1361,15 +1333,15 @@
         return info
 
     def get_smbios_information(self):
         """get_smbios_information.
 
         :param self:
         """
-        if self.p_smbios is not None:
+        if self.p is not None:
             return
 
         # find smbios script
         if self.is_smbios_active:
             smbios_file = Path(str(shutil.which("smbios-sys-info")))
             if not smbios_file.is_file():
                 if self.tray:
@@ -1377,44 +1349,44 @@
                         "i8kgui",
                         "Error please install python3-libsmbios, "
                         "smbios-sys-info not found",
                         icon=QSystemTrayIcon.Critical,
                         msecs=10000)
                 return
             # Keep a reference to the QProcess (e.g. on self) while it's running.
-            self.p_smbios = QProcess()
-            self.p_smbios.readyReadStandardOutput.connect(self.handle_smbios_stdout, type=Qt.QueuedConnection)
-            self.p_smbios.readyReadStandardError.connect(self.handle_smbios_stderr, type=Qt.QueuedConnection)
-            self.p_smbios.stateChanged.connect(self.smbios_handle_process_state, type=Qt.QueuedConnection)
+            self.p = QProcess()
+            self.p.readyReadStandardOutput.connect(self.handle_smbios_stdout)
+            self.p.readyReadStandardError.connect(self.handle_smbios_stderr)
+            self.p.stateChanged.connect(self.handle_process_state)
             # Clean up once complete.
-            self.p_smbios.finished.connect(self.smbios_process_finished, type=Qt.QueuedConnection)
-            self.p_smbios.start("pkexec", [str(smbios_file.resolve())])
+            self.p.finished.connect(self.smbios_process_finished)
+            self.p.start("pkexec", [str(smbios_file.resolve())])
         else:
             print("Error: libsmbios is unavailable")
 
     def handle_smbios_stderr(self):
         """handle_smbios_stderr.
 
         :param self:
         """
-        if self.p_smbios:
-            data = self.p_smbios.readAllStandardError()
+        if self.p:
+            data = self.p.readAllStandardError()
             stderr = bytes(data).decode("utf8")
             if 'Request dismissed' in stderr:
-                self.p_smbios.finished.emit(1, QProcess.CrashExit)
+                self.p.finished.emit(1, QProcess.CrashExit)
             else:
                 print(f"Error: handle_smbios_stderr {stderr}")
 
     def handle_smbios_stdout(self):
         """handle_smbios_stdout.
 
         :param self:
         """
-        if self.p_smbios:
-            data = self.p_smbios.readAllStandardOutput()
+        if self.p:
+            data = self.p.readAllStandardOutput()
             stdout = bytes(data).decode("utf8")
             self.smbios_message(stdout)
 
     def handle_process_state(self, state):
         """handle_process_state.
 
         :param state:
@@ -1422,35 +1394,23 @@
         states = {
             QProcess.NotRunning: 'NotRunning',
             QProcess.Starting: 'Starting',
             QProcess.Running: 'Running',
         }
         self.p_state = states[state]
 
-    def smbios_handle_process_state(self, state):
-        """handle_process_state.
-
-        :param state:
-        """
-        states = {
-            QProcess.NotRunning: 'NotRunning',
-            QProcess.Starting: 'Starting',
-            QProcess.Running: 'Running',
-        }
-        self.p_state_smbios = states[state]
-
     def smbios_process_finished(self):
         """smbios_process_finished.
 
         :param self:
         """
-        if self.p_smbios and self.p_smbios.exitCode() != 0:
-            self.kill_process(self.p_smbios)
+        if self.p and self.p.exitCode() != 0:
+            self.kill_process()
         else:
-            self.close_process(self.p_smbios)
+            self.close_process()
             self.process_smbios_data()
 
     def process_smbios_data(self):
         """process_smbios_data.
 
         :param self:
         """
@@ -1470,20 +1430,18 @@
     def create_info_dialog(self):
         """create_info_dialog.
 
         :param self:
         """
         close_button = QPushButton("close", self.info_dialog)
         close_button.setMaximumWidth(100)
-        close_button.clicked.connect(self.close_info_dialog,
-                                     type=Qt.QueuedConnection)
+        close_button.clicked.connect(self.close_info_dialog)
 
         self.smbios_button.setMaximumWidth(250)
-        self.smbios_button.clicked.connect(self.get_smbios_information,
-                                           type=Qt.QueuedConnection)
+        self.smbios_button.clicked.connect(self.get_smbios_information)
 
         f_layout = QFormLayout()
         f_layout.addRow("CPU Model", self.cpu_model)
         f_layout.addRow("CPU TDP", self.get_cpu_tdp())
         f_layout.addRow("i8k Format Version", self.i8k_format_version)
         f_layout.addRow("BIOS Version", self.bios_version)
         f_layout.addRow("Service Tag", self.service_tag)
@@ -1497,54 +1455,66 @@
         if self.smbios_info:
             for key, value in self.smbios_info.items():
                 f_layout.insertRow(f_layout.rowCount() - 2, str(key),
                                    QLabel(str(value)))
         self.info_dialog.setLayout(f_layout)
         # set dialog geometry
         self.info_dialog.setWindowTitle("Information")
-        self.info_dialog.setModal(False)
-        self.info_dialog.adjustSize()
+        self.info_dialog.setWindowModality(QtCore.Qt.ApplicationModal)
+        self.info_dialog.setMinimumWidth(450)
+        self.info_dialog.setMaximumWidth(600)
+        self.info_dialog.setMaximumHeight(600)
+        center_point = QScreen.availableGeometry(
+            QApplication.primaryScreen()).center()
+        fg = self.info_dialog.frameGeometry()
+        fg.moveCenter(center_point)
+        self.info_dialog.move(fg.topLeft())
 
     def create_settings_dialog(self):
         """create_settings_dialog.
 
         :param self:
         """
         self.save_button.setMaximumWidth(100)
 
         self.always_on_checkbox.setText("Collect statistics continuously")
-        self.always_on_checkbox.stateChanged.connect(self.always_collect,
-                                                     type=Qt.QueuedConnection)
+        self.always_on_checkbox.stateChanged.connect(self.always_collect)
 
         self.thermal_checkbox.setText("Enable BIOS thermal management")
-        self.thermal_checkbox.stateChanged.connect(self.handle_thermal_control, type=Qt.QueuedConnection)
+        self.thermal_checkbox.stateChanged.connect(self.enable_thermal_control)
 
         self.cpu_ave_freq_checkbox.setText("Display average CPU freq.")
         self.cpu_ave_freq_checkbox.stateChanged.connect(
-            self.enable_ave_cpu_freq, type=Qt.QueuedConnection)
+            self.enable_ave_cpu_freq)
 
         self.interval_input.setValidator(QIntValidator())
         self.interval_input.setMaxLength(6)
         self.interval_input.setText(str(self.monitor_interval))
 
-        self.save_button.clicked.connect(self.save_dialog_settings, type=Qt.QueuedConnection)
+        self.save_button.clicked.connect(self.save_dialog_settings)
         f_layout = QFormLayout()
         f_layout.addRow("(requires password)", self.thermal_checkbox)
         f_layout.addRow(" ", self.always_on_checkbox)
         f_layout.addRow(" ", self.cpu_ave_freq_checkbox)
         f_layout.addRow(" ", None)
         f_layout.addRow("Monitoring Interval (milliseconds):",
                         self.interval_input)
         f_layout.addRow(" ", None)
         f_layout.addRow(self.save_button)
         self.settings_dialog.setLayout(f_layout)
         # set dialog geometry
         self.settings_dialog.setWindowTitle("Settings")
-        self.settings_dialog.setModal(False)
-        self.settings_dialog.adjustSize()
+        self.settings_dialog.setWindowModality(QtCore.Qt.ApplicationModal)
+        self.settings_dialog.setMaximumWidth(400)
+        self.settings_dialog.setMaximumHeight(400)
+        center_point = QScreen.availableGeometry(
+            QApplication.primaryScreen()).center()
+        fg = self.settings_dialog.frameGeometry()
+        fg.moveCenter(center_point)
+        self.settings_dialog.move(fg.topLeft())
 
     def load_sys_tray(self):
         """load_sys_tray.
 
         :param self:
         """
         # build desktop system tray
@@ -1556,19 +1526,19 @@
                 icon_file = Path(f'{str(Path.home())}/.local/share/icons/i8kgui_icon.png').resolve()
                 if not icon_file.is_file():
                     pass
             icon = QIcon(str(icon_file))
             if icon.pixmap(QSize(64, 64)).isNull():
                 icon = QIcon('icons/i8kgui_icon.png')
             self.tray.setIcon(icon)
-            self.tray.activated.connect(self.status, type=Qt.QueuedConnection)
-            self.tray.messageClicked.connect(self.message_clicked, type=Qt.QueuedConnection)
+            self.tray.activated.connect(self.status)
+            self.tray.messageClicked.connect(self.message_clicked)
             # workaround because tray activated only works with double click
-            self.tray_menu.aboutToShow.connect(self.monitor, type=Qt.QueuedConnection)
-            self.tray_menu.aboutToHide.connect(self.stop_monitor, type=Qt.QueuedConnection)
+            self.tray_menu.aboutToShow.connect(self.monitor)
+            self.tray_menu.aboutToHide.connect(self.stop_monitor)
             # setup display
             self.tray_menu.addAction(self.cpu_usage)
             self.tray_menu.addAction(self.cpu_temp)
             self.tray_menu.addAction(self.cpu_mhz)
             self.tray_menu.addAction(self.cpu_governor)
             self.connect_cpupower()
             self.tray_menu.addMenu(self.cpu_details)
@@ -1579,24 +1549,24 @@
             self.tray_menu.addAction(self.left_fan_status)
             self.tray_menu.addAction(self.right_fan_status)
             self.tray_menu.addSeparator()
             # setup thermal control management menu
             self.tray_menu.addMenu(self.thermal_control_menu)
             self.thermal_menu_group.setExclusive(True)
             self.thermal_menu_group.triggered.connect(
-                self.thermal_mode_selection, type=Qt.QueuedConnection)
+                self.thermal_mode_selection)
             self.build_thermal_menu()  # menu created based on settings
             self.tray_menu.addSeparator()
             # add info, settings and quit menu items
             action_info = self.tray_menu.addAction("Information")
-            action_info.triggered.connect(self.show_info, type=Qt.QueuedConnection)
+            action_info.triggered.connect(self.show_info)
             action_settings = self.tray_menu.addAction("Settings")
-            action_settings.triggered.connect(self.show_settings, type=Qt.QueuedConnection)
+            action_settings.triggered.connect(self.show_settings)
             action_quit = self.tray_menu.addAction("Quit")
-            action_quit.triggered.connect(self.close_app, type=Qt.QueuedConnection)
+            action_quit.triggered.connect(self.close_app)
 
             self.tray.setContextMenu(self.tray_menu)
             self.tray.setToolTip("i8kgui")
             self.tray.setVisible(True)
         else:
             QMessageBox.critical(
                 None, "i8kgui", "Unable to locate system tray on this system.")
@@ -1606,48 +1576,36 @@
         """connect_cpupower.
 
         :param self:
         """
         # connect to cpupower-gui if found
         cpupower_file = Path(str(shutil.which("cpupower-gui")))
         if cpupower_file.is_file():
-            self.cpu_governor.triggered.connect(self.show_cpupower, type=Qt.QueuedConnection)
+            self.cpu_governor.triggered.connect(self.show_cpupower)
         # TODO - if not found show message to user to install
 
     def show_cpupower(self):
         """show_cpupower.
 
         :param self:
         """
-        if self.cpupower is None:
-            self.cpupower = QProcess()
-            self.cpupower.finished.connect(self.show_cpupower_finished, type=Qt.QueuedConnection)
-            self.cpupower.errorOccurred.connect(self.show_cpupower_error, type=Qt.QueuedConnection)
-            self.cpupower.start(str(shutil.which("cpupower-gui")))
-            self.cpupower.waitForFinished(1000)
-
-    def show_cpupower_finished(self):
-        if self.cpupower:
-            print("Info: cpupower-gui finished")
-            if self.cpupower.state() != 0:
-                self.kill_process(self.cpupower)
-            self.cpupower = None
-
-    def show_cpupower_error(self):
-        if self.cpupower:
-            print("Error: cpupower-gui failed")
-            if self.cpupower.state() != 0:
-                self.kill_process(self.cpupower)
-            self.cpupower = None
-
-    def thermal_mode_selection(self, selected_mode):
-        """thermal_mode_selection. The purpose of this function is to switch the BIOS thermal mode based on the user's
-        input. If the `smbios-thermal-ctl` script is not found, the function prints an error and returns.
+        self.cpupower = QProcess()
+        self.cpupower.start("cpupower-gui")
+        self.cpupower.waitForFinished()
+        result = self.cpupower.readLine()
+        output = bytes(result).decode("utf8")
+        if error := output.strip('\n'):
+            print(f"Error: failed to load cpupower-gui {error}")
+        self.cpupower.close()
+        self.cpupower = None
+
+    def thermal_mode_selection(self, checked):
+        """thermal_mode_selection.
 
-        :param selected_mode: the BIOS thermal mode selected
+        :param checked:
         """
         if self.bios_thermal_control_on:
             if self.p is None:
                 # find libsmbios script
                 thermal_file = Path(str(shutil.which("smbios-thermal-ctl")))
                 if not thermal_file.is_file():
                     if self.tray:
@@ -1655,69 +1613,67 @@
                             "i8kgui",
                             "Error please install python3-libsmbios, "
                             "smbios-thermal-ctl not found.",
                             icon=QSystemTrayIcon.Critical,
                             msecs=10000)
                     return
                 # switch BIOS thermal mode (i.e. performance, balanced, etc)
-                if self.current_thermal_mode != selected_mode.text():
-                    self._set_thermal_mode_selection(selected_mode, thermal_file)
+                if self.current_thermal_mode != checked.text():
+                    self._set_thermal_mode_selection(checked, thermal_file)
         else:
             print("Edit i8kmon config")  # TODO - add i8kmon config updating
 
-    def _set_thermal_mode_selection(self, selected_mode, smbios_ctl_file):
-        """_set_thermal_mode_selection. The purpose of this function is to set the thermal mode by executing `pkexec`
-        with the appropriate arguments. It uses a QProcess to handle the execution of the `pkexec` command
-        and connect the necessary signals to handle the output, errors and state changes.
+    def _set_thermal_mode_selection(self, checked, thermal_file):
+        """_set_thermal_mode_selection.
 
         :param self:
-        :param selected_mode: the BIOS thermal mode selected
-        :param smbios_ctl_file:
+        :param checked:
+        :param thermal_file:
         """
         t_args = "--set-thermal-mode="
         t_args += (
-            self.thermal_modes[selected_mode.text()]
-            if selected_mode.text() in self.thermal_modes
+            self.thermal_modes[checked.text()]
+            if checked.text() in self.thermal_modes
             else 'balanced'
         )
         # Keep a reference to the QProcess (e.g. on self)
         # while it's running.
         self.p = QProcess()
         self.p.readyReadStandardOutput.connect(
-            self.handle_thermal_stdout, type=Qt.QueuedConnection)
+            self.handle_thermal_stdout)
         self.p.readyReadStandardError.connect(
-            self.handle_thermal_stderr, type=Qt.QueuedConnection)
-        self.p.stateChanged.connect(self.handle_process_state, type=Qt.QueuedConnection)
+            self.handle_thermal_stderr)
+        self.p.stateChanged.connect(self.handle_process_state)
         # Clean up once complete.
-        self.p.finished.connect(self.thermal_selection_finished, type=Qt.QueuedConnection)
-        self.p.start("pkexec", [str(smbios_ctl_file.resolve()), t_args])
+        self.p.finished.connect(self.thermal_selection_finished)
+        self.p.start("pkexec", [str(thermal_file.resolve()), t_args])
 
     @Slot()
     def message_clicked(self):
         """message_clicked.
 
         :param self:
         """
         self.close_app()
 
     def read_i8kmon_info(self):
         """read_i8kmon_info.
 
         :param self:
         """
-        with self.open_sysfs_file(self.i8kmon_fan1) as (fan1), \
-                self.open_sysfs_file(self.i8kmon_fan2) as (fan2), \
-                self.open_sysfs_file(self.i8kmon_fan1_target) as (fan1_target), \
-                self.open_sysfs_file(self.i8kmon_fan2_target) as (fan2_target), \
-                self.open_sysfs_file(self.i8kmon_temp) as (temp), \
-                self.open_sysfs_file(self.cpu_no_turbo) as (no_turbo), \
-                self.open_sysfs_file(self.cpu_min_perf) as (min_perf), \
-                self.open_sysfs_file(self.cpu_max_perf) as (max_perf), \
-                self.open_sysfs_file(self.cpu_min_scaling) as (min_scaling), \
-                self.open_sysfs_file(self.cpu_max_scaling) as (max_scaling):
+        with self.opened_w_error(self.i8kmon_fan1) as (fan1, fan1_err), \
+                self.opened_w_error(self.i8kmon_fan2) as (fan2, fan2_err), \
+                self.opened_w_error(self.i8kmon_fan1_target) as (fan1_target, fan1_target_err), \
+                self.opened_w_error(self.i8kmon_fan2_target) as (fan2_target, fan2_target_err), \
+                self.opened_w_error(self.i8kmon_temp) as (temp, temp_err), \
+                self.opened_w_error(self.cpu_no_turbo) as (no_turbo, no_turbo_err), \
+                self.opened_w_error(self.cpu_min_perf) as (min_perf, min_perf_err), \
+                self.opened_w_error(self.cpu_max_perf) as (max_perf, max_perf_err), \
+                self.opened_w_error(self.cpu_min_scaling) as (min_scaling, min_scaling_err), \
+                self.opened_w_error(self.cpu_max_scaling) as (max_scaling, max_scaling_err):
             i8kmon_fan1 = fan1.readline().strip('\n') if fan1 else "0"
             i8kmon_fan2 = fan2.readline().strip('\n') if fan2 else "0"
             i8kmon_fan1_target = fan1_target.readline().strip('\n') if fan1_target else "0"
             i8kmon_fan2_target = fan2_target.readline().strip('\n') if fan2_target else "0"
             i8kmon_temp = temp.readline().strip('\n') if temp else "0"
             cpu_no_turbo = no_turbo.readline().strip('\n') if no_turbo else "0"
             cpu_min_perf = min_perf.readline().strip('\n') if min_perf else "N/A"
@@ -1911,15 +1867,15 @@
             return
         self.read_power_supply_status()
         self.read_i8kmon_info()
         self.read_cpu_info()
         self.read_cpu_gov_info()
         # send fake single-click event as workaround
         if self.tray:
-            self.tray.activated.emit(QSystemTrayIcon.ActivationReason.Trigger)
+            self.tray.activated.emit(QSystemTrayIcon.Trigger)
 
     def update_i8k_ac_power(self):
         """update_i8k_ac_power.
 
         :param self:
         """
         # update i8k thermal menu fan mode based on A/C power supply status
@@ -2024,47 +1980,33 @@
             self.monitorTimer.stop()
 
     def show_settings(self):
         """show_settings.
 
         :param self:
         """
-        center_point = QScreen.availableGeometry(
-            QApplication.primaryScreen()).center()
-        fg = self.settings_dialog.frameGeometry()
-        fg.moveCenter(center_point)
-        self.settings_dialog.move(fg.topLeft())
         if not self.settings_dialog.isVisible():
             self.settings_dialog.show()
         self.settings_dialog.raise_()
         self.settings_dialog.setFocus()
-        pointer = self.cursor()
-        pointer.setPos(center_point)
 
     def show_info(self):
         """show_info.
 
         :param self:
         """
         if not self.is_i8kmon_active:
             return
         if self.i8kmon_ctl:
             with os.popen(self.i8kmon_ctl) as ctl:
                 self._get_i8kctl_info(ctl)
-        center_point = QScreen.availableGeometry(
-            QApplication.primaryScreen()).center()
-        fg = self.info_dialog.frameGeometry()
-        fg.moveCenter(center_point)
-        self.info_dialog.move(fg.topLeft())
         if not self.info_dialog.isVisible():
             self.info_dialog.show()
         self.info_dialog.raise_()
         self.info_dialog.setFocus()
-        pointer = self.cursor()
-        pointer.setPos(center_point)
 
     def _get_i8kctl_info(self, ctl):
         """_get_i8kctl_info.
 
         :param self:
         :param ctl:
         """
@@ -2072,29 +2014,28 @@
         split_line = line.split(" ")
         self.i8k_format_version.setText(split_line[0].strip())
         self.bios_version.setText(split_line[1].strip())
         self.service_tag.setText(split_line[2].strip())
         self.button_status.setText(split_line[9].strip())
 
     @contextmanager
-    def open_sysfs_file(self, f_name, mode="r"):
-        """open_sysfs_file. A context manager for 'with' for opening a possible missing file in Sysfs.
+    def opened_w_error(self, f_name, mode="r"):
+        """opened_w_error. A context manager for 'with' for opening a possible missing file.
 
         :param self:
         :param f_name:
         :param mode:
         """
         try:
             f = open(f_name, mode)
         except IOError as err:
-            print(f"Warn: Sysfs IOError {err}")
-            yield None
+            yield None, err
         else:
             try:
-                yield f
+                yield f, None
             finally:
                 f.close()
 
 
 if __name__ == '__main__':
     app = QApplication([])
     app.setOrganizationName("i8kgui")
@@ -2133,8 +2074,8 @@
     palette.setColor(QPalette.Disabled, QPalette.HighlightedText, Qt.black)
     # add Dark Mode to i8kgui
     app.setPalette(palette)
 
     app.setQuitOnLastWindowClosed(False)
     tray = I8kGui()
 
-    app.exec_()
+    app.exec()
```

### Comparing `i8kgui-0.8.4/i8kgui/i8kgui_thermal_control` & `i8kgui-0.8.4.dev0/i8kgui/i8kgui_thermal_control`

 * *Files identical despite different names*

### Comparing `i8kgui-0.8.4/i8kgui/icons/i8kgui_icon.png` & `i8kgui-0.8.4.dev0/i8kgui/icons/i8kgui_icon.png`

 * *Files identical despite different names*

### Comparing `i8kgui-0.8.4/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy` & `i8kgui-0.8.4.dev0/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy`

 * *Files 3% similar despite different names*

#### Comparing `i8kgui-0.8.4/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy` & `i8kgui-0.8.4.dev0/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy`

```diff
@@ -7,11 +7,11 @@
     <message gettext-domain="i8kgui">Authentication for i8kgui Thermal Control</message>
     <icon_name>i8kgui_icon</icon_name>
     <defaults>
       <allow_any>yes</allow_any>
       <allow_inactive>yes</allow_inactive>
       <allow_active>yes</allow_active>
     </defaults>
-    <annotate key="org.freedesktop.policykit.exec.path">I8KGUI_THERMAL_PATH/.local/bin/i8kgui_thermal_control</annotate>
+    <annotate key="org.freedesktop.policykit.exec.path">/usr/bin/i8kgui_thermal_control</annotate>
     <annotate key="org.freedesktop.policykit.exec.allow_gui">true</annotate>
   </action>
 </policyconfig>
```

### Comparing `i8kgui-0.8.4/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.smbios-thermal-ctl.policy` & `i8kgui-0.8.4.dev0/i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.smbios-thermal-ctl.policy`

 * *Files identical despite different names*

### Comparing `i8kgui-0.8.4/i8kgui.egg-info/PKG-INFO` & `i8kgui-0.8.4.dev0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: i8kgui
-Version: 0.8.4
-Summary: A Dell thermal management GUI to control fan speeds and monitor temperatures.
-Home-page: https://github.com/razman786/i8kgui
-Author: Raz
-Author-email: razman786@users.noreply.github.com
-License: GPL
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # I8KGUI
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/razman786/i8kgui/installation.yml?branch=master)  ![GitHub release (latest by date)](https://img.shields.io/github/v/release/razman786/i8kgui)
 
 ## Introduction
 
 A Dell thermal management GUI to control fan speeds and monitor temperatures.
@@ -53,43 +42,43 @@
 * Adds polkit action configurations to allow users to change fan modes without a
   password
 
 ## Installation
 
 ### Automated Installation (Recommended)
 
-This version has only been tested on Ubuntu 20.04/23.04 (it should also work on 22.04)
+This version has only been tested on Ubuntu 20.04 (it should also work on 22.04)
 and with a Dell laptop (XPS 7590). The installation script undertakes a
 system-wide installation with all optional components (i.e. `cpupower-gui` and
-`undervolt`). i8kgui itself is installed within a users `$HOME` directory. Please see below for other install options.
+`undervolt`). Please see below for other install options.
 
 ```
 git clone https://github.com/razman786/i8kgui
 cd i8kgui
 ./install_i8kgui_ubuntu.sh
 ```
 
 #### Automated Installation Options
 
 Install option | i8kutils | Dell BIOS fan control | libsmbios | cpupower-gui | undervolt
-:---:|:---:|:---:|:---:|:---:|:---:|
-`-all` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | 
-`-norm` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | |
-`-min` | :heavy_check_mark: |
-`-fix` | :heavy_check_mark: | :heavy_check_mark: |
-`-smbios` | :heavy_check_mark: | | :heavy_check_mark: |
-`-power` | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | 
+:---|:---:|:---:|:---:|:---:|:---:
+`-all` | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark:
+`-norm` | :white_check_mark: | :white_check_mark: | :white_check_mark: |  |
+`-min` | :white_check_mark: | | |  |
+`-fix` | :white_check_mark: | :white_check_mark: | |  |
+`-smbios` | :white_check_mark: | | :white_check_mark: |  |
+`-power` | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 
 See `./install_i8kgui_ubuntu.sh -h` for usage information.
 
 ### Manual Installation
 
 #### Prerequisites
 
-This guide has only been tested on Ubuntu 20.04/23.04 and with a Dell XPS laptop.
+This guide has only been tested on Ubuntu 20.04 and with a Dell XPS laptop.
 
 The [dell-smm-hwmon](https://www.kernel.org/doc/html/latest/hwmon/dell-smm-hwmon.html)
 kernel module is required for basic functionality.
 
 ##### i8kutils
 
 Please install and configure i8kutils from
@@ -127,95 +116,79 @@
 sudo cp dell-bios-fan-control.service /etc/systemd/system/
 sudo systemctl enable dell-bios-fan-control.service
 ```
 
 ##### libsmbios (optional)
 
 If supported by your system, libsmbios will allow BIOS thermal modes to be changed, amongst other
-features. On Ubuntu, please install the following package to interface with (SM)BIOS
+features. On Ubuntu 20.04, please install the following package to interface with (SM)BIOS
 information:
 
 ```
 sudo apt install python3-libsmbios
 ```
 
 ##### cpupower-gui (optional)
 
-On Ubuntu, install the following optional package to change the CPU
+On Ubuntu 20.04, install the following optional package to change the CPU
 Governor:
 
 ```
 sudo apt install cpupower-gui
 ```
 
-##### polkit actions (optional)
+#### i8kgui Installation
 
-The polkit action files will allow thermal controls to be changed without
-requiring a user password. If your installation of `i8kgui` is frequently asking
-for a password, please do the following:
+##### System-wide with polkit actions (Recommended)
 
-Using a text editor, change the `I8KGUI_THERMAL_PATH` placeholder in the 
-`i8kgui/polkit_actions/ubuntu/com.ubuntu.pkexec.i8kgui_thermal_control.policy` file to the correct location, i.e. `/home/someuser`
+###### Using PyPI
 
-To manually install the polkit action files, do the following:
 ```
-sudo cp i8kgui/polkit_actions/ubuntu/* /usr/share/polkit-1/actions
+sudo pip3 install i8kgui --prefix=/usr
 ```
 
-Please note that, the installation script by default will use the polkit action files for
-Ubuntu. Polkit action files for Manjaro Linux (tested with version 22.1.3) are
-located in `i8kgui/polkit_actions/manjaro`. 
-
-#### i8kgui Installation
-
-###### Using PyPI
+###### Using Git
 
-On Ubuntu 20.04 and 22.04 use the following:
 ```
-pip3 install i8kgui --user
+git clone https://github.com/razman786/i8kgui
+sudo pip3 install . --prefix=/usr
 ```
 
-For Ubuntu 23.04 the command needs to be altered:
-```
-pip3 install i8kgui --user --break-system-packages
-```
+Please note that the default installation will use the polkit action files for
+Ubuntu. Polkit action files for Manjaro Linux (tested with version 22.1.3) are
+located in `i8kgui/polkit_actions/manjaro`. For example, to manually install the
+polkit action files, do the following `sudo cp i8kgui/polkit_actions/ubuntu/* /usr/share/polkit-1/actions`
 
-###### Using Git
+##### Stable
 
 ```
 git clone https://github.com/razman786/i8kgui
-```
-On Ubuntu 20.04 and 22.04 use the following:
-```
 pip3 install . --user
 ```
 
-For Ubuntu 23.04 the command is as follows:
-```
-pip3 install . --user --break-system-packages
-```
-
-##### Development version
+##### Development
 
 ```
 git clone https://github.com/razman786/i8kgui
 git checkout development && git pull
 pip3 install . --user
 ```
 
 #### Uninstall i8kgui
 
-For Ubuntu 20.04 and 22.04 use the following:
+##### System-wide with polkit actions
+
 ```
-pip3 uninstall i8kgui
+sudo PYTHONUSERBASE=/usr pip3 uninstall i8kgui
 ```
 
-For Ubuntu 23.04 use the following:
+##### Stable or Development
+
 ```
-pip3 uninstall i8kgui --break-system-packages
+pip3 uninstall i8kgui
 ```
 
 ## Usage
 
 Please ensure that you have configured i8kutils *before* starting!
 
 Once i8kutils is correctly configured using the `/etc/i8kmon.conf` file, please
```

### Comparing `i8kgui-0.8.4/setup.py` & `i8kgui-0.8.4.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from pathlib import Path
 
-__version__ = "0.8.4"
+__version__ = "0.8.4-dev"
 
 requirements = [
     'PySide6',
     'psutil',
     'py-cpuinfo',
 ]
```


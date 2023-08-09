# Comparing `tmp/lastfm-mpris2-scrobbler-1.0.0.tar.gz` & `tmp/lastfm-mpris2-scrobbler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastfm-mpris2-scrobbler-1.0.0.tar", last modified: Tue Aug  8 15:25:42 2023, max compression
+gzip compressed data, was "lastfm-mpris2-scrobbler-1.0.1.tar", last modified: Wed Aug  9 02:45:21 2023, max compression
```

## Comparing `lastfm-mpris2-scrobbler-1.0.0.tar` & `lastfm-mpris2-scrobbler-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-1.0.0/LICENSE
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     3561 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     3264 2023-08-08 15:20:01.000000 lastfm-mpris2-scrobbler-1.0.0/README.md
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2460 2023-08-08 14:56:15.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/Cache.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2407 2023-08-08 14:44:07.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/PlayerState.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     5606 2023-08-08 14:57:19.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/Scrobbler.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/__init__.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1449 2023-08-08 14:02:15.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/__main__.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      180 2023-08-08 14:05:27.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/globals.py
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     3561 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      572 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       82 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       45 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/requires.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       24 2023-08-08 15:25:42.000000 lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/top_level.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-08 15:25:42.938163 lastfm-mpris2-scrobbler-1.0.0/setup.cfg
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      912 2023-08-08 15:24:00.000000 lastfm-mpris2-scrobbler-1.0.0/setup.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-09 02:45:21.282813 lastfm-mpris2-scrobbler-1.0.1/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-1.0.1/LICENSE
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     3829 2023-08-09 02:45:21.282813 lastfm-mpris2-scrobbler-1.0.1/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     3532 2023-08-09 02:38:42.000000 lastfm-mpris2-scrobbler-1.0.1/README.md
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-09 02:45:21.282813 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2460 2023-08-08 14:56:15.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/Cache.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2407 2023-08-08 14:44:07.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/PlayerState.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     5958 2023-08-09 02:43:23.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/Scrobbler.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/__init__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1449 2023-08-08 14:02:15.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/__main__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      180 2023-08-09 02:27:10.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/globals.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-09 02:45:21.282813 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     3829 2023-08-09 02:45:21.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      572 2023-08-09 02:45:21.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-09 02:45:21.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       82 2023-08-09 02:45:21.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       45 2023-08-09 02:45:21.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/requires.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       24 2023-08-09 02:45:21.000000 lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/top_level.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-09 02:45:21.282813 lastfm-mpris2-scrobbler-1.0.1/setup.cfg
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      912 2023-08-09 02:30:23.000000 lastfm-mpris2-scrobbler-1.0.1/setup.py
```

### Comparing `lastfm-mpris2-scrobbler-1.0.0/LICENSE` & `lastfm-mpris2-scrobbler-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-1.0.0/PKG-INFO` & `lastfm-mpris2-scrobbler-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -118,7 +118,19 @@
 ```
 
 ## Alternatives
 
 If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez). It additionally provides Spotify related improvement, but doesn't provide stand-alone binary build for installation.
 
 Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
+
+## Known Issues
+
+- ~~If the music title contains unwanted substring (like `.mp3`), then Last.fm won't accept the scrobble~~
+
+    The program can now remove some of the unwanted substrings, including:
+
+    - `.mp3`
+    - `.ogg`
+    - `.wav`
+    - `.acc`
+    - `.flac`
```

### Comparing `lastfm-mpris2-scrobbler-1.0.0/README.md` & `lastfm-mpris2-scrobbler-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -107,7 +107,19 @@
 ```
 
 ## Alternatives
 
 If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez). It additionally provides Spotify related improvement, but doesn't provide stand-alone binary build for installation.
 
 Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
+
+## Known Issues
+
+- ~~If the music title contains unwanted substring (like `.mp3`), then Last.fm won't accept the scrobble~~
+
+    The program can now remove some of the unwanted substrings, including:
+
+    - `.mp3`
+    - `.ogg`
+    - `.wav`
+    - `.acc`
+    - `.flac`
```

### Comparing `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/Cache.py` & `lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/Cache.py`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/PlayerState.py` & `lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/PlayerState.py`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/Scrobbler.py` & `lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/Scrobbler.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             self.init_network()
         scrobble_list = []
         for uri, player_obj in self.player_dict.items():
             if player_obj.playback_status == "Playing" and self.network is not None:
                 try:
                     self.network.update_now_playing(
                         artist=player_obj.artist,
-                        title=player_obj.title,
+                        title=self.fix_title(player_obj.title),
                         album=player_obj.album,
                         album_artist=player_obj.albumArtist,
                         track_number=player_obj.trackNumber,
                     )
                 except Exception as e:
                     logger.error(f"Failed to report now playing status")
             if player_obj.total_played_time >= min(self.scrobble_time_threshold, int(player_obj.length / 2)) and not player_obj.if_scrobbled:
@@ -119,16 +119,29 @@
 
     def obj_list_to_dict_list(self, obj_list):
         dict_list = []
         for obj in obj_list:
             dict_list.append(
                 {
                     "artist": obj.artist,
-                    "title": obj.title,
+                    "title": self.fix_title(obj.title),
                     "timestamp": obj.last_observation_timestamp,
                     "album": obj.album,
                     "album_artist": obj.albumArtist,
                     "track_number": obj.trackNumber,
                     "duration": obj.length,
                 }
             )
         return dict_list
+    
+    def fix_title(self, title):
+        audio_formats = [
+            '.mp3', 
+            '.ogg', 
+            '.wav', 
+            '.aac', 
+            '.flac'
+        ]
+        for format in audio_formats:
+            if title.endswith(format):
+                return title[:-(len(format))]
+        return title
```

### Comparing `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler/__main__.py` & `lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler/__main__.py`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO` & `lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -118,7 +118,19 @@
 ```
 
 ## Alternatives
 
 If you'd like a scrobbler similar to this, there're some choices. I recommand taking a look at [scrobblez](https://github.com/YodaEmbedding/scrobblez). It additionally provides Spotify related improvement, but doesn't provide stand-alone binary build for installation.
 
 Also, although [rescrobbled](https://github.com/InputUsername/rescrobbled) may also work, in my case it raised "Dbus error: argument type mismatch".
+
+## Known Issues
+
+- ~~If the music title contains unwanted substring (like `.mp3`), then Last.fm won't accept the scrobble~~
+
+    The program can now remove some of the unwanted substrings, including:
+
+    - `.mp3`
+    - `.ogg`
+    - `.wav`
+    - `.acc`
+    - `.flac`
```

### Comparing `lastfm-mpris2-scrobbler-1.0.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt` & `lastfm-mpris2-scrobbler-1.0.1/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-1.0.0/setup.py` & `lastfm-mpris2-scrobbler-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 root = path.abspath(path.dirname(__file__))
 with open(path.join(root, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='lastfm-mpris2-scrobbler',
-    version='1.0.0',
+    version='1.0.1',
     description="Last.fm scrobbler via MPRIS2 in Linux",
     url="https://github.com/Ladbaby/lastfm-scrobbler",
     author="Ladbaby",
     author_email="Ladbabyms@outlook.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
```


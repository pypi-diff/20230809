# Comparing `tmp/whisper_mic-1.1.1.tar.gz` & `tmp/whisper_mic-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_mic-1.1.1.tar", last modified: Wed Jul  5 06:08:27 2023, max compression
+gzip compressed data, was "whisper_mic-1.2.0.tar", last modified: Wed Aug  9 05:32:27 2023, max compression
```

## Comparing `whisper_mic-1.1.1.tar` & `whisper_mic-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/
--rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.1.1/LICENSE
--rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)     3231 2023-06-29 22:23:36.000000 whisper_mic-1.1.1/README.md
--rw-rw-r--   0 blake     (1000) blake     (1000)      821 2023-07-05 06:08:00.000000 whisper_mic-1.1.1/pyproject.toml
--rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/setup.cfg
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/whisper_mic/
--rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.1.1/whisper_mic/__init__.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)     1606 2023-07-05 06:07:43.000000 whisper_mic-1.1.1/whisper_mic/cli.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)      480 2023-07-05 05:53:32.000000 whisper_mic-1.1.1/whisper_mic/utils.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)     4383 2023-07-05 06:07:43.000000 whisper_mic-1.1.1/whisper_mic/whisper_mic.py
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/whisper_mic.egg-info/
--rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)      335 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/SOURCES.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/dependency_links.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/entry_points.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)      187 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/requires.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/top_level.txt
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-08-09 05:32:27.524331 whisper_mic-1.2.0/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.2.0/LICENSE
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3653 2023-08-09 05:32:27.524331 whisper_mic-1.2.0/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3356 2023-08-09 05:27:46.000000 whisper_mic-1.2.0/README.md
+-rw-rw-r--   0 blake     (1000) blake     (1000)      835 2023-08-09 05:32:20.000000 whisper_mic-1.2.0/pyproject.toml
+-rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-08-09 05:32:27.524331 whisper_mic-1.2.0/setup.cfg
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-08-09 05:32:27.520331 whisper_mic-1.2.0/whisper_mic/
+-rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.2.0/whisper_mic/__init__.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     2077 2023-08-09 05:27:46.000000 whisper_mic-1.2.0/whisper_mic/cli.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)      480 2023-07-05 05:53:32.000000 whisper_mic-1.2.0/whisper_mic/utils.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     4790 2023-08-09 05:27:46.000000 whisper_mic-1.2.0/whisper_mic/whisper_mic.py
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-08-09 05:32:27.524331 whisper_mic-1.2.0/whisper_mic.egg-info/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3653 2023-08-09 05:32:27.000000 whisper_mic-1.2.0/whisper_mic.egg-info/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)      335 2023-08-09 05:32:27.000000 whisper_mic-1.2.0/whisper_mic.egg-info/SOURCES.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-08-09 05:32:27.000000 whisper_mic-1.2.0/whisper_mic.egg-info/dependency_links.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-08-09 05:32:27.000000 whisper_mic-1.2.0/whisper_mic.egg-info/entry_points.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)      194 2023-08-09 05:32:27.000000 whisper_mic-1.2.0/whisper_mic.egg-info/requires.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-08-09 05:32:27.000000 whisper_mic-1.2.0/whisper_mic.egg-info/top_level.txt
```

### Comparing `whisper_mic-1.1.1/LICENSE` & `whisper_mic-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_mic-1.1.1/PKG-INFO` & `whisper_mic-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: whisper_mic
-Version: 1.1.1
+Version: 1.2.0
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Whisper Mic
-This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
+This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from the original project.
 
 ## Video Tutorial
 
-See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
+The latest video tutorial for this repo can be seen [here](https://youtu.be/S58MGCU7Wgg)
 
-The video is a bit out of date now.  The code is much better now and pip installable
+An older video tutorial for this repo can be seen [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
 
 ### Professional Assistance
 
 If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
 
 ## Setup
 
@@ -47,14 +47,18 @@
 
 ## Microphone Demo
 
 You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
+## Transcribing To A File
+
+Using the command: ```whisper_mic --loop --dictate``` will type the words you say on your active cursor.
+
 ## Usage In Other Projects
 
 You can use this code in other projects rather than just use it for a demo.  You can do this with the ```listen``` method.
 
 ```python
 from whisper_mic.whisper_mic import WhisperMic
 
@@ -63,15 +67,15 @@
 print(result)
 ```
 
 Check out what the possible arguments are by looking at the ```cli.py``` file
 
 ## Troubleshooting
 
-If you are having issues with the ```mic.py``` not running try the following:
+If you are having issues, try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
 ## Contributing
 
 Some ideas that you can add are:
```

### Comparing `whisper_mic-1.1.1/README.md` & `whisper_mic-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Whisper Mic
-This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
+This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from the original project.
 
 ## Video Tutorial
 
-See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
+The latest video tutorial for this repo can be seen [here](https://youtu.be/S58MGCU7Wgg)
 
-The video is a bit out of date now.  The code is much better now and pip installable
+An older video tutorial for this repo can be seen [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
 
 ### Professional Assistance
 
 If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
 
 ## Setup
 
@@ -35,14 +35,18 @@
 
 ## Microphone Demo
 
 You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
+## Transcribing To A File
+
+Using the command: ```whisper_mic --loop --dictate``` will type the words you say on your active cursor.
+
 ## Usage In Other Projects
 
 You can use this code in other projects rather than just use it for a demo.  You can do this with the ```listen``` method.
 
 ```python
 from whisper_mic.whisper_mic import WhisperMic
 
@@ -51,15 +55,15 @@
 print(result)
 ```
 
 Check out what the possible arguments are by looking at the ```cli.py``` file
 
 ## Troubleshooting
 
-If you are having issues with the ```mic.py``` not running try the following:
+If you are having issues, try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
 ## Contributing
 
 Some ideas that you can add are:
```

### Comparing `whisper_mic-1.1.1/pyproject.toml` & `whisper_mic-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_mic"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "speechrecognition",
+    'importlib-metadata; python_version>"3.9"',
+    "attrs",
+    "click",
+    "ffmpeg-python",
+    "more-itertools",
+    "numpy",
+    "openai-whisper",
     "pyaudio",
+    "pydantic",
     "pydub",
+    "pynput",
     "requests",
-    "pydantic",
-    "attrs",
-    "numpy",
+    "rich",
+    "speechrecognition",
     "tdqm",
-    "more-itertools",
-    "transformers",
     "torch",
-    "ffmpeg-python",
-    "click",
-    "openai-whisper",
-    "rich",
-    'importlib-metadata; python_version>"3.9"'
+    "transformers",
 ]
 
 [project.scripts]
 whisper_mic = "whisper_mic.cli:main"
-
```

### Comparing `whisper_mic-1.1.1/whisper_mic/cli.py` & `whisper_mic-1.2.0/whisper_mic/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-import io
-from pydub import AudioSegment
-import speech_recognition as sr
-import whisper
-import queue
-import tempfile
-import os
-import threading
+#!/usr/bin/env python3
+
 import click
 import torch
-import numpy as np
+import speech_recognition as sr
+from typing import Optional
 
 from whisper_mic.whisper_mic import WhisperMic
 
 @click.command()
 @click.option("--model", default="base", help="Model to use", type=click.Choice(["tiny","base", "small","medium","large"]))
 @click.option("--device", default=("cuda" if torch.cuda.is_available() else "cpu"), help="Device to use", type=click.Choice(["cpu","cuda","mps"]))
 @click.option("--english", default=False, help="Whether to use English model",is_flag=True, type=bool)
 @click.option("--verbose", default=False, help="Whether to print verbose output", is_flag=True,type=bool)
 @click.option("--energy", default=300, help="Energy level for mic to detect", type=int)
 @click.option("--dynamic_energy", default=False,is_flag=True, help="Flag to enable dynamic energy", type=bool)
 @click.option("--pause", default=0.8, help="Pause time before entry ends", type=float)
 @click.option("--save_file",default=False, help="Flag to save file", is_flag=True,type=bool)
 @click.option("--loop", default=False, help="Flag to loop", is_flag=True,type=bool)
-def main(model, english,verbose, energy, pause,dynamic_energy,save_file,device,loop):
-    mic = WhisperMic(model=model, english=english, verbose=verbose, energy=energy, pause=pause, dynamic_energy=dynamic_energy, save_file=save_file, device=device)
+@click.option("--dictate", default=False, help="Flag to dictate (implies loop)", is_flag=True,type=bool)
+@click.option("--mic_index", default=None, help="Mic index to use", type=int)
+@click.option("--list_devices",default=False, help="Flag to list devices", is_flag=True,type=bool)
+def main(model: str, english: bool, verbose: bool, energy:  int, pause: float, dynamic_energy: bool, save_file: bool, device: str, loop: bool, dictate: bool,mic_index:Optional[int],list_devices:bool) -> None:
+    if list_devices:
+        print("Possible devices: ",sr.Microphone.list_microphone_names())
+        return
+    mic = WhisperMic(model=model, english=english, verbose=verbose, energy=energy, pause=pause, dynamic_energy=dynamic_energy, save_file=save_file, device=device,mic_index=mic_index)
     if not loop:
         result = mic.listen()
         print("You said: " + result)
     else:
-        mic.listen_loop()
+        mic.listen_loop(dictate=dictate)
 
 if __name__ == "__main__":
     main()
```

### Comparing `whisper_mic-1.1.1/whisper_mic/whisper_mic.py` & `whisper_mic-1.2.0/whisper_mic/whisper_mic.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,55 +6,59 @@
 import io
 import numpy as np
 from pydub import AudioSegment
 import os
 import tempfile
 import time
 import platform
+import pynput.keyboard
 
 from whisper_mic.utils import get_logger
 
 
 class WhisperMic:
-    def __init__(self,model="base",device=("cuda" if torch.cuda.is_available() else "cpu"),english=False,verbose=False,energy=300,pause=0.8,dynamic_energy=False,save_file=False):
+    def __init__(self,model="base",device=("cuda" if torch.cuda.is_available() else "cpu"),english=False,verbose=False,energy=300,pause=0.8,dynamic_energy=False,save_file=False, model_root="~/.cache/whisper",mic_index=None):
         self.logger = get_logger("whisper_mic", "info")
         self.energy = energy
         self.pause = pause
         self.dynamic_energy = dynamic_energy
         self.save_file = save_file
         self.verbose = verbose
         self.english = english
+        self.keyboard = pynput.keyboard.Controller()
 
         self.platform = platform.system()
 
         if self.platform == "darwin":
             if device == "mps":
                 self.logger.warning("Using MPS for Mac, this does not work but may in the future")
                 device = "mps"
                 device = torch.device(device)
 
         if model != "large" and self.english:
             model = model + ".en"
-
-        self.audio_model = whisper.load_model(model).to(device)
+        
+        self.audio_model = whisper.load_model(model, download_root=model_root).to(device)
         self.temp_dir = tempfile.mkdtemp() if save_file else None
 
         self.audio_queue = queue.Queue()
-        self.result_queue = queue.Queue()
+        self.result_queue: "queue.Queue[str]" = queue.Queue()
 
         self.break_threads = False
         self.mic_active = False
 
         self.banned_results = [""," ","\n",None]
 
-        self.setup_mic()
+        self.setup_mic(mic_index)
 
 
-    def setup_mic(self):
-        self.source = sr.Microphone(sample_rate=16000)
+    def setup_mic(self, mic_index):
+        if mic_index is None:
+            self.logger.info("No mic index provided, using default")
+        self.source = sr.Microphone(sample_rate=16000, device_index=mic_index)
 
         self.recorder = sr.Recognizer()
         self.recorder.energy_threshold = self.energy
         self.recorder.pause_threshold = self.pause
         self.recorder.dynamic_energy_threshold = self.dynamic_energy
 
         with self.source:
@@ -62,44 +66,43 @@
 
         self.recorder.listen_in_background(self.source, self.record_callback, phrase_time_limit=2)
         self.logger.info("Mic setup complete, you can now talk")
 
 
     def preprocess(self, data):
         return torch.from_numpy(np.frombuffer(data, np.int16).flatten().astype(np.float32) / 32768.0)
-    
-    def get_all_audio(self,min_time=-1):
+
+    def get_all_audio(self, min_time: float = -1.):
         audio = bytes()
         got_audio = False
         time_start = time.time()
         while not got_audio or time.time() - time_start < min_time:
             while not self.audio_queue.empty():
                 audio += self.audio_queue.get()
                 got_audio = True
 
         data = sr.AudioData(audio,16000,2)
         data = data.get_raw_data()
         return data
 
 
-    def record_callback(self,_, audio:sr.AudioData) -> None:
+    def record_callback(self,_, audio: sr.AudioData) -> None:
         data = audio.get_raw_data()
         self.audio_queue.put_nowait(data)
 
 
-    def transcribe_forever(self):
+    def transcribe_forever(self) -> None:
         while True:
             if self.break_threads:
                 break
             self.transcribe()
 
 
-    def transcribe(self,data=None,realtime=False):
+    def transcribe(self,data=None, realtime: bool = False) -> None:
         if data is None:
-            # audio_data = self.audio_queue.get()
             audio_data = self.get_all_audio()
         else:
             audio_data = data
         audio_data = self.preprocess(audio_data)
         if self.english:
             result = self.audio_model.transcribe(audio_data,language='english')
         else:
@@ -113,31 +116,33 @@
             if predicted_text not in self.banned_results:
                 self.result_queue.put_nowait(result)
 
         if self.save_file:
             os.remove(audio_data)
 
 
-    def listen_loop(self):
+    def listen_loop(self, dictate: bool = False) -> None:
         threading.Thread(target=self.transcribe_forever).start()
         while True:
             result = self.result_queue.get()
-            print(result)
-                
+            if dictate:
+                self.keyboard.type(result)
+            else:
+                print(result)
 
-    def listen(self,timout=3):
-        audio_data = self.get_all_audio(timout)
+
+    def listen(self, timeout: int = 3):
+        audio_data = self.get_all_audio(timeout)
         self.transcribe(data=audio_data)
         while True:
             if not self.result_queue.empty():
                 return self.result_queue.get()
-            
-    def toggle_microphone(self):
+
+    def toggle_microphone(self) -> None:
         #TO DO: make this work
         self.mic_active = not self.mic_active
         if self.mic_active:
             print("Mic on")
         else:
             print("turning off mic")
             self.mic_thread.join()
-            print("Mic off")
-    
+            print("Mic off")
```

### Comparing `whisper_mic-1.1.1/whisper_mic.egg-info/PKG-INFO` & `whisper_mic-1.2.0/whisper_mic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: whisper-mic
-Version: 1.1.1
+Version: 1.2.0
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Whisper Mic
-This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from original project.
+This repo is based on the work done [here](https://github.com/openai/whisper) by OpenAI.  This repo allows you use use a mic as demo. This repo copies some of the README from the original project.
 
 ## Video Tutorial
 
-See the video tutorial for this repo [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
+The latest video tutorial for this repo can be seen [here](https://youtu.be/S58MGCU7Wgg)
 
-The video is a bit out of date now.  The code is much better now and pip installable
+An older video tutorial for this repo can be seen [here](https://www.youtube.com/watch?v=nwPaRSlDSaY)
 
 ### Professional Assistance
 
 If are in need of paid professional help, that is available through this [email](mailto:blakecmallory@gmail.com)
 
 ## Setup
 
@@ -47,14 +47,18 @@
 
 ## Microphone Demo
 
 You can use the model with a microphone using the ```whisper_mic``` program.  Use ```-h``` to see flag options.
 
 Some of the more important flags are the ```--model``` and ```--english``` flags.
 
+## Transcribing To A File
+
+Using the command: ```whisper_mic --loop --dictate``` will type the words you say on your active cursor.
+
 ## Usage In Other Projects
 
 You can use this code in other projects rather than just use it for a demo.  You can do this with the ```listen``` method.
 
 ```python
 from whisper_mic.whisper_mic import WhisperMic
 
@@ -63,15 +67,15 @@
 print(result)
 ```
 
 Check out what the possible arguments are by looking at the ```cli.py``` file
 
 ## Troubleshooting
 
-If you are having issues with the ```mic.py``` not running try the following:
+If you are having issues, try the following:
 ```
 sudo apt install portaudio19-dev python3-pyaudio
 ```
 
 ## Contributing
 
 Some ideas that you can add are:
```


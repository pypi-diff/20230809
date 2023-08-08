# Comparing `tmp/oszsave-1.2.0.tar.gz` & `tmp/oszsave-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oszsave-1.2.0.tar", max compression
+gzip compressed data, was "oszsave-1.3.0.tar", max compression
```

## Comparing `oszsave-1.2.0.tar` & `oszsave-1.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    23818 2023-08-06 01:49:19.559274 oszsave-1.2.0/oszsave.py
--rw-r--r--   0        0        0      404 2023-08-06 14:44:18.300134 oszsave-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6294 2023-08-04 05:52:24.947996 oszsave-1.2.0/README.md
--rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 oszsave-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    28248 2023-08-08 23:26:04.107669 oszsave-1.3.0/oszsave.py
+-rw-r--r--   0        0        0      443 2023-08-08 23:29:56.338727 oszsave-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4076 2023-08-08 23:32:48.868218 oszsave-1.3.0/README.md
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 oszsave-1.3.0/PKG-INFO
```

### Comparing `oszsave-1.2.0/oszsave.py` & `oszsave-1.3.0/oszsave.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,52 @@
 import json
 # random module is used to perform the random generations.
 import random
 # datetime module supplies classes to work with date and time. These classes provide a number of functions to deal with dates, times and time intervals.
 from datetime import datetime
 # shutil module in Python provides many functions of high-level operations on files and collections of files. It comes under Python’s standard utility modules.
 import shutil
+# tqdm provides a fast progress bar for loops and tasks in a visually appealing manner.
+from tqdm import tqdm
+# colorama provides cross-platform support for colored terminal text in Python
+from colorama import init, Fore
+
+
+init(autoreset=True)  # This will auto-reset the color after each print statement.
+CURRENT_VERSION = "1.3.0" # Current version number 
+
+
+# ----------------------------- A story ------------------------------------
+
+# One day, I was trying to move my OSU! Songs to  a different computer via
+# remote desktop software. I somehow, accidentally deleted all my beatmaps,
+# and I REALLY did not want to go down the list of every. single. freaking
+# beatmap that I had ever played. So I started making a javascript console
+# script to go down and open every 'show more' button there was. However, 
+# I still didnt have a way to download them. Finally, what you have now 
+# something that combines the two, and allows you to download every beatmap
+# off of a user profile. And I hope that it is of similar helpfulness to you.
+# - ForgedCore8
+
+
+# --------------------------------------------------------------------------
+
+# Define the banner as ASCII art
+
+banner = """
+  ██████╗ ███████╗███████╗███████╗ █████╗ ██╗   ██╗███████╗
+ ██╔═══██╗██╔════╝╚══███╔╝██╔════╝██╔══██╗██║   ██║██╔════╝
+ ██║   ██║███████╗  ███╔╝ ███████╗███████║██║   ██║█████╗  
+ ██║   ██║╚════██║ ███╔╝  ╚════██║██╔══██║╚██╗ ██╔╝██╔══╝  
+ ╚██████╔╝███████║███████╗███████║██║  ██║ ╚████╔╝ ███████╗
+  ╚═════╝ ╚══════╝╚══════╝╚══════╝╚═╝  ╚═╝  ╚═══╝  ╚══════╝
+ ██████████████████████████████████████████████████████████╗
+ ╚═════════════════════════════════════════════════════════╝
+"""
+
 
 # --------------------------------------------------------------------------
 
 # Function to scrape user profiles and collect download URLs
 def scraper():
 
     # List to store URLs collected
@@ -405,23 +443,35 @@
     qs = parse.parse_qs(url)
     # Define the directory where the file will be downloaded
     download_path = os.path.join(os.getcwd(), 'downloaded')
     # If the directory does not exist, create it
     if not os.path.exists(download_path):
         os.makedirs(download_path)
     # Sanitize the filename and join it with the download path
-    filename = os.path.join(download_path, sanitize(qs[list(qs.keys())[0]][0]))
-    # Open the file and write the content from the URL into it
+    sanitized_filename = sanitize(qs[list(qs.keys())[0]][0])
+    filename = os.path.join(download_path, sanitized_filename)
+
+    # Stream the download with progress bar
     with open(filename, "wb") as fp, httpx.stream("GET", url, headers=headers, timeout=None) as r:
-        for data in r.iter_bytes():
-            fp.write(data)
+        total = int(r.headers.get("content-length", 0))
+
+        # Custom bar_format with progress bar starting at a fixed position
+        bar_format = f"{sanitized_filename[:50]:<50} {' ':<10}|{{bar:40}}| {{n_fmt}}/{{total_fmt}} [{{elapsed}}<{{remaining}}]"
+
+        with tqdm(total=total, unit="B", unit_scale=True, unit_divisor=1024, bar_format=bar_format, position=0, leave=False) as bar:
+            for data in r.iter_bytes():
+                bar.update(len(data))
+                fp.write(data)
+
     return filename
 
+
 # --------------------------------------------------------------------------
 
+
 # Function to check if a particular task is done
 def check_done(chk):
     # It checks from a json file called 'done.json'
     filename = os.path.join(os.getcwd(), 'config', 'done.json')
     # If the file does not exist, create it and write an empty json array
     if not os.path.exists(filename):
         with open(filename, "w") as fp:
@@ -534,39 +584,81 @@
         return
     
     # Create the songs folder if it doesn't already exist
     songs_folder = os.path.join(destination_folder, "Songs")
     os.makedirs(songs_folder, exist_ok=True)
 
     # Define the source folder (where the beatmaps are downloaded to)
-    source_folder = os.path.join(os.path.dirname(__file__), 'downloaded')
+    source_folder = os.path.join(os.getcwd(), 'downloaded')
+
+    # Check if the source folder is empty
+    if not os.listdir(source_folder):
+        print("The downloads folder is empty. No files to move.")
+        return
 
     # Get user confirmation before moving the files
     confirmation = input(f"Do you want to move all beatmaps to {songs_folder}? (y/n): ")
     if confirmation.lower() != 'y':
         print("The beatmaps have been left in the download folder.")
         return
     
     # Move all the .osz files from the source to the songs folder
     for filename in os.listdir(source_folder):
         if filename.endswith(".osz"):
-            shutil.move(os.path.join(source_folder, filename), songs_folder)
+            try:
+                shutil.move(os.path.join(source_folder, filename), songs_folder)
+            except Exception as e:
+                print(f"Error moving {filename}: {e}")
+                continue
 
     # Print a success message
     print(f"All files moved to {songs_folder}")
 
 # --------------------------------------------------------------------------
 
+def clear_console():
+    os.system('cls' if os.name == 'nt' else 'clear')
+
+# --------------------------------------------------------------------------
+
+def check_for_updates():
+    # Define the GitHub API endpoint for your repo's releases
+    repo_url = "https://api.github.com/repos/ForgedCore8/OSZsave/releases/latest"
+    
+    try:
+        response = httpx.get(repo_url)
+        response.raise_for_status()  # Raise exception for bad responses
+        latest_version = response.json()["tag_name"]
+        
+        if latest_version > CURRENT_VERSION:
+            print(f"A new version ({latest_version}) is available!")
+        elif latest_version < CURRENT_VERSION:
+            print("You're running a developer version!")
+        else:
+            return None
+    except Exception as e:
+        print("Could not check for updates. Error:", e)
+
+# --------------------------------------------------------------------------
+
 if __name__ == "__main__":
-    # Starts the scraper
-    scraper()
+    # Clear the console
+    clear_console()
+
+    # Show Banner
+    print(Fore.BLUE + banner)
+
+    check_for_updates()
 
     # Sets up the headers
     headers = get_headers()
 
+    # Starts the scraper
+    scraper()
+
     # Gets a list of urls from a file
     urls = get_urls()
 
     # Initialize the request rate limit trackers
     last_reset_time = None
     requests_since_reset = 0
 
@@ -595,16 +687,21 @@
         if downloaded_filename is None:
             continue
         mark_done(each)
         processed_count += 1
         print(f"Done with {os.path.basename(downloaded_filename)}!")
 
         # Wait a bit before making the next request
-        sleep_duration = random.randint(5, 10)
+        sleep_duration = random.randint(3, 8)
         print(f"Sleeping for {sleep_duration} seconds before the next request...")
         time.sleep(sleep_duration)
 
     # If all urls have been processed, move the beatmaps to the osu! songs folder
     if processed_count == len(urls): 
         print("All URLs have been processed. Done.")
         osu_folder = find_osu_folder()
-        move_files_confirmation(osu_folder)
+        move_files_confirmation(osu_folder)
+
+# Credits:
+
+# ForgedCore8 - https://www.github.com/ForgedCore8
+# DJ Stomp - https://www.github.com/DJStompZone
```


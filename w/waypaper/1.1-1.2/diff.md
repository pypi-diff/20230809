# Comparing `tmp/waypaper-1.1.tar.gz` & `tmp/waypaper-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waypaper-1.1.tar", last modified: Tue Aug  8 07:05:08 2023, max compression
+gzip compressed data, was "waypaper-1.2.tar", last modified: Wed Aug  9 03:18:07 2023, max compression
```

## Comparing `waypaper-1.1.tar` & `waypaper-1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 07:05:08.159047 waypaper-1.1/
--rw-r--r--   0 r         (1000) r         (1000)    35149 2023-08-08 02:44:17.000000 waypaper-1.1/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     2174 2023-08-08 07:05:08.159047 waypaper-1.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     1342 2023-08-08 07:00:55.000000 waypaper-1.1/README.md
--rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 waypaper-1.1/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-08-08 07:05:08.162381 waypaper-1.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1457 2023-08-08 03:51:54.000000 waypaper-1.1/setup.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 07:05:08.159047 waypaper-1.1/waypaper/
--rw-r--r--   0 r         (1000) r         (1000)      470 2023-08-08 07:01:35.000000 waypaper-1.1/waypaper/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     8514 2023-08-08 07:03:15.000000 waypaper-1.1/waypaper/app.py
--rw-r--r--   0 r         (1000) r         (1000)      409 2023-08-08 03:10:14.000000 waypaper-1.1/waypaper/changer.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 07:05:08.159047 waypaper-1.1/waypaper.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     2174 2023-08-08 07:05:08.000000 waypaper-1.1/waypaper.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      292 2023-08-08 07:05:08.000000 waypaper-1.1/waypaper.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-08-08 07:05:08.000000 waypaper-1.1/waypaper.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       51 2023-08-08 07:05:08.000000 waypaper-1.1/waypaper.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2023-08-08 07:05:08.000000 waypaper-1.1/waypaper.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        9 2023-08-08 07:05:08.000000 waypaper-1.1/waypaper.egg-info/top_level.txt
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-09 03:18:07.739169 waypaper-1.2/
+-rw-r--r--   0 r         (1000) r         (1000)    35149 2023-08-08 02:44:17.000000 waypaper-1.2/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     2174 2023-08-09 03:18:07.739169 waypaper-1.2/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     1342 2023-08-08 07:00:55.000000 waypaper-1.2/README.md
+-rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 waypaper-1.2/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-08-09 03:18:07.739169 waypaper-1.2/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1457 2023-08-08 03:51:54.000000 waypaper-1.2/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-09 03:18:07.735835 waypaper-1.2/waypaper/
+-rw-r--r--   0 r         (1000) r         (1000)      661 2023-08-09 03:02:20.000000 waypaper-1.2/waypaper/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     7518 2023-08-09 03:15:14.000000 waypaper-1.2/waypaper/app.py
+-rw-r--r--   0 r         (1000) r         (1000)      417 2023-08-09 02:18:41.000000 waypaper-1.2/waypaper/changer.py
+-rw-r--r--   0 r         (1000) r         (1000)     2529 2023-08-09 03:16:38.000000 waypaper-1.2/waypaper/config.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-09 03:18:07.739169 waypaper-1.2/waypaper.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     2174 2023-08-09 03:18:07.000000 waypaper-1.2/waypaper.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      311 2023-08-09 03:18:07.000000 waypaper-1.2/waypaper.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-08-09 03:18:07.000000 waypaper-1.2/waypaper.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       51 2023-08-09 03:18:07.000000 waypaper-1.2/waypaper.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2023-08-09 03:18:07.000000 waypaper-1.2/waypaper.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        9 2023-08-09 03:18:07.000000 waypaper-1.2/waypaper.egg-info/top_level.txt
```

### Comparing `waypaper-1.1/LICENSE` & `waypaper-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waypaper-1.1/PKG-INFO` & `waypaper-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waypaper
-Version: 1.1
+Version: 1.2
 Summary: GUI wallpaper setter for Wayland
 Home-page: https://github.com/anufrievroman/waypaper
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `waypaper-1.1/README.md` & `waypaper-1.2/README.md`

 * *Files identical despite different names*

### Comparing `waypaper-1.1/setup.py` & `waypaper-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `waypaper-1.1/waypaper/app.py` & `waypaper-1.2/waypaper/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """Module that runs GUI app"""
 
 import gi
 import os
 import subprocess
 import configparser
 
-from waypaper.changer import change_wallpaper
-
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, GdkPixbuf, Gdk
 
+from waypaper.changer import change_wallpaper
+from waypaper.config import cf
+
 
-class App(Gtk.Window):
-    """Main application class that controls GUI"""
+def get_image_paths(root_folder, include_subfolders=False, depth=None):
+    """Get a list of file paths depending of weather we include subfolders and how deep we scan"""
+    file_paths = []
+    for root, directories, files in os.walk(root_folder):
+        if not include_subfolders and root != root_folder:
+            continue
+        if depth is not None and root != root_folder:
+            current_depth = root.count(os.path.sep) - root_folder.count(os.path.sep)
+            if current_depth > depth:
+                continue
+        for filename in files:
+            if filename.endswith(".jpg") or filename.endswith(".png") or filename.endswith(".gif"):
+                file_paths.append(os.path.join(root, filename))
+    return file_paths
 
-    selected_image_path = None
-    thumb_width = 240
-    default_fill_option = "fill"
-
-    config_dir = os.path.expanduser("~/.config/waypaper")
-    config_file_path = os.path.join(config_dir, "config.ini")
-    number_of_columns = 3
-    padding = 0
 
+class App(Gtk.Window):
+    """Main application class that controls GUI"""
 
     def __init__(self):
         super().__init__(title="Waypaper")
         self.set_default_size(780, 600)
 
-
-        # Create the configuration directory if it doesn't exist:
-        os.makedirs(self.config_dir, exist_ok=True)
-
         # Create a vertical box for layout:
         self.main_box = Gtk.VBox(spacing=10)
         self.add(self.main_box)
 
         # Create a button to open folder dialog:
         self.choose_folder_button = Gtk.Button(label="Choose wallpaper folder")
         self.choose_folder_button.connect("clicked", self.on_choose_folder_clicked)
@@ -48,175 +51,143 @@
         # Create a scrolled window for the grid:
         self.scrolled_window = Gtk.ScrolledWindow()
         self.scrolled_window.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
         self.grid_alignment.add(self.scrolled_window)
 
         # Create a grid layout for images:
         self.grid = Gtk.Grid()
-        self.grid.set_row_spacing(self.padding)
-        self.grid.set_column_spacing(self.padding)
+        self.grid.set_row_spacing(0)
+        self.grid.set_column_spacing(0)
         self.scrolled_window.add(self.grid)
 
-        # Set default image folder:
-        self.default_image_folder = os.path.expanduser("~/Pictures")
+        # Create subfolder toggle:
+        self.include_subfolders_checkbox = Gtk.ToggleButton(label="Subfolders")
+        self.include_subfolders_checkbox.set_active(cf.include_subfolders)
+        self.include_subfolders_checkbox.connect("toggled", self.on_include_subfolders_toggled)
 
-        # Create a display option dropdown menu:
-        self.fill_option_label = Gtk.Label(label="Fill option:")
+        # Create a fill option dropdown menu:
+        # self.fill_option_label = Gtk.Label(label="")
         self.fill_option_combo = Gtk.ComboBoxText()
-        self.fill_option_combo.append_text("stretch")
-        self.fill_option_combo.append_text("fit")
-        self.fill_option_combo.append_text("fill")
-        self.fill_option_combo.append_text("center")
-        self.fill_option_combo.append_text("tile")
-        self.fill_option_combo.set_active(2)  # Default to "fill"
+        self.fill_option_combo.append_text("Fill")
+        self.fill_option_combo.append_text("Stretch")
+        self.fill_option_combo.append_text("Fit")
+        self.fill_option_combo.append_text("Center")
+        self.fill_option_combo.append_text("Tile")
+        self.fill_option_combo.set_active(0)
+        self.fill_option_combo.connect("changed", self.on_fill_option_changed)
+
+        # Create exit button:
+        self.exit_button = Gtk.Button(label=" Exit ")
+        self.exit_button.connect("clicked", self.on_exit_clicked)
 
         # Create a box to contain the bottom row of buttons with margin
-        self.bottom_button_box = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL, spacing=10)
+        self.bottom_button_box = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL, spacing=20)
         self.bottom_button_box.set_margin_bottom(10)
         self.main_box.pack_end(self.bottom_button_box, False, False, 0)
 
         # Create an alignment container to center align the row of buttons
         self.button_row_alignment = Gtk.Alignment(xalign=0.5, yalign=0.0, xscale=0.5, yscale=0.5)
         self.bottom_button_box.pack_start(self.button_row_alignment, True, False, 0)
 
         # Create a horizontal box for display option and exit button
-        self.option_exit_box = Gtk.HBox(spacing=10)
-        self.option_exit_box.pack_start(self.fill_option_label, False, False, 0)
-        self.option_exit_box.pack_start(self.fill_option_combo, False, False, 0)
-        self.option_exit_box.pack_end(self.create_exit_button(), False, False, 0)
-        self.button_row_alignment.add(self.option_exit_box)
+        self.options_box = Gtk.HBox(spacing=10)
+        self.options_box.pack_start(self.include_subfolders_checkbox, False, False, 0)
+        # self.options_box.pack_start(self.fill_option_label, False, False, 0)
+        self.options_box.pack_start(self.fill_option_combo, False, False, 0)
+        self.options_box.pack_end(self.exit_button, False, False, 0)
+        self.button_row_alignment.add(self.options_box)
 
         # Connect the "q" key press event to exit the application
         self.connect("key-press-event", self.on_key_pressed)
 
 
-    def create_exit_button(self):
-        exit_button = Gtk.Button(label="Exit")
-        exit_button.connect("clicked", self.on_exit_clicked)
-        return exit_button
-
-
-    def load_data(self):
-        """Load data from the config or use default if it does not exists"""
-        config = configparser.ConfigParser()
-        if os.path.exists(self.config_file_path):
-            config.read(self.config_file_path)
-            self.image_folder = config.get("Settings", "folder", fallback=self.default_image_folder)
-            self.fill_option = config.get("Settings", "fill", fallback=self.default_fill_option)
-            self.current_wallpaper = config.get("Settings", "wallpaper", fallback=None)
-        else:
-            self.image_folder = self.default_image_folder
-
-
-    def save_data(self):
-        """Save the parameters to the configuration file"""
-        config = configparser.ConfigParser()
-        if os.path.exists(self.config_file_path):
-            config.read(self.config_file_path)
-
-        if not config.has_section("Settings"):
-            config.add_section("Settings")
-
-        # Save folder:
-        config.set("Settings", "folder", self.image_folder)
-
-        # Save selected wallpaper:
-        if self.selected_image_path is not None:
-            config.set("Settings", "wallpaper", self.selected_image_path)
-
-        # Save fill option:
-        fill_option = self.fill_option_combo.get_active_text() or self.default_fill_option
-        config.set("Settings", "fill", fill_option)
-
-        with open(self.config_file_path, "w") as configfile:
-            config.write(configfile)
-
-
     def load_images(self):
         """Load images from the selected folder, resize them, and arrange int grid"""
 
-        if not os.path.exists(self.default_image_folder):
-            self.default_image_folder = "/"
-
-        if not os.path.exists(self.image_folder):
-            self.image_folder = self.default_image_folder
-
-
         # Clear existing images:
         for child in self.grid.get_children():
             self.grid.remove(child)
 
         row = 0
         col = 0
 
         # Load images from the folder:
-        for filename in os.listdir(self.image_folder):
-            if filename.endswith(".jpg") or filename.endswith(".png") or filename.endswith(".gif"):
-                image_path = os.path.join(self.image_folder, filename)
+        image_paths = get_image_paths(cf.image_folder, cf.include_subfolders, depth=1)
+        for image_path in image_paths:
 
-                # Load and scale the image:
-                pixbuf = GdkPixbuf.Pixbuf.new_from_file(image_path)
-                aspect_ratio = pixbuf.get_width() / pixbuf.get_height()
-                scaled_width = self.thumb_width
-                scaled_height = int(scaled_width / aspect_ratio)
-                scaled_pixbuf = pixbuf.scale_simple(scaled_width, scaled_height, GdkPixbuf.InterpType.BILINEAR)
-
-                # Create a button with an image inside:
-                image = Gtk.Image.new_from_pixbuf(scaled_pixbuf)
-                button = Gtk.Button()
-                button.set_relief(Gtk.ReliefStyle.NONE)  # Remove border
-                button.add(image)
-
-                # Add button to the grid and connect clicked event:
-                self.grid.attach(button, col, row, 1, 1)
-                button.connect("clicked", self.on_image_clicked, image_path)
-
-                col += 1
-                if col >= self.number_of_columns:
-                    col = 0
-                    row += 1
+            # Load and scale the image:
+            pixbuf = GdkPixbuf.Pixbuf.new_from_file(image_path)
+            aspect_ratio = pixbuf.get_width() / pixbuf.get_height()
+            scaled_width = 240
+            scaled_height = int(scaled_width / aspect_ratio)
+            scaled_pixbuf = pixbuf.scale_simple(scaled_width, scaled_height, GdkPixbuf.InterpType.BILINEAR)
+
+            # Create a button with an image inside:
+            image = Gtk.Image.new_from_pixbuf(scaled_pixbuf)
+            button = Gtk.Button()
+            button.set_relief(Gtk.ReliefStyle.NONE)  # Remove border
+            button.add(image)
+
+            # Add button to the grid and connect clicked event:
+            self.grid.attach(button, col, row, 1, 1)
+            button.connect("clicked", self.on_image_clicked, image_path)
+
+            col += 1
+            if col >= 3:
+                col = 0
+                row += 1
 
         # Show all images:
         self.grid.show_all()
 
 
     def on_choose_folder_clicked(self, widget):
         """Choosing the folder of images, saving the path, and reloading images"""
 
         dialog = Gtk.FileChooserDialog(
             "Please choose a folder", self, Gtk.FileChooserAction.SELECT_FOLDER,
             (Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL, "Select", Gtk.ResponseType.OK)
         )
         response = dialog.run()
         if response == Gtk.ResponseType.OK:
-            self.image_folder = dialog.get_filename()
-            self.save_data()
+            cf.image_folder = dialog.get_filename()
+            cf.save()
             self.load_images()
         dialog.destroy()
 
 
+    def on_include_subfolders_toggled(self, toggle):
+        """On chosing to include subfolders"""
+        cf.include_subfolders = toggle.get_active()
+        self.load_images()
+
+
+    def on_fill_option_changed(self, combo):
+        cf.fill_option = combo.get_active_text()
+
+
     def on_image_clicked(self, widget, user_data):
         """On clicking an image, set it as a wallpaper and save"""
-        self.selected_image_path = user_data
-        print("Selected image path:", self.selected_image_path)
-        fill_option = self.fill_option_combo.get_active_text() or self.default_fill_option
-        change_wallpaper(self.selected_image_path, fill_option)
-        self.save_data()
+        cf.wallpaper = user_data
+        print("Selected image path:", cf.wallpaper)
+        cf.fill_option = self.fill_option_combo.get_active_text() or cf.fill_option
+        change_wallpaper(cf.wallpaper, cf.fill_option)
+        cf.save()
 
 
     def on_exit_clicked(self, widget):
         """On clicking exit button, save the data and quit"""
-        self.save_data()
+        cf.save()
         Gtk.main_quit()
 
 
     def on_key_pressed(self, widget, event):
         """On clicking q, save the data and quit"""
         if event.keyval == Gdk.KEY_q:
-            self.save_data()
+            cf.save()
             Gtk.main_quit()
 
 
     def run(self):
         """Run GUI application"""
         self.load_images()
         self.connect("destroy", self.on_exit_clicked)
```

### Comparing `waypaper-1.1/waypaper.egg-info/PKG-INFO` & `waypaper-1.2/waypaper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waypaper
-Version: 1.1
+Version: 1.2
 Summary: GUI wallpaper setter for Wayland
 Home-page: https://github.com/anufrievroman/waypaper
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```


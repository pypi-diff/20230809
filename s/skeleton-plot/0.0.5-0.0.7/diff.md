# Comparing `tmp/skeleton_plot-0.0.5.tar.gz` & `tmp/skeleton_plot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skeleton_plot-0.0.5.tar", last modified: Thu May 25 22:09:31 2023, max compression
+gzip compressed data, was "dist/skeleton_plot-0.0.7.tar", last modified: Wed Aug  9 03:52:40 2023, max compression
```

## Comparing `skeleton_plot-0.0.5.tar` & `skeleton_plot-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-05-25 22:09:31.458110 skeleton_plot-0.0.5/
--rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-05-25 22:09:31.455377 skeleton_plot-0.0.5/PKG-INFO
--rw-r--r--   0 emily.joyce   (502) staff       (20)     1934 2023-05-11 20:53:34.000000 skeleton_plot-0.0.5/README.md
--rw-r--r--   0 emily.joyce   (502) staff       (20)       38 2023-05-25 22:09:31.458479 skeleton_plot-0.0.5/setup.cfg
--rw-r--r--   0 emily.joyce   (502) staff       (20)     1146 2023-05-11 20:53:50.000000 skeleton_plot-0.0.5/setup.py
-drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-05-25 22:09:31.398989 skeleton_plot-0.0.5/skeleton_plot/
--rw-r--r--   0 emily.joyce   (502) staff       (20)       46 2023-02-17 18:19:45.000000 skeleton_plot-0.0.5/skeleton_plot/__init__.py
--rw-r--r--   0 emily.joyce   (502) staff       (20)    15606 2023-05-18 18:04:06.000000 skeleton_plot-0.0.5/skeleton_plot/plot_tools.py
--rw-r--r--   0 emily.joyce   (502) staff       (20)     4295 2023-04-24 19:54:40.000000 skeleton_plot-0.0.5/skeleton_plot/skel_io.py
--rw-r--r--   0 emily.joyce   (502) staff       (20)     1724 2023-05-18 16:53:22.000000 skeleton_plot-0.0.5/skeleton_plot/utils.py
-drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-05-25 22:09:31.439164 skeleton_plot-0.0.5/skeleton_plot.egg-info/
--rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/PKG-INFO
--rw-r--r--   0 emily.joyce   (502) staff       (20)      304 2023-05-25 22:09:30.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/SOURCES.txt
--rw-r--r--   0 emily.joyce   (502) staff       (20)        1 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/dependency_links.txt
--rw-r--r--   0 emily.joyce   (502) staff       (20)       67 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/requires.txt
--rw-r--r--   0 emily.joyce   (502) staff       (20)       14 2023-05-25 22:09:29.000000 skeleton_plot-0.0.5/skeleton_plot.egg-info/top_level.txt
+drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-08-09 03:52:40.665505 skeleton_plot-0.0.7/
+-rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-08-09 03:52:40.664614 skeleton_plot-0.0.7/PKG-INFO
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     1934 2023-05-11 20:53:34.000000 skeleton_plot-0.0.7/README.md
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       38 2023-08-09 03:52:40.666087 skeleton_plot-0.0.7/setup.cfg
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     1146 2023-08-09 03:45:36.000000 skeleton_plot-0.0.7/setup.py
+drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-08-09 03:52:40.650199 skeleton_plot-0.0.7/skeleton_plot/
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       46 2023-08-09 03:45:34.000000 skeleton_plot-0.0.7/skeleton_plot/__init__.py
+-rw-r--r--   0 emily.joyce   (502) staff       (20)    15876 2023-06-05 06:47:09.000000 skeleton_plot-0.0.7/skeleton_plot/plot_tools.py
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     4344 2023-08-08 17:44:55.000000 skeleton_plot-0.0.7/skeleton_plot/skel_io.py
+-rw-r--r--   0 emily.joyce   (502) staff       (20)     2072 2023-08-08 17:40:39.000000 skeleton_plot-0.0.7/skeleton_plot/utils.py
+drwxr-xr-x   0 emily.joyce   (502) staff       (20)        0 2023-08-09 03:52:40.663517 skeleton_plot-0.0.7/skeleton_plot.egg-info/
+-rw-r--r--   0 emily.joyce   (502) staff       (20)      394 2023-08-09 03:52:40.000000 skeleton_plot-0.0.7/skeleton_plot.egg-info/PKG-INFO
+-rw-r--r--   0 emily.joyce   (502) staff       (20)      304 2023-08-09 03:52:40.000000 skeleton_plot-0.0.7/skeleton_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 emily.joyce   (502) staff       (20)        1 2023-08-09 03:52:40.000000 skeleton_plot-0.0.7/skeleton_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       67 2023-08-09 03:52:40.000000 skeleton_plot-0.0.7/skeleton_plot.egg-info/requires.txt
+-rw-r--r--   0 emily.joyce   (502) staff       (20)       14 2023-08-09 03:52:40.000000 skeleton_plot-0.0.7/skeleton_plot.egg-info/top_level.txt
```

### Comparing `skeleton_plot-0.0.5/README.md` & `skeleton_plot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `skeleton_plot-0.0.5/setup.py` & `skeleton_plot-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #     raise RuntimeError("Unable to find version string.")
 
 
 with open("requirements.txt", "r") as f:
     required = f.read().splitlines()
 
 setup(
-    version='0.0.5',
+    version='0.0.7',
     name="skeleton_plot",
     description="package for plotting skeletons",
     author="Emily Joyce, Forrest Collman, Casey Schneider-Mizell",
     author_email="emily.joyce@alleninstitute.org, forrestc@alleninstute.org,caseys@alleninstitute.org,",
     url="https://github.com/AllenInstitute/skeleton_plot",
     packages=find_packages(where="."),
     extras_require={"cloud": ["caveclient>=4.0.0", "cloudfiles"]},
```

### Comparing `skeleton_plot-0.0.5/skeleton_plot/plot_tools.py` & `skeleton_plot-0.0.7/skeleton_plot/plot_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,23 +202,25 @@
 
     # add synapses
 
     if plot_presyn:
         pre_anno_table = list(pre_anno.keys())[0]
         pre_column = list(pre_anno.values())[0]
         presyn_verts = np.array([np.array(x) for x in (mw.anno[pre_anno_table][pre_column]).values])*syn_res
+        plot_synapses(presyn_verts = presyn_verts, x = x, y = y, presyn_size = presyn_size, 
+                postsyn_size = postsyn_size, presyn_color = presyn_color, postsyn_color = postsyn_color, 
+                presyn_alpha = presyn_alpha, postsyn_alpha = postsyn_alpha, ax = ax)
 
     if plot_postsyn:
         post_anno_table = list(post_anno.keys())[0]
         post_column = list(post_anno.values())[0]
         postsyn_verts = np.array([np.array(x) for x in (mw.anno[post_anno_table][post_column]).values])*syn_res
-
-    plot_synapses(presyn_verts = presyn_verts, postsyn_verts = postsyn_verts, x = x, y = y, presyn_size = presyn_size, 
-                    postsyn_size = postsyn_size, presyn_color = presyn_color, postsyn_color = postsyn_color, 
-                    presyn_alpha = presyn_alpha, postsyn_alpha = postsyn_alpha, ax = ax)
+        plot_synapses(postsyn_verts = postsyn_verts, x = x, y = y, presyn_size = presyn_size, 
+                        postsyn_size = postsyn_size, presyn_color = presyn_color, postsyn_color = postsyn_color, 
+                        presyn_alpha = presyn_alpha, postsyn_alpha = postsyn_alpha, ax = ax)
     
     # plot verts 
     plot_verts(sk.vertices, sk.edges, ax = ax, radius = radius,
                 skel_colors = skel_colors, title = title, skel_alpha = skel_alpha,
                 line_width = line_width, x = x, y = y,  plot_soma = plot_soma, soma_node = soma_node,
                 color = color, soma_size = soma_size, invert_y = invert_y, 
                 skel_color_map = skel_color_map, x_min_max = x_min_max, 
@@ -263,16 +265,16 @@
     x, y = axis_dict[x], axis_dict[y]
 
     if presyn_verts is not None:
         ax.scatter(presyn_verts[:,x], presyn_verts[:,y], s = presyn_size, c = presyn_color, alpha = presyn_alpha)
     if postsyn_verts is not None:
         ax.scatter(postsyn_verts[:,x], postsyn_verts[:,y], s = postsyn_size, c = postsyn_color, alpha = postsyn_alpha)
 
-    utils.set_xy_lims(ax, verts = np.vstack((presyn_verts, postsyn_verts)), invert_y = invert_y, 
-            x_min_max = x_min_max, y_min_max = y_min_max, x = x, y = y)
+    # utils.set_xy_lims(ax, verts = np.vstack((presyn_verts, postsyn_verts)), invert_y = invert_y, 
+    #         x_min_max = x_min_max, y_min_max = y_min_max, x = x, y = y)
 
 
 def plot_layer_lines(y_vals, ax = None, labels = None, buffer_space = .01, line_styles = None):
     """    
     takes a list of y values on which to plot horizontal line across the current x ax.
     Optionally, labels can be provided to label each line.
```

### Comparing `skeleton_plot-0.0.5/skeleton_plot/skel_io.py` & `skeleton_plot-0.0.7/skeleton_plot/skel_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,17 @@
     filename (str): full .swc filename 
     df (pd.DataFrame, optional): _description_. Defaults to None.
 
     Returns:
         skeleton: (meshparty.meshwork.skeleton) skeleton object containing .swc data
     """
     if '://' not in directory:
-        directory = 'file://' + directory
-    file_path = os.path.join(directory, filename)
+        directory = utils.cloud_path_join(directory, use_file_scheme = True)
+    
+    file_path = utils.cloud_path_join(directory, filename)
     df = read_swc(file_path)
     if not all(df.index == df['id']):
         # remap id and parent to index to 
         id_map = dict(zip(df['id'], df.index))
         id_map[-1] = -1
         df['id'] = [id_map[x] for x in df['id']]
         df['parent'] = [id_map[x] for x in df['parent']]
```

### Comparing `skeleton_plot-0.0.5/skeleton_plot/utils.py` & `skeleton_plot-0.0.7/skeleton_plot/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,8 +47,21 @@
 
     
     elif x_min_max is None and y_min_max is None:
         if invert_y:
             ax.set_ylim(max(verts[:,y]), min(verts[:,y]))
         else:
             ax.set_ylim(min(verts[:,y]), max(verts[:,y]))
-        ax.set_xlim(min(verts[:,x]), max(verts[:,x]))
+        ax.set_xlim(min(verts[:,x]), max(verts[:,x]))
+
+def cloud_path_join(*args, use_file_scheme = False):
+    """
+    Joins given arguments into a cloud path format with only forward slashes.
+    """
+    
+    stripped_parts = [part.strip('/') for part in args]
+    joined_path = '/'.join(stripped_parts)
+    
+    if use_file_scheme:
+        return f'file://{joined_path}'
+    
+    return joined_path
```


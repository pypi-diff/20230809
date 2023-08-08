# Comparing `tmp/simfire-1.4.38.tar.gz` & `tmp/simfire-1.4.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfire-1.4.38.tar", max compression
+gzip compressed data, was "simfire-1.4.39.tar", max compression
```

## Comparing `simfire-1.4.38.tar` & `simfire-1.4.39.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    10789 2023-08-07 20:08:26.923408 simfire-1.4.38/LICENSE
--rw-r--r--   0        0        0     2662 2023-08-07 20:08:26.923408 simfire-1.4.38/README.md
--rw-r--r--   0        0        0     1852 2023-08-07 20:08:27.155418 simfire-1.4.38/pyproject.toml
--rw-r--r--   0        0        0     1111 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/__init__.py
--rw-r--r--   0        0        0    10729 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/enums.py
--rw-r--r--   0        0        0       37 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/__init__.py
--rw-r--r--   0        0        0      874 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/_tests/__init__.py
--rw-r--r--   0        0        0    15523 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/_tests/test_game.py
--rw-r--r--   0        0        0     9928 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/_tests/test_sprites.py
--rw-r--r--   0        0        0    14937 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/game.py
--rw-r--r--   0        0        0     1318 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/image.py
--rw-r--r--   0        0        0      379 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/_tests/__init__.py
--rw-r--r--   0        0        0    18385 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/_tests/test_fire.py
--rw-r--r--   0        0        0     8301 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/_tests/test_mitigation.py
--rw-r--r--   0        0        0    29897 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/fire.py
--rw-r--r--   0        0        0     7321 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/mitigation.py
--rw-r--r--   0        0        0    15972 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/sprites.py
--rw-r--r--   0        0        0       49 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/_tests/__init__.py
--rw-r--r--   0        0        0    14392 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/_tests/test_simulation.py
--rw-r--r--   0        0        0    37815 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/simulation.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/__init__.py
--rw-r--r--   0        0        0     2771 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_config.py
--rw-r--r--   0        0        0     1925 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config.yml
--rw-r--r--   0        0        0       47 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_bad.yml
--rw-r--r--   0        0        0     1874 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
--rw-r--r--   0        0        0     1876 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_gaussian.yml
--rw-r--r--   0        0        0     1851 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
--rw-r--r--   0        0        0     4693 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_graph.py
--rw-r--r--   0        0        0    17172 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_layers.py
--rw-r--r--   0        0        0      622 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_log.py
--rw-r--r--   0        0        0     4495 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_terrain.py
--rw-r--r--   0        0        0     1472 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_units.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/assets/__init__.py
--rw-r--r--   0        0        0     1854 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/assets/fireline_logo.png
--rw-r--r--   0        0        0    39144 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/config.py
--rw-r--r--   0        0        0      499 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/decorators.py
--rw-r--r--   0        0        0     4153 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/generate_cfd_wind_layer.py
--rw-r--r--   0        0        0    10189 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/graph.py
--rw-r--r--   0        0        0    51105 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/layers.py
--rw-r--r--   0        0        0     2030 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/log.py
--rw-r--r--   0        0        0   143776 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
--rw-r--r--   0        0        0   143776 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
--rw-r--r--   0        0        0     3647 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/terrain.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/textures/__init__.py
--rw-r--r--   0        0        0   204702 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/textures/terrain.jpg
--rw-r--r--   0        0        0     2555 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/utils/units.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/__init__.py
--rw-r--r--   0        0        0     2184 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_cfd_wind.py
--rw-r--r--   0        0        0     2423 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_elevation_functions.py
--rw-r--r--   0        0        0     2821 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_rothermel.py
--rw-r--r--   0        0        0     1466 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_wind.py
--rw-r--r--   0        0        0     3703 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/elevation_functions.py
--rw-r--r--   0        0        0     1054 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/fuel_array_functions.py
--rw-r--r--   0        0        0     2306 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/parameters.py
--rw-r--r--   0        0        0     2083 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/presets.py
--rw-r--r--   0        0        0     4306 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/rothermel.py
--rw-r--r--   0        0        0        0 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/__init__.py
--rw-r--r--   0        0        0     8781 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/cfd_wind.py
--rw-r--r--   0        0        0     3132 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/perlin_wind.py
--rw-r--r--   0        0        0     6578 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/wind_controller.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 simfire-1.4.38/PKG-INFO
+-rw-r--r--   0        0        0    10789 2023-08-08 19:52:48.698352 simfire-1.4.39/LICENSE
+-rw-r--r--   0        0        0     2662 2023-08-08 19:52:48.698352 simfire-1.4.39/README.md
+-rw-r--r--   0        0        0     1852 2023-08-08 19:52:48.934357 simfire-1.4.39/pyproject.toml
+-rw-r--r--   0        0        0     1111 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/__init__.py
+-rw-r--r--   0        0        0    10729 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/enums.py
+-rw-r--r--   0        0        0       37 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/__init__.py
+-rw-r--r--   0        0        0      874 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/_tests/__init__.py
+-rw-r--r--   0        0        0    15523 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/_tests/test_game.py
+-rw-r--r--   0        0        0     9928 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/_tests/test_sprites.py
+-rw-r--r--   0        0        0    14937 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/game.py
+-rw-r--r--   0        0        0     1318 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/image.py
+-rw-r--r--   0        0        0      379 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/managers/_tests/__init__.py
+-rw-r--r--   0        0        0    18385 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/managers/_tests/test_fire.py
+-rw-r--r--   0        0        0     8301 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/managers/_tests/test_mitigation.py
+-rw-r--r--   0        0        0    29897 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/managers/fire.py
+-rw-r--r--   0        0        0     7321 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/managers/mitigation.py
+-rw-r--r--   0        0        0    15972 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/game/sprites.py
+-rw-r--r--   0        0        0       49 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/sim/_tests/__init__.py
+-rw-r--r--   0        0        0    14392 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/sim/_tests/test_simulation.py
+-rw-r--r--   0        0        0    37815 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/sim/simulation.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/__init__.py
+-rw-r--r--   0        0        0     2771 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_config.py
+-rw-r--r--   0        0        0     1925 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_configs/test_config.yml
+-rw-r--r--   0        0        0       47 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_bad.yml
+-rw-r--r--   0        0        0     1874 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
+-rw-r--r--   0        0        0     1876 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_gaussian.yml
+-rw-r--r--   0        0        0     1851 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
+-rw-r--r--   0        0        0     4693 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_graph.py
+-rw-r--r--   0        0        0    17172 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_layers.py
+-rw-r--r--   0        0        0      622 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_log.py
+-rw-r--r--   0        0        0     4495 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_terrain.py
+-rw-r--r--   0        0        0     1472 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/_tests/test_units.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/assets/__init__.py
+-rw-r--r--   0        0        0     1854 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/assets/fireline_logo.png
+-rw-r--r--   0        0        0    39144 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/config.py
+-rw-r--r--   0        0        0      499 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/decorators.py
+-rw-r--r--   0        0        0     4153 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/generate_cfd_wind_layer.py
+-rw-r--r--   0        0        0    10189 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/graph.py
+-rw-r--r--   0        0        0    51105 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/layers.py
+-rw-r--r--   0        0        0     2030 2023-08-08 19:52:48.934357 simfire-1.4.39/simfire/utils/log.py
+-rw-r--r--   0        0        0   143776 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
+-rw-r--r--   0        0        0   143776 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
+-rw-r--r--   0        0        0     3647 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/utils/terrain.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/utils/textures/__init__.py
+-rw-r--r--   0        0        0   204702 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/utils/textures/terrain.jpg
+-rw-r--r--   0        0        0     2555 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/utils/units.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/_tests/__init__.py
+-rw-r--r--   0        0        0     2184 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/_tests/test_cfd_wind.py
+-rw-r--r--   0        0        0     2423 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/_tests/test_elevation_functions.py
+-rw-r--r--   0        0        0     2821 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/_tests/test_rothermel.py
+-rw-r--r--   0        0        0     1466 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/_tests/test_wind.py
+-rw-r--r--   0        0        0     3703 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/elevation_functions.py
+-rw-r--r--   0        0        0     1054 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/fuel_array_functions.py
+-rw-r--r--   0        0        0     2306 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/parameters.py
+-rw-r--r--   0        0        0     2083 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/presets.py
+-rw-r--r--   0        0        0     5313 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/rothermel.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/wind_mechanics/__init__.py
+-rw-r--r--   0        0        0     8781 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/wind_mechanics/cfd_wind.py
+-rw-r--r--   0        0        0     3132 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/wind_mechanics/perlin_wind.py
+-rw-r--r--   0        0        0     6578 2023-08-08 19:52:48.938357 simfire-1.4.39/simfire/world/wind_mechanics/wind_controller.py
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 simfire-1.4.39/PKG-INFO
```

### Comparing `simfire-1.4.38/LICENSE` & `simfire-1.4.39/LICENSE`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/README.md` & `simfire-1.4.39/README.md`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/pyproject.toml` & `simfire-1.4.39/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simfire"
-version = "1.4.38"
+version = "1.4.39"
 description = "Fire simulator built in Python"
 authors = ["Tim Welsh <twelsh@mitre.org>", "Marissa Dotter <mdotter@mitre.org>",
            "Michael Doyle <mdoyle@mitre.org>", "Dhanuj Gandikota <dgandikota@mitre.org>",
            "Chris Kempis <ckempis@mitre.org>", "Lauren Schambach <lschambach@mitre.org>",
            "Alex Tapley <atapley@mitre.org>", "Michael Threet <mthreet@mitre.org>"]
 readme = "README.md"
 include = ["simfire/utils/textures/terrain.jpg", "simfire/utils/assets/fireline_logo.png"]
```

### Comparing `simfire-1.4.38/simfire/__init__.py` & `simfire-1.4.39/simfire/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/enums.py` & `simfire-1.4.39/simfire/enums.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/_tests/__init__.py` & `simfire-1.4.39/simfire/game/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/_tests/test_game.py` & `simfire-1.4.39/simfire/game/_tests/test_game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/_tests/test_sprites.py` & `simfire-1.4.39/simfire/game/_tests/test_sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/game.py` & `simfire-1.4.39/simfire/game/game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/image.py` & `simfire-1.4.39/simfire/game/image.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/managers/_tests/test_fire.py` & `simfire-1.4.39/simfire/game/managers/_tests/test_fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/managers/_tests/test_mitigation.py` & `simfire-1.4.39/simfire/game/managers/_tests/test_mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/managers/fire.py` & `simfire-1.4.39/simfire/game/managers/fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/managers/mitigation.py` & `simfire-1.4.39/simfire/game/managers/mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/game/sprites.py` & `simfire-1.4.39/simfire/game/sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/sim/_tests/test_simulation.py` & `simfire-1.4.39/simfire/sim/_tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/sim/simulation.py` & `simfire-1.4.39/simfire/sim/simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_config.py` & `simfire-1.4.39/simfire/utils/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config.yml` & `simfire-1.4.39/simfire/utils/_tests/test_configs/test_config.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_flat_simple.yml` & `simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_flat_simple.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_gaussian.yml` & `simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_gaussian.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml` & `simfire-1.4.39/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_graph.py` & `simfire-1.4.39/simfire/utils/_tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_layers.py` & `simfire-1.4.39/simfire/utils/_tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_log.py` & `simfire-1.4.39/simfire/utils/_tests/test_log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_terrain.py` & `simfire-1.4.39/simfire/utils/_tests/test_terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/_tests/test_units.py` & `simfire-1.4.39/simfire/utils/_tests/test_units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/assets/fireline_logo.png` & `simfire-1.4.39/simfire/utils/assets/fireline_logo.png`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/config.py` & `simfire-1.4.39/simfire/utils/config.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/generate_cfd_wind_layer.py` & `simfire-1.4.39/simfire/utils/generate_cfd_wind_layer.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/graph.py` & `simfire-1.4.39/simfire/utils/graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/layers.py` & `simfire-1.4.39/simfire/utils/layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/log.py` & `simfire-1.4.39/simfire/utils/log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy` & `simfire-1.4.39/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy` & `simfire-1.4.39/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/terrain.py` & `simfire-1.4.39/simfire/utils/terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/textures/terrain.jpg` & `simfire-1.4.39/simfire/utils/textures/terrain.jpg`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/utils/units.py` & `simfire-1.4.39/simfire/utils/units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/_tests/test_cfd_wind.py` & `simfire-1.4.39/simfire/world/_tests/test_cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/_tests/test_elevation_functions.py` & `simfire-1.4.39/simfire/world/_tests/test_elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/_tests/test_rothermel.py` & `simfire-1.4.39/simfire/world/_tests/test_rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/_tests/test_wind.py` & `simfire-1.4.39/simfire/world/_tests/test_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/elevation_functions.py` & `simfire-1.4.39/simfire/world/elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/fuel_array_functions.py` & `simfire-1.4.39/simfire/world/fuel_array_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/parameters.py` & `simfire-1.4.39/simfire/world/parameters.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/presets.py` & `simfire-1.4.39/simfire/world/presets.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/rothermel.py` & `simfire-1.4.39/simfire/world/rothermel.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,17 +43,37 @@
         U: The envrionment wind speed
         U_dir: The envrionment wind direction (degrees clockwise from North)
         slope_dir: The angle of the steepest ascent at the location
 
     Returns:
         R: The computed rate of spread in ft/min
     """
-    # Check for non-burnable fuel and return 0 (no spread)
-    if w_0.all() == 0:
-        return np.zeros_like(loc_x)
+    # Retain the original number of values from the inputs
+    orig_shape = w_0.shape
+    # Keep only the non-zero w0 values for calculation
+    # This will avoid division by zero, NaN, and overflow errors
+    w_0_idxs_non_zero = np.argwhere(w_0 > 0)
+    loc_x = loc_x[w_0_idxs_non_zero]
+    loc_y = loc_y[w_0_idxs_non_zero]
+    new_loc_x = new_loc_x[w_0_idxs_non_zero]
+    new_loc_y = new_loc_y[w_0_idxs_non_zero]
+    w_0 = w_0[w_0_idxs_non_zero]
+    delta = delta[w_0_idxs_non_zero]
+    M_x = M_x[w_0_idxs_non_zero]
+    sigma = sigma[w_0_idxs_non_zero]
+    h = h[w_0_idxs_non_zero]
+    S_T = S_T[w_0_idxs_non_zero]
+    S_e = S_e[w_0_idxs_non_zero]
+    p_p = p_p[w_0_idxs_non_zero]
+    M_f = M_f[w_0_idxs_non_zero]
+    U = U[w_0_idxs_non_zero]
+    U_dir = U_dir[w_0_idxs_non_zero]
+    slope_mag = slope_mag[w_0_idxs_non_zero]
+    slope_dir = slope_dir[w_0_idxs_non_zero]
+
     # Mineral Damping Coefficient
     eta_S = np.minimum(0.174 * S_e**-0.19, np.ones_like(S_e))
     # Moisture Damping Coefficient
     r_M = np.minimum(M_f / M_x, np.ones_like(M_f))
     eta_M = 1 - 2.59 * r_M + 5.11 * r_M**2 - 3.52 * r_M**3
     # Net Fuel Load (lb/ft^2)
     w_n = w_0 * (1 - S_T)
@@ -68,15 +88,14 @@
     A = 133 * sigma**-0.7913
     # Optimum Reaction Velocity (1/min)
     gamma_prime = gamma_prime_max * (B / B_op) ** A * np.exp(A * (1 - B / B_op))
     # Reaction Intensity (BTU/ft^2-min)
     I_R = gamma_prime * w_n * h * eta_M * eta_S
     # Propagating Flux Ratio
     xi = np.exp((0.792 + 0.681 * sigma**0.5) * (B + 0.1)) / (192 + 0.25 * sigma)
-
     # Wind Factor
     c = 7.47 * np.exp(-0.133 * sigma**0.55)
     b = 0.02526 * sigma**0.54
     e = 0.715 * np.exp(-3.59e-4 * sigma)
     # Need to find wind component in direction of travel
     # Switch order of y-component subtraction since image y coordintates
     # increase from top to bottom
@@ -86,29 +105,32 @@
     wind_along_angle_of_travel = U * np.cos(wind_angle_radians - angle_of_travel)
     # This is the wind speed in in this direction
     U = wind_along_angle_of_travel
     # Negative wind leads to trouble with calculation and doesn't
     # physically make sense
     U = np.maximum(U, np.zeros_like(U))
     phi_w = c * U**b * (B / B_op) ** -e
-
     # Slope Factor
     # Phi is the slope between the two locations (i.e. the change in elevation).
     # The model calls for the tangent of the slope angle between the two points,
     # but we can approximate this by projecting the slope along the direction
     # of travel
     slope_along_angle_of_travel = -slope_mag * np.cos(slope_dir + angle_of_travel)
     sign = -1 + 2 * (slope_along_angle_of_travel > 0)
     phi_s = 5.275 * B**-0.3 * sign * slope_along_angle_of_travel**2
-
     # Effective Heating Number
     epsilon = np.exp(-138 / sigma)
     # Heat of Preignition (BTU/lb)
     Q_ig = 250 + 1116 * M_f
 
     # Rate of Spread (ft/min)
-    R = ((I_R * xi) * (1 + phi_w + phi_s)) / (p_b * epsilon * Q_ig)
+    # Default everything to 0. This will set all w0=0 values to 0
+    R = np.zeros(orig_shape)
+    R_w_0_non_zero = ((I_R * xi) * (1 + phi_w + phi_s)) / (p_b * epsilon * Q_ig)
+    # Set the non-zero w0 values to the calculated rate of spread
+    R[w_0_idxs_non_zero] = R_w_0_non_zero
 
-    # Take the minimum with 0 because a fire cannot put itself out
+    # Take the maximum with 0 because a fire cannot put itself out
+    # Don't want negative values for R
     R = np.maximum(R, np.zeros_like(R))
 
     return R
```

### Comparing `simfire-1.4.38/simfire/world/wind_mechanics/cfd_wind.py` & `simfire-1.4.39/simfire/world/wind_mechanics/cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/wind_mechanics/perlin_wind.py` & `simfire-1.4.39/simfire/world/wind_mechanics/perlin_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/simfire/world/wind_mechanics/wind_controller.py` & `simfire-1.4.39/simfire/world/wind_mechanics/wind_controller.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.38/PKG-INFO` & `simfire-1.4.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfire
-Version: 1.4.38
+Version: 1.4.39
 Summary: Fire simulator built in Python
 Home-page: https://gitlab.mitre.org/fireline/simfire
 Keywords: python,reinforcement learning,simulation,fire
 Author: Tim Welsh
 Author-email: twelsh@mitre.org
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/open-dread-rando-2.4.0.tar.gz` & `tmp/open-dread-rando-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-dread-rando-2.4.0.tar", last modified: Mon Jul 17 10:10:51 2023, max compression
+gzip compressed data, was "open-dread-rando-2.4.1.tar", last modified: Wed Aug  9 03:38:44 2023, max compression
```

## Comparing `open-dread-rando-2.4.0.tar` & `open-dread-rando-2.4.1.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.064011 open-dread-rando-2.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.064011 open-dread-rando-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.github/workflows/patch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.064011 open-dread-rando-2.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.052011 open-dread-rando-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/custom_door_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/door_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/dread_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/elevator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/exefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/
--rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/custom_scenario.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/main.npdm
--rw-r--r--   0 runner    (1001) docker     (123)   190964 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/subsdk9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/exefs_patches/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/exefs_patches/debug_input.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s010_cave.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s020_magma.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s030_baselab.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s040_aqua.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s050_forest.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s060_quarantine.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s070_basesanc.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s080_shipyard.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s090_skybase.lc.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/bit.lua
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/data_structures.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/death_counter.lua
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/input_handling.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/msemenu_mainmenu.lua
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/randomizer_powerup.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.072011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.056011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    37130 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    49869 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)   128743 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex
--rw-r--r--   0 runner    (1001) docker     (123)   102269 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    31290 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    45613 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    39003 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.060011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.076011 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   431407 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    29925 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/lua_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/material_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/missile_color_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    27001 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/model_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/model_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/output_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/patcher_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/pickup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/static_fixes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/src/open_dread_rando/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/boss_powerup_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x.lua
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x_superquetzoa.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/randomizer_progressive_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_energy_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_hexs_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_tris_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/tilegroup_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/src/open_dread_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.068011 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-17 10:10:51.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 10:10:50.000000 open-dread-rando-2.4.0/src/open_dread_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_dread_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:10:51.080011 open-dread-rando-2.4.0/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_files/randomizer_progressive_expected.lua
--rw-r--r--   0 runner    (1001) docker     (123)   154075 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 10:10:38.000000 open-dread-rando-2.4.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.763816 open-dread-rando-2.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/.github/workflows/patch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-09 03:38:44.763816 open-dread-rando-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:38:44.763816 open-dread-rando-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.735815 open-dread-rando-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.747815 open-dread-rando-2.4.1/src/open_dread_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/custom_door_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21290 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/door_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/dread_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/elevator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/environmental_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/environmental_damage_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/exefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15151 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/custom_scenario.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/files/dread_depackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/dread_depackager/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/dread_depackager/main.npdm
+-rw-r--r--   0 runner    (1001) docker     (123)   190964 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/dread_depackager/subsdk9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/files/exefs_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/exefs_patches/debug_input.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s010_cave.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s020_magma.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s030_baselab.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    32062 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s040_aqua.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s050_forest.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s060_quarantine.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    30569 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s070_basesanc.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s080_shipyard.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s090_skybase.lc.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/bit.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/data_structures.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/death_counter.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/input_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/msemenu_mainmenu.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/randomizer_powerup.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.739815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.755815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    28577 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    37130 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    49869 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   128743 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)   102269 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    31290 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    45613 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    39003 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.743815 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/system/minimap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/system/minimap/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   431407 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    29925 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/lua_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/material_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/missile_color_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27001 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/model_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/patcher_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/static_fixes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.759816 open-dread-rando-2.4.1/src/open_dread_rando/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/boss_powerup_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/custom_core_x.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/custom_core_x_superquetzoa.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/randomizer_progressive_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/template_doorshield_energy_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/template_doorshield_hexs_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/template_doorshield_tris_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/tilegroup_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/src/open_dread_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.751815 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-09 03:38:44.000000 open-dread-rando-2.4.1/src/open_dread_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.763816 open-dread-rando-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/tests/test_dread_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:38:44.763816 open-dread-rando-2.4.1/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/tests/test_files/randomizer_progressive_expected.lua
+-rw-r--r--   0 runner    (1001) docker     (123)   154075 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/tests/test_lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-09 03:38:33.000000 open-dread-rando-2.4.1/tests/test_schema.py
```

### Comparing `open-dread-rando-2.4.0/.github/dependabot.yml` & `open-dread-rando-2.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/.github/workflows/patch.yml` & `open-dread-rando-2.4.1/.github/workflows/patch.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/.github/workflows/python.yml` & `open-dread-rando-2.4.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/.gitignore` & `open-dread-rando-2.4.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -127,9 +127,13 @@
 
 # Pyre type checker
 .pyre/
 
 # PyCharm
 .idea/
 
+# Deny certain files at root
+/*.txt
+/*.json
+
 # Project
 src/open_dread_rando/version.py
```

### Comparing `open-dread-rando-2.4.0/LICENSE` & `open-dread-rando-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/PKG-INFO` & `open-dread-rando-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.4.0
+Version: 2.4.1
 Summary: An open source randomizer patcher for Metroid Dread.
 Project-URL: Homepage, https://github.com/randovania/open-dread-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
```

### Comparing `open-dread-rando-2.4.0/README.md` & `open-dread-rando-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/pyproject.toml` & `open-dread-rando-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/cli.py` & `open-dread-rando-2.4.1/src/open_dread_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/cosmetic_patches.py` & `open-dread-rando-2.4.1/src/open_dread_rando/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/custom_door_types.py` & `open-dread-rando-2.4.1/src/open_dread_rando/custom_door_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     alternate_mats: list[MaterialData] # a list of materials needed for the alternate model
     alternate_mdl: ModelData = None # if none, ALTERNATE shields use default model and only change materials
     collision: str = None
 
 ALL_SHIELD_DATA: dict[str, ShieldData] = {
     "ice_missile": ShieldData(
         name="doorshieldicemissile",
-        type=DoorTemplates.TRIANGLES,
+        type=DoorTemplates.HEXAGONS,
         weaknesses=["ICE_MISSILE"],
         actordef="actors/props/doorshieldicemissile/charclasses/doorshieldicemissile.bmsad",
         default_mdl=ModelData(
             base_model=SUPER_MDL,
             new_path="actors/props/doorshieldicemissile/models/doorshieldicemissile.bcmdl",
             materials={
                 "mp_opaque_01": "actors/props/doorshieldicemissile/models/imats/doorshieldicemissile_mp_opaque_01.bsmat"
```

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/door_patcher.py` & `open-dread-rando-2.4.1/src/open_dread_rando/door_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,17 @@
     ICE_MISSILE = ("ice_missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_ICE_MISSILE, True, True,
                    ["actors/props/doorshieldmissile"])
     STORM_MISSILE = ("storm_missile", ActorData.DOOR_POWER, True, ActorData.SHIELD_STORM_MISSILE, True, True,
                      ["actors/props/doorshieldmissile"])
     BOMB = ("bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_BOMB, True, True,
             ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
     CROSS_BOMB = ("cross_bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_CROSS_BOMB, True, True,
-                  ["actors/props/doorshieldmissile"])
+                  ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
     POWER_BOMB = ("power_bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_POWER_BOMB, True, True,
-                  ["actors/props/door_shield_plasma"])
+                  ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
     GRAPPLE = ("grapple_beam", ActorData.DOOR_GRAPPLE, False, None, True, True,
                ["actors/props/door"])
     PRESENCE = ("phantom_cloak", ActorData.DOOR_PRESENCE, False, None, True, False,
                 ["actors/props/door"])
 
     def __init__(self, rdv_door_type: str, door_data: ActorData, need_shield: bool = False,
                  shield_data: ActorData = None, can_be_removed: bool = True, can_be_added: bool = True,
```

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/dread_patcher.py` & `open-dread-rando-2.4.1/src/open_dread_rando/dread_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/elevator.py` & `open-dread-rando-2.4.1/src/open_dread_rando/elevator.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage.py` & `open-dread-rando-2.4.1/src/open_dread_rando/environmental_damage.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/environmental_damage_sources.py` & `open-dread-rando-2.4.1/src/open_dread_rando/environmental_damage_sources.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/exefs.py` & `open-dread-rando-2.4.1/src/open_dread_rando/exefs.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/custom_scenario.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/custom_scenario.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/main.npdm` & `open-dread-rando-2.4.1/src/open_dread_rando/files/dread_depackager/main.npdm`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/dread_depackager/subsdk9` & `open-dread-rando-2.4.1/src/open_dread_rando/files/dread_depackager/subsdk9`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/exefs_patches/debug_input.s` & `open-dread-rando-2.4.1/src/open_dread_rando/files/exefs_patches/debug_input.s`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s010_cave.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s010_cave.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s020_magma.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s020_magma.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s030_baselab.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s030_baselab.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s040_aqua.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s040_aqua.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s050_forest.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s050_forest.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s060_quarantine.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s060_quarantine.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s070_basesanc.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s070_basesanc.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s080_shipyard.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s080_shipyard.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/levels/s090_skybase.lc.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/levels/s090_skybase.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/bit.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/bit.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/data_structures.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/data_structures.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/death_counter.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/death_counter.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/guilib.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/guilib.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/input_handling.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/input_handling.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/lua_libraries/room_names.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/lua_libraries/room_names.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/msemenu_mainmenu.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/msemenu_mainmenu.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/randomizer_powerup.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/files/randomizer_powerup.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex` & `open-dread-rando-2.4.1/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/files/schema.json` & `open-dread-rando-2.4.1/src/open_dread_rando/files/schema.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/game_patches.py` & `open-dread-rando-2.4.1/src/open_dread_rando/game_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/lua_editor.py` & `open-dread-rando-2.4.1/src/open_dread_rando/lua_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/lua_util.py` & `open-dread-rando-2.4.1/src/open_dread_rando/lua_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/map_icons.py` & `open-dread-rando-2.4.1/src/open_dread_rando/map_icons.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/material_patcher.py` & `open-dread-rando-2.4.1/src/open_dread_rando/material_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/missile_color_patcher.py` & `open-dread-rando-2.4.1/src/open_dread_rando/missile_color_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/model_data.py` & `open-dread-rando-2.4.1/src/open_dread_rando/model_data.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/model_patcher.py` & `open-dread-rando-2.4.1/src/open_dread_rando/model_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/objective.py` & `open-dread-rando-2.4.1/src/open_dread_rando/objective.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/output_config.py` & `open-dread-rando-2.4.1/src/open_dread_rando/output_config.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/patch_util.py` & `open-dread-rando-2.4.1/src/open_dread_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/patcher_editor.py` & `open-dread-rando-2.4.1/src/open_dread_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/pickup.py` & `open-dread-rando-2.4.1/src/open_dread_rando/pickup.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/static_fixes.py` & `open-dread-rando-2.4.1/src/open_dread_rando/static_fixes.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/custom_core_x.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_core_x_superquetzoa.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/custom_core_x_superquetzoa.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/custom_init.lua` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_energy_bmsad.json` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/template_doorshield_energy_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_hexs_bmsad.json` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/template_doorshield_hexs_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_doorshield_tris_bmsad.json` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/template_doorshield_tris_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/templates/template_powerup_bmsad.json` & `open-dread-rando-2.4.1/src/open_dread_rando/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/text_patches.py` & `open-dread-rando-2.4.1/src/open_dread_rando/text_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/tilegroup_patcher.py` & `open-dread-rando-2.4.1/src/open_dread_rando/tilegroup_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando/validator_with_default.py` & `open-dread-rando-2.4.1/src/open_dread_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando.egg-info/PKG-INFO` & `open-dread-rando-2.4.1/src/open_dread_rando.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.4.0
+Version: 2.4.1
 Summary: An open source randomizer patcher for Metroid Dread.
 Project-URL: Homepage, https://github.com/randovania/open-dread-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
```

### Comparing `open-dread-rando-2.4.0/src/open_dread_rando.egg-info/SOURCES.txt` & `open-dread-rando-2.4.1/src/open_dread_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/tests/test_dread_patcher.py` & `open-dread-rando-2.4.1/tests/test_dread_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/tests/test_files/starter_preset_patcher.json` & `open-dread-rando-2.4.1/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.4.0/tests/test_lua_util.py` & `open-dread-rando-2.4.1/tests/test_lua_util.py`

 * *Files identical despite different names*


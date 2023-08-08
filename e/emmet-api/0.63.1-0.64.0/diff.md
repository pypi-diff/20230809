# Comparing `tmp/emmet-api-0.63.1.tar.gz` & `tmp/emmet-api-0.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.63.1.tar", last modified: Tue Jul 25 23:02:15 2023, max compression
+gzip compressed data, was "emmet-api-0.64.0.tar", last modified: Tue Aug  8 22:25:12 2023, max compression
```

## Comparing `emmet-api-0.63.1.tar` & `emmet-api-0.64.0.tar`

### file list

```diff
@@ -1,358 +1,357 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-25 23:02:09.000000 emmet-api-0.63.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 23:02:15.944869 emmet-api-0.63.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 23:02:09.000000 emmet-api-0.63.1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.912868 emmet-api-0.63.1/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.920868 emmet-api-0.63.1/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.924868 emmet-api-0.63.1/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.928868 emmet-api-0.63.1/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/metal_binding/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/metal_binding/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.932869 emmet-api-0.63.1/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-25 23:02:09.000000 emmet-api-0.63.1/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 23:02:15.000000 emmet-api-0.63.1/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-07-25 23:02:15.000000 emmet-api-0.63.1/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:02:15.000000 emmet-api-0.63.1/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:02:15.000000 emmet-api-0.63.1/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 23:02:15.000000 emmet-api-0.63.1/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 23:02:15.000000 emmet-api-0.63.1/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-25 23:02:09.000000 emmet-api-0.63.1/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-07-25 23:02:09.000000 emmet-api-0.63.1/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-25 23:02:09.000000 emmet-api-0.63.1/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-25 23:02:09.000000 emmet-api-0.63.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:02:15.944869 emmet-api-0.63.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-25 23:02:09.000000 emmet-api-0.63.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-25 23:02:09.000000 emmet-api-0.63.1/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.916868 emmet-api-0.63.1/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.916868 emmet-api-0.63.1/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.936869 emmet-api-0.63.1/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.940869 emmet-api-0.63.1/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/metal_binding/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:15.944869 emmet-api-0.63.1/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-25 23:02:09.000000 emmet-api-0.63.1/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-08 22:25:05.000000 emmet-api-0.64.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-08 22:25:12.874932 emmet-api-0.64.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 22:25:05.000000 emmet-api-0.64.0/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.842932 emmet-api-0.64.0/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.850932 emmet-api-0.64.0/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.854932 emmet-api-0.64.0/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.858932 emmet-api-0.64.0/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.862932 emmet-api-0.64.0/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-08 22:25:05.000000 emmet-api-0.64.0/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-08 22:25:12.000000 emmet-api-0.64.0/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-08-08 22:25:12.000000 emmet-api-0.64.0/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:25:12.000000 emmet-api-0.64.0/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:25:12.000000 emmet-api-0.64.0/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-08 22:25:12.000000 emmet-api-0.64.0/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 22:25:12.000000 emmet-api-0.64.0/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-08-08 22:25:05.000000 emmet-api-0.64.0/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-08 22:25:05.000000 emmet-api-0.64.0/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-08-08 22:25:05.000000 emmet-api-0.64.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:25:12.874932 emmet-api-0.64.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-08 22:25:05.000000 emmet-api-0.64.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 22:25:05.000000 emmet-api-0.64.0/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.846932 emmet-api-0.64.0/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.846932 emmet-api-0.64.0/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.866932 emmet-api-0.64.0/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.870932 emmet-api-0.64.0/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:12.874932 emmet-api-0.64.0/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-08 22:25:05.000000 emmet-api-0.64.0/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.63.1/Dockerfile` & `emmet-api-0.64.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/core/api.py` & `emmet-api-0.64.0/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.64.0/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.64.0/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/core/documentation.py` & `emmet-api-0.64.0/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/core/global_header.py` & `emmet-api-0.64.0/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/core/settings.py` & `emmet-api-0.64.0/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.64.0/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.64.0/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.64.0/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.64.0/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.64.0/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/_messages/resources.py` & `emmet-api-0.64.0/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/dois/resources.py` & `emmet-api-0.64.0/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.64.0/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.64.0/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.64.0/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.64.0/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.64.0/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.64.0/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.64.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.64.0/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.64.0/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.64.0/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.64.0/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/metal_binding/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/metal_binding/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/metal_binding/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/tasks/utils.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/utils.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.64.0/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.64.0/emmet_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 Dockerfile
 app.py
-legacy_resources.py
 material_resources.py
 molecule_resources.py
 setup.py
 start.sh
 emmet/api/__init__.py
 emmet/api/core/__init__.py
 emmet/api/core/api.py
```

### Comparing `emmet-api-0.63.1/material_resources.py` & `emmet-api-0.64.0/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/molecule_resources.py` & `emmet-api-0.64.0/molecule_resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from emmet.api.routes.molecules.bonds.resources import bonding_resource
 from emmet.api.routes.molecules.metal_binding.resources import metal_binding_resource
 from emmet.api.routes.molecules.orbitals.resources import orbitals_resource
 from emmet.api.routes.molecules.redox.resources import redox_resource
 from emmet.api.routes.molecules.thermo.resources import thermo_resource
 from emmet.api.routes.molecules.vibrations.resources import vibration_resource
 from emmet.api.routes.molecules.summary.resources import summary_resource
+from emmet.api.routes.legacy.jcesr.resources import jcesr_resource
 
 
 resources = {}
 
 default_settings = MAPISettings()
 
 db_uri = os.environ.get("MPCONTRIBS_MONGO_HOST", None)
@@ -120,14 +121,18 @@
     summary_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="molecule_id",
         collection_name="molecules_summary",
     )
 
+    jcesr_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="task_id", collection_name="molecules"
+    )
+
 else:
     raise RuntimeError("Must specify MongoDB URI containing inputs.")
 
 
 mp_molecules_resources = list()
 
 # Tasks
@@ -175,8 +180,11 @@
 
 # Vibes
 mp_molecules_resources.extend([vibration_resource(vibes_store)])
 
 # Summary
 mp_molecules_resources.extend([summary_resource(summary_store)])
 
+# Legacy JCESR
+mp_molecules_resources.extend([jcesr_resource(jcesr_store)])
+
 resources.update({"molecules": mp_molecules_resources})
```

### Comparing `emmet-api-0.63.1/requirements/deployment.txt` & `emmet-api-0.64.0/requirements/deployment.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,102 +3,92 @@
 # by the following command:
 #
 #    pip-compile --output-file=emmet/emmet-api/requirements/deployment.txt emmet/emmet-api/setup.py python/requirements.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.20
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.20
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.100.0
+fastapi==0.101.0
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (emmet/emmet-api/setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via opentelemetry-api
 inflect==7.0.0
@@ -112,23 +102,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.19.0
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (emmet/emmet-api/setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -173,30 +163,30 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.19.0
     # via ddtrace
-orjson==3.9.2
+orjson==3.9.3
     # via maggma
 packaging==23.1
     # via
     #   gunicorn
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   -r python/requirements.txt
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
@@ -207,22 +197,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -249,15 +239,15 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0.1
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-referencing==0.30.0
+referencing==0.30.2
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
@@ -300,18 +290,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.10.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.9.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,110 +1,104 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -112,23 +106,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -154,15 +148,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -184,15 +178,15 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
@@ -203,22 +197,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -295,18 +289,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -326,22 +317,25 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -349,11 +343,13 @@
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.16.2
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,128 +1,118 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -147,47 +137,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -200,15 +191,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -242,15 +233,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -274,20 +265,24 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -297,32 +292,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -421,18 +416,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -484,15 +476,15 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.11.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,100 +1,94 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.11.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.100.0
+exceptiongroup==1.1.2
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via opentelemetry-api
 inflect==7.0.0
@@ -108,23 +102,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -150,15 +144,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -180,15 +174,15 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
@@ -199,22 +193,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -291,18 +285,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -322,14 +313,15 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,123 +1,118 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.100.0
+exceptiongroup==1.1.2
+    # via
+    #   anyio
+    #   cattrs
+    #   pytest
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -142,47 +137,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -195,15 +191,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -237,15 +233,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -269,20 +265,24 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -292,32 +292,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -416,18 +416,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -442,14 +439,19 @@
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
 threadpoolctl==3.2.0
     # via scikit-learn
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
@@ -457,14 +459,15 @@
     # via emmet-api (setup.py)
 types-setuptools==68.0.0.3
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.14
     # via types-requests
 typing-extensions==4.7.1
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   mypy
     #   pydantic
@@ -473,15 +476,15 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.8.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,117 +1,104 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==6.0.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -119,23 +106,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -161,15 +148,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.24.4
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -191,20 +178,18 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -212,22 +197,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -281,15 +266,15 @@
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -304,18 +289,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,126 +3,116 @@
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -157,47 +147,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -210,15 +201,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -284,22 +275,26 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -309,32 +304,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -433,18 +428,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -500,15 +492,15 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.9.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,114 +1,107 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==6.0.0
-    # via matplotlib
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -116,23 +109,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -158,15 +151,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.24.4
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -188,18 +181,20 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -207,22 +202,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -276,15 +271,15 @@
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.11.1
+scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -299,18 +294,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
```

### Comparing `emmet-api-0.63.1/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,128 +1,118 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -154,47 +144,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -207,15 +198,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -249,15 +240,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -281,20 +272,24 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -304,32 +299,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -428,18 +423,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -495,15 +487,15 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,102 +3,92 @@
 # by the following command:
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via opentelemetry-api
 inflect==7.0.0
@@ -112,23 +102,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -154,15 +144,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -184,15 +174,15 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
@@ -203,22 +193,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -295,18 +285,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,136 +1,133 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -147,47 +144,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -200,15 +198,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -242,15 +240,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -274,20 +272,24 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -297,32 +299,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -421,18 +423,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -467,43 +466,49 @@
     # via emmet-api (setup.py)
 types-setuptools==68.0.0.3
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.14
     # via types-requests
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.16.2
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,98 +3,88 @@
 # by the following command:
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via opentelemetry-api
 inflect==7.0.0
@@ -108,23 +98,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -150,15 +140,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -180,15 +170,15 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
@@ -199,22 +189,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -291,18 +281,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,121 +3,111 @@
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -142,47 +132,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -195,15 +186,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -237,15 +228,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -269,20 +260,24 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -292,32 +287,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -416,18 +411,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -473,15 +465,15 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.11.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,117 +1,96 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.11.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.2
-    # via
-    #   anyio
-    #   cattrs
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==6.0.0
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -119,23 +98,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -161,15 +140,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.24.4
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -191,20 +170,18 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -212,22 +189,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -281,15 +258,15 @@
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -304,18 +281,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
@@ -335,25 +309,21 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -361,13 +331,11 @@
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.16.2
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,126 +3,116 @@
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
@@ -157,47 +147,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -210,15 +201,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -284,22 +275,26 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -309,32 +304,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -433,18 +428,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -500,15 +492,15 @@
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.64.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,114 +1,107 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
-httpcore==0.17.3
-    # via dnspython
+    # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==6.0.0
-    # via matplotlib
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -116,23 +109,23 @@
     #   boto3
     #   botocore
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -158,15 +151,15 @@
     # via
     #   maggma
     #   mp-api
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
-numpy==1.25.1
+numpy==1.24.4
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -188,18 +181,20 @@
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via pymatgen
 protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -207,22 +202,22 @@
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -276,15 +271,15 @@
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.3.0
     # via matminer
-scipy==1.11.1
+scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
@@ -299,18 +294,15 @@
     # via
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
```

### Comparing `emmet-api-0.63.1/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.64.0/requirements/macos-latest_py3.11_extras.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,143 +1,121 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
-    # via
-    #   httpcore
-    #   starlette
+    # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.9
+boto3==1.28.17
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.9
+botocore==1.31.17
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.2.0
     # via requests
 click==8.1.6
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
-cmake==3.27.0
-    # via ddtrace
 colorama==0.4.6
     # via griffe
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.17.1
+ddtrace==1.17.3
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.63.0
+emmet-core[all]==0.63.1
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.2
-    # via
-    #   anyio
-    #   cattrs
-    #   pytest
-fastapi==0.100.0
+fastapi==0.100.1
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
-flake8==6.0.0
+flake8==6.1.0
     # via emmet-api (setup.py)
 flask==2.3.2
     # via mongogrant
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
 griffe==0.32.3
     # via mkdocstrings-python
 gunicorn==21.2.0
     # via emmet-api (setup.py)
 h11==0.14.0
-    # via
-    #   httpcore
-    #   uvicorn-tschaume
+    # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
-httpcore==0.17.3
-    # via dnspython
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.8.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   mkdocstrings
-    #   opentelemetry-api
-importlib-resources==6.0.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -154,47 +132,48 @@
 joblib==1.3.1
     # via
     #   pymatgen
     #   pymatgen-analysis-diffusion
     #   scikit-learn
 jsmin==3.0.1
     # via mkdocs-minify-plugin
-jsonschema==4.18.4
+jsonschema==4.18.5
     # via maggma
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.24
+maggma==0.53.0
     # via emmet-api (setup.py)
-markdown==3.3.7
+markdown==3.4.4
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.3
     # via
     #   jinja2
+    #   mkdocs
     #   mkdocstrings
     #   werkzeug
 matminer==0.9.0
     # via robocrys
 matplotlib==3.7.2
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.3
+mkdocs==1.5.2
     # via
     #   emmet-api (setup.py)
     #   mkdocs-autorefs
     #   mkdocs-awesome-pages-plugin
     #   mkdocs-markdownextradata-plugin
     #   mkdocs-material
     #   mkdocs-minify-plugin
@@ -207,15 +186,15 @@
     # via emmet-api (setup.py)
 mkdocs-material==8.2.16
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
-mkdocs-minify-plugin==0.6.4
+mkdocs-minify-plugin==0.7.1
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
 mkdocstrings-python==1.2.1
     # via mkdocstrings
@@ -249,15 +228,15 @@
     # via mkdocs-awesome-pages-plugin
 networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.8.0
     # via pre-commit
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   maggma
     #   matminer
     #   matplotlib
     #   pandas
     #   pymatgen
@@ -281,20 +260,24 @@
     #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==1.5.3
     # via
     #   matminer
     #   pymatgen
-paramiko==3.2.0
+paramiko==3.3.1
     # via sshtunnel
+pathspec==0.11.2
+    # via mkdocs
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.9.1
-    # via virtualenv
+platformdirs==3.10.0
+    # via
+    #   mkdocs
+    #   virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
 protobuf==4.23.4
@@ -304,32 +287,32 @@
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.11
+pydantic==1.10.12
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
     #   pymatgen
-pydash==7.0.5
+pydash==7.0.6
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
-pyflakes==3.0.1
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
 pymatgen==2023.7.20
     # via
     #   emmet-core
     #   matminer
@@ -428,18 +411,15 @@
     #   ddsketch
     #   ddtrace
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
+    # via anyio
 snowballstemmer==2.2.0
     # via pydocstyle
 spglib==2.0.2
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
@@ -454,19 +434,14 @@
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
 threadpoolctl==3.2.0
     # via scikit-learn
-tomli==2.0.1
-    # via
-    #   coverage
-    #   mypy
-    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
@@ -474,49 +449,42 @@
     # via emmet-api (setup.py)
 types-setuptools==68.0.0.3
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.14
     # via types-requests
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
-    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
-virtualenv==20.24.1
+virtualenv==20.24.2
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.3.6
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.16.2
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.63.1/setup.py` & `emmet-api-0.64.0/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/_consumer/test_query_operators.py` & `emmet-api-0.64.0/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/_general_store/test_query_operators.py` & `emmet-api-0.64.0/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/core/test_mapi.py` & `emmet-api-0.64.0/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.64.0/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/electrodes/test_utils.py` & `emmet-api-0.64.0/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/materials/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/materials/test_utils.py` & `emmet-api-0.64.0/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/summary/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.64.0/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.64.0/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/synthesis/test_utils.py` & `emmet-api-0.64.0/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/tasks/test_utils.py` & `emmet-api-0.64.0/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/materials/xas/test_query_operators.py` & `emmet-api-0.64.0/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/metal_binding/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/metal_binding/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/tasks/test_utils.py` & `emmet-api-0.64.0/tests/molecules/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.63.1/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.64.0/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*


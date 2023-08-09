# Comparing `tmp/harmony-1.2.3126.tar.gz` & `tmp/harmony-1.2.3127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/harmony-1.2.3126.tar", last modified: Mon Jan 30 15:18:48 2023, max compression
+gzip compressed data, was "dist/harmony-1.2.3127.tar", last modified: Sat Feb 18 21:24:28 2023, max compression
```

## Comparing `harmony-1.2.3126.tar` & `harmony-1.2.3127.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony.egg-info/
--rw-r--r--   0 ayang     (1000) ayang     (1000)       28 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony.egg-info/top_level.txt
--rw-r--r--   0 ayang     (1000) ayang     (1000)        1 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony.egg-info/dependency_links.txt
--rw-r--r--   0 ayang     (1000) ayang     (1000)      102 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony.egg-info/entry_points.txt
--rw-r--r--   0 ayang     (1000) ayang     (1000)     3733 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony.egg-info/SOURCES.txt
--rw-r--r--   0 ayang     (1000) ayang     (1000)       78 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony.egg-info/requires.txt
--rw-r--r--   0 ayang     (1000) ayang     (1000)    10512 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony.egg-info/PKG-INFO
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/tests/
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2965 2022-09-18 03:23:24.000000 harmony-1.2.3126/tests/test_h2py_runtime.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     6226 2022-09-18 03:23:24.000000 harmony-1.2.3126/tests/test_h2py.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-09-18 03:23:24.000000 harmony-1.2.3126/tests/__init__.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1480 2022-04-24 01:30:00.000000 harmony-1.2.3126/LICENSE
--rw-r--r--   0 ayang     (1000) ayang     (1000)     8625 2023-01-29 02:41:47.000000 harmony-1.2.3126/README.md
--rw-r--r--   0 ayang     (1000) ayang     (1000)       91 2022-04-24 01:30:00.000000 harmony-1.2.3126/pyproject.toml
--rw-r--r--   0 ayang     (1000) ayang     (1000)      364 2022-09-18 03:23:24.000000 harmony-1.2.3126/MANIFEST.in
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/
--rw-r--r--   0 ayang     (1000) ayang     (1000)     9804 2023-01-30 01:58:57.000000 harmony-1.2.3126/harmony_model_checker/compile.py
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/charm/
--rw-r--r--   0 ayang     (1000) ayang     (1000)      714 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/code.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)    48475 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/value.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2537 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/hashdict.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1698 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/queue.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     6377 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/value.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2080 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/ops.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)    13391 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/hashdict.c
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/charm/python_ext/
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1200 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/python_ext/ext.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      736 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/dot.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)      241 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/head.h
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/charm/iface/
--rw-r--r--   0 ayang     (1000) ayang     (1000)      375 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/iface/iface.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1307 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/iface/iface_graph.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     7949 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/iface/iface_graph.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)    12902 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/iface/iface.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)   140410 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/ops.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2360 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/strbuf.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      955 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/hashset.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     3918 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/graph.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)      362 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/dfa.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     9063 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/json.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      185 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/spawn.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     8194 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/graph.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)    14218 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/hashtab.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     5970 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/dfa.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      468 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/minheap.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2982 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/dot.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      946 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/stack.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      994 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/json.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)   104030 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/charm.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      786 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/global.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1458 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/thread.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)      525 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/strbuf.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1845 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/code.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1468 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/global.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     6378 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/thread.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)      630 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/queue.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     3703 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/charm.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)      437 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/stack.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2921 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/minheap.c
--rw-r--r--   0 ayang     (1000) ayang     (1000)     3872 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/charm/hashtab.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)      643 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/charm/hashset.h
--rw-r--r--   0 ayang     (1000) ayang     (1000)     9918 2023-01-30 02:47:52.000000 harmony-1.2.3126/harmony_model_checker/main.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2313 2023-01-30 15:15:15.000000 harmony-1.2.3126/harmony_model_checker/config.py
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/util/
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1843 2022-10-16 18:42:24.000000 harmony-1.2.3126/harmony_model_checker/util/logger.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-04-24 01:30:00.000000 harmony-1.2.3126/harmony_model_checker/util/__init__.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1764 2023-01-30 01:58:57.000000 harmony-1.2.3126/harmony_model_checker/dfacmp.py
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/harmony/
--rw-r--r--   0 ayang     (1000) ayang     (1000)    20494 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/harmony/charm.js
--rw-r--r--   0 ayang     (1000) ayang     (1000)      435 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/harmony/charm.css
--rw-r--r--   0 ayang     (1000) ayang     (1000)    59592 2023-01-30 01:58:57.000000 harmony-1.2.3126/harmony_model_checker/harmony/ops.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     7953 2022-10-02 03:14:50.000000 harmony-1.2.3126/harmony_model_checker/harmony/DumpASTVisitor.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     3833 2023-01-30 01:56:50.000000 harmony-1.2.3126/harmony_model_checker/harmony/state.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     5207 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/harmony/AbstractASTVisitor.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    14731 2023-01-30 01:58:57.000000 harmony-1.2.3126/harmony_model_checker/harmony/value.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1817 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/harmony/jsonstring.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    11649 2023-01-30 03:54:29.000000 harmony-1.2.3126/harmony_model_checker/harmony/verbose.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     5663 2023-01-30 01:59:01.000000 harmony-1.2.3126/harmony_model_checker/harmony/code.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    14068 2023-01-30 03:54:29.000000 harmony-1.2.3126/harmony_model_checker/harmony/genhtml.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)      271 2023-01-30 01:58:33.000000 harmony-1.2.3126/harmony_model_checker/harmony/bag_util.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    16383 2023-01-30 03:54:29.000000 harmony-1.2.3126/harmony_model_checker/harmony/behavior.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     5616 2023-01-30 03:54:29.000000 harmony-1.2.3126/harmony_model_checker/harmony/brief.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    81993 2023-01-30 01:58:57.000000 harmony-1.2.3126/harmony_model_checker/harmony/ast.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    67448 2023-01-30 03:54:29.000000 harmony-1.2.3126/harmony_model_checker/harmony/harmony.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/harmony/__init__.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     7409 2023-01-30 01:56:50.000000 harmony-1.2.3126/harmony_model_checker/harmony/tex.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2134 2023-01-30 01:58:57.000000 harmony-1.2.3126/harmony_model_checker/harmony/scope.py
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/parser/
--rw-r--r--   0 ayang     (1000) ayang     (1000)    12141 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony_model_checker/parser/HarmonyVisitor.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    40122 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony_model_checker/parser/HarmonyLexer.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2555 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/parser/HarmonyErrorListener.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)   178763 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony_model_checker/parser/HarmonyParser.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2734 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/parser/custom_denter.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    34049 2023-01-30 01:58:33.000000 harmony-1.2.3126/harmony_model_checker/parser/antlr_rule_visitor.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-04-24 01:30:00.000000 harmony-1.2.3126/harmony_model_checker/parser/__init__.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)      916 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/exception.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     8891 2023-01-30 03:54:29.000000 harmony-1.2.3126/harmony_model_checker/iface.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)       64 2023-01-30 15:18:47.000000 harmony-1.2.3126/harmony_model_checker/__init__.py
-drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-01-30 15:18:48.000000 harmony-1.2.3126/harmony_model_checker/modules/
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1441 2022-09-22 01:00:21.000000 harmony-1.2.3126/harmony_model_checker/modules/bag.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)      470 2022-04-24 01:30:00.000000 harmony-1.2.3126/harmony_model_checker/modules/synchBusy.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)      794 2022-04-24 01:30:00.000000 harmony-1.2.3126/harmony_model_checker/modules/synchImprecise.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1451 2022-09-22 01:00:21.000000 harmony-1.2.3126/harmony_model_checker/modules/synch.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)      402 2022-09-22 01:00:21.000000 harmony-1.2.3126/harmony_model_checker/modules/alloc.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)      418 2022-04-24 01:30:00.000000 harmony-1.2.3126/harmony_model_checker/modules/hoare.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)     2262 2022-09-18 03:23:24.000000 harmony-1.2.3126/harmony_model_checker/modules/synchS.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1396 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/modules/set.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)      367 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/modules/fork.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)      326 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/modules/action.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-04-24 01:30:00.000000 harmony-1.2.3126/harmony_model_checker/modules/__init__.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)     1784 2023-01-29 02:41:47.000000 harmony-1.2.3126/harmony_model_checker/modules/list.hny
--rw-r--r--   0 ayang     (1000) ayang     (1000)       38 2023-01-30 15:18:48.000000 harmony-1.2.3126/setup.cfg
--rw-r--r--   0 ayang     (1000) ayang     (1000)     5226 2023-01-22 05:13:24.000000 harmony-1.2.3126/setup.py
--rw-r--r--   0 ayang     (1000) ayang     (1000)    10512 2023-01-30 15:18:48.000000 harmony-1.2.3126/PKG-INFO
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)       28 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/top_level.txt
+-rw-r--r--   0 ayang     (1000) ayang     (1000)        1 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/dependency_links.txt
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      102 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/entry_points.txt
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     3733 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/SOURCES.txt
+-rw-r--r--   0 ayang     (1000) ayang     (1000)       78 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/requires.txt
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    10512 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony.egg-info/PKG-INFO
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/tests/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2965 2022-09-18 03:23:24.000000 harmony-1.2.3127/tests/test_h2py_runtime.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     6226 2022-09-18 03:23:24.000000 harmony-1.2.3127/tests/test_h2py.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-09-18 03:23:24.000000 harmony-1.2.3127/tests/__init__.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1480 2022-04-24 01:30:00.000000 harmony-1.2.3127/LICENSE
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     8625 2023-01-29 02:41:47.000000 harmony-1.2.3127/README.md
+-rw-r--r--   0 ayang     (1000) ayang     (1000)       91 2022-04-24 01:30:00.000000 harmony-1.2.3127/pyproject.toml
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      364 2022-09-18 03:23:24.000000 harmony-1.2.3127/MANIFEST.in
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     9804 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/compile.py
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/charm/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      714 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/code.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    48475 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/value.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2537 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/hashdict.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1698 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/queue.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     6377 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/value.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2080 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/ops.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    13391 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/hashdict.c
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/charm/python_ext/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1200 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/python_ext/ext.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      736 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/dot.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      241 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/head.h
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/charm/iface/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      375 2023-01-29 02:41:47.000000 harmony-1.2.3127/harmony_model_checker/charm/iface/iface.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1307 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/iface/iface_graph.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     7949 2023-01-29 02:41:47.000000 harmony-1.2.3127/harmony_model_checker/charm/iface/iface_graph.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    12902 2023-02-18 21:14:26.000000 harmony-1.2.3127/harmony_model_checker/charm/iface/iface.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)   140410 2023-02-18 21:14:26.000000 harmony-1.2.3127/harmony_model_checker/charm/ops.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2360 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/strbuf.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      955 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/hashset.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     3918 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/graph.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      362 2023-01-29 02:41:47.000000 harmony-1.2.3127/harmony_model_checker/charm/dfa.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     9063 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/json.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      185 2023-01-29 02:41:47.000000 harmony-1.2.3127/harmony_model_checker/charm/spawn.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     8194 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/graph.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    14218 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/hashtab.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     5970 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/dfa.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      468 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/minheap.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2982 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/dot.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      946 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/stack.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      994 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/json.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)   104030 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/charm.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      786 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/global.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1458 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/thread.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      525 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/strbuf.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1845 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/code.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1468 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/global.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     6378 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/thread.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      630 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/queue.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     3703 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/charm.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      437 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/stack.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2921 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/minheap.c
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     3872 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/charm/hashtab.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      643 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/charm/hashset.h
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     9918 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/main.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2313 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/config.py
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/util/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1843 2022-10-16 18:42:24.000000 harmony-1.2.3127/harmony_model_checker/util/logger.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-04-24 01:30:00.000000 harmony-1.2.3127/harmony_model_checker/util/__init__.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1764 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/dfacmp.py
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/harmony/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    20494 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/charm.js
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      435 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/harmony/charm.css
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    59592 2023-02-18 21:14:26.000000 harmony-1.2.3127/harmony_model_checker/harmony/ops.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     7953 2022-10-02 03:14:50.000000 harmony-1.2.3127/harmony_model_checker/harmony/DumpASTVisitor.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     3833 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/state.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     5207 2023-01-31 18:40:22.000000 harmony-1.2.3127/harmony_model_checker/harmony/AbstractASTVisitor.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    14731 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/value.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1817 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/jsonstring.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    11649 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/verbose.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     5663 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/code.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    14068 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/genhtml.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      271 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/bag_util.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    16387 2023-02-18 21:14:54.000000 harmony-1.2.3127/harmony_model_checker/harmony/behavior.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     5616 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/brief.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    81993 2023-02-18 21:14:26.000000 harmony-1.2.3127/harmony_model_checker/harmony/ast.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    67448 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/harmony.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/harmony/__init__.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     7409 2023-02-18 21:14:26.000000 harmony-1.2.3127/harmony_model_checker/harmony/tex.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2134 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/harmony/scope.py
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/parser/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    12141 2023-02-18 21:24:27.000000 harmony-1.2.3127/harmony_model_checker/parser/HarmonyVisitor.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    40122 2023-02-18 21:24:27.000000 harmony-1.2.3127/harmony_model_checker/parser/HarmonyLexer.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2555 2023-01-31 03:26:54.000000 harmony-1.2.3127/harmony_model_checker/parser/HarmonyErrorListener.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)   178763 2023-02-18 21:24:27.000000 harmony-1.2.3127/harmony_model_checker/parser/HarmonyParser.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2734 2023-01-31 03:26:54.000000 harmony-1.2.3127/harmony_model_checker/parser/custom_denter.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    34049 2023-02-18 21:14:26.000000 harmony-1.2.3127/harmony_model_checker/parser/antlr_rule_visitor.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-04-24 01:30:00.000000 harmony-1.2.3127/harmony_model_checker/parser/__init__.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      916 2023-01-31 03:26:54.000000 harmony-1.2.3127/harmony_model_checker/exception.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     8891 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/iface.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)       64 2023-02-18 21:24:27.000000 harmony-1.2.3127/harmony_model_checker/__init__.py
+drwxr-xr-x   0 ayang     (1000) ayang     (1000)        0 2023-02-18 21:24:28.000000 harmony-1.2.3127/harmony_model_checker/modules/
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1441 2022-09-22 01:00:21.000000 harmony-1.2.3127/harmony_model_checker/modules/bag.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      470 2022-04-24 01:30:00.000000 harmony-1.2.3127/harmony_model_checker/modules/synchBusy.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      794 2022-04-24 01:30:00.000000 harmony-1.2.3127/harmony_model_checker/modules/synchImprecise.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1451 2022-09-22 01:00:21.000000 harmony-1.2.3127/harmony_model_checker/modules/synch.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      402 2022-09-22 01:00:21.000000 harmony-1.2.3127/harmony_model_checker/modules/alloc.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      418 2022-04-24 01:30:00.000000 harmony-1.2.3127/harmony_model_checker/modules/hoare.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     2262 2022-09-18 03:23:24.000000 harmony-1.2.3127/harmony_model_checker/modules/synchS.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1396 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/modules/set.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      367 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/modules/fork.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)      326 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/modules/action.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)        0 2022-04-24 01:30:00.000000 harmony-1.2.3127/harmony_model_checker/modules/__init__.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     1784 2023-02-18 21:12:43.000000 harmony-1.2.3127/harmony_model_checker/modules/list.hny
+-rw-r--r--   0 ayang     (1000) ayang     (1000)       38 2023-02-18 21:24:28.000000 harmony-1.2.3127/setup.cfg
+-rw-r--r--   0 ayang     (1000) ayang     (1000)     5226 2023-02-18 20:08:02.000000 harmony-1.2.3127/setup.py
+-rw-r--r--   0 ayang     (1000) ayang     (1000)    10512 2023-02-18 21:24:28.000000 harmony-1.2.3127/PKG-INFO
```

### Comparing `harmony-1.2.3126/harmony.egg-info/SOURCES.txt` & `harmony-1.2.3127/harmony.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony.egg-info/PKG-INFO` & `harmony-1.2.3127/harmony.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony
-Version: 1.2.3126
+Version: 1.2.3127
 Summary: Harmony Programming Language
 Home-page: https://harmony.cs.cornell.edu
 Author: Robbert van Renesse
 Author-email: rvr@cs.cornell.edu
 License: BSD
 Description: # Harmony
```

### Comparing `harmony-1.2.3126/tests/test_h2py_runtime.py` & `harmony-1.2.3127/tests/test_h2py_runtime.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/tests/test_h2py.py` & `harmony-1.2.3127/tests/test_h2py.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/LICENSE` & `harmony-1.2.3127/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/README.md` & `harmony-1.2.3127/README.md`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/compile.py` & `harmony-1.2.3127/harmony_model_checker/compile.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/code.h` & `harmony-1.2.3127/harmony_model_checker/charm/code.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/value.c` & `harmony-1.2.3127/harmony_model_checker/charm/value.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/hashdict.h` & `harmony-1.2.3127/harmony_model_checker/charm/hashdict.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/queue.c` & `harmony-1.2.3127/harmony_model_checker/charm/queue.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/value.h` & `harmony-1.2.3127/harmony_model_checker/charm/value.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/ops.h` & `harmony-1.2.3127/harmony_model_checker/charm/ops.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/hashdict.c` & `harmony-1.2.3127/harmony_model_checker/charm/hashdict.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/python_ext/ext.c` & `harmony-1.2.3127/harmony_model_checker/charm/python_ext/ext.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/dot.h` & `harmony-1.2.3127/harmony_model_checker/charm/dot.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/iface/iface_graph.h` & `harmony-1.2.3127/harmony_model_checker/charm/iface/iface_graph.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/iface/iface_graph.c` & `harmony-1.2.3127/harmony_model_checker/charm/iface/iface_graph.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/iface/iface.c` & `harmony-1.2.3127/harmony_model_checker/charm/iface/iface.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/ops.c` & `harmony-1.2.3127/harmony_model_checker/charm/ops.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/strbuf.c` & `harmony-1.2.3127/harmony_model_checker/charm/strbuf.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/hashset.c` & `harmony-1.2.3127/harmony_model_checker/charm/hashset.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/graph.h` & `harmony-1.2.3127/harmony_model_checker/charm/graph.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/json.c` & `harmony-1.2.3127/harmony_model_checker/charm/json.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/graph.c` & `harmony-1.2.3127/harmony_model_checker/charm/graph.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/hashtab.c` & `harmony-1.2.3127/harmony_model_checker/charm/hashtab.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/dfa.c` & `harmony-1.2.3127/harmony_model_checker/charm/dfa.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/dot.c` & `harmony-1.2.3127/harmony_model_checker/charm/dot.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/stack.c` & `harmony-1.2.3127/harmony_model_checker/charm/stack.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/json.h` & `harmony-1.2.3127/harmony_model_checker/charm/json.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/charm.c` & `harmony-1.2.3127/harmony_model_checker/charm/charm.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/global.h` & `harmony-1.2.3127/harmony_model_checker/charm/global.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/thread.h` & `harmony-1.2.3127/harmony_model_checker/charm/thread.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/strbuf.h` & `harmony-1.2.3127/harmony_model_checker/charm/strbuf.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/code.c` & `harmony-1.2.3127/harmony_model_checker/charm/code.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/global.c` & `harmony-1.2.3127/harmony_model_checker/charm/global.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/thread.c` & `harmony-1.2.3127/harmony_model_checker/charm/thread.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/queue.h` & `harmony-1.2.3127/harmony_model_checker/charm/queue.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/charm.h` & `harmony-1.2.3127/harmony_model_checker/charm/charm.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/minheap.c` & `harmony-1.2.3127/harmony_model_checker/charm/minheap.c`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/hashtab.h` & `harmony-1.2.3127/harmony_model_checker/charm/hashtab.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/charm/hashset.h` & `harmony-1.2.3127/harmony_model_checker/charm/hashset.h`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/main.py` & `harmony-1.2.3127/harmony_model_checker/main.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/config.py` & `harmony-1.2.3127/harmony_model_checker/config.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/util/logger.py` & `harmony-1.2.3127/harmony_model_checker/util/logger.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/dfacmp.py` & `harmony-1.2.3127/harmony_model_checker/dfacmp.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/charm.js` & `harmony-1.2.3127/harmony_model_checker/harmony/charm.js`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/ops.py` & `harmony-1.2.3127/harmony_model_checker/harmony/ops.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/DumpASTVisitor.py` & `harmony-1.2.3127/harmony_model_checker/harmony/DumpASTVisitor.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/state.py` & `harmony-1.2.3127/harmony_model_checker/harmony/state.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/AbstractASTVisitor.py` & `harmony-1.2.3127/harmony_model_checker/harmony/AbstractASTVisitor.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/value.py` & `harmony-1.2.3127/harmony_model_checker/harmony/value.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/jsonstring.py` & `harmony-1.2.3127/harmony_model_checker/harmony/jsonstring.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/verbose.py` & `harmony-1.2.3127/harmony_model_checker/harmony/verbose.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/code.py` & `harmony-1.2.3127/harmony_model_checker/harmony/code.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/genhtml.py` & `harmony-1.2.3127/harmony_model_checker/harmony/genhtml.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/behavior.py` & `harmony-1.2.3127/harmony_model_checker/harmony/behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
         )
         intermediate_dfa = DFA.from_nfa(nfa)  # returns an equivalent DFA
         if minify and len(final_states) != 0:
             print("minify #states=%d"%len(intermediate_dfa.states))
             dfa = intermediate_dfa.minify(retain_names = True)
             print("minify done #states=%d"%len(dfa.states))
         else:
-            dfa = intermediate
+            dfa = intermediate_dfa
         dfa_states = dfa.states
         (dfa_transitions,) = dfa.transitions,
         dfa_initial_state = dfa.initial_state
         dfa_final_states = dfa.final_states
     else:
         # Compute the epsilon closure for each state
         eps_closures = { s:eps_closure(states, transitions, s) for s in states }
```

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/brief.py` & `harmony-1.2.3127/harmony_model_checker/harmony/brief.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/ast.py` & `harmony-1.2.3127/harmony_model_checker/harmony/ast.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/harmony.py` & `harmony-1.2.3127/harmony_model_checker/harmony/harmony.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/tex.py` & `harmony-1.2.3127/harmony_model_checker/harmony/tex.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/harmony/scope.py` & `harmony-1.2.3127/harmony_model_checker/harmony/scope.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/parser/HarmonyVisitor.py` & `harmony-1.2.3127/harmony_model_checker/parser/HarmonyVisitor.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/parser/HarmonyLexer.py` & `harmony-1.2.3127/harmony_model_checker/parser/HarmonyLexer.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/parser/HarmonyErrorListener.py` & `harmony-1.2.3127/harmony_model_checker/parser/HarmonyErrorListener.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/parser/HarmonyParser.py` & `harmony-1.2.3127/harmony_model_checker/parser/HarmonyParser.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/parser/custom_denter.py` & `harmony-1.2.3127/harmony_model_checker/parser/custom_denter.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/parser/antlr_rule_visitor.py` & `harmony-1.2.3127/harmony_model_checker/parser/antlr_rule_visitor.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/exception.py` & `harmony-1.2.3127/harmony_model_checker/exception.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/iface.py` & `harmony-1.2.3127/harmony_model_checker/iface.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/modules/bag.hny` & `harmony-1.2.3127/harmony_model_checker/modules/bag.hny`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/modules/synchImprecise.hny` & `harmony-1.2.3127/harmony_model_checker/modules/synchImprecise.hny`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/modules/synch.hny` & `harmony-1.2.3127/harmony_model_checker/modules/synch.hny`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/modules/synchS.hny` & `harmony-1.2.3127/harmony_model_checker/modules/synchS.hny`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/modules/set.hny` & `harmony-1.2.3127/harmony_model_checker/modules/set.hny`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/harmony_model_checker/modules/list.hny` & `harmony-1.2.3127/harmony_model_checker/modules/list.hny`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/setup.py` & `harmony-1.2.3127/setup.py`

 * *Files identical despite different names*

### Comparing `harmony-1.2.3126/PKG-INFO` & `harmony-1.2.3127/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony
-Version: 1.2.3126
+Version: 1.2.3127
 Summary: Harmony Programming Language
 Home-page: https://harmony.cs.cornell.edu
 Author: Robbert van Renesse
 Author-email: rvr@cs.cornell.edu
 License: BSD
 Description: # Harmony
```


# Comparing `tmp/grapes-graph-0.0.3.tar.gz` & `tmp/grapes-graph-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grapes-graph-0.0.3.tar", last modified: Mon Jul 31 03:13:09 2023, max compression
+gzip compressed data, was "grapes-graph-0.0.4.tar", last modified: Wed Aug  9 04:11:53 2023, max compression
```

## Comparing `grapes-graph-0.0.3.tar` & `grapes-graph-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.113387 grapes-graph-0.0.3/
--rw-r--r--   0 ericwang   (501) staff       (20)     1069 2023-07-23 02:02:04.000000 grapes-graph-0.0.3/LICENSE.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       27 2023-07-24 20:57:07.000000 grapes-graph-0.0.3/MANIFEST.in
--rw-r--r--   0 ericwang   (501) staff       (20)      783 2023-07-31 03:13:09.113222 grapes-graph-0.0.3/PKG-INFO
--rw-r--r--   0 ericwang   (501) staff       (20)      153 2023-07-31 01:25:30.000000 grapes-graph-0.0.3/README.md
--rw-r--r--   0 ericwang   (501) staff       (20)      851 2023-07-31 03:12:23.000000 grapes-graph-0.0.3/pyproject.toml
--rw-r--r--   0 ericwang   (501) staff       (20)       24 2023-07-24 23:55:23.000000 grapes-graph-0.0.3/requirements.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       38 2023-07-31 03:13:09.113441 grapes-graph-0.0.3/setup.cfg
--rw-r--r--   0 ericwang   (501) staff       (20)      268 2023-07-30 05:43:41.000000 grapes-graph-0.0.3/setup.py
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.108455 grapes-graph-0.0.3/src/
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.109688 grapes-graph-0.0.3/src/grapes/
--rw-r--r--   0 ericwang   (501) staff       (20)       43 2023-07-24 19:27:07.000000 grapes-graph-0.0.3/src/grapes/__init__.py
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.111817 grapes-graph-0.0.3/src/grapes/cgraph/
--rw-r--r--   0 ericwang   (501) staff       (20)     2668 2023-07-31 03:03:53.000000 grapes-graph-0.0.3/src/grapes/cgraph/__init__.pyi
--rw-r--r--   0 ericwang   (501) staff       (20)    18397 2023-07-31 03:09:10.000000 grapes-graph-0.0.3/src/grapes/cgraph/cgraph.c
--rw-r--r--   0 ericwang   (501) staff       (20)     2013 2023-07-31 03:08:41.000000 grapes-graph-0.0.3/src/grapes/cgraph/cgraph.h
--rw-r--r--   0 ericwang   (501) staff       (20)     2331 2023-07-31 01:23:45.000000 grapes-graph-0.0.3/src/grapes/cgraph/deque.c
--rw-r--r--   0 ericwang   (501) staff       (20)      579 2023-07-31 01:23:47.000000 grapes-graph-0.0.3/src/grapes/cgraph/deque.h
--rw-r--r--   0 ericwang   (501) staff       (20)     2993 2023-07-31 01:23:50.000000 grapes-graph-0.0.3/src/grapes/cgraph/heap.c
--rw-r--r--   0 ericwang   (501) staff       (20)      657 2023-07-31 01:23:52.000000 grapes-graph-0.0.3/src/grapes/cgraph/heap.h
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.112900 grapes-graph-0.0.3/src/grapes_graph.egg-info/
--rw-r--r--   0 ericwang   (501) staff       (20)      783 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/PKG-INFO
--rw-r--r--   0 ericwang   (501) staff       (20)      506 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/SOURCES.txt
--rw-r--r--   0 ericwang   (501) staff       (20)        1 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/dependency_links.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       25 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/requires.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       14 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/top_level.txt
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.113025 grapes-graph-0.0.3/tests/
--rw-r--r--   0 ericwang   (501) staff       (20)      248 2023-07-23 01:49:03.000000 grapes-graph-0.0.3/tests/test_dijkstra.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-08-09 04:11:53.025358 grapes-graph-0.0.4/
+-rw-r--r--   0 ericwang   (501) staff       (20)     1069 2023-07-23 02:02:04.000000 grapes-graph-0.0.4/LICENSE.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       27 2023-08-02 01:47:05.000000 grapes-graph-0.0.4/MANIFEST.in
+-rw-r--r--   0 ericwang   (501) staff       (20)      865 2023-08-09 04:11:53.025202 grapes-graph-0.0.4/PKG-INFO
+-rw-r--r--   0 ericwang   (501) staff       (20)      235 2023-08-02 23:43:26.000000 grapes-graph-0.0.4/README.md
+-rw-r--r--   0 ericwang   (501) staff       (20)      851 2023-08-09 04:07:12.000000 grapes-graph-0.0.4/pyproject.toml
+-rw-r--r--   0 ericwang   (501) staff       (20)       24 2023-07-24 23:55:23.000000 grapes-graph-0.0.4/requirements.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       38 2023-08-09 04:11:53.025398 grapes-graph-0.0.4/setup.cfg
+-rw-r--r--   0 ericwang   (501) staff       (20)      344 2023-08-08 23:43:01.000000 grapes-graph-0.0.4/setup.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-08-09 04:11:53.018885 grapes-graph-0.0.4/src/
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-08-09 04:11:53.020013 grapes-graph-0.0.4/src/grapes/
+-rw-r--r--   0 ericwang   (501) staff       (20)       43 2023-07-31 03:25:55.000000 grapes-graph-0.0.4/src/grapes/__init__.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-08-09 04:11:53.022878 grapes-graph-0.0.4/src/grapes/cgraph/
+-rw-r--r--   0 ericwang   (501) staff       (20)     2814 2023-08-09 03:53:54.000000 grapes-graph-0.0.4/src/grapes/cgraph/__init__.pyi
+-rw-r--r--   0 ericwang   (501) staff       (20)    16889 2023-08-09 04:04:57.000000 grapes-graph-0.0.4/src/grapes/cgraph/cgraph.c
+-rw-r--r--   0 ericwang   (501) staff       (20)     2167 2023-08-09 00:40:48.000000 grapes-graph-0.0.4/src/grapes/cgraph/cgraph.h
+-rw-r--r--   0 ericwang   (501) staff       (20)     2373 2023-08-02 18:58:53.000000 grapes-graph-0.0.4/src/grapes/cgraph/deque.c
+-rw-r--r--   0 ericwang   (501) staff       (20)      579 2023-07-31 01:23:47.000000 grapes-graph-0.0.4/src/grapes/cgraph/deque.h
+-rw-r--r--   0 ericwang   (501) staff       (20)     3077 2023-08-04 02:12:26.000000 grapes-graph-0.0.4/src/grapes/cgraph/heap.c
+-rw-r--r--   0 ericwang   (501) staff       (20)      657 2023-07-31 01:23:52.000000 grapes-graph-0.0.4/src/grapes/cgraph/heap.h
+-rw-r--r--   0 ericwang   (501) staff       (20)      236 2023-08-02 17:53:27.000000 grapes-graph-0.0.4/src/grapes/cgraph/macros.h
+-rw-r--r--   0 ericwang   (501) staff       (20)     3838 2023-08-09 04:00:34.000000 grapes-graph-0.0.4/src/grapes/cgraph/trav.c
+-rw-r--r--   0 ericwang   (501) staff       (20)      626 2023-08-09 04:05:04.000000 grapes-graph-0.0.4/src/grapes/cgraph/trav.h
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-08-09 04:11:53.024612 grapes-graph-0.0.4/src/grapes_graph.egg-info/
+-rw-r--r--   0 ericwang   (501) staff       (20)      865 2023-08-09 04:11:53.000000 grapes-graph-0.0.4/src/grapes_graph.egg-info/PKG-INFO
+-rw-r--r--   0 ericwang   (501) staff       (20)      583 2023-08-09 04:11:53.000000 grapes-graph-0.0.4/src/grapes_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)        1 2023-08-09 04:11:53.000000 grapes-graph-0.0.4/src/grapes_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       25 2023-08-09 04:11:53.000000 grapes-graph-0.0.4/src/grapes_graph.egg-info/requires.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       14 2023-08-09 04:11:53.000000 grapes-graph-0.0.4/src/grapes_graph.egg-info/top_level.txt
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-08-09 04:11:53.025003 grapes-graph-0.0.4/tests/
+-rw-r--r--   0 ericwang   (501) staff       (20)      712 2023-08-09 01:15:47.000000 grapes-graph-0.0.4/tests/test_dijkstra.py
```

### Comparing `grapes-graph-0.0.3/LICENSE.txt` & `grapes-graph-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.3/PKG-INFO` & `grapes-graph-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grapes-graph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python graph library written in C
 Author-email: Eric Wang <ericwangyy@ucla.edu>
 License: MIT License
 Keywords: graph
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -19,8 +19,10 @@
 # Grapes
 Python graph library written in C
 
 ## Documentation
 Documentation found here: https://nouturnsign.github.io/grapes-doc/
 
 ## TODO
+*   ensure all values are freed even if exception occurs
+*   prevent XSS with svg
 *   more algos!
```

### Comparing `grapes-graph-0.0.3/pyproject.toml` & `grapes-graph-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 63.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grapes-graph"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python graph library written in C"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT License" }
 authors = [{ name = "Eric Wang", email = "ericwangyy@ucla.edu" }]
 keywords = ["graph"]
 classifiers = [
```

### Comparing `grapes-graph-0.0.3/src/grapes/cgraph/__init__.pyi` & `grapes-graph-0.0.4/src/grapes/cgraph/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,83 @@
-from typing import Callable
+from typing import Type
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class Graph:
-    """Simple, undirected graph.
+class Multigraph:
+    """Underlying graph type.
 
     .. note::
         Nodes are represented as 0-based indices.
     """
 
-    def __init__(self: Self, node_count: int) -> None:
-        """Initialize a simple, undirected graph.
+    def __init__(self: Self, is_directed: bool, node_count: int = 0) -> None:
+        """Initialize a graph.
 
-        :param node_count: The initial number of nodes within the graph.
+        :param is_directed: Whether or not the graph is directed.
+        :type is_directed: bool
+        :param node_count: The initial number of nodes within the graph,
+            defaults to 0.
         :type node_count: int
+        :rtype: None
         """
     def get_node_count(self: Self) -> int:
         """Get the number of nodes in the graph.
 
         :rtype: int
         """
     def get_edge_count(self: Self) -> int:
         """Get the number of edges in the graph.
 
+        .. note::
+            Edges are considered as having their own identity, so multiple
+            edges with the same nodes will be counted separately.
+
         :rtype: int
         """
     def get_edges(self: Self) -> list[tuple[int, int]]:
         """Get the edges in the graph.
 
-        .. warning::
-            If (u, v) is in edges, (v, u) will not also be returned. However,
-            duplicate inserted edges will still be duplicated.
+        .. note::
+            If the graph is undirected and (u, v) is in edges, (v, u) will not
+            also be returned. However, edges are considered as having their own
+            identity, so multiple edges will be returned.
 
         :returns: List of edges
         :rtype: list[tuple[int, int]]
         """
     def add_node(self: Self) -> int:
         """Add a node to the graph.
 
         :returns: The index to the new node added.
         :rtype: int
         """
-    def add_edge(self: Self, u: int, v: int) -> None:
-        """Add an undirected edge between two nodes.
+    def add_edge(self: Self, u: int, v: int, *, weight: float = 1.0) -> None:
+        """Add an edge between two nodes.
 
-        .. warning::
-            Adding duplicate edges will not raise an error.
+        .. note::
+            Edges are considered as having their own identity.
 
         :param u: node
         :type u: int
         :param v: node
         :type v: int
+        :param weight: weight of edge, defaults to 1.0
+        :type weight: float
         :rtype: None
         """
-    def dijkstra_path(
-        self: Self, src: int, dst: int, weight: Callable[[int, int], float]
-    ) -> list[int]:
+    def dijkstra_path(self: Self, src: int, dst: int) -> list[int]:
         """Get the shortest path in the graph using Dijkstra's algorithm.
 
-        .. note::
-            The weight function should accept both (u, v) and (v, u) as
-            potential inputs.
-
         :param src: Begin (source) node
         :type src: int
         :param dst: End (destination) node
         :type dst: int
-        :param weight: Weight function that accepts two nodes and returns the
-            weight as a float.
-        :type weight: Callable[[int, int], float]
         :return: List of nodes, starting from `src` and ending with `dst`.
             Returns an empty list if no path found.
         :rtype: list[int]
         """
     def get_component_sizes(self: Self) -> list[int]:
         """Return the sizes of the (connected) components in the graph.
```

### Comparing `grapes-graph-0.0.3/src/grapes/cgraph/cgraph.c` & `grapes-graph-0.0.4/src/grapes/cgraph/cgraph.c`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,136 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "cgraph.h"
 
 #include "deque.h"
 #include "heap.h"
+#include "macros.h"
+#include "trav.h"
 
 PyMODINIT_FUNC
 PyInit_cgraph(void)
 {
     PyObject *m;
-    if (PyType_Ready(&GraphType) < 0) {
+    if (PyType_Ready(&MultigraphType) < 0) {
         return NULL;
     }
 
     m = PyModule_Create(&cgraphmodule);
     if (m == NULL) {
         return NULL;
     }
 
-    Py_INCREF(&GraphType);
-    if (PyModule_AddObject(m, "Graph", (PyObject *) &GraphType) < 0) {
-        Py_DECREF(&GraphType);
+    Py_INCREF(&MultigraphType);
+    if (PyModule_AddObject(m, "Multigraph", (PyObject *) &MultigraphType) <
+        0) {
+        Py_DECREF(&MultigraphType);
         Py_DECREF(m);
         return NULL;
     }
 
     return m;
 }
 
 static struct PyModuleDef cgraphmodule = {
     PyModuleDef_HEAD_INIT,
     .m_name = "cgraph",
     .m_doc = PyDoc_STR("Grapes core functionality written in C"),
     .m_size = -1,
 };
 
-typedef struct GraphObject {
-    PyObject_HEAD Py_ssize_t *
-        *adj_list;  // list of adjacency lists (adj_list[i]
-                    // = array of neighbors to node i)
-    Py_ssize_t  node_count;
-    Py_ssize_t  max_node_count;  // current maximum number of nodes allocated
+typedef struct MultigraphObject {
+    PyObject_HEAD
+    int          is_directed;
+    Py_ssize_t **adj_list;  // list of adjacency lists (adj_list[i]
+    // = array of neighbors to node i)
     Py_ssize_t *neighbor_count;
     Py_ssize_t
         *max_neighbor_count;  // current maximum number of neighbors
                               // (max_neighbor_count[i] = current maximum
                               // number of neighbors allocated to node i)
+    Py_ssize_t node_count;
+    Py_ssize_t max_node_count;  // current maximum number of nodes allocated
+    double   **weight;          // list of weight lists (by index)
     Py_ssize_t edge_count;
-} GraphObject;
+} MultigraphObject;
 
-static PyTypeObject GraphType = {
-    PyVarObject_HEAD_INIT(NULL, 0).tp_name = "grapes.cgraph.Graph",
-    .tp_doc = PyDoc_STR("Undirected graph object."),
-    .tp_basicsize = sizeof(GraphObject),
+static PyTypeObject MultigraphType = {
+    PyVarObject_HEAD_INIT(NULL, 0)  // clang-format off
+    .tp_name = "grapes.cgraph.Multigraph",  // clang-format on
+    .tp_doc = PyDoc_STR("Underlying graph type."),
+    .tp_basicsize = sizeof(MultigraphObject),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
-    .tp_dealloc = (destructor) Graph_dealloc,
-    .tp_new = Graph_new,
-    .tp_init = (initproc) Graph_init,
-    .tp_methods = Graph_methods,
+    .tp_dealloc = (destructor) Multigraph_dealloc,
+    .tp_new = Multigraph_new,
+    .tp_init = (initproc) Multigraph_init,
+    .tp_methods = Multigraph_methods,
 };
 
 static void
-Graph_dealloc(GraphObject *self)
+Multigraph_dealloc(MultigraphObject *self)
 {
     for (Py_ssize_t i = 0; i < self->max_node_count; ++i) {
         free(self->adj_list[i]);
         self->adj_list[i] = NULL;
     }
+    for (Py_ssize_t i = 0; i < self->max_node_count; ++i) {
+        free(self->weight[i]);
+        self->weight[i] = NULL;
+    }
     free(self->adj_list);
     self->adj_list = NULL;
     free(self->neighbor_count);
     self->neighbor_count = NULL;
     free(self->max_neighbor_count);
     self->max_neighbor_count = NULL;
+    free(self->weight);
+    self->weight = NULL;
     Py_TYPE(self)->tp_free((PyObject *) self);
 }
 
 static PyObject *
-Graph_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
+Multigraph_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
 {
-    GraphObject *self;
-    self = (GraphObject *) type->tp_alloc(type, 0);
+    MultigraphObject *self;
+    self = (MultigraphObject *) type->tp_alloc(type, 0);
     if (self != NULL) {
         self->adj_list = NULL;
         self->node_count = 0;
         self->max_node_count = 0;
         self->neighbor_count = NULL;
         self->max_neighbor_count = NULL;
+        self->weight = NULL;
         self->edge_count = 0;
     }
     return (PyObject *) self;
 }
 
 static int
-Graph_init(GraphObject *self, PyObject *args, PyObject *kwds)
+Multigraph_init(MultigraphObject *self, PyObject *args, PyObject *kwds)
 {
-    static char *kwlist[] = {"node_count", NULL};
-    Py_ssize_t   node_count;
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "n", kwlist, &node_count)) {
+    static char *kwlist[] = {"is_directed", "node_count", NULL};
+    int          is_directed;
+    Py_ssize_t   node_count = 0;
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "p|n", kwlist, &is_directed,
+                                     &node_count)) {
         return -1;
     }
 
     if (node_count < 0) {
         PyErr_Format(PyExc_ValueError,
                      "node_count should be nonnegative, but given %ld",
                      node_count);
         return -1;
     }
 
+    self->is_directed = is_directed;
+
     self->adj_list = malloc(sizeof(*self->adj_list) * node_count);
     if (self->adj_list == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc adj_list at memory address %p",
                      (void *) self->adj_list);
         return -1;
     }
@@ -144,65 +161,77 @@
             (void *) self->max_neighbor_count);
         return -1;
     }
     for (Py_ssize_t i = 0; i < node_count; ++i) {
         self->max_neighbor_count[i] = 0;
     }
 
+    self->weight = malloc(sizeof(*self->weight) * node_count);
+    if (self->weight == NULL) {
+        PyErr_Format(PyExc_MemoryError,
+                     "Unable to malloc weight at memory address %p",
+                     (void *) self->weight);
+        return -1;
+    }
+    for (Py_ssize_t i = 0; i < node_count; ++i) {
+        self->weight[i] = NULL;
+    }
+
     self->edge_count = 0;
 
     return 0;
 }
 
-static PyMethodDef Graph_methods[] = {
-    {"get_node_count", (PyCFunction) Graph_get_node_count, METH_NOARGS,
+static PyMethodDef Multigraph_methods[] = {
+    {"get_node_count", (PyCFunction) Multigraph_get_node_count, METH_NOARGS,
      "Return the number of nodes in the graph."},
-    {"get_edge_count", (PyCFunction) Graph_get_edge_count, METH_NOARGS,
+    {"get_edge_count", (PyCFunction) Multigraph_get_edge_count, METH_NOARGS,
      "Return the number of edges in the graph."},
-    {"get_edges", (PyCFunction) Graph_get_edges, METH_NOARGS,
+    {"get_edges", (PyCFunction) Multigraph_get_edges, METH_NOARGS,
      "Return the edges in the graph."},
-    {"add_node", (PyCFunction) Graph_add_node, METH_NOARGS,
+    {"add_node", (PyCFunction) Multigraph_add_node, METH_NOARGS,
      "Add a node to the graph, returning the newest node."},
-    {"add_edge", (PyCFunction) Graph_add_edge, METH_VARARGS | METH_KEYWORDS,
+    {"add_edge", (PyCFunction) Multigraph_add_edge,
+     METH_VARARGS | METH_KEYWORDS,
      "Add an undirected edge to the graph given existing nodes."},
-    {"dijkstra_path", (PyCFunction) Graph_dijkstra_path,
+    {"dijkstra_path", (PyCFunction) Multigraph_dijkstra_path,
      METH_VARARGS | METH_KEYWORDS,
      "Find the shortest path between two nodes using Dijkstra's algorithm"},
-    {"get_component_sizes", (PyCFunction) Graph_get_component_sizes,
+    {"get_component_sizes", (PyCFunction) Multigraph_get_component_sizes,
      METH_NOARGS, "Return the sizes of the components in the graph."},
-    {"is_bipartite", (PyCFunction) Graph_is_bipartite, METH_NOARGS,
+    {"is_bipartite", (PyCFunction) Multigraph_is_bipartite, METH_NOARGS,
      "Return whether the graph is bipartite or not."},
     {NULL}};
 
 static PyObject *
-Graph_get_node_count(GraphObject *self, PyObject *Py_UNUSED(ignored))
+Multigraph_get_node_count(MultigraphObject *self, PyObject *Py_UNUSED(ignored))
 {
     return PyLong_FromSsize_t(self->node_count);
 }
 
 static PyObject *
-Graph_get_edge_count(GraphObject *self, PyObject *Py_UNUSED(ignored))
+Multigraph_get_edge_count(MultigraphObject *self, PyObject *Py_UNUSED(ignored))
 {
     return PyLong_FromSsize_t(self->edge_count);
 }
 
 static PyObject *
-Graph_get_edges(GraphObject *self, PyObject *Py_UNUSED(ignored))
+Multigraph_get_edges(MultigraphObject *self, PyObject *Py_UNUSED(ignored))
 {
     PyObject *edges = PyList_New(self->edge_count);
     if (edges == NULL) {
         PyErr_SetString(PyExc_MemoryError, "Unable to initialize edges list");
     }
 
     Py_ssize_t i = 0;
     PyObject  *uv;
     for (Py_ssize_t u = 0; u < self->node_count; ++u) {
         for (Py_ssize_t j = 0; j < self->neighbor_count[u]; ++j) {
             Py_ssize_t v = self->adj_list[u][j];
-            if (u > v) {
+            if (!self->is_directed && u > v) {
                 continue;
             }
             uv = Py_BuildValue("(nn)", u, v);
             if (uv == NULL) {
                 PyErr_Format(PyExc_TypeError,
                              "Unable to format uv given u=%ld and v=%ld", u,
                              v);
@@ -214,15 +243,15 @@
             ++i;
         }
     }
     return edges;
 }
 
 static PyObject *
-Graph_add_node(GraphObject *self, PyObject *Py_UNUSED(ignored))
+Multigraph_add_node(MultigraphObject *self, PyObject *Py_UNUSED(ignored))
 {
     if (self->node_count >= self->max_node_count) {
         // approximately a growth factor of 112.5%
         self->max_node_count =
             (self->max_node_count + (self->max_node_count >> 3) + 6) &
             (~(Py_ssize_t) 3);
         self->adj_list = realloc(
@@ -233,14 +262,26 @@
                          (void *) self->adj_list);
             return NULL;
         }
         for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i) {
             self->adj_list[i] = NULL;
         }
 
+        self->weight = realloc(self->weight,
+                               sizeof(*self->weight) * self->max_node_count);
+        if (self->weight == NULL) {
+            PyErr_Format(PyExc_MemoryError,
+                         "Unable to realloc weight at memory address %p",
+                         (void *) self->weight);
+            return NULL;
+        }
+        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i) {
+            self->weight[i] = NULL;
+        }
+
         self->neighbor_count =
             realloc(self->neighbor_count,
                     sizeof(*self->neighbor_count) * self->max_node_count);
         if (self->neighbor_count == NULL) {
             PyErr_Format(
                 PyExc_MemoryError,
                 "Unable to realloc neighbor_count at memory address %p",
@@ -266,330 +307,233 @@
         }
     }
 
     return PyLong_FromSsize_t(self->node_count++);
 }
 
 static PyObject *
-Graph_add_edge(GraphObject *self, PyObject *args, PyObject *kwds)
+Multigraph_add_edge(MultigraphObject *self, PyObject *args, PyObject *kwds)
 {
-    static char *kwlist[] = {"u", "v", NULL};
+    static char *kwlist[] = {"u", "v", "weight", NULL};
     Py_ssize_t   u, v;
+    double       weight = 1.0;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "nn", kwlist, &u, &v)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "nn|$d", kwlist, &u, &v,
+                                     &weight)) {
         return NULL;
     }
 
     if (u < 0 || u >= self->node_count || v < 0 || v >= self->node_count) {
         PyErr_Format(PyExc_ValueError,
-                     "u and v should be existing nodes. Graph has "
+                     "u and v should be existing nodes. Multigraph has "
                      "node_count=%ld but given u=%ld and v=%ld",
                      self->node_count, u, v);
         return NULL;
     }
 
+    if (add_directed_edge_noinc(self, u, v, weight) == -1) {
+        return NULL;
+    }
+    if (!self->is_directed) {
+        if (add_directed_edge_noinc(self, v, u, weight) == -1) {
+            return NULL;
+        }
+    }
+
+    ++self->edge_count;
+
+    Py_RETURN_NONE;
+}
+
+int
+add_directed_edge_noinc(MultigraphObject *self, Py_ssize_t u, Py_ssize_t v,
+                        double weight)
+{
     if (self->neighbor_count[u] >= self->max_neighbor_count[u]) {
         self->max_neighbor_count[u] =
             (self->max_neighbor_count[u] + (self->max_neighbor_count[u] >> 3) +
              6) &
             (~(Py_ssize_t) 3);
         self->adj_list[u] =
             realloc(self->adj_list[u],
                     sizeof(*self->adj_list[u]) * self->max_neighbor_count[u]);
         if (self->adj_list[u] == NULL) {
             PyErr_Format(PyExc_MemoryError,
                          "Unable to realloc adj_list[u] at memory address %p "
                          "with u=%ld",
                          (void *) self->adj_list[u], u);
-            return NULL;
+            return -1;
         }
-    }
-    self->adj_list[u][self->neighbor_count[u]++] = v;
-
-    if (self->neighbor_count[v] >= self->max_neighbor_count[v]) {
-        self->max_neighbor_count[v] =
-            (self->max_neighbor_count[v] + (self->max_neighbor_count[v] >> 3) +
-             6) &
-            (~(Py_ssize_t) 3);
-        self->adj_list[v] =
-            realloc(self->adj_list[v],
-                    sizeof(*self->adj_list[v]) * self->max_neighbor_count[v]);
-        if (self->adj_list[v] == NULL) {
+        self->weight[u] =
+            realloc(self->weight[u],
+                    sizeof(*self->weight[u]) * self->max_neighbor_count[u]);
+        if (self->weight[u] == NULL) {
             PyErr_Format(PyExc_MemoryError,
-                         "Unable to realloc adj_list[v] at memory address %p "
-                         "with v=%ld",
-                         (void *) self->adj_list[v], v);
-            return NULL;
+                         "Unable to realloc weight[u] at memory address %p "
+                         "with u=%ld",
+                         (void *) self->weight[u], u);
+            return -1;
         }
     }
-    self->adj_list[v][self->neighbor_count[v]++] = u;
-
-    ++self->edge_count;
-
-    Py_RETURN_NONE;
+    self->adj_list[u][self->neighbor_count[u]] = v;
+    self->weight[u][self->neighbor_count[u]] = weight;
+    ++self->neighbor_count[u];
+    return 0;
 }
 
 static PyObject *
-Graph_dijkstra_path(GraphObject *self, PyObject *args, PyObject *kwds)
+Multigraph_dijkstra_path(MultigraphObject *self, PyObject *args,
+                         PyObject *kwds)
 {
-    static char *kwlist[] = {"src", "dst", "weight", NULL};
+    static char *kwlist[] = {"src", "dst", NULL};
     Py_ssize_t   src, dst;
-    PyObject    *weight = NULL;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "nnO", kwlist, &src, &dst,
-                                     &weight)) {
-        return NULL;
-    }
 
-    if (!PyCallable_Check(weight)) {
-        PyErr_SetString(PyExc_TypeError, "weight must be callable.");
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "nn", kwlist, &src, &dst)) {
         return NULL;
     }
 
-    Py_ssize_t *dist = malloc(sizeof(*dist) * self->node_count);
+    double *dist = malloc(sizeof(*dist) * self->node_count);
     if (dist == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc dist at memory address %p",
                      (void *) dist);
         return NULL;
     }
 
-    short *visited = malloc(sizeof(*visited) * self->node_count);
-    if (visited == NULL) {
-        PyErr_Format(PyExc_MemoryError,
-                     "Unable to malloc visited at memory address %p",
-                     (void *) visited);
-        return NULL;
-    }
-
     Py_ssize_t *prev = malloc(sizeof(*prev) * self->node_count);
     if (prev == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc prev at memory address %p",
                      (void *) prev);
+        free(dist);
         return NULL;
     }
 
-    for (Py_ssize_t i = 0; i < self->node_count; ++i) {
-        dist[i] = PY_SSIZE_T_MAX;
-        visited[i] = GRAPES_FALSE;
-        prev[i] = self->node_count;
-    }
-    dist[src] = 0;
-    visited[src] = GRAPES_TRUE;
-    prev[src] = src;
-
-    MinHeap *heap =
-        MinHeap_alloc((self->node_count * (self->node_count - 1)) / 2);
-    MinHeap_insert(heap, src, 0);
-    Py_ssize_t u, v;
-    double     w;
-    while (!MinHeap_is_empty(heap)) {
-        u = MinHeap_extract_min(heap);
-        visited[u] = GRAPES_TRUE;
-        for (Py_ssize_t i = 0; i < self->neighbor_count[u]; ++i) {
-            v = self->adj_list[u][i];
-            if (visited[v]) {
-                continue;
-            }
-            w = get_weight(weight, u, v);
-            if (w == -1 && PyErr_Occurred() != NULL) {
-                return NULL;
-            }
-
-            if (dist[v] - dist[u] > w) {
-                dist[v] = dist[u] + w;
-                prev[v] = u;
-                MinHeap_insert(heap, v, dist[v]);
-            }
-        }
+    visit_dijkstra(self->adj_list, self->neighbor_count, self->node_count, src,
+                   self->weight, dist, prev);
+    if (PyErr_Occurred() != NULL) {
+        free(dist);
+        free(prev);
+        return NULL;
     }
 
     PyObject *path = PyList_New(0);
     if (path == NULL) {
         PyErr_SetString(PyExc_MemoryError, "Unable to initialize path");
     }
     if (prev[dst] == self->node_count) {
+        free(dist);
+        free(prev);
         return path;
     }
 
     if (PyList_Append(path, PyLong_FromSsize_t(dst)) == -1) {
+        free(dist);
+        free(prev);
         return NULL;
     }
     Py_ssize_t curr = dst;
     do {
         curr = prev[curr];
         if (PyList_Append(path, PyLong_FromSsize_t(curr)) == -1) {
+            free(dist);
+            free(prev);
             return NULL;
         }
     } while (curr != src);
 
     if (PyList_Reverse(path) == -1) {
+        free(dist);
+        free(prev);
         return NULL;
     }
 
     free(dist);
-    dist = NULL;
-    free(visited);
-    visited = NULL;
     free(prev);
-    prev = NULL;
-    MinHeap_free(heap);
-    heap = NULL;
-
     return path;
 }
 
 static PyObject *
-Graph_get_component_sizes(GraphObject *self, PyObject *args, PyObject *kwds)
+Multigraph_get_component_sizes(MultigraphObject *self, PyObject *args,
+                               PyObject *kwds)
 {
     Py_ssize_t *sizes = malloc(sizeof(*sizes) * self->node_count);
     if (sizes == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc sizes at memory address %p",
                      (void *) sizes);
         return NULL;
     }
     short *visited = malloc(sizeof(*visited) * self->node_count);
     if (visited == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc visited at memory address %p",
                      (void *) visited);
+        free(sizes);
         return NULL;
     }
     for (Py_ssize_t i = 0; i < self->node_count; ++i) {
         sizes[i] = 0;
         visited[i] = GRAPES_FALSE;
     }
 
     Py_ssize_t count = 0;
     for (Py_ssize_t i = 0; i < self->node_count; ++i) {
         if (!visited[i]) {
-            sizes[count++] = visit(self, i, visited);
+            sizes[count++] =
+                visit(self->adj_list, self->neighbor_count, i, visited);
+        }
+        if (PyErr_Occurred() != NULL) {
+            free(sizes);
+            free(visited);
+            return NULL;
         }
     }
 
     PyObject *component_sizes = PyList_New(count);
     if (component_sizes == NULL) {
         PyErr_SetString(PyExc_MemoryError,
                         "Unable to initialize component_sizes");
     }
 
     for (Py_ssize_t i = 0; i < count; ++i) {
         if (PyList_SetItem(component_sizes, i, PyLong_FromSsize_t(sizes[i])) ==
             -1) {
+            free(sizes);
+            free(visited);
             return NULL;
         }
     }
 
     free(sizes);
-    sizes = NULL;
     free(visited);
-    visited = NULL;
     return component_sizes;
 }
 
 static PyObject *
-Graph_is_bipartite(GraphObject *self, PyObject *args, PyObject *kwds)
+Multigraph_is_bipartite(MultigraphObject *self, PyObject *args, PyObject *kwds)
 {
     short *color = malloc(sizeof(*color) * self->node_count);
     if (color == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc color at memory address %p",
                      (void *) color);
         return NULL;
     }
     for (Py_ssize_t i = 0; i < self->node_count; ++i) {
         color[i] = GRAPES_NO_COLOR;
     }
 
     for (Py_ssize_t i = 0; i < self->node_count; ++i) {
-        if (!visit_color(self, i, color)) {
+        if (!visit_color(self->adj_list, self->neighbor_count, i, color)) {
+            free(color);
             Py_RETURN_FALSE;
         }
-    }
-    Py_RETURN_TRUE;
-}
-
-double
-get_weight(PyObject *weight, Py_ssize_t u, Py_ssize_t v)
-{
-    const int failed = -1;
-    double    w;
-    PyObject *uvargs;
-    PyObject *ret_value;
-
-    uvargs = Py_BuildValue("(nn)", u, v);
-    if (uvargs == NULL) {
-        PyErr_Format(PyExc_TypeError,
-                     "Unable to format args given u=%ld and v=%ld", u, v);
-        return failed;
-    }
-    ret_value = PyObject_Call(weight, uvargs, NULL);
-    if (ret_value == NULL) {
-        PyErr_Format(PyExc_TypeError,
-                     "Unable to call weight function on args given "
-                     "weight=%R and uvargs=%R",
-                     weight, uvargs);
-        return failed;
-    }
-    w = PyFloat_AsDouble(ret_value);
-    if (w == -1 && PyErr_Occurred() != NULL) {
-        PyErr_Format(PyExc_ValueError,
-                     "weight function returned a non-float value "
-                     "given ret_value=%R",
-                     ret_value);
-        return failed;
-    }
-
-    return w;
-}
-
-Py_ssize_t
-visit(GraphObject *graph, Py_ssize_t src, short *visited)
-{
-    visited[src] = GRAPES_TRUE;
-    Py_ssize_t size = 1;
-    Deque     *queue = Deque_alloc();  // push_back, pop_front
-    Deque_push_back(queue, src);
-    while (!Deque_is_empty(queue)) {
-        Py_ssize_t curr = Deque_pop_front(queue);
-        for (Py_ssize_t j = 0; j < graph->neighbor_count[curr]; ++j) {
-            Py_ssize_t neighbor = graph->adj_list[curr][j];
-            if (!visited[neighbor]) {
-                visited[neighbor] = GRAPES_TRUE;
-                ++size;
-                Deque_push_back(queue, neighbor);
-            }
+        if (PyErr_Occurred() != NULL) {
+            free(color);
+            return NULL;
         }
     }
-    Deque_free(queue);
-    return size;
-}
 
-short
-visit_color(GraphObject *graph, Py_ssize_t src, short *color)
-{
-    if (color[src] != GRAPES_NO_COLOR) {
-        return GRAPES_TRUE;
-    }
-    color[src] = GRAPES_RED;
-    Deque *queue = Deque_alloc();  // push_back, pop_front
-    Deque_push_back(queue, src);
-    while (!Deque_is_empty(queue)) {
-        Py_ssize_t curr = Deque_pop_front(queue);
-        for (Py_ssize_t j = 0; j < graph->neighbor_count[curr]; ++j) {
-            Py_ssize_t neighbor = graph->adj_list[curr][j];
-            if (color[neighbor] == GRAPES_NO_COLOR) {
-                color[neighbor] =
-                    (color[curr] == GRAPES_RED) ? GRAPES_BLUE : GRAPES_RED;
-                Deque_push_back(queue, neighbor);
-            }
-            else if (color[neighbor] == color[curr]) {
-                Deque_free(queue);
-                return GRAPES_FALSE;
-            }
-        }
-    }
-    Deque_free(queue);
-    return GRAPES_TRUE;
+    free(color);
+    Py_RETURN_TRUE;
 }
```

### Comparing `grapes-graph-0.0.3/src/grapes/cgraph/deque.c` & `grapes-graph-0.0.4/src/grapes/cgraph/deque.c`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 } Deque;
 
 Deque *
 Deque_alloc()
 {
     Deque *deque = malloc(sizeof(*deque));
     if (deque == NULL) {
-        fprintf(stderr, "Failed to allocate deque\n");
+        PyErr_Format(PyExc_MemoryError, "Failed to allocate deque");
         return NULL;
     }
 
     deque->head = NULL;
     deque->tail = NULL;
     return deque;
 }
@@ -43,15 +43,15 @@
 }
 
 void
 Deque_push_front(Deque *deque, Py_ssize_t value)
 {
     DequeNode *curr = malloc(sizeof(*curr));
     if (curr == NULL) {
-        fprintf(stderr, "Failed to allocate curr node\n");
+        PyErr_Format(PyExc_MemoryError, "Failed to allocate curr node");
         return;
     }
 
     curr->prev = NULL;
     curr->value = value;
     DequeNode *head = deque->head;
     if (head == NULL) {
@@ -77,15 +77,15 @@
 }
 
 void
 Deque_push_back(Deque *deque, Py_ssize_t value)
 {
     DequeNode *curr = malloc(sizeof(*curr));
     if (curr == NULL) {
-        fprintf(stderr, "Failed to allocate curr node\n");
+        PyErr_Format(PyExc_MemoryError, "Failed to allocate curr node");
         return;
     }
 
     curr->next = NULL;
     curr->value = value;
     DequeNode *tail = deque->tail;
     if (tail == NULL) {
```

### Comparing `grapes-graph-0.0.3/src/grapes/cgraph/deque.h` & `grapes-graph-0.0.4/src/grapes/cgraph/deque.h`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.3/src/grapes/cgraph/heap.c` & `grapes-graph-0.0.4/src/grapes/cgraph/heap.c`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 } MinHeap;
 
 MinHeap *
 MinHeap_alloc(Py_ssize_t max_size)
 {
     MinHeap *heap = malloc(sizeof(*heap));
     if (heap == NULL) {
-        fprintf(stderr, "Failed to allocate heap\n");
+        PyErr_Format(PyExc_MemoryError, "Failed to allocate heap");
         return NULL;
     }
 
     heap->size = 0;
     heap->max_size = max_size;
     heap->array = malloc(sizeof(*heap->array) * max_size);
     if (heap->array == NULL) {
-        fprintf(stderr, "Failed to allocate heap array\n");
+        PyErr_Format(PyExc_MemoryError, "Failed to allocate heap array");
+        free(heap);
         return NULL;
     }
 
     return heap;
 }
 
 void
@@ -48,15 +49,16 @@
     return;
 }
 
 void
 MinHeap_insert(MinHeap *heap, Py_ssize_t key, Py_ssize_t priority)
 {
     if (heap->size >= heap->max_size) {
-        fprintf(stderr, "Cannot insert key %ld. Heap is already full!\n", key);
+        PyErr_Format(PyExc_MemoryError,
+                     "Cannot insert key %ld. Heap is already full!", key);
         return;
     }
 
     Py_ssize_t i = heap->size++;
     heap->array[i].priority = priority;
     heap->array[i].key = key;
 
@@ -131,8 +133,8 @@
 MinHeap_print(MinHeap *heap)
 {
     printf("heap size=%ld values=", heap->size);
     for (Py_ssize_t i = 0; i < heap->size; ++i) {
         printf("%ld, ", heap->array[i].key);
     }
     printf("\n");
-}
+}
```

### Comparing `grapes-graph-0.0.3/src/grapes/cgraph/heap.h` & `grapes-graph-0.0.4/src/grapes/cgraph/heap.h`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.3/src/grapes_graph.egg-info/PKG-INFO` & `grapes-graph-0.0.4/src/grapes_graph.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grapes-graph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python graph library written in C
 Author-email: Eric Wang <ericwangyy@ucla.edu>
 License: MIT License
 Keywords: graph
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -19,8 +19,10 @@
 # Grapes
 Python graph library written in C
 
 ## Documentation
 Documentation found here: https://nouturnsign.github.io/grapes-doc/
 
 ## TODO
+*   ensure all values are freed even if exception occurs
+*   prevent XSS with svg
 *   more algos!
```


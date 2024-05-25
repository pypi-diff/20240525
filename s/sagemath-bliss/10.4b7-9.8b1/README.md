# Comparing `tmp/sagemath_bliss-10.4b7.tar.gz` & `tmp/sagemath-bliss-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_bliss-10.4b7.tar", last modified: Sat May 25 10:17:02 2024, max compression
+gzip compressed data, was "sagemath-bliss-9.8b1.tar", last modified: Mon Nov 21 07:31:28 2022, max compression
```

## Comparing `sagemath_bliss-10.4b7.tar` & `sagemath-bliss-9.8b1.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:02.605115 sagemath_bliss-10.4b7/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-25 10:17:02.601115 sagemath_bliss-10.4b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-25 10:11:48.000000 sagemath_bliss-10.4b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:02.601115 sagemath_bliss-10.4b7/sage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/sage/all__sagemath_bliss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:02.601115 sagemath_bliss-10.4b7/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/sage/graphs/all__sagemath_bliss.py
--rw-r--r--   0 runner    (1001) docker     (127)    32471 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/sage/graphs/bliss.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:02.601115 sagemath_bliss-10.4b7/sage/graphs/bliss_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/sage/graphs/bliss_cpp/bliss_find_automorphisms.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:17:02.601115 sagemath_bliss-10.4b7/sagemath_bliss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-25 10:17:01.000000 sagemath_bliss-10.4b7/sagemath_bliss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-25 10:17:02.000000 sagemath_bliss-10.4b7/sagemath_bliss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:17:01.000000 sagemath_bliss-10.4b7/sagemath_bliss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 10:17:01.000000 sagemath_bliss-10.4b7/sagemath_bliss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 10:17:01.000000 sagemath_bliss-10.4b7/sagemath_bliss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:17:02.605115 sagemath_bliss-10.4b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-25 10:11:38.000000 sagemath_bliss-10.4b7/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.289780 sagemath-bliss-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2370 2022-11-21 07:31:28.289916 sagemath-bliss-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1296 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-bliss-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.285772 sagemath-bliss-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.287619 sagemath-bliss-9.8b1/sage/graphs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    34899 2022-11-16 06:02:58.000000 sagemath-bliss-9.8b1/sage/graphs/bliss.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:28.289510 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2370 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      267 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:28.000000 sagemath-bliss-9.8b1/sagemath_bliss.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1093 2022-11-21 07:31:28.290521 sagemath-bliss-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2057 2022-11-20 23:45:29.000000 sagemath-bliss-9.8b1/setup.py
```

### Comparing `sagemath_bliss-10.4b7/PKG-INFO` & `sagemath-bliss-9.8b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-bliss
-Version: 10.4b7
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: cysignals>=1.10.2
-Provides-Extra: test
-Requires-Dist: sagemath-repl~=10.4b7; extra == "test"
 
 ==============================================================================
  Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
 ==============================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_bliss-10.4b7/README.rst` & `sagemath-bliss-9.8b1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_bliss-10.4b7/sage/graphs/bliss.pyx` & `sagemath-bliss-9.8b1/sage/graphs/bliss.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # distutils: language = c++
-# distutils: extra_compile_args = -std=c++11
 # distutils: libraries = bliss
 # sage_setup: distribution = sagemath-bliss
 
 r"""
 Interface with bliss: graph (iso/auto)morphism
 
 Implemented functions:
@@ -44,46 +43,46 @@
 
     cdef cppclass AbstractGraph:
         pass
 
     cdef cppclass Graph(AbstractGraph):
         Graph(const unsigned int)
         void add_edge(const unsigned int, const unsigned int)
+        void find_automorphisms(Stats&, void (*)(void*, unsigned int,
+                                                 const unsigned int*), void*)
         void change_color(const unsigned int, const unsigned int)
-        const unsigned int* canonical_form(Stats&)
-
-cdef extern from "bliss/digraph.hh" namespace "bliss":
+        const unsigned int* canonical_form(Stats&, void (*)(void*, unsigned int,
+                                                            const unsigned int*), void*)
 
     cdef cppclass Digraph(AbstractGraph):
         Digraph(const unsigned int)
         void add_edge(const unsigned int, const unsigned int)
+        void find_automorphisms(Stats&, void (*)(void*, unsigned int,
+                                                 const unsigned int*), void*)
         void change_color(const unsigned int, const unsigned int)
-        const unsigned int* canonical_form(Stats&)
+        const unsigned int* canonical_form(Stats&, void (*)(void*, unsigned int,
+                                                            const unsigned int*), void*)
         unsigned int get_hash()
 
-cdef extern from "bliss_cpp/bliss_find_automorphisms.h":
-
-    void bliss_find_automorphisms(Graph*, void (*)(void*, unsigned int, const unsigned int*), void*, Stats&)
-    void bliss_find_automorphisms(Digraph*, void (*)(void*, unsigned int, const unsigned int*), void*, Stats&)
 
-cdef int encoding_numbits(int n) noexcept:
+cdef int encoding_numbits(int n):
     r"""
-    Return the number of bits needed to encode the `n` numbers from `1` to
-    `n`. In other words, the last bit set in `n`.
+    Return the number of bits needed to encode the ``n`` numbers from ``1`` to ``n``. In
+    other words, the last bit set in ``n``.
     """
     if n <= 0:
         return 0
     cdef int i = 0
     while n:
         n >>= 1
         i += 1
     return i
 
 
-cdef void add_gen(void *user_param, unsigned int n, const unsigned int *aut) noexcept:
+cdef void add_gen(void *user_param, unsigned int n, const unsigned int *aut):
     r"""
     Function called each time a new generator of the automorphism group is
     found.
 
     This function is used to append the new generators to a Python list. Its
     main job is to translate a permutation into disjoint cycles.
 
@@ -98,14 +97,15 @@
     - ``aut`` -- ``int *``; an automorphism of the graph
     """
     cdef int N
     cdef int tmp = 0
     cdef int cur = 0
     cdef list perm = []
     cdef bint* done = <bint*> check_calloc(n, sizeof(bint))
+    cdef int i
 
     gens, int_to_vertex, N = <object>user_param
 
     while cur < N:
         if not done[cur]:
             tmp = cur
             cycle = [int_to_vertex[cur]]
@@ -120,19 +120,23 @@
 
         cur += 1
 
     gens.append(perm)
 
     sig_free(done)
 
+
+cdef void empty_hook(void *user_param, unsigned int n, const unsigned int *aut):
+    return
+
 #####################################################
 # constructing bliss graphs from edge lists
 #####################################################
 
-cdef Graph *bliss_graph_from_labelled_edges(int Vnr, int Lnr, Vout, Vin, labels, partition) noexcept:
+cdef Graph *bliss_graph_from_labelled_edges(int Vnr, int Lnr, Vout, Vin, labels, partition):
     r"""
     Return a bliss graph from the input data
 
     For edge labelled graphs, the bliss graph is constructed using `Vnr *
     \log(Lnr)` many vertices as described in Sec. 14 of the `nauty reference
     manual <http://pallini.di.uniroma1.it/Guide.html>`_.
 
@@ -215,15 +219,15 @@
     else:
         for j in range(logLnr):
             for v in range(Vnr):
                 g.change_color(j * Vnr + v, j)
 
     return g
 
-cdef Digraph *bliss_digraph_from_labelled_edges(int Vnr, int Lnr, Vout, Vin, labels, partition) noexcept:
+cdef Digraph *bliss_digraph_from_labelled_edges(int Vnr, int Lnr, Vout, Vin, labels, partition):
     r"""
     Return a bliss digraph from the input data
 
     For edge labelled graphs, the bliss graph is constructed using `Vnr *
     \log(Lnr)` many vertices as described in Sec 14 in the `nauty reference
     manual <http://pallini.di.uniroma1.it/Guide.html>`_.
 
@@ -296,15 +300,15 @@
     return g
 
 #####################################################
 # canonical form from graph or edge list
 #####################################################
 
 cdef canonical_form_from_edge_list(int Vnr, list Vout, list Vin, int Lnr=1, list labels=[],
-                                   list partition=None, bint directed=False, bint certificate=False) noexcept:
+                                   list partition=None, bint directed=False, bint certificate=False):
     r"""
     Return an unsorted list of labelled edges of a canonical form.
 
     INPUT:
 
     - ``Vnr`` -- ``int``; number of vertices, such that the vertices are `0,
       \ldots, Vnr-1`
@@ -338,18 +342,18 @@
     cdef dict relabel
 
     cdef list new_edges = []
     cdef long e, f
 
     if directed:
         d = bliss_digraph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        aut = d.canonical_form(s)
+        aut = d.canonical_form(s, empty_hook, NULL)
     else:
         g = bliss_graph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        aut = g.canonical_form(s)
+        aut = g.canonical_form(s, empty_hook, NULL)
 
     for i in range(len(Vout)):
         x = Vout[i]
         y = Vin[i]
         e = aut[x]
         f = aut[y]
         if Lnr == 1:
@@ -370,18 +374,19 @@
     if directed:
         del d
     else:
         del g
 
     if certificate:
         return new_edges, relabel
-    return new_edges
+    else:
+        return new_edges
 
 
-cpdef canonical_form(G, partition=None, return_graph=False, use_edge_labels=True, certificate=False) noexcept:
+cpdef canonical_form(G, partition=None, return_graph=False, use_edge_labels=True, certificate=False):
     r"""
     Return a canonical label for the given (di)graph.
 
     A canonical label ``canonical_form(G)`` of ``G`` is a (di)graph defined on
     `\{0,...,n-1\}` such that ``G`` is isomorphic to ``H`` if and only if
     ``canonical_form(G)`` is equal to ``canonical_form(H)``.
 
@@ -392,18 +397,17 @@
     - ``partition`` -- ``list`` (default: ``None``); a partition of the vertices
       of ``G`` into color classes
 
     - ``return_graph`` -- boolean (default: ``False``); whether to return the
       canonical graph of ``G`` or its set of edges
 
     - ``use_edge_labels`` -- boolean (default: ``True``); whether to consider
-      edge labels. The edge labels are assumed to be hashable and
-      sortable. If this is not the case (ie a :class:`TypeError` is
-      raised), the algorithm will consider the string representations
-      of the labels instead of the labels.
+      edge labels. The edge labels are assumed to be hashable and sortable. If
+      this is not the case (ie a ``TypeError`` is raised), the algorithm will
+      consider the string representations of the labels instead of the labels.
 
     - ``certificate`` -- boolean (default: ``False``); when set to ``True``,
       returns the labeling of G into a canonical graph
 
     TESTS::
 
         sage: from sage.graphs.bliss import canonical_form                  # optional - bliss
@@ -432,37 +436,36 @@
 
         sage: canonical_form(Graph(15), return_graph=True)                  # optional - bliss
         Graph on 15 vertices
         sage: g = digraphs.RandomTournament(40)                             # optional - bliss
         sage: g.is_isomorphic(canonical_form(g, return_graph=True))         # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: g1 = graphs.RandomGNP(100, .4)
-        sage: r = Permutations(range(100)).random_element()
-        sage: g2 = Graph([(r[u],r[v]) for u,v in g1.edges(sort=True, labels=False)])
-        sage: g1 = canonical_form(g1, return_graph=True)
-        sage: g2 = canonical_form(g2, return_graph=True)
-        sage: g2 == g2
+        sage: g1 = graphs.RandomGNP(100, .4)                                # optional - bliss
+        sage: r = Permutations(range(100)).random_element()                 # optional - bliss
+        sage: g2 = Graph([(r[u],r[v]) for u,v in g1.edges(sort=True, labels=False)])   # optional - bliss
+        sage: g1 = canonical_form(g1, return_graph=True)                    # optional - bliss
+        sage: g2 = canonical_form(g2, return_graph=True)                    # optional - bliss
+        sage: g2 == g2                                                      # optional - bliss
         True
 
         sage: g = Graph({1: [2]})
         sage: g_ = canonical_form(g, return_graph=True, certificate=True)   # optional - bliss
         sage: 0 in g_[0]                                                    # optional - bliss
         True
 
-    Check that parameter ``use_edge_labels`` can be used (:issue:`27571`)::
+    Check that parameter ``use_edge_labels`` can be used (:trac:`27571`)::
 
         sage: g = Graph({1: {2: 'a'}})
         sage: canonical_form(g, use_edge_labels=True)                       # optional - bliss
         [(1, 0, 'a')]
         sage: canonical_form(g, use_edge_labels=False)                      # optional - bliss
         [(1, 0, None)]
 
-    Check that :issue:`28531` is fixed::
+    Check that :trac:`28531` is fixed::
 
         sage: from itertools import product, permutations
         sage: edges_list = [[(0,1), (1,2)],
         ....:               [(0,1),(1,2),(2,3)],
         ....:               [(0,1),(1,2),(2,3),(3,0)]]
         sage: for edges in edges_list:                                      # optional - bliss
         ....:     for labels in product([0,1], repeat=len(edges)):
@@ -472,23 +475,22 @@
         ....:             h = Graph([(p[u], p[v], lab) for u,v,lab in g.edges(sort=True)])
         ....:             hcan = canonical_form(h, use_edge_labels=True)
         ....:             if gcan != hcan: print(edges, labels, p)
 
     Check that it works with non hashable non sortable edge labels (relying
     on string representations of the labels)::
 
-        sage: # needs sage.modules
         sage: g1 = Graph([(0, 1, matrix(ZZ, 2)), (0, 2, RDF.pi()), (1, 2, 'a')])
         sage: g2 = Graph([(1, 2, matrix(ZZ, 2)), (2, 0, RDF.pi()), (0, 1, 'a')])
-        sage: g1can = canonical_form(g1, use_edge_labels=True)              # optional - bliss
-        sage: g2can = canonical_form(g2, use_edge_labels=True)              # optional - bliss
-        sage: g1can == g2can                                                # optional - bliss
+        sage: g1can = canonical_form(g1, use_edge_labels=True)               # optional - bliss
+        sage: g2can = canonical_form(g2, use_edge_labels=True)               # optional - bliss
+        sage: g1can == g2can                                                 # optional - bliss
         True
 
-    Check that :issue:`32395` is fixed::
+    Check that :trac:`32395` is fixed::
 
         sage: g = Graph([[0, 2]])  # 1 is not a vertex!
         sage: g.canonical_label(partition=[[0], [1], [2]], algorithm="bliss")  # optional - bliss
         Traceback (most recent call last):
         ...
         ValueError: vertex 1 of the partition is not a vertex of the graph
         sage: g.canonical_label(partition=[[0], [0, 2]], algorithm="bliss")  # optional - bliss
@@ -507,14 +509,15 @@
     # We need this to convert the numbers from <unsigned int> to <long>.
     # This assertion should be true simply for memory reasons.
     cdef unsigned long Vnr = G.order()
     assert Vnr <= <unsigned long> LONG_MAX
 
     cdef bint directed = G.is_directed()
 
+    cdef int labInd
     cdef list Vout = []
     cdef list Vin = []
     cdef list labels = []
 
     cdef list int2vert
     cdef dict vert2int
     cdef dict lab_to_index
@@ -576,15 +579,15 @@
     new_edges, relabel = canonical_form_from_edge_list(Vnr, Vout, Vin, Lnr, labels, partition, directed, certificate=True)
 
     new_edges = [(x, y, edge_labels[lab]) for x, y, lab in new_edges]
     relabel = {int2vert[i]: j for i, j in relabel.items()}
 
     if return_graph:
         if directed:
-            from sage.graphs.digraph import DiGraph
+            from sage.graphs.graph import DiGraph
             H = DiGraph(new_edges, loops=G.allows_loops(), multiedges=G.allows_multiple_edges())
         else:
             from sage.graphs.graph import Graph
             H = Graph(new_edges, loops=G.allows_loops(), multiedges=G.allows_multiple_edges())
 
         H.add_vertices(range(G.order()))
         return (H, relabel) if certificate else H
@@ -594,15 +597,15 @@
 
 
 #####################################################
 # automorphism group from graphs
 #####################################################
 
 cdef automorphism_group_gens_from_edge_list(int Vnr, Vout, Vin, int Lnr=1, labels=[],
-                                            int2vert=[], partition=None, bint directed=False) noexcept:
+                                            int2vert=[], partition=None, bint directed=False):
     r"""
     Return an unsorted list of labelled edges of a canonical form.
 
     INPUT:
 
     - ``Vnr`` -- ``int``; number of vertices, such that the vertices are `0,
       \ldots, Vnr-1`
@@ -636,166 +639,158 @@
         int2vert = list(range(Vnr))
 
     cdef list gens = []
     cdef tuple data = (gens, int2vert, Vnr)
 
     if directed:
         d = bliss_digraph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        bliss_find_automorphisms(d, add_gen, <void*>data, s)
+        d.find_automorphisms(s, add_gen, <void*>data)
         del d
     else:
         g = bliss_graph_from_labelled_edges(Vnr, Lnr, Vout, Vin, labels, partition)
-        bliss_find_automorphisms(g, add_gen, <void*>data, s)
+        g.find_automorphisms(s, add_gen, <void*>data)
         del g
 
     return [[cyc for cyc in gen if cyc[0] is not None] for gen in gens]
 
-cpdef automorphism_group(G, partition=None, use_edge_labels=True) noexcept:
+cpdef automorphism_group(G, partition=None, use_edge_labels=True):
     """
     Return the automorphism group of the given (di)graph.
 
     Compute the automorphism group of ``G`` subject to the vertex coloring
     ``partition``, if given.  The graph ``G`` can be a directed or undirected
     graph with or without edge labellings.
 
     Observe the neither the vertex colorings nor the edge colorings are
     interchangeable.
 
     INPUT:
 
     - ``G`` -- a Sage graph
 
-    - ``partition`` -- ``list`` (default: ``None``); a partition of the vertices
+    - ``partition`` -- ``list``(default: ``None``); a partition of the vertices
       of ``G`` into color classes. Defaults to ``None``, which is equivalent to
       a partition of size 1.
 
-    - ``use_edge_labels`` -- boolean (default: ``True``); whether to consider
-      edge labels
+    - ``use_edge_labels`` -- boolean (default: ``True``); whether to consider edge
+      labels
 
     EXAMPLES::
 
         sage: from sage.graphs.bliss import automorphism_group                  # optional - bliss
 
     Computing the automorphism group of a graph or digraph::
 
-        sage: # optional - bliss
-        sage: G = graphs.CompleteMultipartiteGraph([1, 1, 1, 2])
-        sage: automorphism_group(G).cardinality()
+        sage: G = graphs.CompleteMultipartiteGraph([1, 1, 1, 2])                # optional - bliss
+        sage: automorphism_group(G).cardinality()                               # optional - bliss
         12
-        sage: D = DiGraph(G.edges(sort=True))
-        sage: automorphism_group(D).cardinality()
+        sage: D = DiGraph(G.edges(sort=True))                                   # optional - bliss
+        sage: automorphism_group(D).cardinality()                               # optional - bliss
         2
 
-    Observe that the order 12 is given by permuting the first three vertices, or
-    the last two in the case of a graph, while only the latter two are possible
-    in the case of a directed graph.
+    Observe that the order 12 is given by permuting the first three vertices, or the last two
+    in the case of a graph, while only the latter two are possible in the case of a directed
+    graph.
 
     Partitioning the vertices into classes::
 
-        sage: # optional - bliss
-        sage: G = graphs.CompleteMultipartiteGraph([3, 2])
-        sage: automorphism_group(G).cardinality()
+        sage: G = graphs.CompleteMultipartiteGraph([3, 2])                      # optional - bliss
+        sage: automorphism_group(G).cardinality()                               # optional - bliss
         12
-        sage: automorphism_group(G,partition=[[0],[1],[2],[3,4]]).cardinality()
+        sage: automorphism_group(G,partition=[[0],[1],[2],[3,4]]).cardinality() # optional - bliss
         2
-        sage: automorphism_group(G,partition=[[0],[1,2],[3,4]]).cardinality()
+        sage: automorphism_group(G,partition=[[0],[1,2],[3,4]]).cardinality()   # optional - bliss
         4
-        sage: automorphism_group(G,partition=[[1,2],[0,3],[4]]).cardinality()
+
+        sage: automorphism_group(G,partition=[[1,2],[0,3],[4]]).cardinality()   # optional - bliss
         2
 
     Partitioning the edges into classes::
 
-        sage: # optional - bliss
-        sage: G = Graph(graphs.CompleteMultipartiteGraph([8, 2]), sparse=True)
-        sage: for i,j in G.edges(labels=False, sort=False):
-        ....:     if 0 <= i < 3:
-        ....:         G.set_edge_label(i, j, "A")
-        ....:     if 3 <= i < 6:
-        ....:         G.set_edge_label(i, j, "B")
-        ....:     if 6 <= i < 8:
-        ....:         G.set_edge_label(i, j, "C")
-        sage: factor(automorphism_group(G).cardinality())
+        sage: G = Graph(graphs.CompleteMultipartiteGraph([8, 2]), sparse=True)  # optional - bliss
+        sage: for i,j in G.edges(labels=False, sort=False):                     # optional - bliss
+        ....:     if 0 <= i < 3:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "A")                               # optional - bliss
+        ....:     if 3 <= i < 6:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "B")                               # optional - bliss
+        ....:     if 6 <= i < 8:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "C")                               # optional - bliss
+
+        sage: factor(automorphism_group(G).cardinality())                       # optional - bliss
         2^4 * 3^2
-        sage: automorphism_group(G,[[0],[1],[2,3],[4,5],[6,7],[8],[9]]).cardinality()
+        sage: automorphism_group(G,[[0],[1],[2,3],[4,5],[6,7],[8],[9]]).cardinality()   # optional - bliss
         4
 
     TESTS::
 
         sage: from sage.graphs.bliss import automorphism_group                  # optional - bliss
         sage: G = graphs.PetersenGraph()                                        # optional - bliss
         sage: automorphism_group(G).is_isomorphic(G.automorphism_group())       # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: G = graphs.HeawoodGraph()
-        sage: p = G.bipartite_sets()
-        sage: A = G.automorphism_group(partition=[list(p[0]), list(p[1])])
-        sage: automorphism_group(G, partition=p).is_isomorphic(A)
+        sage: G = graphs.HeawoodGraph()                                         # optional - bliss
+        sage: p = G.bipartite_sets()                                            # optional - bliss
+        sage: A = G.automorphism_group(partition=[list(p[0]), list(p[1])])      # optional - bliss
+        sage: automorphism_group(G, partition=p).is_isomorphic(A)               # optional - bliss
         True
 
-        sage: G = graphs.CompleteMultipartiteGraph([5, 7, 11])
+        sage: G = graphs.CompleteMultipartiteGraph([5,7,11])
         sage: B = automorphism_group(G)                                         # optional - bliss
-        sage: B.cardinality() == prod(factorial(n) for n in [5, 7, 11])         # optional - bliss
+        sage: B.cardinality() == prod(factorial(n) for n in [5,7,11])           # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: G = Graph(graphs.CompleteMultipartiteGraph([8,8,8,5]),sparse=True)
-        sage: for i,j in G.edges(labels=False, sort=False):
-        ....:     if 0 <= i < 3:
-        ....:         G.set_edge_label(i, j, "A")
-        ....:     if 3 <= i < 6:
-        ....:         G.set_edge_label(i, j, "B")
-        ....:     if 6 <= i < 8:
-        ....:         G.set_edge_label(i, j, "C")
-        sage: card = automorphism_group(G).cardinality()
-        sage: card == prod(factorial(n) for n in [3, 3, 2, 8, 8, 5, 2])
-        True
-        sage: card = automorphism_group(G, use_edge_labels=False).cardinality()
-        sage: card == prod(factorial(n) for n in [8, 8, 8, 5, 3])
-        True
-        sage: card = automorphism_group(G, [[0 .. 7], [8 .. 11] ,[12 .. 28]]).cardinality()
-        sage: card == prod(factorial(n) for n in [3, 3, 2, 4, 4, 8, 5])
-        True
-
-        sage: # optional - bliss
-        sage: G = Graph()
-        sage: G.add_edges((i,j,"A") for i in range(0, 2) for j in range(14,20))
-        sage: G.add_edges((i,j,"B") for i in range(2, 5) for j in range(14,20))
-        sage: G.add_edges((i,j,"C") for i in range(5, 9) for j in range(14,20))
-        sage: G.add_edges((i,j,"D") for i in range(9,14) for j in range(14,20))
-        sage: A = automorphism_group(G)
-        sage: print(A.gens())               # random
-        ((12,13), (11,12), (10,11), (9,10), (7,8), (6,7), (5,6), (3,4),
-         (2,3), (1,0), (18,19), (17,18), (16,17), (15,16), (14,15))
-        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])
+        sage: G = Graph(graphs.CompleteMultipartiteGraph([8,8,8,5]),sparse=True)# optional - bliss
+        sage: for i,j in G.edges(labels=False, sort=False):                     # optional - bliss
+        ....:     if 0 <= i < 3:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "A")                               # optional - bliss
+        ....:     if 3 <= i < 6:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "B")                               # optional - bliss
+        ....:     if 6 <= i < 8:                                                # optional - bliss
+        ....:         G.set_edge_label(i, j, "C")                               # optional - bliss
+        sage: automorphism_group(G).cardinality() == prod( factorial(n) for n in [3,3,2,8,8,5,2] )  # optional - bliss
+        True
+        sage: automorphism_group(G, use_edge_labels=False).cardinality() == prod( factorial(n) for n in [8,8,8,5,3] )  # optional - bliss
+        True
+        sage: automorphism_group(G,[[0 .. 7],[8 .. 11],[12 .. 28]]).cardinality() == prod( factorial(n) for n in [3,3,2,4,4,8,5] )  # optional - bliss
+        True
+
+        sage: G = Graph()                                                       # optional - bliss
+        sage: G.add_edges((i,j,"A") for i in range(0, 2) for j in range(14,20)) # optional - bliss
+        sage: G.add_edges((i,j,"B") for i in range(2, 5) for j in range(14,20)) # optional - bliss
+        sage: G.add_edges((i,j,"C") for i in range(5, 9) for j in range(14,20)) # optional - bliss
+        sage: G.add_edges((i,j,"D") for i in range(9,14) for j in range(14,20)) # optional - bliss
+        sage: A = automorphism_group(G)                                         # optional - bliss
+        sage: print(A.gens())                                                   # random, optional - bliss
+        [(9,13), (18,19), (17,18), (16,17), (15,16), (14,15), (12,9), (11,12),
+         (10,11), (7,8), (6,7), (5,6), (3,4), (2,3), (0,1)]
+        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])        # optional - bliss
         True
 
-        sage: # optional - bliss
-        sage: G = Graph()
         sage: alpha = "abcdefghijklmnopqrstuvwxyz"
-        sage: G.add_edges((alpha[i],alpha[j],"A") for i in range(0, 2) for j in range(14,20))
-        sage: G.add_edges((alpha[i],alpha[j],"B") for i in range(2, 5) for j in range(14,20))
-        sage: G.add_edges((alpha[i],alpha[j],"C") for i in range(5, 9) for j in range(14,20))
-        sage: G.add_edges((alpha[i],alpha[j],"D") for i in range(9,14) for j in range(14,20))
-        sage: A = automorphism_group(G)
-        sage: print(A.gens())
-        (('m','n'), ('l','m'), ('k','l'), ('j','k'), ('h','i'),
-         ('g','h'), ('f','g'), ('d','e'), ('c','d'), ('s','t'),
-         ('r','s'), ('q','r'), ('p','q'), ('o','p'), ('a','b'))
-        sage: A.cardinality() == prod(factorial(n) for n in [2, 3, 4, 5, 6])
-        True
-
-        sage: # optional - bliss
-        sage: gg = graphs.CompleteGraph(5)
-        sage: gg.allow_loops(True)
-        sage: gg.add_edge(0, 0)
-        sage: gg.add_edge(1, 1)
-        sage: automorphism_group(gg).cardinality()
+
+        sage: G = Graph()                                                       # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"A") for i in range(0, 2) for j in range(14,20))   # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"B") for i in range(2, 5) for j in range(14,20))   # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"C") for i in range(5, 9) for j in range(14,20))   # optional - bliss
+        sage: G.add_edges((alpha[i],alpha[j],"D") for i in range(9,14) for j in range(14,20))   # optional - bliss
+        sage: A = automorphism_group(G)                                         # optional - bliss
+        sage: print(A.gens())                                                   # random, optional - bliss
+        [('r','t'), ('s','r'), ('p','s'), ('q','p'), ('o','q'), ('l','n'),
+         ('m','l'), ('j','m'), ('k','j'), ('i','h'), ('f','i'), ('g','f'),
+         ('e','d'), ('c','e'), ('a','b')]
+        sage: A.cardinality() == prod(factorial(n) for n in [2,3,4,5,6])        # optional - bliss
+        True
+
+        sage: gg = graphs.CompleteGraph(5)                                      # optional - bliss
+        sage: gg.allow_loops(True)                                              # optional - bliss
+        sage: gg.add_edge(0,0)                                                  # optional - bliss
+        sage: gg.add_edge(1,1)                                                  # optional - bliss
+        sage: automorphism_group(gg).cardinality()                              # optional - bliss
         12
-        sage: automorphism_group(gg, [[0], [1, 2, 3, 4]]).cardinality()
+        sage: automorphism_group(gg,[[0],[1,2,3,4]]).cardinality()              # optional - bliss
         6
     """
     # We need this to convert the numbers from <unsigned int> to
     # <long>. This assertion should be true simply for memory reasons.
     cdef unsigned long Vnr = G.order()
     assert Vnr <= <unsigned long>LONG_MAX
 
@@ -843,15 +838,15 @@
     return PermutationGroup(gens, domain=int2vert[:G.order()])
 
 
 #####################################################
 # old direct interactions graphs <-> bliss graphs
 #####################################################
 
-cdef Graph *bliss_graph(G, partition, vert2int, int2vert) noexcept:
+cdef Graph *bliss_graph(G, partition, vert2int, int2vert):
     r"""
     Return a bliss copy of a graph G
 
     INPUT:
 
     - ``G`` -- a Sage Graph
 
@@ -877,15 +872,15 @@
     if partition:
         for i in range(1, len(partition)):
             for v in partition[i]:
                 g.change_color(vert2int[v], i)
     return g
 
 
-cdef Digraph *bliss_digraph(G, partition, vert2int, int2vert) noexcept:
+cdef Digraph *bliss_digraph(G, partition, vert2int, int2vert):
     r"""
     Return a bliss copy of a digraph G
 
     INPUT:
 
     - ``G`` -- a Sage DiGraph
```

### Comparing `sagemath_bliss-10.4b7/sagemath_bliss.egg-info/PKG-INFO` & `sagemath-bliss-9.8b1/sagemath_bliss.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-bliss
-Version: 10.4b7
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: cysignals>=1.10.2
-Provides-Extra: test
-Requires-Dist: sagemath-repl~=10.4b7; extra == "test"
 
 ==============================================================================
  Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with bliss
 ==============================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_bliss-10.4b7/setup.py` & `sagemath-bliss-9.8b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-bliss']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-bliss'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-bliss'])
 
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```


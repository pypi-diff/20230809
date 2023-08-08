# Comparing `tmp/gssnng-0.2.6.2.tar.gz` & `tmp/gssnng-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gssnng-0.2.6.2.tar", last modified: Tue Mar 21 00:44:52 2023, max compression
+gzip compressed data, was "gssnng-0.4.2.tar", last modified: Tue Aug  8 22:07:42 2023, max compression
```

## Comparing `gssnng-0.2.6.2.tar` & `gssnng-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 daveg     (1000) daveg     (1000)        0 2023-03-21 00:44:52.091032 gssnng-0.2.6.2/
--rw-r--r--   0 daveg     (1000) daveg     (1000)      192 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/MANIFEST.in
--rw-r--r--   0 daveg     (1000) daveg     (1000)     8156 2023-03-21 00:44:52.091032 gssnng-0.2.6.2/PKG-INFO
--rw-r--r--   0 daveg     (1000) daveg     (1000)     7864 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/README.md
-drwxr-xr-x   0 daveg     (1000) daveg     (1000)        0 2023-03-21 00:44:52.091032 gssnng-0.2.6.2/gssnng/
--rw-r--r--   0 daveg     (1000) daveg     (1000)      416 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/gssnng/__init__.py
--rw-r--r--   0 daveg     (1000) daveg     (1000)     4388 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/gssnng/gene_sets.py
--rw-r--r--   0 daveg     (1000) daveg     (1000)    11145 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/gssnng/score_cells.py
--rw-r--r--   0 daveg     (1000) daveg     (1000)     9920 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/gssnng/score_funs.py
--rw-r--r--   0 daveg     (1000) daveg     (1000)     4441 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/gssnng/smoothing.py
--rw-r--r--   0 daveg     (1000) daveg     (1000)     7342 2023-03-20 23:32:22.000000 gssnng-0.2.6.2/gssnng/util.py
-drwxr-xr-x   0 daveg     (1000) daveg     (1000)        0 2023-03-21 00:44:52.091032 gssnng-0.2.6.2/gssnng.egg-info/
--rw-r--r--   0 daveg     (1000) daveg     (1000)     8156 2023-03-21 00:44:52.000000 gssnng-0.2.6.2/gssnng.egg-info/PKG-INFO
--rw-r--r--   0 daveg     (1000) daveg     (1000)      335 2023-03-21 00:44:52.000000 gssnng-0.2.6.2/gssnng.egg-info/SOURCES.txt
--rw-r--r--   0 daveg     (1000) daveg     (1000)        1 2023-03-21 00:44:52.000000 gssnng-0.2.6.2/gssnng.egg-info/dependency_links.txt
--rw-r--r--   0 daveg     (1000) daveg     (1000)        1 2023-03-20 23:33:53.000000 gssnng-0.2.6.2/gssnng.egg-info/not-zip-safe
--rw-r--r--   0 daveg     (1000) daveg     (1000)       62 2023-03-21 00:44:52.000000 gssnng-0.2.6.2/gssnng.egg-info/requires.txt
--rw-r--r--   0 daveg     (1000) daveg     (1000)        7 2023-03-21 00:44:52.000000 gssnng-0.2.6.2/gssnng.egg-info/top_level.txt
--rw-r--r--   0 daveg     (1000) daveg     (1000)      159 2023-03-21 00:44:52.091032 gssnng-0.2.6.2/setup.cfg
--rw-r--r--   0 daveg     (1000) daveg     (1000)      563 2023-03-21 00:44:29.000000 gssnng-0.2.6.2/setup.py
+drwxr-xr-x   0 daveg     (1000) daveg     (1000)        0 2023-08-08 22:07:42.364653 gssnng-0.4.2/
+-rw-r--r--   0 daveg     (1000) daveg     (1000)      192 2023-08-08 21:22:01.000000 gssnng-0.4.2/MANIFEST.in
+-rw-r--r--   0 daveg     (1000) daveg     (1000)     8796 2023-08-08 22:07:42.364653 gssnng-0.4.2/PKG-INFO
+-rw-r--r--   0 daveg     (1000) daveg     (1000)     8501 2023-08-08 22:07:26.000000 gssnng-0.4.2/README.md
+drwxr-xr-x   0 daveg     (1000) daveg     (1000)        0 2023-08-08 22:07:42.364653 gssnng-0.4.2/gssnng/
+-rw-r--r--   0 daveg     (1000) daveg     (1000)      416 2023-08-08 21:22:01.000000 gssnng-0.4.2/gssnng/__init__.py
+-rw-r--r--   0 daveg     (1000) daveg     (1000)     6732 2023-08-08 21:22:01.000000 gssnng-0.4.2/gssnng/gene_sets.py
+-rw-r--r--   0 daveg     (1000) daveg     (1000)    14471 2023-08-08 21:22:01.000000 gssnng-0.4.2/gssnng/score_cells.py
+-rw-r--r--   0 daveg     (1000) daveg     (1000)    11721 2023-08-08 21:22:01.000000 gssnng-0.4.2/gssnng/score_funs.py
+-rw-r--r--   0 daveg     (1000) daveg     (1000)     4495 2023-08-08 21:22:01.000000 gssnng-0.4.2/gssnng/smoothing.py
+-rw-r--r--   0 daveg     (1000) daveg     (1000)     7412 2023-08-08 21:22:01.000000 gssnng-0.4.2/gssnng/util.py
+drwxr-xr-x   0 daveg     (1000) daveg     (1000)        0 2023-08-08 22:07:42.364653 gssnng-0.4.2/gssnng.egg-info/
+-rw-r--r--   0 daveg     (1000) daveg     (1000)     8796 2023-08-08 22:07:42.000000 gssnng-0.4.2/gssnng.egg-info/PKG-INFO
+-rw-r--r--   0 daveg     (1000) daveg     (1000)      335 2023-08-08 22:07:42.000000 gssnng-0.4.2/gssnng.egg-info/SOURCES.txt
+-rw-r--r--   0 daveg     (1000) daveg     (1000)        1 2023-08-08 22:07:42.000000 gssnng-0.4.2/gssnng.egg-info/dependency_links.txt
+-rw-r--r--   0 daveg     (1000) daveg     (1000)        1 2023-08-08 21:36:18.000000 gssnng-0.4.2/gssnng.egg-info/not-zip-safe
+-rw-r--r--   0 daveg     (1000) daveg     (1000)       62 2023-08-08 22:07:42.000000 gssnng-0.4.2/gssnng.egg-info/requires.txt
+-rw-r--r--   0 daveg     (1000) daveg     (1000)        7 2023-08-08 22:07:42.000000 gssnng-0.4.2/gssnng.egg-info/top_level.txt
+-rw-r--r--   0 daveg     (1000) daveg     (1000)      159 2023-08-08 22:07:42.364653 gssnng-0.4.2/setup.cfg
+-rw-r--r--   0 daveg     (1000) daveg     (1000)      566 2023-08-08 22:07:38.000000 gssnng-0.4.2/setup.py
```

### Comparing `gssnng-0.2.6.2/PKG-INFO` & `gssnng-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: gssnng
-Version: 0.2.6.2
+Version: 0.4.2
 Summary: Gene Set Scoring on the Nearest Neighbor Graph (gssnng)
-Home-page: http://github.com/gibbsdavidl/gssnng
+Home-page: http://github.com/IlyaLab/gssnng
 Author: David Gibbs,Michael Strasser
-Author-email: gibbsdavidl@gmail.com
+Author-email: david.gibbs@systemsbiology.org
 License: MIT
 Description-Content-Type: text/markdown
 
 # gssnng
 
-**Try it out!  ===>>>**  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Gibbsdavidl/gssnng/blob/main/notebooks/gssnng_quick_start.ipynb)
+**Try it out!  ===>>>**  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IlyaLab/gssnng/blob/main/notebooks/gssnng_quick_start.ipynb)
 
 **See the paper ===>>>** [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.29.518384v1)
 
 Gene Set Scoring on the Nearest Neighbor Graph (gssnng) for Single Cell RNA-seq (scRNA-seq).
 
 The problem:  The sparsity of scRNA-seq data creates a poor overlap with many gene sets, 
 which in turn makes gene set scoring difficult. 
@@ -25,61 +25,67 @@
 
 Nearest neighbor graphs (NNG) are constructed based on user defined groups (see the 'groupby' parameter below). 
 The defined groups can be processed in parallel, speeding up the calculations. For example, a NNG could be 
 constructed within each cluster or jointly by cluster *and* sample. Smoothing can be performed using either the 
 adjacency matrix (all 1s) or the weighted graph to give less weight to more distant cells.
 
 This package works with AnnData objects stored as h5ad files. Expression values are taken from adata.X.
-For creating groups, up to four categorical variables can be used, which are found in the adata.obs table.
+For creating groups, up to four categorical variables can be used, which are found in the adata.obs table. 
+Gene sets can be provided by using .gmt files or through the OmniPath API (see below).
 
 Scoring functions work with ranked or unranked data (**"your mileage may vary"**):
 
-Some method references (singscore, RBO) are below.
+Method references (singscore, RBO) are below. 
+
+Some methods have additional parameters, see below!
 
 ```
-    singscore:            Normalised mean (median centered) ranks (requires ranked data)
+    geneset_overlap: Number (or fraction) of genes, past an expression threshold, that overlap with each geneset.
+
+    singscore:       Normalised mean (median centered) ranks (requires ranked data)
     
-    ssgsea:               The well known single sample GSEA.
+    ssgsea:          The well known single sample GSEA.
         
     rank_biased_overlap:  RBO, Weighted average of agreement between sorted ranks and gene set.
 
-    robust_std:     Med(x-med / mad), median of robust standardized values (recommend unranked).
+    robust_std:      Med(x-med / mad), median of robust standardized values (recommend unranked).
+    
+    mean_z:          Mean( (x - mean)/stddv ), average z score. (recommend unranked).
     
-    mean_z:         Mean( (x - mean)/stddv ), average z score. (recommend unranked).
+    average_score:   Mean ranks or counts     
     
-    average_score:  Mean ranks or counts     
+    median_score:    Median of counts or ranks
     
-    median_score:   Median of counts or ranks
+    summed_up:       Sum up the ranks or counts.
     
-    summed_up:      Sum up the ranks or counts.
 ```
 
 ## Installation from PyPI
 ```
 pip3 install gssnng
 ```
 
 
 ## Installation from GitHub
 
 ```
 # also gets you the demo data and some gene sets.
-git clone https://github.com/Gibbsdavidl/gssnng
+git clone https://github.com/IlyaLab/gssnng
 
 pip install -e gssnng
 ```
 
 ## Example script
 
 Copy the script out from the cloned repo and run, check the paths if you get an error.
 
 ```
  cp gssnng/gssnng/test/example_script.py  .
  
- python3.8 test_gssnng.py
+ python3 test_gssnng.py
 ```
 
 
 ## Usage 
 
 See gssnng/notebooks for examples on all methods
 
@@ -88,26 +94,23 @@
 2. Get your gene sets formatted as a .gmt file. (default is undirected, can take _UP,  _DN, and split gene sets _UP+_DN)
 
 3. Score cells, each gene set will show up as a column in adata.obs.
 
 ```
 from gssnng import score_cells
 
-q = sc.read_h5ad('gssnng/gssnng/test/data/pbmc3k_processed.h5ad')
+q = sc.datasets.pbmc3k_processed()
 
-sc.pp.neighbors(q, n_neighbors=32)
-
-score_cells.with_gene_sets(adata=q,                            # AnnData object
+score_cells.with_gene_sets(adata=adata,                         # AnnData object
                             gene_set_file='cibersort_lm22.gmt', # File path of gene sets
                             groupby='louvain',                  # Will sample neighbors within this group
                             smooth_mode='connectivity',         # Smooths matrix using distance weights from NN graph.
-                            recompute_neighbors=0,              # Rebuild nearest neighbor graph with groups, 0 turns off function
+                            recompute_neighbors=32,             # Rebuild nearest neighbor graph with groups, 0 turns off function
                             score_method='singscore',           # Method of scoring
                             method_params={'normalization':'theoretical'},  # Special parameters for some methods 
-                            samp_neighbors=27,                  # Number of sampled neighbors for pseudobulk
                             ranked=True,                        # Use ranked data, True or False
                             cores=8)                            # Groups are scored in parallel.
     
 
 sc.pl.umap(q, color=['louvain','T.cells.CD8.up'], wspace=0.35)
 ```
 
@@ -119,69 +122,76 @@
     gene_set_file: str[path]
     The gene set file with list of gene sets, gmt, one per line. See `this definition <https://software.broadinstitute.org/cancer/software/gsea/wiki/index.php/Data_formats#GMT:_Gene_Matrix_Transposed_file_format_.28.2A.gmt.29>`_ .
 
     groupby: [str, list, dict]
     either a column label in adata.obs, and all categories taken, or a dict specifies one group.
     SEE DESCRIPTION BELOW
 
-    smooth_mode: "adjacency" or "connectivity",
+    smooth_mode: "adjacency", "connectivity", or "off"
     Dictates how to use the neighborhood graph.
-    `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more
+    `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more, `off` does no smoothing.
 
     recompute_neighbors: int
     should neighbors be recomputed within each group, 0 for no, >0 for yes and specifies N
 
     score_method: str
     which scoring method to use
 
     method_params: dict
     python dict with XGBoost params.
 
-    samp_neighbors: int
-    number of neighbors to sample
-
     ranked: bool
     whether the gene expression counts should be rank ordered
 
     cores: int
     number of parallel processes to work through groupby groups
 
 ## Groupby
 
-The specific neighborhood for each cell can be controlled by using the groupby parameter. In the example
+The group of cells available for constructing the neighborhood graph can be controlled by using the groupby parameter. In the example
 above, by setting groupby='louvain', only cells within a louvain cluster will be considered as being part of the
 neighborhood and will available for sampling.
-Groupby specifies a column name that's found in the AnnData.obs table, and it can also take a list of column names.
+
+Groupby specifies a column name (or list of columns) that's found in the AnnData.obs table.
 In that case, cells will be grouped as the intersection of categories. For example, using groupby=['louvain','phenotype']
 will take cells that are first in a given louvain cluster and then also in a given phenotype group. By also setting
 the recompute_neighbors, the nearest neighbor graph is recomputed within this subset of cells. Controlling the
 neighborhood leads to more controlled smoothing of the count matrix and is more suitable for downstream comparisons.
 
 ## Gene sets
 
 We are following the MSigDB nomenclature, where gene sets default to undirected, but can be marked with the suffix "_UP"
 (example: CD8_signature_UP or CD8.signature.up).  In this case, when data is ranked, genes with higher expression have larger ranks. If the 
 gene set has suffix "_DN" (example: CD8_signature_DN or CD8.signature.dn), then lowest expressed genes have largest ranks. In the 
 use of singscore or Z scores, the undirected case is based on absolute values, so either direction, in the extreme, will result in a large score.
 
+To access OmniPath signatures, see the ["decoupler-style"](https://github.com/IlyaLab/gssnng/blob/main/notebooks/gssnng_decoupler.ipynb) notebook.
+
 ## Method options
 
 Some methods have some additional options. They are passed as a dictionary, method_params={param_name: param_value}.
 
+    geneset_overlap: {'threshold': 0, 'fraction': False}
+    
+The geneset overlap compares the smoothed value or rank of geneset genes to the threshold. If ranked=False, then ranks are used.
+If smooth_mode is set to "off", this method can be used with untransformed counts.  If 'percent' is set to True, then 
+the overlap will be given as a percentage of the total number of genes in the gene set.
+
     singscore:  {'normalization': 'theoretical'}, {'normalization': 'standard'}
 
 The singscore manuscript describes the theoretical method of standarization which involves determining the theoretical max and minimum ranks for the given gene set.
 
-    ssGSEA: {'omega': 0.25}
+    ssGSEA: {'omega': 0.75}
     
-The ssGSEA method uses this parameter as a exponent to the ranks.
+The ssGSEA method uses this parameter as a exponent to the ranks. It has been strongly suggested to use 0.75.
 
     rank_biased_overlap:  {'rbo_depth': n}  (n: int)
 
-Here, n is the depth that is decended down the ranks, where at each step, the overlap with the gene set is measured and added to the score.
+Here, n is the depth that we decend down the ranks, where at each step, the overlap with the gene set is measured and added to the score.
+
 
 *The following methods do not have additional options.*
 
     robust_std
     mean_z
     average_score
     median_score
```

### Comparing `gssnng-0.2.6.2/README.md` & `gssnng-0.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gssnng
 
-**Try it out!  ===>>>**  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Gibbsdavidl/gssnng/blob/main/notebooks/gssnng_quick_start.ipynb)
+**Try it out!  ===>>>**  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IlyaLab/gssnng/blob/main/notebooks/gssnng_quick_start.ipynb)
 
 **See the paper ===>>>** [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.29.518384v1)
 
 Gene Set Scoring on the Nearest Neighbor Graph (gssnng) for Single Cell RNA-seq (scRNA-seq).
 
 The problem:  The sparsity of scRNA-seq data creates a poor overlap with many gene sets, 
 which in turn makes gene set scoring difficult. 
@@ -15,61 +15,67 @@
 
 Nearest neighbor graphs (NNG) are constructed based on user defined groups (see the 'groupby' parameter below). 
 The defined groups can be processed in parallel, speeding up the calculations. For example, a NNG could be 
 constructed within each cluster or jointly by cluster *and* sample. Smoothing can be performed using either the 
 adjacency matrix (all 1s) or the weighted graph to give less weight to more distant cells.
 
 This package works with AnnData objects stored as h5ad files. Expression values are taken from adata.X.
-For creating groups, up to four categorical variables can be used, which are found in the adata.obs table.
+For creating groups, up to four categorical variables can be used, which are found in the adata.obs table. 
+Gene sets can be provided by using .gmt files or through the OmniPath API (see below).
 
 Scoring functions work with ranked or unranked data (**"your mileage may vary"**):
 
-Some method references (singscore, RBO) are below.
+Method references (singscore, RBO) are below. 
+
+Some methods have additional parameters, see below!
 
 ```
-    singscore:            Normalised mean (median centered) ranks (requires ranked data)
+    geneset_overlap: Number (or fraction) of genes, past an expression threshold, that overlap with each geneset.
+
+    singscore:       Normalised mean (median centered) ranks (requires ranked data)
     
-    ssgsea:               The well known single sample GSEA.
+    ssgsea:          The well known single sample GSEA.
         
     rank_biased_overlap:  RBO, Weighted average of agreement between sorted ranks and gene set.
 
-    robust_std:     Med(x-med / mad), median of robust standardized values (recommend unranked).
+    robust_std:      Med(x-med / mad), median of robust standardized values (recommend unranked).
+    
+    mean_z:          Mean( (x - mean)/stddv ), average z score. (recommend unranked).
     
-    mean_z:         Mean( (x - mean)/stddv ), average z score. (recommend unranked).
+    average_score:   Mean ranks or counts     
     
-    average_score:  Mean ranks or counts     
+    median_score:    Median of counts or ranks
     
-    median_score:   Median of counts or ranks
+    summed_up:       Sum up the ranks or counts.
     
-    summed_up:      Sum up the ranks or counts.
 ```
 
 ## Installation from PyPI
 ```
 pip3 install gssnng
 ```
 
 
 ## Installation from GitHub
 
 ```
 # also gets you the demo data and some gene sets.
-git clone https://github.com/Gibbsdavidl/gssnng
+git clone https://github.com/IlyaLab/gssnng
 
 pip install -e gssnng
 ```
 
 ## Example script
 
 Copy the script out from the cloned repo and run, check the paths if you get an error.
 
 ```
  cp gssnng/gssnng/test/example_script.py  .
  
- python3.8 test_gssnng.py
+ python3 test_gssnng.py
 ```
 
 
 ## Usage 
 
 See gssnng/notebooks for examples on all methods
 
@@ -78,26 +84,23 @@
 2. Get your gene sets formatted as a .gmt file. (default is undirected, can take _UP,  _DN, and split gene sets _UP+_DN)
 
 3. Score cells, each gene set will show up as a column in adata.obs.
 
 ```
 from gssnng import score_cells
 
-q = sc.read_h5ad('gssnng/gssnng/test/data/pbmc3k_processed.h5ad')
+q = sc.datasets.pbmc3k_processed()
 
-sc.pp.neighbors(q, n_neighbors=32)
-
-score_cells.with_gene_sets(adata=q,                            # AnnData object
+score_cells.with_gene_sets(adata=adata,                         # AnnData object
                             gene_set_file='cibersort_lm22.gmt', # File path of gene sets
                             groupby='louvain',                  # Will sample neighbors within this group
                             smooth_mode='connectivity',         # Smooths matrix using distance weights from NN graph.
-                            recompute_neighbors=0,              # Rebuild nearest neighbor graph with groups, 0 turns off function
+                            recompute_neighbors=32,             # Rebuild nearest neighbor graph with groups, 0 turns off function
                             score_method='singscore',           # Method of scoring
                             method_params={'normalization':'theoretical'},  # Special parameters for some methods 
-                            samp_neighbors=27,                  # Number of sampled neighbors for pseudobulk
                             ranked=True,                        # Use ranked data, True or False
                             cores=8)                            # Groups are scored in parallel.
     
 
 sc.pl.umap(q, color=['louvain','T.cells.CD8.up'], wspace=0.35)
 ```
 
@@ -109,69 +112,76 @@
     gene_set_file: str[path]
     The gene set file with list of gene sets, gmt, one per line. See `this definition <https://software.broadinstitute.org/cancer/software/gsea/wiki/index.php/Data_formats#GMT:_Gene_Matrix_Transposed_file_format_.28.2A.gmt.29>`_ .
 
     groupby: [str, list, dict]
     either a column label in adata.obs, and all categories taken, or a dict specifies one group.
     SEE DESCRIPTION BELOW
 
-    smooth_mode: "adjacency" or "connectivity",
+    smooth_mode: "adjacency", "connectivity", or "off"
     Dictates how to use the neighborhood graph.
-    `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more
+    `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more, `off` does no smoothing.
 
     recompute_neighbors: int
     should neighbors be recomputed within each group, 0 for no, >0 for yes and specifies N
 
     score_method: str
     which scoring method to use
 
     method_params: dict
     python dict with XGBoost params.
 
-    samp_neighbors: int
-    number of neighbors to sample
-
     ranked: bool
     whether the gene expression counts should be rank ordered
 
     cores: int
     number of parallel processes to work through groupby groups
 
 ## Groupby
 
-The specific neighborhood for each cell can be controlled by using the groupby parameter. In the example
+The group of cells available for constructing the neighborhood graph can be controlled by using the groupby parameter. In the example
 above, by setting groupby='louvain', only cells within a louvain cluster will be considered as being part of the
 neighborhood and will available for sampling.
-Groupby specifies a column name that's found in the AnnData.obs table, and it can also take a list of column names.
+
+Groupby specifies a column name (or list of columns) that's found in the AnnData.obs table.
 In that case, cells will be grouped as the intersection of categories. For example, using groupby=['louvain','phenotype']
 will take cells that are first in a given louvain cluster and then also in a given phenotype group. By also setting
 the recompute_neighbors, the nearest neighbor graph is recomputed within this subset of cells. Controlling the
 neighborhood leads to more controlled smoothing of the count matrix and is more suitable for downstream comparisons.
 
 ## Gene sets
 
 We are following the MSigDB nomenclature, where gene sets default to undirected, but can be marked with the suffix "_UP"
 (example: CD8_signature_UP or CD8.signature.up).  In this case, when data is ranked, genes with higher expression have larger ranks. If the 
 gene set has suffix "_DN" (example: CD8_signature_DN or CD8.signature.dn), then lowest expressed genes have largest ranks. In the 
 use of singscore or Z scores, the undirected case is based on absolute values, so either direction, in the extreme, will result in a large score.
 
+To access OmniPath signatures, see the ["decoupler-style"](https://github.com/IlyaLab/gssnng/blob/main/notebooks/gssnng_decoupler.ipynb) notebook.
+
 ## Method options
 
 Some methods have some additional options. They are passed as a dictionary, method_params={param_name: param_value}.
 
+    geneset_overlap: {'threshold': 0, 'fraction': False}
+    
+The geneset overlap compares the smoothed value or rank of geneset genes to the threshold. If ranked=False, then ranks are used.
+If smooth_mode is set to "off", this method can be used with untransformed counts.  If 'percent' is set to True, then 
+the overlap will be given as a percentage of the total number of genes in the gene set.
+
     singscore:  {'normalization': 'theoretical'}, {'normalization': 'standard'}
 
 The singscore manuscript describes the theoretical method of standarization which involves determining the theoretical max and minimum ranks for the given gene set.
 
-    ssGSEA: {'omega': 0.25}
+    ssGSEA: {'omega': 0.75}
     
-The ssGSEA method uses this parameter as a exponent to the ranks.
+The ssGSEA method uses this parameter as a exponent to the ranks. It has been strongly suggested to use 0.75.
 
     rank_biased_overlap:  {'rbo_depth': n}  (n: int)
 
-Here, n is the depth that is decended down the ranks, where at each step, the overlap with the gene set is measured and added to the score.
+Here, n is the depth that we decend down the ranks, where at each step, the overlap with the gene set is measured and added to the score.
+
 
 *The following methods do not have additional options.*
 
     robust_std
     mean_z
     average_score
     median_score
```

### Comparing `gssnng-0.2.6.2/gssnng/score_cells.py` & `gssnng-0.4.2/gssnng/score_cells.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,60 +3,160 @@
 from scipy import sparse
 import pandas as pd
 import scanpy as sc
 from anndata import AnnData
 from gssnng.smoothing import nn_smoothing
 from gssnng.util import error_checking
 from gssnng.score_funs import scorefun
-from gssnng.gene_sets import genesets
+from gssnng.gene_sets import genesets_from_gmt, Genesets, genesets_from_decoupler_model
 from typing import Union
 from multiprocessing import Pool
 
 
+def run_gssnng(
+    mat, net, source, target, weight, 
+    groupby: Union[str, list, dict],
+    smooth_mode: str,
+    recompute_neighbors: int,
+    score_method: str,
+    method_params: dict,
+    #samp_neighbors: int,
+    ranked: bool,
+    cores: int,
+    verbose=False,
+    use_raw=True
+    ):
+    
+    """
+    GSSNNG: gene set scoring (all gene sets in file) with nearest neighbor smoothing of the expression matrix
+
+    Improved single cell scoring by:
+    - smoothing the data matrix
+        - adding noise to the nearest neighbor smoothing via `samp_neighbors`
+    - adding noise to the expression data itself (via noise_trials)
+
+
+    Parameters
+    ----------
+    mat : list, DataFrame or AnnData
+        List of [features, matrix], dataframe (samples x features) or an AnnData
+        instance.
+    net : DataFrame
+        Network in long format.
+    source : str
+        Column name in net with source nodes.
+    target : str
+        Column name in net with target nodes.
+    weight : str
+        Column name in net with weights.
+    groupby : str
+        Either a column label in adata.obs, and all categories taken, or a dict specifies one group.
+    smooth_mode : ['adjacency','connectivity']
+        Which representation of the neighborhood graph to use.
+        `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more
+    recompute_neighbors : bool
+        should neighbors be recomputed within each group, 0 for no, >0 for yes and specifies N.
+    score_method : str
+        Which scoring method to use.
+    method_params: dict
+        specific params for each method.
+    ranked: int
+        Whether the gene expression counts should be rank ordered
+    cores: int
+        number of parallel processes to work through groupby groups
+
+    Returns
+    -------
+    if mat is an AnnData object:
+        gssnng scores in `mat.obsm['gssnng_estimate']` 
+    else:
+        pd.DataFrame with the scores
+    """
+
+    # This whole function is basically a wrapper around the old gssnng-API
+    # but working with decoupler-input and -output
+    noise_trials = 0  ### !TODO! not used currently
+
+    # our gene set data object list
+    gs_obj = genesets_from_decoupler_model(net, source, target , weight)
+
+    samp_neighbors = None
+    error_checking(mat, samp_neighbors, recompute_neighbors,
+                   gs_obj, score_method, ranked, method_params)
+
+    if method_params == None:
+        method_params = dict()
+
+    # score each cell with the list of gene sets
+    all_scores = _proc_data(mat, gs_obj, groupby, smooth_mode, recompute_neighbors,
+                                  score_method, method_params, samp_neighbors,
+                                  noise_trials, ranked, cores)
+
+    # warning: the all_scores rows might have a diferent order!
+    # make sure to resort them according to the mat.obs.index
+    all_scores = all_scores.loc[mat.obs.index]
+
+    # AnnData support
+    if isinstance(mat, AnnData):
+        # Update obsm AnnData object
+        mat.obsm['gssnng_estimate'] = all_scores
+    else:
+        return all_scores
+
+
 def with_gene_sets(
         adata: anndata.AnnData,
         gene_set_file: str,
         groupby: Union[str, list, dict],
         smooth_mode: str,
         recompute_neighbors: int,
         score_method: str,
         method_params: dict,
-        samp_neighbors: int,
+        #samp_neighbors: int,
         ranked: bool,
         cores: int
     ) -> anndata.AnnData:
 
     """
     gene set scoring (all gene sets in file) with nearest neighbor smoothing of the expression matrix
 
     Improved single cell scoring by:
     - smoothing the data matrix
         - adding noise to the nearest neighbor smoothing via `samp_neighbors`
     - adding noise to the expression data itself (via noise_trials)
 
-    :param adata: anndata.AnnData containing the cells to be scored
-    :param gene_set_file: the gene set file with list of gene sets, gmt, one per line
-    :param groupby: either a column label in adata.obs, and all categories taken, or a dict specifies one group.
-    :param smooth_mode: `adjacency` or `connectivity`, which representation of the neighborhood graph to use.
+    :param adata
+        anndata.AnnData containing the cells to be scored
+    :param gene_set_file
+        the gene set file with list of gene sets, gmt, one per line
+    :param groupby
+        either a column label in adata.obs, and all categories taken, or a dict specifies one group.
+    :param smooth_mode
+        `adjacency` or `connectivity`, which representation of the neighborhood graph to use.
         `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more
-    :param recompute_neighbors: should neighbors be recomputed within each group, 0 for no, >0 for yes and specifies N
-    :param score_method: which scoring method to use
-    :param method_params: specific params for each method.
-    :param samp_neighbors: number of neighbors to sample
-    :param ranked: whether the gene expression counts should be rank ordered
-    :param cores: number of parallel processes to work through groupby groups
+    :param recompute_neighbors
+        should neighbors be recomputed within each group, 0 for no, >0 for yes and specifies N
+    :param score_method
+        which scoring method to use
+    :param method_params
+        specific params for each method.
+    :param ranked
+        whether the gene expression counts should be rank ordered
+    :param cores
+        number of parallel processes to work through groupby groups
 
     :returns: adata with gene set scores in .obs
     """
 
     noise_trials = 0  ### not used currently
 
     # our gene set data object list
-    gs_obj = genesets(gene_set_file)
+    gs_obj = genesets_from_gmt(gene_set_file)
 
+    samp_neighbors = None
     error_checking(adata, samp_neighbors, recompute_neighbors,
                    gs_obj, score_method, ranked, method_params)
 
     if method_params == None:
         method_params = dict()
 
     # score each cell with the list of gene sets
@@ -74,21 +174,24 @@
     """
     calculates a neighourhood-smoothed signal of adata.X.
     :param samp_neighbors: how many NN to subsample (hence introducing some noise)
     :param smooth_mode: 'connectivity', 'adjacency', see nn_smoothing()
 
     Returns a complete AnnData with smooeth adata.X
     """
-    if smooth_mode not in ['connectivity', 'adjacency']:
-        print("ERROR:  please use smooth mode: `adjacency` or `connectivity`")
-        exit()
-    smoothed_matrix = nn_smoothing(adata.X, adata, smooth_mode, samp_neighbors)
-    # for easier handling with gene names
-    # smoothed_adata = AnnData(smoothed_matrix, obs=adata.obs, var=adata.var)
-    adata.obsm['X_smooth'] = smoothed_matrix
+    if smooth_mode not in ['connectivity', 'adjacency', 'off']:
+        raise Exception("ERROR:  please use smooth mode: `adjacency`, `connectivity`, or `off`.")
+
+    if smooth_mode == 'off':
+        adata.obsm['X_smooth'] = sparse.csr_matrix(adata.X)
+    else:
+        smoothed_matrix = nn_smoothing(adata.X, adata, smooth_mode, samp_neighbors)
+        # for easier handling with gene names
+        # smoothed_adata = AnnData(smoothed_matrix, obs=adata.obs, var=adata.var)
+        adata.obsm['X_smooth'] = smoothed_matrix
     return(adata)
 
 
 def _build_data_list(
         adata,
         groupby,
         cats,
@@ -113,15 +216,15 @@
         data_list.append(params)
     # send off for scores
     return(data_list)
 
 
 def _proc_data(
         adata: anndata.AnnData,
-        gs_obj: genesets,
+        gs_obj: Genesets,
         groupby: Union[str, list, dict],
         smooth_mode: str,
         recompute_neighbors: int,
         score_method: str,
         method_params: dict,
         samp_neighbors: int,
         noise_trials: int,
@@ -217,15 +320,16 @@
     # for each cell, rank the expression
     #gene_mat = smoothed_adata.X[cell_ix]
     gene_mat = (smoothed_adata.obsm['X_smooth'])[cell_ix]
     # then we subset it to only the genes with counts
     _, gdx, _ = sparse.find(gene_mat)
 
     if gene_mat.ndim == 2:
-        df = pd.DataFrame(gene_mat[:, gdx].A.flatten(), index=smoothed_adata.var.index[gdx])  ## ????
+        df = pd.DataFrame(gene_mat[:, gdx].A.flatten(),
+                          index=smoothed_adata.var.index[gdx])  ## ????
     else:
         df = pd.DataFrame(gene_mat[gdx],
                           index=smoothed_adata.var.index[gdx])  ## not sure why it's coming off as an array
     df.columns = ['counts']
 
     if ('normalization' in method_params) and (method_params['normalization'] == 'average') and (noise_trials > 0):
         # add some noise to gene counts.. create a n numbers of examples
@@ -240,15 +344,15 @@
         df_noise['dnrank'] = np.max(df['uprank']) - df['uprank']
 
     return(df_noise)
 
 
 def _score_all_cells_all_sets(
         smoothed_adata: AnnData,
-        gene_set_obj: genesets,
+        gene_set_obj: Genesets,
         score_method: str,
         method_params: dict,
         noise_trials: int,
         ranked: bool,
         group_name: str
         ) -> pd.DataFrame:
     """
```

### Comparing `gssnng-0.2.6.2/gssnng/score_funs.py` & `gssnng-0.4.2/gssnng/score_funs.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,68 +139,114 @@
 
     if gs.mode != '?':
         norm_up = norm_up - 0.5
 
     return(norm_up)
 
 
+def max_deviation_from_zero(x):
+    """
+    for vector x, get its biggest deviation from zero (inlcuding its sign)
+    e.g:
+    x = [0,1,-1, 2]  -> 2
+    x = [0,1,-2, 1]  -> -2
+
+    This is different than np.max(np.abs(x))!!
+    """
+    themax = np.max(x)
+    themin = np.min(x)
+
+    if np.abs(themax) > np.abs(themin):
+        return themax
+    else:
+        return themin
+
+
 def ssgsea(x, su, sig_len, omega, gs):
     """
     The ssGSEA method
+    see https://www.pathwaycommons.org/guide/primers/data_analysis/gsea/ for some details
 
     :param x: the pandas data frame of ranks, all genes
     :param su: the ranked list of genes *IN* the gene set
     :param sig_len: the number of expressed genes matched in the set
     :param norm_method: 'standard or theoretical' # from singscore
     :param score_up: is the rank up or down?  True or False
     :param gene_set: gene set object
 
     """
     # The gene expression values for a given sample were rank-normalized
 
     gene_set = set(gs)
-
+    assert isinstance(x, pd.Series), "x must be a pd.Series"
     #first sort by absolute expression value, starting with the highest expressed genes first
     xsorted = x.sort_values(axis=0, ascending=False, inplace=False)
     keys_sorted = xsorted.index.tolist()
 
+    # increments will always be positive, |s_t| in the above link
+    xsorted = np.abs(xsorted)
+
     #values representing the ECDF of genes in the geneset
     P_GW_numerator = 0
     P_GW_denominator = 0
 
     #determining denominator value
-    i = 1 #current rank stepping through listing of sorted genes
     for gene in keys_sorted:
         if gene in gene_set:
-            P_GW_denominator += i ** omega
-        i += 1
+            s = xsorted.loc[gene]
+            P_GW_denominator += s ** omega
 
     P_GW = lambda : P_GW_numerator / P_GW_denominator
 
     #values representing the ECDF of genes not in the geneset
     P_NG_numerator = 0
     P_NG_denominator = len(x) - len(gene_set)
     P_NG = lambda : P_NG_numerator / P_NG_denominator
 
     #integrate different in P_GW and P_NG
-    i = 1 #current index in the traversal of sorted genes
     scores = []
     for gene in keys_sorted:
         if gene in gene_set:
-            P_GW_numerator += i ** omega
+            s = xsorted.loc[gene]
+            P_GW_numerator += s ** omega
         else:
             P_NG_numerator += 1
         scores.append(P_GW() - P_NG())
-        i += 1
 
-    return sum(scores)
+    # up to debate if we return max.dev or just sum(score)
+    # max.dev is argued to be more robust. Also relates to the KS-test (omega=0)
+    return max_deviation_from_zero(scores)
+
+
+def geneset_overlap(su, threshold, geneset_len):
+    """
+    Median of median standardized counts
+
+    :param exprdat: the pandas data frame of ranks, all genes
+    :param treshold: the value compared to exprdat['counts']
+    """
+    if geneset_len > 0:
+        score = float(np.sum([x > threshold for x in su])) / float(geneset_len)
+    else:
+        score = np.sum([x > threshold for x in su])
+
+    return(score)
 
 
 
 def expr_format(x, exprcol, geneset_genes):
+    """
+    Prepare the cell's expression for scoring.
+    :param x: the gene expr data frame, columns are: counts, uprank, dnrank
+    :param exprcol: the column containing values we'll compute on
+    :param geneset_genes: genes in the gene set
+
+    :return su: values for the genes *IN* the gene set, ranked or not
+    :return sig_len: the number of expressed genes matched in the set
+    """
     sig_len_up = len(geneset_genes)
     su = []
     for j in geneset_genes:
         if j in x.index:
             su.append(x[exprcol][j])
         else:
             sig_len_up = sig_len_up - 1
@@ -245,14 +291,20 @@
     elif method == 'rank_biased_overlap':
         res0 = rank_biased_overlap(x, exprcol, gs, geneset_genes, method_params['rbo_depth'])
 
     elif method == 'ssgsea':
         #x, su, sig_len, omega, gene_set
         res0 = ssgsea(exprdat, su, sig_len, method_params['omega'], geneset_genes)
 
+    elif method == 'geneset_overlap':
+        if ('fraction' in method_params) and (method_params['fraction'] == True):
+            res0 = geneset_overlap(su, method_params['threshold'], len(geneset_genes))
+        else:
+            res0 = geneset_overlap(su, method_params['threshold'], 0)
+
     else:
         return(np.nan)
 
     return(res0)
 
 
 def scorefun(gs,
@@ -278,15 +330,15 @@
 
         elif (gs.mode == 'DN') and (ranked == False):
             res0 = method_selector(gs, x, 'counts', gs.genes_dn, method, method_params)
 
         elif (gs.mode == 'BOTH') and (ranked == False):
             res0_up = method_selector(gs, x, 'counts', gs.genes_up, method, method_params)
             res0_dn = method_selector(gs, x, 'counts', gs.genes_dn, method, method_params)
-            res0 = (res0_up + res0_dn)
+            res0 = (res0_up - res0_dn)
 
         elif (gs.mode == '?') and (ranked == False):
             res0 = method_selector(gs, x, 'counts', gs.genes_up, method, method_params)
 
         elif (gs.mode == 'UP') and (ranked == True):
             res0 = method_selector(gs, x, 'uprank', gs.genes_up, method, method_params)
```

### Comparing `gssnng-0.2.6.2/gssnng/smoothing.py` & `gssnng-0.4.2/gssnng/smoothing.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,21 @@
         assert np.all(A.diagonal() == 0), "diagonal of distance matrix not 0!!"
         if add_diag:
             A = A + sparse.diags(np.ones(A.shape[0]))
 
         # normalize to sum=1 per  row
         row_scaler = 1 / A.sum(axis=1).A.flatten()
 
-        # multiplying with a diag matrix d on the left multiplys each row i by d_i
+        # multiplying with a diag matrix d on the left multiplies each row i by d_i
         normA = sparse.diags(row_scaler) @ A
         return normA
 
     # actually works exactly the same; could just switch out the obsp key
     elif mode == 'connectivity':
-        A = adata.obsp[NN_CONN_KEY]
+        A = adata.obsp[NN_CONN_KEY] ## neighbor graph
         # add the diagnoal, ie. the datapoint itself should be represented
         # in the smoothing! Note that the max connectivity == 1
         assert np.all(A.diagonal() == 0), "diagonal of connectivity matrix not 0!!"
         if add_diag:
             A = A + sparse.diags(np.ones(A.shape[0]))
         # normalize to sum=1 per  row
         row_scaler = 1 / A.sum(axis=1).A.flatten()
@@ -102,15 +102,15 @@
 
     :return: scipy.sparse matrix with the smoothed signals
     """
     assert X.shape[0] == adata.shape[0], "cell number mismatch"
     logging.info("creating smoothing matrix")
     smoothing_mat = get_smoothing_matrix(adata, mode, add_diag)
 
-    if samp_neighbors > 0:
+    if (samp_neighbors is not None) and (samp_neighbors > 0):
         # randomly set some edges/neighbours to zero
         # experimental and pretty slow!
         logging.info("creating random mask")
         smoothing_mat = random_mask_a_nn_matrix(smoothing_mat, samp_neighbors)
 
     smooth_signals = smoothing_mat @ X
```

### Comparing `gssnng-0.2.6.2/gssnng/util.py` & `gssnng-0.4.2/gssnng/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,36 +26,38 @@
     if type(method_params) != type(dict()):
         raise Exception('ERROR: please use a dictionary to pass method params')
 
     if any([xi in adata.obs.columns for xi in gs_obj.get_gs_names()]):
         #raise Exception('ERROR: gene set names in columns of adata.obs, please drop.')
         print("Warning! Dropping gene set names from obs!")
         genesetlist = [x.name for x in gs_obj.set_list]
-        adata.obs.drop(columns=genesetlist, inplace=True)
+        for gsi in genesetlist:
+            print('dropping: ' + gsi)
+            adata.obs.drop(columns=[gsi], inplace=True)
 
     if 'gssnng_groupby' in adata.obs.columns:
         adata.obs.drop(columns='gssnng_groupby', inplace=True)
         #raise Exception("Error: please drop 'gssnng_groupby' as a column name.")
         print('... and dropping gssnng_groupby column...')
 
     if ranked == False and score_method == 'singscore':
         raise Exception('ERROR: singscore requires ranked data, set ranked parameter to True')
 
     if (recompute_neighbors == None) or (recompute_neighbors == 0):
         n_neighbors = adata.uns['neighbors']['params']['n_neighbors'] #[0]# in older AnnData versions need this??
     else:
         n_neighbors = recompute_neighbors
 
-    if n_neighbors < samp_neighbors:
-        print('*******')
-        print('WARNING: Number of neighbors too low for sampling parameter!')
-        print('Please reduce number of neighbor samples or recompute neighbor graph.')
-        raise Exception('Samp Neighbors Error')
-    else:
-        return(True)
+    #if n_neighbors < samp_neighbors:
+    #    print('*******')
+    #    print('WARNING: Number of neighbors too low for sampling parameter!')
+    #    print('Please reduce number of neighbor samples or recompute neighbor graph.')
+    #    raise Exception('Samp Neighbors Error')
+    #else:
+    return(True)
 
 
 def read_gene_sets(filepath):
     txt = open(filepath).read().split('\n')
     gd = dict()
     for line in txt:
         bits = line.split('\t')
```

### Comparing `gssnng-0.2.6.2/gssnng.egg-info/PKG-INFO` & `gssnng-0.4.2/gssnng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: gssnng
-Version: 0.2.6.2
+Version: 0.4.2
 Summary: Gene Set Scoring on the Nearest Neighbor Graph (gssnng)
-Home-page: http://github.com/gibbsdavidl/gssnng
+Home-page: http://github.com/IlyaLab/gssnng
 Author: David Gibbs,Michael Strasser
-Author-email: gibbsdavidl@gmail.com
+Author-email: david.gibbs@systemsbiology.org
 License: MIT
 Description-Content-Type: text/markdown
 
 # gssnng
 
-**Try it out!  ===>>>**  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Gibbsdavidl/gssnng/blob/main/notebooks/gssnng_quick_start.ipynb)
+**Try it out!  ===>>>**  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IlyaLab/gssnng/blob/main/notebooks/gssnng_quick_start.ipynb)
 
 **See the paper ===>>>** [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.29.518384v1)
 
 Gene Set Scoring on the Nearest Neighbor Graph (gssnng) for Single Cell RNA-seq (scRNA-seq).
 
 The problem:  The sparsity of scRNA-seq data creates a poor overlap with many gene sets, 
 which in turn makes gene set scoring difficult. 
@@ -25,61 +25,67 @@
 
 Nearest neighbor graphs (NNG) are constructed based on user defined groups (see the 'groupby' parameter below). 
 The defined groups can be processed in parallel, speeding up the calculations. For example, a NNG could be 
 constructed within each cluster or jointly by cluster *and* sample. Smoothing can be performed using either the 
 adjacency matrix (all 1s) or the weighted graph to give less weight to more distant cells.
 
 This package works with AnnData objects stored as h5ad files. Expression values are taken from adata.X.
-For creating groups, up to four categorical variables can be used, which are found in the adata.obs table.
+For creating groups, up to four categorical variables can be used, which are found in the adata.obs table. 
+Gene sets can be provided by using .gmt files or through the OmniPath API (see below).
 
 Scoring functions work with ranked or unranked data (**"your mileage may vary"**):
 
-Some method references (singscore, RBO) are below.
+Method references (singscore, RBO) are below. 
+
+Some methods have additional parameters, see below!
 
 ```
-    singscore:            Normalised mean (median centered) ranks (requires ranked data)
+    geneset_overlap: Number (or fraction) of genes, past an expression threshold, that overlap with each geneset.
+
+    singscore:       Normalised mean (median centered) ranks (requires ranked data)
     
-    ssgsea:               The well known single sample GSEA.
+    ssgsea:          The well known single sample GSEA.
         
     rank_biased_overlap:  RBO, Weighted average of agreement between sorted ranks and gene set.
 
-    robust_std:     Med(x-med / mad), median of robust standardized values (recommend unranked).
+    robust_std:      Med(x-med / mad), median of robust standardized values (recommend unranked).
+    
+    mean_z:          Mean( (x - mean)/stddv ), average z score. (recommend unranked).
     
-    mean_z:         Mean( (x - mean)/stddv ), average z score. (recommend unranked).
+    average_score:   Mean ranks or counts     
     
-    average_score:  Mean ranks or counts     
+    median_score:    Median of counts or ranks
     
-    median_score:   Median of counts or ranks
+    summed_up:       Sum up the ranks or counts.
     
-    summed_up:      Sum up the ranks or counts.
 ```
 
 ## Installation from PyPI
 ```
 pip3 install gssnng
 ```
 
 
 ## Installation from GitHub
 
 ```
 # also gets you the demo data and some gene sets.
-git clone https://github.com/Gibbsdavidl/gssnng
+git clone https://github.com/IlyaLab/gssnng
 
 pip install -e gssnng
 ```
 
 ## Example script
 
 Copy the script out from the cloned repo and run, check the paths if you get an error.
 
 ```
  cp gssnng/gssnng/test/example_script.py  .
  
- python3.8 test_gssnng.py
+ python3 test_gssnng.py
 ```
 
 
 ## Usage 
 
 See gssnng/notebooks for examples on all methods
 
@@ -88,26 +94,23 @@
 2. Get your gene sets formatted as a .gmt file. (default is undirected, can take _UP,  _DN, and split gene sets _UP+_DN)
 
 3. Score cells, each gene set will show up as a column in adata.obs.
 
 ```
 from gssnng import score_cells
 
-q = sc.read_h5ad('gssnng/gssnng/test/data/pbmc3k_processed.h5ad')
+q = sc.datasets.pbmc3k_processed()
 
-sc.pp.neighbors(q, n_neighbors=32)
-
-score_cells.with_gene_sets(adata=q,                            # AnnData object
+score_cells.with_gene_sets(adata=adata,                         # AnnData object
                             gene_set_file='cibersort_lm22.gmt', # File path of gene sets
                             groupby='louvain',                  # Will sample neighbors within this group
                             smooth_mode='connectivity',         # Smooths matrix using distance weights from NN graph.
-                            recompute_neighbors=0,              # Rebuild nearest neighbor graph with groups, 0 turns off function
+                            recompute_neighbors=32,             # Rebuild nearest neighbor graph with groups, 0 turns off function
                             score_method='singscore',           # Method of scoring
                             method_params={'normalization':'theoretical'},  # Special parameters for some methods 
-                            samp_neighbors=27,                  # Number of sampled neighbors for pseudobulk
                             ranked=True,                        # Use ranked data, True or False
                             cores=8)                            # Groups are scored in parallel.
     
 
 sc.pl.umap(q, color=['louvain','T.cells.CD8.up'], wspace=0.35)
 ```
 
@@ -119,69 +122,76 @@
     gene_set_file: str[path]
     The gene set file with list of gene sets, gmt, one per line. See `this definition <https://software.broadinstitute.org/cancer/software/gsea/wiki/index.php/Data_formats#GMT:_Gene_Matrix_Transposed_file_format_.28.2A.gmt.29>`_ .
 
     groupby: [str, list, dict]
     either a column label in adata.obs, and all categories taken, or a dict specifies one group.
     SEE DESCRIPTION BELOW
 
-    smooth_mode: "adjacency" or "connectivity",
+    smooth_mode: "adjacency", "connectivity", or "off"
     Dictates how to use the neighborhood graph.
-    `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more
+    `adjacency` weights all neighbors equally, `connectivity` weights close neighbors more, `off` does no smoothing.
 
     recompute_neighbors: int
     should neighbors be recomputed within each group, 0 for no, >0 for yes and specifies N
 
     score_method: str
     which scoring method to use
 
     method_params: dict
     python dict with XGBoost params.
 
-    samp_neighbors: int
-    number of neighbors to sample
-
     ranked: bool
     whether the gene expression counts should be rank ordered
 
     cores: int
     number of parallel processes to work through groupby groups
 
 ## Groupby
 
-The specific neighborhood for each cell can be controlled by using the groupby parameter. In the example
+The group of cells available for constructing the neighborhood graph can be controlled by using the groupby parameter. In the example
 above, by setting groupby='louvain', only cells within a louvain cluster will be considered as being part of the
 neighborhood and will available for sampling.
-Groupby specifies a column name that's found in the AnnData.obs table, and it can also take a list of column names.
+
+Groupby specifies a column name (or list of columns) that's found in the AnnData.obs table.
 In that case, cells will be grouped as the intersection of categories. For example, using groupby=['louvain','phenotype']
 will take cells that are first in a given louvain cluster and then also in a given phenotype group. By also setting
 the recompute_neighbors, the nearest neighbor graph is recomputed within this subset of cells. Controlling the
 neighborhood leads to more controlled smoothing of the count matrix and is more suitable for downstream comparisons.
 
 ## Gene sets
 
 We are following the MSigDB nomenclature, where gene sets default to undirected, but can be marked with the suffix "_UP"
 (example: CD8_signature_UP or CD8.signature.up).  In this case, when data is ranked, genes with higher expression have larger ranks. If the 
 gene set has suffix "_DN" (example: CD8_signature_DN or CD8.signature.dn), then lowest expressed genes have largest ranks. In the 
 use of singscore or Z scores, the undirected case is based on absolute values, so either direction, in the extreme, will result in a large score.
 
+To access OmniPath signatures, see the ["decoupler-style"](https://github.com/IlyaLab/gssnng/blob/main/notebooks/gssnng_decoupler.ipynb) notebook.
+
 ## Method options
 
 Some methods have some additional options. They are passed as a dictionary, method_params={param_name: param_value}.
 
+    geneset_overlap: {'threshold': 0, 'fraction': False}
+    
+The geneset overlap compares the smoothed value or rank of geneset genes to the threshold. If ranked=False, then ranks are used.
+If smooth_mode is set to "off", this method can be used with untransformed counts.  If 'percent' is set to True, then 
+the overlap will be given as a percentage of the total number of genes in the gene set.
+
     singscore:  {'normalization': 'theoretical'}, {'normalization': 'standard'}
 
 The singscore manuscript describes the theoretical method of standarization which involves determining the theoretical max and minimum ranks for the given gene set.
 
-    ssGSEA: {'omega': 0.25}
+    ssGSEA: {'omega': 0.75}
     
-The ssGSEA method uses this parameter as a exponent to the ranks.
+The ssGSEA method uses this parameter as a exponent to the ranks. It has been strongly suggested to use 0.75.
 
     rank_biased_overlap:  {'rbo_depth': n}  (n: int)
 
-Here, n is the depth that is decended down the ranks, where at each step, the overlap with the gene set is measured and added to the score.
+Here, n is the depth that we decend down the ranks, where at each step, the overlap with the gene set is measured and added to the score.
+
 
 *The following methods do not have additional options.*
 
     robust_std
     mean_z
     average_score
     median_score
```

### Comparing `gssnng-0.2.6.2/setup.py` & `gssnng-0.4.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name='gssnng',
-      version='0.2.6.2',
+      version='0.4.2',
       description='Gene Set Scoring on the Nearest Neighbor Graph (gssnng)',
-      url='http://github.com/gibbsdavidl/gssnng',
+      url='http://github.com/IlyaLab/gssnng',
       author='David Gibbs,Michael Strasser',
-      author_email='gibbsdavidl@gmail.com',
+      author_email='david.gibbs@systemsbiology.org',
       license='MIT',
       packages=['gssnng'],
       install_requires=[
           'pandas', 'numpy', 'matplotlib', 'seaborn', 'scipy', 'statsmodels', 'scanpy', 'tqdm'
       ],
       zip_safe=False)
```


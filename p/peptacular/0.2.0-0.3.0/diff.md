# Comparing `tmp/peptacular-0.2.0.tar.gz` & `tmp/peptacular-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptacular-0.2.0.tar", last modified: Thu Jul 27 18:33:55 2023, max compression
+gzip compressed data, was "peptacular-0.3.0.tar", last modified: Tue Aug  8 22:18:20 2023, max compression
```

## Comparing `peptacular-0.2.0.tar` & `peptacular-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.749860 peptacular-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 18:33:45.000000 peptacular-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 18:33:55.745860 peptacular-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 18:33:45.000000 peptacular-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 18:33:45.000000 peptacular-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:33:55.749860 peptacular-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 18:33:45.000000 peptacular-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/src/peptacular/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/fragmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/spans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/src/peptacular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_spans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:18:20.038586 peptacular-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 22:18:08.000000 peptacular-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-08 22:18:20.038586 peptacular-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-08 22:18:08.000000 peptacular-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 22:18:08.000000 peptacular-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:18:20.038586 peptacular-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-08 22:18:08.000000 peptacular-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:18:20.034586 peptacular-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:18:20.034586 peptacular-0.3.0/src/peptacular/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/fragmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-08-08 22:18:08.000000 peptacular-0.3.0/src/peptacular/spans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:18:20.034586 peptacular-0.3.0/src/peptacular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-08 22:18:20.000000 peptacular-0.3.0/src/peptacular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 22:18:20.000000 peptacular-0.3.0/src/peptacular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:18:20.000000 peptacular-0.3.0/src/peptacular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 22:18:20.000000 peptacular-0.3.0/src/peptacular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 22:18:20.000000 peptacular-0.3.0/src/peptacular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:18:20.038586 peptacular-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-08 22:18:08.000000 peptacular-0.3.0/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-08-08 22:18:08.000000 peptacular-0.3.0/tests/test_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-08 22:18:08.000000 peptacular-0.3.0/tests/test_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-08-08 22:18:08.000000 peptacular-0.3.0/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-08-08 22:18:08.000000 peptacular-0.3.0/tests/test_spans.py
```

### Comparing `peptacular-0.2.0/LICENSE` & `peptacular-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peptacular-0.2.0/PKG-INFO` & `peptacular-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.2.0
-Summary: Utility package for handling peptide and protein sequences
+Version: 0.3.0
+Summary: Overly simple mass spectrometry based proteomics python package
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `peptacular-0.2.0/README.md` & `peptacular-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `peptacular-0.2.0/pyproject.toml` & `peptacular-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 requires = ["setuptools"]
 
 [project]
 name = "peptacular"
 authors = [
     {name = "Patrick Garrett", email = "pgarrett@scripps.edu"},
 ]
-description = "Utility package for handling peptide and protein sequences"
+description = "Overly simple mass spectrometry based proteomics python package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "regex",
-    "numpy"
 ]
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project.urls]
 repository = "https://github.com/pgarrett-scripps/peptacular.git"
 
 [tool.setuptools.dynamic]
 version = {attr = "peptacular.__version__"}
 
 [tool.pylint]
 max-line-length = 120
 fail-under = 9.5
-good-names = ["db"]
+good-names = ["db", "i", "j", "aa", "n", "k", "p", "Na", "Nb", "Nc", "Nx", "Ny", "Nz", "mz"]
 extension-pkg-whitelist='pydantic'
```

### Comparing `peptacular-0.2.0/src/peptacular/constants.py` & `peptacular-0.3.0/src/peptacular/constants.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.2.0/src/peptacular/fragmenter.py` & `peptacular-0.3.0/src/peptacular/fragmenter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import List
 
-from peptacular.mass import calculate_mz
-from peptacular.sequence import get_fragment_sequences, get_internal_fragment_sequences, strip_modifications
+from .mass import calculate_mz
+from .sequence import get_fragment_sequences, get_internal_fragment_sequences, strip_modifications
 
 
-@dataclass
+@dataclass(frozen=True)
 class Fragment:
     """
     Represents a fragment resulting from breaking a sequence at specific points.
 
     Attributes:
         sequence (str): The sequence of the fragment.
         mass (float): The mass-to-charge (m/z) ratio of the fragment.
@@ -26,34 +26,47 @@
     ion_type: str
     number: int
     internal: bool
     parent_number: int
 
     @property
     def start(self):
+        """
+        Returns the start index of the fragment in the parent sequence.
+        """
         if self.ion_type in 'abc':
             if self.internal is False:
                 return 0
-            else:
-                return self.parent_number - self.number
-        elif self.ion_type in 'xyz':
+            return self.parent_number - self.number
+
+        if self.ion_type in 'xyz':
             return -self.parent_number
 
+        raise ValueError(f"Invalid ion type: {self.ion_type}")
+
     @property
     def end(self):
+        """
+        Returns the end index of the fragment in the parent sequence.
+        """
         if self.ion_type in 'abc':
             return self.parent_number
-        elif self.ion_type in 'xyz':
+
+        if self.ion_type in 'xyz':
             if self.internal is False:
                 return None
-            else:
-                return self.start + self.number
+            return self.start + self.number
+
+        raise ValueError(f"Invalid ion type: {self.ion_type}")
 
     @property
     def label(self):
+        """
+        Returns the label of the fragment, e.g., b2, y3i, etc.
+        """
         return f"{'+' * self.charge}" \
                f"{self.ion_type}" \
                f"{self.parent_number}" \
                f"{'i' if self.internal else ''}" \
                f"{self.number if self.internal else ''}"
 
 
@@ -63,15 +76,15 @@
     Generate a list of fragments for a given peptide sequence.
 
     Args:
         sequence (str): The peptide sequence (can be modified).
         ion_types (List[str]): A list of ion types to consider, e.g., ['b', 'y'].
         charges (List[int]): A list of charge states for the fragments.
         monoisotopic (bool): If True, use monoisotopic masses for calculations.
-        internal_fragments (bool): If True, include internal fragments; otherwise, only terminal fragments are generated.
+        internal_fragments (bool): If True, include internal fragments.
 
     Returns:
         List[Fragment]: A list of Fragment objects representing the generated fragments.
 
     Example:
         sequence = "PEPTIDE"
         ion_types = ['b', 'y']
```

### Comparing `peptacular-0.2.0/src/peptacular/protein.py` & `peptacular-0.3.0/src/peptacular/protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.2.0/src/peptacular/sequence.py` & `peptacular-0.3.0/src/peptacular/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     stack = []
     for i, char in enumerate(text):
         if char == '(':
             stack.append(i)
         elif char == ')':
             if not stack:
                 return False
-            else:
-                stack.pop()
+            stack.pop()
     return len(stack) == 0
 
 
 def convert_to_ms2_pip_style(sequence: str) -> str:
     """
     Converts a peptide sequence to the format used by MS2PIP prediction software.
 
@@ -353,16 +352,16 @@
         forward (bool): If True, start generating from the front; else, start from the back.
 
     Returns:
         generator: A generator yielding amino acid sequences.
     """
     if forward:
         return _sequence_generator_front(sequence)
-    else:
-        return _sequence_generator_back(sequence)
+
+    return _sequence_generator_back(sequence)
 
 
 def _sequence_generator_back(sequence: str) -> Generator[str, None, None]:
     """
     Generates amino acid sequences starting from the back of the sequence.
 
     Args:
@@ -376,15 +375,15 @@
     """
     while sequence:
         index = 0
         if sequence[-1] == ')':
             start_of_modification = sequence.rfind('(')
 
             if start_of_modification == 0:
-                return None
+                return
 
             index = start_of_modification
 
         yield sequence
         sequence = sequence[:index - 1]
 
 
@@ -403,27 +402,27 @@
     """
     if sequence[0] == '(':
         yield sequence
         end_of_modification = sequence.find(')')
         sequence = sequence[end_of_modification + 2:]
 
         if sequence == '':
-            return None
+            return
 
         if sequence[0] == '(':
             end_of_modification = sequence.find(')')
             sequence = sequence[end_of_modification + 1:]
 
     while sequence:
         index = 0
         if len(sequence) > 1 and sequence[1] == '(':
             end_of_modification = sequence.find(')')
 
             if end_of_modification == len(sequence):
-                return None
+                return
 
             index = end_of_modification
 
         yield sequence
         sequence = sequence[index + 1:]
 
 
@@ -490,16 +489,15 @@
     enzyme_sites = []
     for site in reg.finditer(enzyme_regex, protein_sequence, overlapped=True):
         enzyme_sites.append(site.span(0))
     return [site[0] + 1 for site in enzyme_sites]
 
 
 def digest_sequence(sequence: str, enzyme_regex: Union[List[str], str], missed_cleavages: int, min_len: int = None,
-                    max_len: int = None, semi: bool = False) -> List[
-    str]:
+                    max_len: int = None, semi: bool = False) -> List[str]:
     """
     Digests a given amino acid sequence using specified enzyme rules and parameters, returning a list of peptides.
 
     The sequence is broken down into peptides based on the enzyme's cleavage rules, with the number of
     missed cleavages taken into account. The returned peptides are filtered based on minimum and maximum length.
 
     Args:
@@ -550,8 +548,8 @@
     Args:
         sequence (str): The peptide sequence.
         ion_type (str): The type of ion for which internal fragments are generated.
 
     Returns:
         List[str]: The internal fragment sequences.
     """
-    return list(sequence_generator(sequence, forward=ion_type not in 'xyz'))
+    return list(sequence_generator(sequence, forward=ion_type not in 'xyz'))
```

### Comparing `peptacular-0.2.0/src/peptacular/spans.py` & `peptacular-0.3.0/src/peptacular/spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import wraps
 from typing import Tuple, List, Optional
 from itertools import groupby
 
-# TODO: Remove wrapper function? Its confusing and hurts readability
 
+# TODO: Remove wrapper function? Its confusing and hurts readability
 
 def span_processing(func):
     """
     A decorator to enforce constraints on the span and min_len and max_len arguments of decorated functions.
     The span should be a tuple of length 3 and min_len and max_len should be None or an integer.
     """
 
@@ -35,15 +35,15 @@
     Args:
         span (Tuple[int, int, int]): A tuple representing the span, structured as (start, end, value).
 
     Raises:
         ValueError: If the span is not valid.
 
     """
-    start, end, value = span
+    start, end, _ = span
     if start < 0:
         raise ValueError(f'Start of span should be non-negative, got {start}.')
     if end < 0:
         raise ValueError(f'End of span should be non-negative, got {end}.')
     if start > end:
         raise ValueError(f'Start of span {start} should be less than or equal to end of span {end}.')
 
@@ -60,15 +60,15 @@
         min_len (int, optional): The minimum length of sub-spans to be generated. Defaults to 1.
         max_len (int, optional): The maximum length of sub-spans to be generated. If not provided, it defaults to the
                                  length of the input span.
 
     Returns:
         List[Tuple[int, int, int]]: A list of all possible sub-spans as tuples, each structured as (start, end, value).
     """
-    start, end, value = span
+    start, end, _ = span
     return [(i, j, 0) for i in range(start, end + 1) for j in range(i + min_len, min(end + 1, i + max_len + 1))]
 
 
 @span_processing
 def build_left_semi_spans(span: Tuple[int, int, int], min_len: int, max_len: int) -> List[Tuple[int, int, int]]:
     """
     This function generates and returns all possible sub-spans of the given span starting from the left.
@@ -158,15 +158,16 @@
     if max_len is None:
         max_len = max_index
 
     enzyme_sites = [0] + enzyme_sites + [max_index]
 
     spans = []
     for i, start_site in enumerate(enzyme_sites):
-        spans.extend([(start_site, end_site, j) for j, end_site in enumerate(enzyme_sites[i+1:i+missed_cleavages+2])])
+        spans.extend(
+            [(start_site, end_site, j) for j, end_site in enumerate(enzyme_sites[i + 1:i + missed_cleavages + 2])])
 
     # Filter spans based on length
     spans = [span for span in spans if min_len <= span[1] - span[0] <= max_len]
 
     return spans
```

### Comparing `peptacular-0.2.0/src/peptacular.egg-info/PKG-INFO` & `peptacular-0.3.0/src/peptacular.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.2.0
-Summary: Utility package for handling peptide and protein sequences
+Version: 0.3.0
+Summary: Overly simple mass spectrometry based proteomics python package
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `peptacular-0.2.0/tests/test_mass.py` & `peptacular-0.3.0/tests/test_mass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import numpy as np
-
-from peptacular.mass import fragment_sequence, calculate_mass_array
+from peptacular.mass import fragment_sequence
 
 import unittest
 
 class TestPeptide(unittest.TestCase):
     def test_peptide_fragments(self):
         pyteomics_y_frags = [346.1608765557, 173.584076511235, 249.10811270685, 125.05769458680999, 120.06551961887999,
                              60.536398042825]
@@ -35,28 +33,14 @@
         for f in pyteomics_y_frags:
             self.assertTrue(f in y_frags)
 
         self.assertEqual(len(pyteomics_b_frags), len(b_frags))
         for f in pyteomics_b_frags:
             self.assertTrue(f in b_frags)
 
-
-    def test_convert_to_mass_array(self):
-        FRAGS = np.array([97.05276384885, 129.04259308796998, 97.05276384885, 101.04767846841,
-                          113.08406397713001, 115.02694302383001, 129.04259308796998], dtype=np.float32)
-        mass_arr = calculate_mass_array('PEPTIDE')
-        for m in FRAGS:
-            self.assertTrue(m in mass_arr)
-
-        FRAGS = np.array([197.05276384885, 129.04259308796998, 197.05276384885, 101.04767846841,
-                          113.08406397713001, 115.02694302383001, 229.04259308796998], dtype=np.float32)
-        mass_arr = calculate_mass_array('(100)PEP(100)TIDE(100)')
-        for m in FRAGS:
-            self.assertTrue(m in mass_arr)
-
     def test_fragment2(self):
         pyteomics = {'a': [70.06512569606001, 199.10771878403003, 300.15539725243997],
                      'b': [98.06004031562, 227.10263340359, 328.150311872],
                      'c': [115.08658941662999, 244.1291825046, 345.17686097301],
                      'x': [372.14014111112, 275.08737726226997, 146.0447841743],
                      'y': [346.1608765557, 249.10811270685, 120.06551961887999],
                      'z': [329.13432745469, 232.08156360584, 103.03897051786998],
```

### Comparing `peptacular-0.2.0/tests/test_protein.py` & `peptacular-0.3.0/tests/test_protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.2.0/tests/test_sequence.py` & `peptacular-0.3.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.2.0/tests/test_spans.py` & `peptacular-0.3.0/tests/test_spans.py`

 * *Files identical despite different names*


# Comparing `tmp/metasnek-0.0.5.tar.gz` & `tmp/metasnek-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasnek-0.0.5.tar", last modified: Fri Jul 14 07:45:47 2023, max compression
+gzip compressed data, was "metasnek-0.0.6.tar", last modified: Wed Aug  9 04:48:58 2023, max compression
```

## Comparing `metasnek-0.0.5.tar` & `metasnek-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.229712 metasnek-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 07:45:33.000000 metasnek-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 07:45:33.000000 metasnek-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 07:45:47.229712 metasnek-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-14 07:45:33.000000 metasnek-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 07:45:33.000000 metasnek-0.0.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.225712 metasnek-0.0.5/metasnek/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 07:45:33.000000 metasnek-0.0.5/metasnek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-07-14 07:45:33.000000 metasnek-0.0.5/metasnek/fastq_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.229712 metasnek-0.0.5/metasnek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:45:47.229712 metasnek-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-14 07:45:33.000000 metasnek-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.229712 metasnek-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-07-14 07:45:33.000000 metasnek-0.0.5/tests/test_fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:48:58.099063 metasnek-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 04:48:48.000000 metasnek-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-09 04:48:48.000000 metasnek-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-09 04:48:58.099063 metasnek-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-09 04:48:48.000000 metasnek-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-09 04:48:48.000000 metasnek-0.0.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:48:58.099063 metasnek-0.0.6/metasnek/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-09 04:48:48.000000 metasnek-0.0.6/metasnek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-08-09 04:48:48.000000 metasnek-0.0.6/metasnek/fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:48:58.099063 metasnek-0.0.6/metasnek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-09 04:48:58.000000 metasnek-0.0.6/metasnek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-09 04:48:58.000000 metasnek-0.0.6/metasnek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 04:48:58.000000 metasnek-0.0.6/metasnek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-09 04:48:58.000000 metasnek-0.0.6/metasnek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 04:48:58.099063 metasnek-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-09 04:48:48.000000 metasnek-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:48:58.099063 metasnek-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-08-09 04:48:48.000000 metasnek-0.0.6/tests/test_fastq_finder.py
```

### Comparing `metasnek-0.0.5/LICENSE` & `metasnek-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.5/PKG-INFO` & `metasnek-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasnek
-Version: 0.0.5
+Version: 0.0.6
 Summary: Misc functions for metagenomics pipelines
 Home-page: https://github.com/beardymcjohnface/metasnek
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metasnek-0.0.5/README.md` & `metasnek-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.5/metasnek/fastq_finder.py` & `metasnek-0.0.6/metasnek/fastq_finder.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,53 +14,52 @@
     Returns:
         tuple: A tuple containing two sets:
             - paired_files: A set of tuples with the sample name, unpaired file path, and paired file path.
             - unpaired_files: A set of tuples with the sample name and unpaired file path.
     """
 
     paired_files = set()
-    unpaired_files = set()
+    out_paired = set()
+    out_unpaired = set()
 
+    ext_pattern = r"\.(fasta|fastq|fq)(\.gz)?$"
+    r1_possible_patterns = ["_R1", ".R1", "_1", ".1"]
+    r2_possible_patterns = ["_R2", ".R2", "_2", ".2"]
+
+    # find paired reads
     for file in file_list:
-        file_path, file_ext = os.path.splitext(file)
         file_name = os.path.basename(file)
-        file_ext = file_ext.lower()
-
-        pattern = r"\.(fasta|fastq)(\.gz)?$"
-        if re.search(pattern, file_name, re.IGNORECASE):
-            R1_file = None
-            R2_file = None
-
-            if "_R1" in file_name:
-                sample_name = file_name.rsplit("_R1", 1)[0]
-                R2_file = file_path.replace("_R1", "_R2") + file_ext
-                S_file = file_path.replace("_R1", "_S") + file_ext
-                R1_file = file
-            elif "_R2" in file_name:
-                sample_name = file_name.rsplit("_R2", 1)[0]
-                R1_file = file_path.replace("_R2", "_R1") + file_ext
-                S_file = file_path.replace("_R2", "_S") + file_ext
-                R2_file = file
-            elif "_S" in file_name:
-                sample_name = file_name.rsplit("_S", 1)[0]
-                R1_file = file_path.replace("_S", "_R1") + file_ext
-                R2_file = file_path.replace("_S", "_R2") + file_ext
-                S_file = file
-            if R1_file and R2_file and R1_file in file_list and R2_file in file_list:
-                if S_file and S_file in file_list:
-                    paired_files.add((sample_name, R1_file, R2_file, S_file))
-                else:
-                    paired_files.add((sample_name, R1_file, R2_file, None))
-            else:
+        if re.search(ext_pattern, file_name, re.IGNORECASE):
+            for r1_pattern in r1_possible_patterns:
+                if r1_pattern in file_name:
+                    sample_name = file_name.rsplit(r1_pattern, 1)[0]
+                    r2_pattern = r1_pattern.replace("1", "2")
+                    s_pattern = re.sub("(R?)1", "S", r1_pattern)
+                    r2_file = file.replace(r1_pattern, r2_pattern)
+                    s_file = file.replace(r1_pattern, s_pattern)
+                    if r2_file in file_list:
+                        paired_files.add(file)
+                        paired_files.add(r2_file)
+                        if s_file in file_list:
+                            paired_files.add(s_file)
+                            out_paired.add((sample_name, file, r2_file, s_file))
+                        else:
+                            out_paired.add((sample_name, file, r2_file, None))
+    # add remaining files as singletons
+    for file in file_list:
+        file_name = os.path.basename(file)
+        if re.search(ext_pattern, file_name, re.IGNORECASE):
+            if file not in paired_files:
                 sample_name = re.split(r"\.(fasta|fastq)(\.gz)?$", file_name)[0]
-                if "_R1" in sample_name or "_R2" in sample_name:
-                    warnings.warn("Orphaned paired read detected for " + file_name, Warning)
-                unpaired_files.add((sample_name, file))
+                for r_pattern in r1_possible_patterns + r2_possible_patterns:
+                    if r_pattern in sample_name:
+                        warnings.warn(f"Possible orphaned paired read detected for {file_name} with tag {r_pattern}", Warning)
+                out_unpaired.add((sample_name, file))
 
-    return paired_files, unpaired_files
+    return out_paired, out_unpaired
 
 
 def parse_tsv_file(file_path):
     """Parses a 2-4 column TSV file of sample names and sequencing reads (column 3/4 is optional)
 
     Args:
         file_path (str): Path to the TSV file.
@@ -173,15 +172,15 @@
     sample_dictionary = convert_to_dictionary(paired, unpaired)
     return sample_dictionary
 
 
 def write_samples_tsv(dictionary, output_file):
     """Write the samples dictionary to a TSV file
 
-    Args:
+    Args:one
         dictionary:
             - sample name (dict):
                 - R1 (str): filepath of R1 reads file
                 - R2 (str): filepath of R2 reads file or None
                 - S (str): filepath of singleton reads file or None
         output_file (str): filepath of output file for writing
     """
```

### Comparing `metasnek-0.0.5/metasnek.egg-info/PKG-INFO` & `metasnek-0.0.6/metasnek.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasnek
-Version: 0.0.5
+Version: 0.0.6
 Summary: Misc functions for metagenomics pipelines
 Home-page: https://github.com/beardymcjohnface/metasnek
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `metasnek-0.0.5/setup.py` & `metasnek-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.5/tests/test_fastq_finder.py` & `metasnek-0.0.6/tests/test_fastq_finder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import os
 import warnings
 import pytest
 import shutil
-from metasnek.fastq_finder import parse_directory, parse_tsv_file, parse_samples, convert_to_dictionary, parse_samples_to_dictionary, write_samples_tsv
+from metasnek.fastq_finder import (
+    parse_directory,
+    parse_tsv_file,
+    parse_samples,
+    convert_to_dictionary,
+    parse_samples_to_dictionary,
+    write_samples_tsv,
+)
 
 
 @pytest.fixture(scope="session")
 def temp_directory(request, tmpdir_factory):
     temp_dir = tmpdir_factory.mktemp("temp_directory")
     temp_dir_path = str(temp_dir)
 
@@ -26,40 +33,77 @@
         os.path.join(str(temp_directory), "sample2_R1_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample2_R2_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample2_S_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample3.fastq"),
         os.path.join(str(temp_directory), "sample4_R2.fastq"),
         os.path.join(str(temp_directory), "sample5.fasta.gz"),
         os.path.join(str(temp_directory), "sample6.fastq.gz"),
+        os.path.join(str(temp_directory), "sample7.R1.fastq"),
+        os.path.join(str(temp_directory), "sample7.R2.fastq"),
+        os.path.join(str(temp_directory), "sample8_1.FASTQ.GZ"),
+        os.path.join(str(temp_directory), "sample8_2.FASTQ.GZ"),
+        os.path.join(str(temp_directory), "sample9.1.001.fq.gz"),
+        os.path.join(str(temp_directory), "sample9.2.001.fq.gz"),
     ]
 
     for file_path in _file_list:
         open(file_path, "w").close()
 
     return _file_list
 
 
 def assert_parsed_files(paired_files, unpaired_files, temp_directory):
     # Assert paired files
-    assert ("sample1",
-            os.path.join(str(temp_directory), "sample1_R1.fastq"),
-            os.path.join(str(temp_directory), "sample1_R2.fastq"),
-            None
-            ) in paired_files
+    assert (
+        "sample1",
+        os.path.join(str(temp_directory), "sample1_R1.fastq"),
+        os.path.join(str(temp_directory), "sample1_R2.fastq"),
+        None,
+    ) in paired_files
     assert (
         "sample2",
         os.path.join(str(temp_directory), "sample2_R1_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample2_R2_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample2_S_001.fastq.gz"),
     ) in paired_files
+    assert (
+        "sample7",
+        os.path.join(str(temp_directory), "sample7.R1.fastq"),
+        os.path.join(str(temp_directory), "sample7.R2.fastq"),
+        None,
+    ) in paired_files
+    assert (
+        "sample8",
+        os.path.join(str(temp_directory), "sample8_1.FASTQ.GZ"),
+        os.path.join(str(temp_directory), "sample8_2.FASTQ.GZ"),
+        None,
+    ) in paired_files
+    assert (
+        "sample9",
+        os.path.join(str(temp_directory), "sample9.1.001.fq.gz"),
+        os.path.join(str(temp_directory), "sample9.2.001.fq.gz"),
+        None,
+    ) in paired_files
     # Assert unpaired files
-    assert ("sample3", os.path.join(str(temp_directory), "sample3.fastq")) in unpaired_files
-    assert ("sample4_R2", os.path.join(str(temp_directory), "sample4_R2.fastq")) in unpaired_files
-    assert ("sample5", os.path.join(str(temp_directory), "sample5.fasta.gz")) in unpaired_files
-    assert ("sample6", os.path.join(str(temp_directory), "sample6.fastq.gz")) in unpaired_files
+    assert (
+        "sample3",
+        os.path.join(str(temp_directory), "sample3.fastq"),
+    ) in unpaired_files
+    assert (
+        "sample4_R2",
+        os.path.join(str(temp_directory), "sample4_R2.fastq"),
+    ) in unpaired_files
+    assert (
+        "sample5",
+        os.path.join(str(temp_directory), "sample5.fasta.gz"),
+    ) in unpaired_files
+    assert (
+        "sample6",
+        os.path.join(str(temp_directory), "sample6.fastq.gz"),
+    ) in unpaired_files
 
 
 @pytest.fixture(scope="session")
 def create_sample_tsv(temp_directory, file_list):
     tsv_file_path = os.path.join(temp_directory, "sample.tsv")
 
     with open(tsv_file_path, "w") as tsv_file:
@@ -78,48 +122,116 @@
             + "\n"
             "sample3\t" + os.path.join(str(temp_directory), "sample3.fastq") + "\n"
             "sample4_R2\t"
             + os.path.join(str(temp_directory), "sample4_R2.fastq")
             + "\n"
             "sample5\t" + os.path.join(str(temp_directory), "sample5.fasta.gz") + "\n"
             "sample6\t" + os.path.join(str(temp_directory), "sample6.fastq.gz") + "\n"
+            "sample7\t"
+            + os.path.join(str(temp_directory), "sample7.R1.fastq")
+            + "\t"
+            + os.path.join(str(temp_directory), "sample7.R2.fastq")
+            + "\n"
+            "sample8\t"
+            + os.path.join(str(temp_directory), "sample8_1.FASTQ.GZ")
+            + "\t"
+            + os.path.join(str(temp_directory), "sample8_2.FASTQ.GZ")
+            + "\n"
+            "sample9\t"
+            + os.path.join(str(temp_directory), "sample9.1.001.fq.gz")
+            + "\t"
+            + os.path.join(str(temp_directory), "sample9.2.001.fq.gz")
         )
 
     return tsv_file_path
 
 
+@pytest.fixture(scope="session")
+def expected_dictionary(temp_directory, file_list):
+    directory_dictionary = {
+        "sample1": {
+            "R1": os.path.join(temp_directory, "sample1_R1.fastq"),
+            "R2": os.path.join(temp_directory, "sample1_R2.fastq"),
+            "S": None,
+        },
+        "sample2": {
+            "R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
+            "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
+            "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz"),
+        },
+        "sample3": {
+            "R1": os.path.join(temp_directory, "sample3.fastq"),
+            "R2": None,
+            "S": None,
+        },
+        "sample4_R2": {
+            "R1": os.path.join(temp_directory, "sample4_R2.fastq"),
+            "R2": None,
+            "S": None,
+        },
+        "sample5": {
+            "R1": os.path.join(temp_directory, "sample5.fasta.gz"),
+            "R2": None,
+            "S": None,
+        },
+        "sample6": {
+            "R1": os.path.join(temp_directory, "sample6.fastq.gz"),
+            "R2": None,
+            "S": None,
+        },
+        "sample7": {
+            "R1": os.path.join(str(temp_directory), "sample7.R1.fastq"),
+            "R2": os.path.join(str(temp_directory), "sample7.R2.fastq"),
+            "S": None,
+        },
+        "sample8": {
+            "R1": os.path.join(str(temp_directory), "sample8_1.FASTQ.GZ"),
+            "R2": os.path.join(str(temp_directory), "sample8_2.FASTQ.GZ"),
+            "S": None,
+        },
+        "sample9": {
+            "R1": os.path.join(str(temp_directory), "sample9.1.001.fq.gz"),
+            "R2": os.path.join(str(temp_directory), "sample9.2.001.fq.gz"),
+            "S": None,
+        },
+    }
+    return directory_dictionary
+
+
 @pytest.mark.filterwarnings("ignore:Orphaned paired")
 def test_parse_directory(file_list, temp_directory):
     paired_files, unpaired_files = parse_directory(file_list)
     assert_parsed_files(paired_files, unpaired_files, temp_directory)
 
 
 def test_parse_directory_orphand_r():
     # Assert warning for orphaned paired read
     with warnings.catch_warnings(record=True) as warning_list:
         parse_directory(["sample7_R2.fastq"])
         assert len(warning_list) == 1
-        assert "Orphaned paired read detected" in str(warning_list[0].message)
+        assert "Possible orphaned paired read detected for" in str(
+            warning_list[0].message
+        )
 
 
 def test_parse_tsv_file(create_sample_tsv, temp_directory):
     paired_reads, unpaired_reads = parse_tsv_file(create_sample_tsv)
     assert_parsed_files(paired_reads, unpaired_reads, temp_directory)
 
     # Assert file not found error for missing R1 file
     invalid_tsv_file = os.path.join(temp_directory, "invalid_reads.tsv")
-    with open(invalid_tsv_file, 'w') as f:
+    with open(invalid_tsv_file, "w") as f:
         f.write("sample1\tnonexistent_R1.fastq\t")
 
     with pytest.raises(FileNotFoundError):
         parse_tsv_file(str(invalid_tsv_file))
 
     # Assert file not found error for missing R2 file
     invalid_tsv_file = os.path.join(temp_directory, "invalid_reads.tsv")
-    with open(invalid_tsv_file, 'w') as f:
+    with open(invalid_tsv_file, "w") as f:
         f.write(
             "sample1\t"
             + os.path.join(str(temp_directory), "sample1_R1.fastq")
             + "\tnonexistent_R2.fastq"
         )
 
     with pytest.raises(FileNotFoundError):
@@ -152,71 +264,41 @@
         tsv_file.write(invalid_tsv_content)
 
     with pytest.raises(ValueError):
         parse_samples(invalid_tsv_file)
 
 
 def test_convert_to_dictionary():
-    paired_reads = {("sample1", "sample1_R1.fastq", "sample1_R2.fastq", None),
-                    ("sample2", "sample2_R1.fastq", "sample2_R2.fastq", "sample2_S.fastq")}
+    paired_reads = {
+        ("sample1", "sample1_R1.fastq", "sample1_R2.fastq", None),
+        ("sample2", "sample2_R1.fastq", "sample2_R2.fastq", "sample2_S.fastq"),
+    }
     unpaired_reads = {("sample3", "sample3_R1.fastq"), ("sample4", "sample4_R1.fastq")}
 
     expected_dictionary = {
         "sample1": {"R1": "sample1_R1.fastq", "R2": "sample1_R2.fastq", "S": None},
-        "sample2": {"R1": "sample2_R1.fastq", "R2": "sample2_R2.fastq", "S": "sample2_S.fastq"},
+        "sample2": {
+            "R1": "sample2_R1.fastq",
+            "R2": "sample2_R2.fastq",
+            "S": "sample2_S.fastq",
+        },
         "sample3": {"R1": "sample3_R1.fastq", "R2": None, "S": None},
         "sample4": {"R1": "sample4_R1.fastq", "R2": None, "S": None},
     }
 
     assert convert_to_dictionary(paired_reads, unpaired_reads) == expected_dictionary
 
 
 @pytest.mark.filterwarnings("ignore:Orphaned paired")
-def test_parse_samples_to_dictionary(temp_directory, create_sample_tsv):
-    # Test parsing a directory
-    directory_dictionary = {
-        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"),
-                    "R2": os.path.join(temp_directory, "sample1_R2.fastq"),
-                    "S": None},
-        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
-                    "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
-                    "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz")},
-        "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"),
-                    "R2": None,
-                    "S": None},
-        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"),
-                       "R2": None,
-                       "S": None},
-        "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"),
-                    "R2": None,
-                    "S": None},
-        "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"),
-                    "R2": None,
-                    "S": None},
-    }
-
-    assert parse_samples_to_dictionary(temp_directory) == directory_dictionary
-
-    # Test parsing a TSV file
-    tsv_dictionary = {
-        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"),
-                    "R2": os.path.join(temp_directory, "sample1_R2.fastq"),
-                    "S": None},
-        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
-                    "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
-                    "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz")},
-        "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"),
-                    "R2": None,
-                    "S": None},
-        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"), "R2": None, "S": None},
-        "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"), "R2": None, "S": None},
-        "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"), "R2": None, "S": None},
-    }
+def test_parse_samples_to_dictionary(
+    temp_directory, create_sample_tsv, expected_dictionary
+):
+    assert parse_samples_to_dictionary(temp_directory) == expected_dictionary
 
-    assert parse_samples_to_dictionary(create_sample_tsv) == tsv_dictionary
+    assert parse_samples_to_dictionary(create_sample_tsv) == expected_dictionary
 
     # Test parsing an invalid file or directory
     invalid_path = os.path.join(temp_directory, "nonexistent_file.tsv")
     with pytest.raises(ValueError):
         parse_samples_to_dictionary(invalid_path)
 
     invalid_path = os.path.join(temp_directory, "nonexistent_directory")
@@ -232,35 +314,51 @@
 
     with pytest.raises(ValueError):
         parse_samples_to_dictionary(invalid_tsv_file)
 
 
 def test_write_samples_tsv(temp_directory):
     samples_dictionary = {
-        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"), "R2": os.path.join(temp_directory, "sample1_R2.fastq")},
-        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
-                    "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
-                    "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz")},
+        "sample1": {
+            "R1": os.path.join(temp_directory, "sample1_R1.fastq"),
+            "R2": os.path.join(temp_directory, "sample1_R2.fastq"),
+        },
+        "sample2": {
+            "R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
+            "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
+            "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz"),
+        },
         "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"), "R2": None},
-        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"), "R2": None},
+        "sample4_R2": {
+            "R1": os.path.join(temp_directory, "sample4_R2.fastq"),
+            "R2": None,
+        },
         "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"), "R2": None},
         "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"), "R2": None},
     }
 
     output_file = os.path.join(temp_directory, "output.tsv")
     write_samples_tsv(samples_dictionary, output_file)
 
     with open(output_file, "r") as file:
         content = file.read()
 
     expected_content = (
-        "sample1\t" + os.path.join(temp_directory, "sample1_R1.fastq") + "\t" + os.path.join(temp_directory, "sample1_R2.fastq") + "\n"
-        "sample2\t" + os.path.join(temp_directory, "sample2_R1_001.fastq.gz") +
-        "\t" + os.path.join(temp_directory, "sample2_R2_001.fastq.gz") +
-        "\t" + os.path.join(temp_directory, "sample2_S_001.fastq.gz") + "\n"
+        "sample1\t"
+        + os.path.join(temp_directory, "sample1_R1.fastq")
+        + "\t"
+        + os.path.join(temp_directory, "sample1_R2.fastq")
+        + "\n"
+        "sample2\t"
+        + os.path.join(temp_directory, "sample2_R1_001.fastq.gz")
+        + "\t"
+        + os.path.join(temp_directory, "sample2_R2_001.fastq.gz")
+        + "\t"
+        + os.path.join(temp_directory, "sample2_S_001.fastq.gz")
+        + "\n"
         "sample3\t" + os.path.join(temp_directory, "sample3.fastq") + "\n"
         "sample4_R2\t" + os.path.join(temp_directory, "sample4_R2.fastq") + "\n"
         "sample5\t" + os.path.join(temp_directory, "sample5.fasta.gz") + "\n"
         "sample6\t" + os.path.join(temp_directory, "sample6.fastq.gz") + "\n"
     )
 
     assert content == expected_content
```


# Comparing `tmp/ai2_kit-0.5.5.tar.gz` & `tmp/ai2_kit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.5.5.tar", max compression
+gzip compressed data, was "ai2_kit-0.6.0.tar", max compression
```

## Comparing `ai2_kit-0.5.5.tar` & `ai2_kit-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.5/LICENSE
--rw-r--r--   0        0        0     2081 2023-07-26 13:52:05.868290 ai2_kit-0.5.5/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.5/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.5/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.5/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.5/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.5.5/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.5/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.5/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9721 2023-07-26 07:51:36.614431 ai2_kit-0.5.5/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2391 2023-07-26 09:20:42.973178 ai2_kit-0.5.5/ai2_kit/core/script.py
--rw-r--r--   0        0        0     6704 2023-07-27 04:45:11.760090 ai2_kit-0.5.5/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.5/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.5/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     1773 2023-07-28 10:17:35.722445 ai2_kit-0.5.5/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.5/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.5/ai2_kit/domain/data.py
--rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.5.5/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.5/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    17292 2023-07-27 01:48:54.442571 ai2_kit-0.5.5/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.5/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0    13433 2023-07-26 03:43:28.387903 ai2_kit-0.5.5/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      191 2023-07-31 01:35:39.925006 ai2_kit-0.5.5/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.5/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7678 2023-07-25 03:06:53.751626 ai2_kit-0.5.5/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.5/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.5/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-07-27 03:31:46.483603 ai2_kit-0.5.5/ai2_kit/tool/misc.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0    10063 2023-07-31 01:28:49.995095 ai2_kit-0.5.5/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.5/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      953 2023-07-31 02:15:55.574445 ai2_kit-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 ai2_kit-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2081 2023-07-26 13:52:05.868290 ai2_kit-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.6.0/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.6.0/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.6.0/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.6.0/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.6.0/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.6.0/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.6.0/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.6.0/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.6.0/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.6.0/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.6.0/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.6.0/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9721 2023-07-26 07:51:36.614431 ai2_kit-0.6.0/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.6.0/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2391 2023-07-26 09:20:42.973178 ai2_kit-0.6.0/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     7075 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.6.0/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.6.0/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     5525 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     4463 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6536 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     5454 2023-08-01 09:31:46.734548 ai2_kit-0.6.0/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.6.0/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.6.0/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    18826 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.6.0/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    13973 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      191 2023-07-31 01:35:39.925006 ai2_kit-0.6.0/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-08-01 08:44:50.875193 ai2_kit-0.6.0/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7678 2023-07-25 03:06:53.751626 ai2_kit-0.6.0/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.6.0/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.6.0/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0     2944 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-08-07 01:44:40.511630 ai2_kit-0.6.0/ai2_kit/tool/misc.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.6.0/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     9996 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9114 2023-08-09 01:43:32.676524 ai2_kit-0.6.0/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-08-09 01:49:24.796448 ai2_kit-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 ai2_kit-0.6.0/PKG-INFO
```

### Comparing `ai2_kit-0.5.5/LICENSE` & `ai2_kit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/README.md` & `ai2_kit-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.6.0/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/artifact.py` & `ai2_kit-0.6.0/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/checkpoint.py` & `ai2_kit-0.6.0/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/connector.py` & `ai2_kit-0.6.0/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/executor.py` & `ai2_kit-0.6.0/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/job.py` & `ai2_kit-0.6.0/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/queue_system.py` & `ai2_kit-0.6.0/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/resource_manager.py` & `ai2_kit-0.6.0/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/script.py` & `ai2_kit-0.6.0/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/core/util.py` & `ai2_kit-0.6.0/ai2_kit/core/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,26 +153,28 @@
     else:
         raise ValueError(f'Unknown node type {type(node)}')
 
 
 def __export_remote_functions():
     """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
 
-    def merge_dict(lo: dict, ro: dict, path=None):
+    def merge_dict(lo: dict, ro: dict, path=None, ignore_none=True):
         """
         Merge two dict, the left dict will be overridden.
         Note: list will be replaced instead of merged.
         """
         if path is None:
             path = []
         for key, value in ro.items():
+            if ignore_none and value is None:
+                continue
             if key in lo:
                 current_path = path + [str(key)]
                 if isinstance(lo[key], dict) and isinstance(value, dict):
-                    merge_dict(lo[key], value, current_path)
+                    merge_dict(lo[key], value, path=current_path, ignore_none=ignore_none)
                 else:
                     print('.'.join(current_path) + ' has been overridden')
                     lo[key] = value
             else:
                 lo[key] = value
         return lo
 
@@ -220,16 +222,23 @@
         [1, 4, 7, 2, 5, 8, 3, 6, 9]
         Ref: https://stackoverflow.com/questions/76751171/how-to-flat-a-list-of-lists-and-ensure-the-output-result-distributed-evenly-in-p
         """
         return [e for tup in zip_longest(*list_of_lists) for e in tup if e is not None]
 
 
     def dump_json(obj, path: str):
+        default = lambda o: f"<<non-serializable: {type(o).__qualname__}>>"
         with open(path, 'w', encoding='utf-8') as f:
-            json.dump(obj, f, indent=2)
+            json.dump(obj, f, indent=2, default=default)
+
+
+    def dump_text(text: str, path: str, **kwargs):
+        with open(path, 'w', **kwargs) as f:
+            f.write(text)
+
 
     def flush_stdio():
         import sys
         sys.stdout.flush()
         sys.stderr.flush()
 
 
@@ -239,22 +248,24 @@
         dict_nested_get,
         dict_nested_set,
         list_even_sample,
         list_random_sample,
         list_sample,
         flat_evenly,
         dump_json,
+        dump_text,
         flush_stdio,
     )
 
 
 (
     merge_dict,
     dict_nested_get,
     dict_nested_set,
     list_even_sample,
     list_random_sample,
     list_sample,
     flat_evenly,
     dump_json,
+    dump_text,
     flush_stdio,
 ) = __export_remote_functions()
```

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/asap.py` & `ai2_kit-0.6.0/ai2_kit/domain/asap.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,20 +97,21 @@
 
     def reduce_dimension(descriptors: np.ndarray, setting: dict):
         reducer = Dimension_Reducers(setting)
         reduced_descriptors = reducer.fit_transform(descriptors)
         return reduced_descriptors
 
 
-    def get_dbscan_trainer(descriptor: np.ndarray, metric='euclidean', eps=None, min_samples=2, eval_sample=50):
+    def get_dbscan_trainer(descriptors: np.ndarray, metric='euclidean', eps=None, min_samples=2, eval_sample=50):
         if eps is None:
-            n = len(descriptor)
-            sample = descriptor[np.random.choice(n, min(n, eval_sample), replace=False)]
+            n = len(descriptors)
+            samples = descriptors[np.random.choice(n, min(n, eval_sample), replace=False)]
             # FIXME: the method to estimate eps is strange
-            eps = np.percentile(cdist(sample, descriptor, metric), min(100 * 10. / n, 100))  # type: ignore
+            # FIXME: this will be broken when len of descriptors small
+            eps = np.percentile(cdist(samples, descriptors, metric), min(100 * 10. / n, 99))  # type: ignore
         return sklearn_DB(eps, min_samples, metrictype=metric)
 
 
     def get_laio_db_trainer(**kwargs):
         return LAIO_DB(**kwargs)
```

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/cp2k.py` & `ai2_kit-0.6.0/ai2_kit/domain/cp2k.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 
 from .data import DataFormat, ase_atoms_to_cp2k_input_data, artifacts_to_ase_atoms
 from .iface import ICllLabelOutput, BaseCllContext
 from .util import loads_cp2k_input, load_cp2k_input, dump_cp2k_input
 
 logger = get_logger(__name__)
 
+
 class CllCp2kInputConfig(BaseModel):
     init_system_files: List[str] = []
-    input_template: Union[dict, str]
+    input_template: Union[dict, str] = dict()
     """
     Input template for cp2k. Could be a dict or content of a cp2k input file.
     """
     limit: int = 50
     """
     Limit of the number of systems to be labeled.
     """
     limit_method: Literal["even", "random", "truncate"] = "even"
 
+
 class CllCp2kContextConfig(BaseModel):
     script_template: BashTemplate
     cp2k_cmd: str = 'cp2k'
     post_cp2k_cmd: Optional[str] = None
     concurrency: int = 5
 
 
@@ -140,28 +142,27 @@
 
         task_dirs = []
         atoms_list: List[Tuple[ArtifactDict, Atoms]] = artifacts_to_ase_atoms(system_files, type_map=type_map)
 
         if limit > 0:
             atoms_list = list_sample(atoms_list, limit, method=sample_method)
 
-        for i, (file, atoms) in enumerate(atoms_list):
+        for i, (data_file, atoms) in enumerate(atoms_list):
             # create task dir
             task_dir = os.path.join(base_dir, f'{str(i).zfill(6)}')
             os.makedirs(task_dir, exist_ok=True)
 
-            # TODO: should also support input_template
-            # find input template in data_file attrs, if not found, use input_template as default
-            input_data_file = dict_nested_get(file, ['attrs', 'cp2k', 'input_template_file'],  None)  # type: ignore
-            if isinstance(input_data_file, str):
-                with open(input_data_file, 'r') as f:
-                    input_data = load_cp2k_input(f)
-            else:
-                input_data = copy.deepcopy(input_template)
+            overridable_params: dict = dict_nested_get(data_file, ['attrs', 'cp2k'], dict())  # type: ignore
+            input_template = overridable_params.get('input_template', input_template)
+
+            if input_template is str:
+                input_template = loads_cp2k_input(input_template)
+            assert input_template is not None, 'input_template is not found'
 
+            input_data = copy.deepcopy(input_template)
             coords, cell = ase_atoms_to_cp2k_input_data(atoms)
             merge_dict(input_data, {
                 'FORCE_EVAL': {
                     'SUBSYS': {
                         # FIXME: this is a dirty hack, we should make dump_cp2k_input support COORD
                         'COORD': dict.fromkeys(coords, ''),
                         'CELL': {
@@ -173,15 +174,15 @@
                 }
             })
             with open(os.path.join(task_dir, input_file_name), 'w') as f:
                 dump_cp2k_input(input_data, f)
 
             task_dirs.append({
                 'url': task_dir,
-                'attrs': file['attrs'],
+                'attrs': data_file['attrs'],
             })
 
         return task_dirs
 
     return (
         make_cp2k_task_dirs,
     )
```

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/data.py` & `ai2_kit-0.6.0/ai2_kit/domain/data.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/deepmd.py` & `ai2_kit-0.6.0/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/iface.py` & `ai2_kit-0.6.0/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/lammps.py` & `ai2_kit-0.6.0/ai2_kit/domain/lammps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,154 @@
 from ai2_kit.core.script import BashTemplate, BashStep, BashScript
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.job import gather_jobs
-from ai2_kit.core.util import list_split, dict_nested_get
+from ai2_kit.core.util import list_split, dict_nested_get, dump_json, dump_text
 
 from typing import List, Literal, Optional, Mapping, Sequence, Any
-from pydantic import BaseModel
+from pydantic import BaseModel, validator, root_validator
 from dataclasses import dataclass
 from string import Template
 from allpairspy import AllPairs
+from collections import defaultdict
+
 import os
 import itertools
 import random
+import ase.io
 
 
 from .iface import BaseCllContext, ICllExploreOutput
 from .constant import (
-    MODEL_DEVI_OUT,
-    MODEL_DEVI_NEU_OUT,
-    MODEL_DEVI_RED_OUT,
-    LAMMPS_TRAJ_DIR,
-    LAMMPS_TRAJ_SUFFIX,
+    LAMMPS_DUMP_DIR,
+    LAMMPS_DUMP_SUFFIX,
+    PRESET_LAMMPS_INPUT_TEMPLATE,
 )
-from .data import convert_to_lammps_input_data, DataFormat
+from .data import DataFormat, artifacts_to_ase_atoms
 
 logger = get_logger(__name__)
 
 
-class ExploreVariants(BaseModel):
-    temp: List[float]
-    """Temperatures variants."""
-    pres: List[float]
-    """Pressures variants."""
-    others: Mapping[str, Sequence[Any]] = dict()
-    """
-    Other variants to be combined with.
-    The key is the name of the variant, and the value is the list of values.
-    For example, if you want to combine the variant 'LAMBDA' with values [0.0, 0.5, 1.0],
-    you can set the others field to {'LAMBDA': [0.0, 0.5, 1.0]}.
-    And in LAMMPS input template, you can use the variable ${LAMBDA} and v_LAMBDA to access the value.
-    """
-
-
 class CllLammpsInputConfig(BaseModel):
-    explore_vars: ExploreVariants
-    """Variants to be explored."""
-
     n_wise: int = 0
-    """The way of combining variants.
-    0 means cartesian product, 2 means 2-wise, etc.
-    If n_wise is less than 2 or greater than total fields,
-    the full combination will be used.
+    """
+    The way of combining variants.
+    if n_wise is less than 2 or greater than total fields, the full combination will be used.
+    Or else, the n_wise combination will be used.
     It is strongly recommended to use n_wise when the full combination is too large.
     """
-    system_files: List[str]
-    """Artifacts of initial system data."""
+
+    explore_vars: Mapping[str, List[Any]]
+    """
+    Variants to be explored.
+    Variables defined here will become **LAMMPS variables**.
+    If multiple value has been set for a variable,
+    the cartesian product will be used to generate the combination.
+    For example,
+
+    ```yaml
+    TEMP: [330, 430, 530]  # Can be a scalar, e.g. 330
+    PRES: 1                # Can be a vector, e.g. [1, 2, 3]
+    LAMBDA_f: [0.0, 0.25, 0.5, 0.75, 1.0]
+    ```
+    Then you can reference them in the LAMMPS input template as ${TEMP}, ${LAMBDA_f}, ${N_STEPS}, etc.
+    """
+    preset_template: Optional[str] = None
+    """
+    Name of the preset template.
+    """
+    input_template: Optional[str] = None
+    """
+    LAMMPS input template file content.
+    If set, the preset_template will be ignored.
+    """
+    template_vars: Mapping[str, Any] = dict()
+    """
+    input_template may provide extra injection points for user to inject custom settings.
+    Those value could be set here.
+    """
+
     plumed_config: Optional[str]
     """Plumed config file content."""
-    plumed_config_file: Optional[str]
-    """Plumed config file path."""
 
-    # ensemble specific params
-    tau_t: float = 0.1
-    tau_p: float = 0.5
-    time_const: float = 0.1
+    system_files: List[str]
+    """
+    Artifacts key of lammps input data
+    """
     ensemble: Literal['nvt', 'nvt-i', 'nvt-a', 'nvt-iso', 'nvt-aniso', 'npt', 'npt-t', 'npt-tri', 'nve', 'csvr']
-
     no_pbc: bool = False
-    timestep: float = 0.0005
-    sample_freq: int
     nsteps: int
+    timestep: float = 0.0005
+    sample_freq: int = 100
+    mode: Literal['default', 'fep'] = 'default'
 
-    """Ensemble to be used.
-    nvt means constant volume and temperature.
-    nvt-i means constant volume and temperature, with isotropic scaling.
-    nvt-a means constant volume and temperature, with anisotropic scaling.
-    nvt-iso means constant volume and temperature, with isotropic scaling.
-    npt means constant pressure and temperature.
-    npt-t means constant pressure and temperature, with isotropic scaling.
-    npt-tri means constant pressure and temperature, with anisotropic scaling.
-    nve means constant energy.
-    """
-
-    input_template: Optional[str]
-    """Lammps input template file content."""
-
-    post_variables_section: str = ''
-    post_init_section: str = ''
-    post_read_data_section: str = ''
-    post_force_field_section: str = ''
-    post_md_section: str = ''
-    post_run_section: str = ''
+
+    type_alias: Mapping[str, List[str]] = dict()
+    '''
+    Type alias for atoms. For example, if you want to distinguish ghost H and H of HF molecule from other H atoms,
+    you can define the alias as follows:
+    ```yaml
+    type_alias:
+        H: [ H_ghost, H_hf ]
+    ```
+    And then you can reference them in the LAMMPS input template, for example
+    ```
+    set atom 1 type ${H_hf}
+    set atom 2 type ${H_ghost}
+    ```
+    '''
+
+    @validator('explore_vars', pre=True)
+    @classmethod
+    def validate_explore_variants(cls, value):
+        if not isinstance(value, dict):
+            raise ValueError('explore_vars must be a dict')
+        for k in ['TEMP', 'PRES']:
+            if k not in value:
+                raise ValueError(f'{k} must be set in explore_variants')
+        # override default values
+        value = {
+            'TAU_T': 0.1,
+            'TAU_P': 0.5,
+            'TIME_CONST': 0.1,
+            **value,
+        }
+        result = {}
+        for k, v in value.items():
+            if not isinstance(v, list):
+                v = [v]
+            result[k] = v
+        return result
+
+    @root_validator()
+    @classmethod
+    def validate_domain(cls, values):
+        ensemble = values.get('ensemble')
+        no_pbc = values.get('no_pbc')
+        if ensemble.startswith('npt') and no_pbc:
+            raise ValueError('ensemble npt conflict with no_pcb')
+        if not ensemble.startswith('npt'):
+            logger.info('ensemble is not npt, force PRES to -1')
+            values['explore_vars']['PRES'] = [-1]
+        return values
 
 
 class CllLammpsContextConfig(BaseModel):
     script_template: BashTemplate
     lammps_cmd: str = 'lmp'
     concurrency: int = 5
 
 
 @dataclass
 class CllLammpsInput:
-
-    @dataclass
-    class MdOptions:
-        models: List[Artifact]
-
-    @dataclass
-    class FepOptions:
-        red_models: List[Artifact]
-        neu_models: List[Artifact]
-
     config: CllLammpsInputConfig
     type_map: List[str]
     mass_map: List[float]
-
-    # The following options are mutex
-    md_options: Optional[MdOptions] = None
-    fep_options: Optional[FepOptions] = None
+    dp_models: Mapping[str, List[Artifact]]
+    preset_template: str
 
 
 @dataclass
 class CllLammpsContext(BaseCllContext):
     config: CllLammpsContextConfig
 
 
@@ -131,130 +158,46 @@
 
     def get_model_devi_dataset(self) -> List[Artifact]:
         return self.model_devi_outputs
 
 
 async def cll_lammps(input: CllLammpsInput, ctx: CllLammpsContext):
     executor = ctx.resource_manager.default_executor
-
-    # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
-    input_data_dir, tasks_dir = executor.setup_workspace(work_dir, ['input_data', 'tasks'])
-    systems = ctx.resource_manager.resolve_artifacts(input.config.system_files)
+    data_files = ctx.resource_manager.resolve_artifacts(input.config.system_files)
+    assert len(data_files) > 0, 'no data files found'
 
-    # TODO: the whole process to generate task dirs should be run remotely
-    # Reference: lasp.py
-    input_data_files: List[ArtifactDict] = executor.run_python_fn(convert_to_lammps_input_data)(
-        systems=[a.to_dict() for a in systems],
-        base_dir=input_data_dir,
+    tasks_dir, task_dirs = executor.run_python_fn(make_lammps_task_dirs)(
+        combination_vars=input.config.explore_vars,
+        data_files=[a.to_dict() for a in data_files],
+        dp_models={k: [m.url for m in v] for k, v in input.dp_models.items()},
+        n_steps=input.config.nsteps,
+        timestep=input.config.timestep,
+        sample_freq=input.config.sample_freq,
+        no_pbc=input.config.no_pbc,
+        n_wise=input.config.n_wise,
+        ensemble=input.config.ensemble,
+        preset_template=input.config.preset_template or input.preset_template,
+        input_template=input.config.input_template,
+        plumed_config=input.config.plumed_config,
+        extra_template_vars=input.config.template_vars,
         type_map=input.type_map,
+        mass_map=input.mass_map,
+        type_alias=input.config.type_alias,
+        work_dir=work_dir,
     )
 
-    combination_fields: List[str] = [
-        'data_file',
-        'temp',
-        'pres'
-    ]
-    combination_values: Sequence[Sequence[Any]] = [
-        input_data_files,
-        input.config.explore_vars.temp,
-        input.config.explore_vars.pres,
-    ]
-
-    for k, v in input.config.explore_vars.others.items():
-        combination_fields.append(k)
-        combination_values.append(v)  # type: ignore
-
-    if 1 < input.config.n_wise <= len(combination_fields):
-        logger.info('using %d-wise combination', input.config.n_wise)
-        combinations = AllPairs(combination_values, n=input.config.n_wise)
-    else:
-        logger.info('using full combination')
-        combinations = itertools.product(*combination_values)
-
-    lammps_task_dirs: List[ArtifactDict] = []
-    lammps_input_file_name = 'lammps.input'
-
-    for i, combination in enumerate(combinations):
-        data_file: ArtifactDict = combination[0]
-        temp, pres = combination[1:3]
-        others_dict = dict(zip(combination_fields[3:], combination[3:]))
-        lammps_task_dir = os.path.join(tasks_dir, f'{i:06d}')
-        executor.mkdir(os.path.join(lammps_task_dir, LAMMPS_TRAJ_DIR))  # create dump directory for lammps or else will get error
-
-        if input.md_options:
-            force_field_section = make_md_force_field_section(
-                models=[a.url for a in input.md_options.models],
-            )
-        elif input.fep_options:
-            if 'LAMBDA_f' not in others_dict:
-                raise ValueError('LAMBDA_f must be set when using FEP mode!')
-            # inject the following variables for FEP mode
-            others_dict['LAMBDA_i'] = '1-v_LAMBDA_f' # should not have space, or you must quote
-            others_dict['plus'] = 1
-            others_dict['minus'] = -1
-            force_field_section = make_fep_force_field_section(
-                neu_models=[a.url for a in input.fep_options.neu_models],
-                red_models=[a.url for a in input.fep_options.red_models],
-            )
-        else:
-            raise ValueError('one and only one of md_options or fep_options must be set')
-
-        # Config plumed if either plumed_config_file or plumed_config is set.
-        # The plumed config can be set in both workflow config and input data file.
-        # The config in input data file has higher priority.
-        plumed_config_file = dict_nested_get(data_file, ['attrs', 'lammps', 'plumed_config_file'],
-                                             input.config.plumed_config_file)
-        plumed_config = dict_nested_get(data_file, ['attrs', 'lammps', 'plumed_config'],
-                                        input.config.plumed_config)
-        if plumed_config_file is None and isinstance(plumed_config, str):
-            plumed_config_file = 'plumed.input'
-            plumed_file_path = os.path.join(lammps_task_dir, plumed_config_file)
-            logger.info(f'found plumed config, generate {plumed_file_path}')
-            executor.dump_text(plumed_config, plumed_file_path)
-
-        template = input.config.input_template or  DEFAULT_LAMMPS_INPUT_TEMPLATE
-        input_text = make_lammps_input(data_file=data_file['url'],
-                                       nsteps=input.config.nsteps,
-                                       timestep=input.config.timestep,
-                                       trj_freq=input.config.sample_freq,
-                                       temp=temp,
-                                       pres=pres,
-                                       tau_t=input.config.tau_t,
-                                       tau_p=input.config.tau_p,
-                                       time_const=input.config.time_const,
-                                       ensemble=input.config.ensemble,
-                                       mass_map=input.mass_map,
-                                       others_dict=others_dict,
-                                       force_field_section=force_field_section,
-                                       template=template,
-                                       post_variables_section=input.config.post_variables_section,
-                                       post_init_section=input.config.post_init_section,
-                                       post_read_data_section=input.config.post_read_data_section,
-                                       post_force_field_section=input.config.post_force_field_section,
-                                       post_md_section=input.config.post_md_section,
-                                       post_run_section=input.config.post_run_section,
-                                       plumed_config_file=plumed_config_file,  # type: ignore
-                                       no_pbc=False,
-                                       rand_start=1_000_000)
-        input_file_path = os.path.join(lammps_task_dir, lammps_input_file_name)
-        logger.info(f'generate lammps config {input_file_path}')
-
-        executor.dump_text(input_text, input_file_path)
-        lammps_task_dirs.append({'url': lammps_task_dir, 'attrs': data_file['attrs']})  # type: ignore
-
     # build scripts and submit
-    lammps_cmd = ctx.config.lammps_cmd
-    base_cmd = f'{lammps_cmd} -i {lammps_input_file_name}'
+    base_cmd = f'{ctx.config.lammps_cmd} -i lammps.input'
     cmd = f'''if [ -f md.restart.* ]; then {base_cmd} -v restart 1; else {base_cmd} -v restart 0; fi'''
 
     # generate steps
     steps = []
-    for lammps_task_dir in lammps_task_dirs:
-        steps.append(BashStep(cwd=lammps_task_dir['url'], cmd=cmd, checkpoint='lammps'))
+    for task_dir in task_dirs:
+        steps.append(BashStep(cwd=task_dir['url'], cmd=cmd, checkpoint='lammps'))
 
     # submit jobs by the number of concurrency
     jobs = []
     for i, steps_group in enumerate(list_split(steps, ctx.config.concurrency)):
         if not steps_group:
             continue
         script = BashScript(
@@ -263,206 +206,275 @@
         )
         job = executor.submit(script.render(), cwd=tasks_dir,
                               checkpoint_key=f'queue-job/lammps/{i}:{tasks_dir}')
         jobs.append(job)
 
     await gather_jobs(jobs, max_tries=2)
 
-    outputs = [
-        Artifact.of(
-            url=task_dir['url'],
-            executor=executor.name,
-            format=DataFormat.LAMMPS_OUTPUT_DIR,
-            attrs=task_dir['attrs'],
-        ) for task_dir in lammps_task_dirs]  # type: ignore
+    # build outputs
+    outputs = []
+    for task_dir in task_dirs:
+        common = dict(url=task_dir['url'], executor=executor.name, format=DataFormat.LAMMPS_OUTPUT_DIR)
+        # TODO: a more generic way to dealing multiple model_devi outputs
+        if input.config.mode == 'fep':
+            outputs += [
+                Artifact.of(**common, attrs={
+                    **task_dir['attrs'], 'model_devi_file': 'model_devi_ini.out', 'lammps_dump_dir': 'traj-ini',
+                    **task_dir['attrs']['fep-ini'],
+                }),
+                Artifact.of(**common, attrs={
+                    **task_dir['attrs'], 'model_devi_file': 'model_devi_fin.out', 'lammps_dump_dir': 'traj-fin',
+                    **task_dir['attrs']['fep-fin'],
+                    'ancestor': task_dir['attrs']['ancestor'] + '-fin',  # only fin needs
+                }),
+            ]
+        else:
+            outputs += [
+                Artifact.of(**common, attrs={ **task_dir['attrs'] }),
+            ]
 
     return GenericLammpsOutput(model_devi_outputs=outputs)
 
 
-def make_md_force_field_section(models: List[str]):
-    deepmd_args = ""
-    settings = [
-        'pair_style deepmd %s out_freq ${THERMO_FREQ} out_file %s %s' % (' '.join(models), MODEL_DEVI_OUT, deepmd_args),
-        'pair_coeff * *',
-    ]
-    return settings
-
-
-def make_fep_force_field_section(neu_models: List[str], red_models: List[str]):
-    deepmd_args = ""
-    settings = [
-        'pair_style hybrid/overlay &',
-        '           deepmd %s out_freq ${THERMO_FREQ} out_file %s %s &' %(' '.join(neu_models), MODEL_DEVI_NEU_OUT, deepmd_args),
-        '           deepmd %s out_freq ${THERMO_FREQ} out_file %s %s'   %(' '.join(red_models), MODEL_DEVI_RED_OUT, deepmd_args),
-        'pair_coeff  * * deepmd 1 *',
-        'pair_coeff  * * deepmd 2 *',
-        '',
-        'fix sampling_PES all adapt 0 &',
-        '    pair deepmd:1 scale * * v_LAMBDA_f &',
-        '    pair deepmd:2 scale * * v_LAMBDA_i &',
-        '    scale yes',
-    ]
-    return settings
-
-
-def make_lammps_input(data_file: str,
-                      nsteps: int,
-                      timestep: float,
-                      trj_freq: int,
-                      temp: float,
-                      pres: float,
-                      tau_t: float,
-                      tau_p: float,
-                      ensemble: str,
-                      mass_map: List[float],
-                      others_dict: Mapping[str, Any],
-
-                      template: str,
-                      post_variables_section: str,
-                      post_init_section: str,
-                      post_read_data_section: str,
-                      post_force_field_section: str,
-                      post_md_section: str,
-                      post_run_section: str,
-
-                      force_field_section: List[str],
-                      plumed_config_file: Optional[str] = None,
-                      time_const = 0.1,
-                      no_pbc=False,
-                      rand_start=1_000_000,
-                      ):
-
-    # FIXME: I am not sure if it is a good idea to fix it automatically
-    # maybe we should consider raise an error here
-    if not ensemble.startswith('npt'):
-        pres = -1
-
-    variables = [
-        '# required variables',
-        'variable NSTEPS      equal %d' % nsteps,
-        'variable THERMO_FREQ equal %d' % trj_freq,
-        'variable DUMP_FREQ   equal %d' % trj_freq,
-        'variable TEMP        equal %f' % temp,
-        'variable PRES        equal %f' % pres,
-        'variable TAU_T       equal %f' % tau_t,
-        'variable TAU_P       equal %f' % tau_p,
-        'variable TIME_CONST  equal %f' % time_const,
-        '',
-        '# custom variables (if any)',
-    ]
-
-    for k, v in others_dict.items():
-        variables.append(f'variable {k} equal {v}')
-
-    init_section = [
-        'boundary ' + ('f f f' if no_pbc else 'p p p'),
-    ]
-
-    read_data_section = [
-        '''if "${restart} > 0" then "read_restart md.restart.*" else "read_data %s"''' % data_file,
-        *("mass {id} {mass}".format(id=i+1, mass=m) for i, m in enumerate(mass_map))
-    ]
-
-    md_section = [
-        '''if "${restart} == 0" then "velocity all create ${TEMP} %d"''' % (random.randrange(rand_start - 1) + 1)
-    ]
-
-    if ensemble.startswith('npt') and no_pbc:
-        raise ValueError('ensemble npt conflict with no_pcb')
-    if ensemble in ('npt', 'npt-i', 'npt-iso',):
-        md_section.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} iso ${PRES} ${PRES} ${TAU_P}')
-    elif ensemble in ('npt-a', 'npt-aniso',):
-        md_section.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} aniso ${PRES} ${PRES} ${TAU_P}')
-    elif ensemble in ('npt-t', 'npt-tri',):
-        md_section.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} tri ${PRES} ${PRES} ${TAU_P}')
-    elif ensemble in ('nvt',):
-        md_section.append('fix 1 all nvt temp ${TEMP} ${TEMP} ${TAU_T}')
-    elif ensemble in ('nve',):
-        md_section.append('fix 1 all nve')
-    elif ensemble in ('csvr',):
-        md_section.append('fix 1 all nve')
-        md_section.append('fix 2 all temp/csvr ${TEMP} ${TEMP} ${TIME_CONST} %d' % (random.randrange(rand_start - 1) + 1))
-    else:
-        raise ValueError('unknown ensemble: ' + ensemble)
-
-    if plumed_config_file:
-        md_section.append(f'fix dpgen_plm all plumed plumedfile {plumed_config_file} outfile plumed.out')
-
-    if no_pbc:
-        md_section.extend([
-            'velocity all zero linear',
-            'fix      fm all momentum 1 linear 1 1 1',
-        ])
-
-    md_section.extend([
-        'thermo_style custom step temp pe ke etotal press vol lx ly lz xy xz yz',
-        'thermo       ${THERMO_FREQ}',
-        'dump         1 all custom ${DUMP_FREQ} %s/*%s id type x y z fx fy fz' % (LAMMPS_TRAJ_DIR, LAMMPS_TRAJ_SUFFIX),
-        'restart      10000 md.restart',
-    ])
-
-    run_section = [
-        'timestep %f' % timestep,
-        'run      ${NSTEPS} upto',
-    ]
-
-    return LammpsInputTemplate(template).substitute(dict(
-        variables_section='\n'.join(variables),
-        post_variables_section=post_variables_section,
-
-        init_section='\n'.join(init_section),
-        post_init_section=post_init_section,
-
-        read_data_section='\n'.join(read_data_section),
-        post_read_data_section=post_read_data_section,
-
-        md_section='\n'.join(md_section),
-        post_md_section=post_md_section,
-
-        force_field_section='\n'.join(force_field_section),
-        post_force_field_section=post_force_field_section,
-
-        run_section='\n'.join(run_section),
-        post_run_section=post_run_section,
-    ))
-
-
-class LammpsInputTemplate(Template):
-    """
-    change delimiter from $ to $$ as $ is used a lot in lammps input file
-    """
-    delimiter = '$$'
-
-
-DEFAULT_LAMMPS_INPUT_TEMPLATE = '''\
-## variables_section
-$$variables_section
-## post_variables_section
-$$post_variables_section
-
-## init_section
-units      metal
-atom_style atomic
-$$init_section
-## post_init_section
-$$post_init_section
-
-## read_data_section
-$$read_data_section
-## post_read_data_section
-$$post_read_data_section
-
-## force_field_section
-$$force_field_section
-## post_force_field_section
-$$post_force_field_section
-
-## md_section
-$$md_section
-## post_md_section
-$$post_md_section
-
-## run_section
-$$run_section
-## post_run_section
-$$post_run_section
-'''
+def __export_remote_functions():
+
+    class LammpsInputTemplate(Template):
+        delimiter = '$$'
+
+    def make_lammps_task_dirs(combination_vars: Mapping[str, Sequence[Any]],
+                              data_files: List[ArtifactDict],
+                              dp_models: Mapping[str, List[str]],
+                              n_steps: int,
+                              timestep: float,
+                              sample_freq: float,
+                              no_pbc: bool,
+                              n_wise: int,
+                              ensemble: str,
+                              preset_template: str,
+                              input_template: Optional[str],
+                              plumed_config: Optional[str],
+                              extra_template_vars: Mapping[str, Any],
+                              type_map: List[str],
+                              mass_map: List[float],
+                              type_alias: Mapping[str, List[str]],
+                              work_dir: str,
+                              ):
+        # setup workspace
+        input_data_dir = os.path.join(work_dir, 'input_data')
+        tasks_dir = os.path.join(work_dir, 'tasks')
+        for path in (input_data_dir, tasks_dir):
+            os.makedirs(path, exist_ok=True)
+
+        # create data files
+        input_dataset = []
+        atoms_list = artifacts_to_ase_atoms(data_files, type_map=type_map)
+        for i, (artifact, atoms) in enumerate(atoms_list):
+            #  create data file
+            data_file = os.path.join(input_data_dir, f'{i:06d}.lammps.data')
+            ase.io.write(data_file, atoms, format='lammps-data', specorder=type_map)  # type: ignore
+            input_dataset.append({
+                'url': data_file,
+                'attrs': artifact['attrs'],
+            })
+
+        # generate combinations of variants
+        combination_fields: List[str] = ['DATA_FILE']
+        combination_values: List[List[Any]] = [input_dataset]
+        for k, v in combination_vars.items():
+            combination_fields.append(k)
+            combination_values.append(v)  # type: ignore
+        if 1 < n_wise <= len(combination_fields):
+            logger.info(f'using {n_wise}-wise combination')
+            combinations = AllPairs(combination_values, n=n_wise)
+        else:
+            logger.info('using full combination')
+            combinations = itertools.product(*combination_values)
+
+        # generate tasks input
+        task_dirs = []
+        for i, combination in enumerate(combinations):
+            template_vars = {}
+            lammps_vars = dict(zip(combination_fields, combination))
+
+            # setup task dir
+            task_dir = os.path.join(tasks_dir, f'{i:06d}')
+            os.makedirs(os.path.join(task_dir, LAMMPS_DUMP_DIR), exist_ok=True)
+
+            data_file = lammps_vars.pop('DATA_FILE')
+
+            # override default values with data file attrs
+            overridable_params: dict = dict_nested_get(data_file, ['attrs', 'lammps'], dict())  # type: ignore
+            plumed_config = overridable_params.get('plumed_config', plumed_config)
+            type_alias = overridable_params.get('type_alias', type_alias)
+            extra_template_vars = {**extra_template_vars, **overridable_params.get('template_vars', dict())}
+
+            # build type map and type order
+            type_to_mass = dict(zip(type_map, mass_map))
+
+            ext_type_map = []
+            ext_type_map_to_origin = []
+            ext_mass_map = []
+            ghost_loc = []  # location of ghost atom type
+            DP_GHOST = len(type_map)
+
+            for origin_type, alias in type_alias.items():
+                for t in alias:
+                    if 'ghost' in t:  # atom type with 'ghost' in its name is considered as ghost atom type
+                        ghost_loc.append(DP_GHOST)
+
+                    ext_type_map.append(t)
+                    ext_type_map_to_origin.append(origin_type)
+                    ext_mass_map.append(type_to_mass[origin_type])
+
+            # SPECORDER is used to specify the order of types in the lammps data file
+            # For example, if the complete type_map is [H, O, O_1, O_2, H_1, H_2],
+            # then the specorder should be [H, O, O, O, H, H]
+            specorder = type_map + ext_type_map_to_origin
+
+            # *_type_order is use to remap the lammps atom type to dp atom type
+            # For example, if the full_type_map is     [H, O, O_1, O_2, H_1, H_2],
+            # then the fep_ini_type_order should be    [0, 1, 1  , 1,   0  , 0]
+            fep_ini_type_order = [ type_map.index(t) for t in specorder]
+            # fep_fin_type_order is the same as fep_ini_type_order, except that the ghost atom type should be len(type_map)
+            fep_fin_type_order = fep_ini_type_order.copy()
+            for loc in ghost_loc:
+                fep_fin_type_order[loc] = DP_GHOST
+
+            template_vars['SPECORDER'] = specorder
+            template_vars['DP_DEFAULT_TYPE_ORDER'] = ' '.join(map(str, range(len(type_map))))
+            template_vars['DP_FEP_INI_TYPE_ORDER'] = ' '.join(map(str, fep_ini_type_order))
+            template_vars['DP_FEP_FIN_TYPE_ORDER'] = ' '.join(map(str, fep_fin_type_order))
+
+            template_vars['MASS_MAP_FULL'] = _get_masses(type_map + ext_type_map, mass_map + ext_mass_map)
+            template_vars['MASS_MAP'] =  template_vars['MASS_MAP_FULL']
+            template_vars['MASS_MAP_BASE'] = _get_masses(type_map, mass_map)
+
+            ## build variables section
+            lammps_vars['DATA_FILE'] = data_file['url']
+            lammps_vars['N_STEPS'] = n_steps
+            lammps_vars['THERMO_FREQ'] = sample_freq
+            lammps_vars['DUMP_FREQ'] = sample_freq
+            lammps_vars['SAMPLE_FREQ'] = sample_freq
+
+            dump_json(lammps_vars, os.path.join(task_dir, 'debug.lammps_vars.json'))  # for debug
+            template_vars['VARIABLES'] = _get_lammps_variables(lammps_vars)
+            ## build init settings
+            template_vars['INITIALIZE'] =  '\n'.join([
+                'units           metal',
+                'atom_style      atomic',
+                'boundary ' + ('f f f' if no_pbc else 'p p p'),
+            ])
+            ## build read data section
+            template_vars['READ_DATA'] = (
+                '''if "${restart} > 0" '''
+                '''then "read_restart md.restart.*" '''
+                '''else "read_data ${DATA_FILE} extra/atom/types %s"''' % (len(ext_type_map))
+            )
+
+            ## build simulation
+            simulation = [
+                '''if "${restart} == 0" then "velocity all create ${TEMP} %d"''' % (random.randrange(10^6 - 1) + 1),
+                _get_ensemble(ensemble),
+            ]
+
+            if plumed_config:
+                plumed_config_file = os.path.join(task_dir, 'plumed.input')
+                dump_text(plumed_config, plumed_config_file)
+                simulation.append(f'fix cll_plumed all plumed plumedfile {plumed_config_file} outfile plumed.out')
+
+            if no_pbc:
+                simulation.extend([
+                    'velocity all zero linear',
+                    'fix      fm all momentum 1 linear 1 1 1',
+                ])
+            simulation.extend([
+                'thermo_style custom step temp pe ke etotal press vol lx ly lz xy xz yz',
+                'thermo       ${THERMO_FREQ}',
+                'dump         1 all custom ${DUMP_FREQ} %s/*%s id type x y z fx fy fz' % (LAMMPS_DUMP_DIR, LAMMPS_DUMP_SUFFIX),
+                'restart      10000 md.restart',
+            ])
+            template_vars['SIMULATION'] = '\n'.join(simulation)
+            ## build run section
+            template_vars['RUN'] = '\n'.join([
+                'timestep %f' % timestep,
+                'run      ${N_STEPS} upto',
+            ])
+
+            dp_models_vars = _get_dp_models_variables(dp_models)
+
+            template_vars = {**template_vars, **dp_models_vars, **extra_template_vars}
+            dump_json(template_vars, os.path.join(task_dir, 'debug.template_vars.json'))  # for debug
+
+            input_template = PRESET_LAMMPS_INPUT_TEMPLATE[preset_template] if input_template is None else input_template
+            dump_text(input_template, os.path.join(task_dir, 'debug.input_template.txt'))  # for debug
+            lammps_input = LammpsInputTemplate(input_template).substitute(defaultdict(str),**template_vars)
+            dump_text(lammps_input, os.path.join(task_dir, 'lammps.input'))
+
+            task_dirs.append({'url': task_dir, 'attrs': data_file['attrs']})  # type: ignore
+        return tasks_dir, task_dirs
+
+
+    def _get_type_map_vars(type_map: List[str]):
+        return dict(zip(type_map, range(1, len(type_map) + 1)))
+
+
+    def _get_masses(type_map: List[str], mass_map: List[float]):
+        lines = [
+            _get_lammps_variables(_get_type_map_vars(type_map)),
+            '',
+        ]
+        for t, m in zip(type_map, mass_map):
+            lines.append(f'mass ${{{t}}} {m}')
+        return '\n'.join(lines)
+
+
+    def _get_dp_models_variables(models: Mapping[str, List[str]]):
+        vars = {}
+        for k, v in models.items():
+            prefix = 'DP_MODELS' if k == '' else f'DP_{k}_MODELS'
+            vars[prefix] = ' '.join(v)
+            for i, m in enumerate(v):
+                vars[f'{prefix}_{i}'] = m
+        return vars
+
+
+    def _get_lammps_variables(vars: Mapping[str, Any]):
+        lines = []
+        for k, v in vars.items():
+            if isinstance(v, str):
+                # TODO: should escape `v` in case of special characters
+                line = f'variable    {k:16} string "{v}"'
+            else:
+                line = f'variable    {k:16} equal {v}'
+            lines.append(line)
+        return '\n'.join(lines)
+
+
+    def _get_ensemble(ensemble: str):
+        lines = []
+        if ensemble in ('npt', 'npt-i', 'npt-iso',):
+            lines.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} iso ${PRES} ${PRES} ${TAU_P}')
+        elif ensemble in ('npt-a', 'npt-aniso',):
+            lines.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} aniso ${PRES} ${PRES} ${TAU_P}')
+        elif ensemble in ('npt-t', 'npt-tri',):
+            lines.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} tri ${PRES} ${PRES} ${TAU_P}')
+        elif ensemble in ('nvt',):
+            lines.append('fix 1 all nvt temp ${TEMP} ${TEMP} ${TAU_T}')
+        elif ensemble in ('nve',):
+            lines.append('fix 1 all nve')
+        elif ensemble in ('csvr',):
+            lines.append('fix 1 all nve')
+            lines.append('fix 2 all temp/csvr ${TEMP} ${TEMP} ${TIME_CONST} %d' % (random.randrange(10^6 - 1) + 1))
+        else:
+            raise ValueError('unknown ensemble: ' + ensemble)
+        return '\n'.join(lines)
+
+    return (
+        LammpsInputTemplate,
+        make_lammps_task_dirs,
+    )
+
+
+(
+    LammpsInputTemplate,
+    make_lammps_task_dirs,
+) = __export_remote_functions()
```

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/lasp.py` & `ai2_kit-0.6.0/ai2_kit/domain/lasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/selector.py` & `ai2_kit-0.6.0/ai2_kit/domain/selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 import pandas as pd
 from tabulate import tabulate
 from itertools import groupby
 from operator import itemgetter
 
 import ase.io
 import os
+import numpy as np
 
 from .data import get_data_format, DataFormat, artifacts_to_ase_atoms
 from .iface import ICllSelectorOutput, BaseCllContext
-from .constant import LAMMPS_TRAJ_DIR, LAMMPS_TRAJ_SUFFIX, DEFAULT_ASAP_SOAP_DESC, DEFAULT_ASAP_PCA_REDUCER
+from .constant import LAMMPS_DUMP_DIR, LAMMPS_DUMP_SUFFIX, DEFAULT_ASAP_SOAP_DESC, DEFAULT_ASAP_PCA_REDUCER
 from .asap import get_descriptor, reduce_dimension, get_trainer, get_cluster
 
 
 logger = get_logger(__name__)
 
 
 class CllModelDeviSelectorInputConfig(BaseModel):
@@ -57,15 +58,15 @@
         return self.passing_rate
 
 
 @dataclass
 class CllModelDeviSelectorInput:
     config: CllModelDeviSelectorInputConfig
     model_devi_data: List[Artifact]
-    model_devi_out_filename: str
+    model_devi_file: str
     type_map: List[str]
 
     def set_model_devi_dataset(self, data: List[Artifact]):
         self.model_devi_data = data
 
 
 async def cll_model_devi_selector(input: CllModelDeviSelectorInput, ctx: CllModelDevSelectorContext):
@@ -74,15 +75,15 @@
     executor.mkdir(work_dir)
 
     f_trust_lo = input.config.f_trust_lo
     f_trust_hi = input.config.f_trust_hi
 
     results = executor.run_python_fn(bulk_select_structures_by_model_devi)(
         model_devi_outputs=[a.to_dict() for a in input.model_devi_data],
-        model_devi_filename=input.model_devi_out_filename,
+        model_devi_file=input.model_devi_file,
         f_trust_lo=f_trust_lo, f_trust_hi=f_trust_hi,
         type_map=input.type_map, work_dir=work_dir,
     )
 
     candidates = [candidate for candidate, _ in results if candidate is not None]  # filter out None
     stats = [stats for _, stats in results]
 
@@ -122,101 +123,106 @@
         passing_rate=total_good / total,
     )
 
 
 def __export_remote_functions():
 
     def bulk_select_structures_by_model_devi(model_devi_outputs: List[ArtifactDict],
-                                             model_devi_filename: str,
+                                             model_devi_file: str,
                                              f_trust_lo: float,
                                              f_trust_hi: float,
                                              type_map: List[str],
                                              work_dir: str,
                                              workers: int = 4,
                                              ) -> List[Tuple[Optional[ArtifactDict], dict]]:
         import joblib
         return joblib.Parallel(n_jobs=workers)(
             joblib.delayed(select_structures_by_model_devi)(
                 model_devi_output=output,
-                model_devi_filename=model_devi_filename,
+                model_devi_file=model_devi_file,
                 f_trust_lo=f_trust_lo, f_trust_hi=f_trust_hi,
                 type_map=type_map,
                 work_dir=os.path.join(work_dir, 'model_devi', f'{i:06}')
             )
             for i, output in enumerate(model_devi_outputs)
         )  # type: ignore
 
 
     def select_structures_by_model_devi(model_devi_output: ArtifactDict,
-                                        model_devi_filename: str,
+                                        model_devi_file: str,
                                         f_trust_lo: float,
                                         f_trust_hi: float,
                                         type_map: List[str],
                                         work_dir: str,
                                         ) -> Tuple[Optional[ArtifactDict], dict]:
         """
         analysis the model_devi output of explore stage and select candidates
         """
+
+
         os.makedirs(work_dir, exist_ok=True)
-        model_devi_out_url = model_devi_output['url']
+        dump_json(model_devi_output, os.path.join(work_dir, 'model_devi_output.debug.json'))
+
+        model_devi_dir = model_devi_output['url']
+        model_devi_file = model_devi_output['attrs'].pop('model_devi_file', model_devi_file)
+
         force_col = 'max_devi_f'
         print(f'criteria: {f_trust_lo} <= {force_col} < {f_trust_hi}')
 
         # get path of model_devi file
         data_format = get_data_format(model_devi_output)  # type: ignore
         if data_format in (DataFormat.LAMMPS_OUTPUT_DIR, DataFormat.LASP_LAMMPS_OUT_DIR):
-            model_devi_out_file = os.path.join(model_devi_out_url, model_devi_filename)
+            model_devi_file = os.path.join(model_devi_dir, model_devi_file)
         else:
             raise ValueError('unknown model_devi_data types')
-        logger.info('start to analysis file: %s', model_devi_out_file)
+        logger.info('start to analysis file: %s', model_devi_file)
 
         # load model_devi data
-        with open(model_devi_out_file, 'r') as f:
+        with open(model_devi_file, 'r') as f:
             text = f.read()
         df = pd.read_csv(StringIO(text.lstrip('#')), delim_whitespace=True)
-
         # layout:
         #        step  max_devi_v  min_devi_v  avg_devi_v  max_devi_f  min_devi_f  avg_devi_f
         # 0        0    0.006793    0.000672    0.003490    0.143317    0.005612    0.026106
         # 1      100    0.006987    0.000550    0.003952    0.128178    0.006042    0.022608
 
         # evaluate new found structures by their model_devi score in 3 levels: good, decent, poor
         good_df   = df[df[force_col] < f_trust_lo]
         decent_df = df[(df[force_col] >= f_trust_lo) & (df[force_col] < f_trust_hi)]
         poor_df   = df[df[force_col] >= f_trust_hi]
 
         stats = {
-            'src': model_devi_out_file,
+            'src': model_devi_file,
             'total': len(df),
             'good': len(good_df),
             'decent': len(decent_df),
             'poor': len(poor_df),
         }
 
         # write decent structures into ase atoms and write to file
         decent_structures_artifact = None
         if len(decent_df) > 0:
             model_devi_decent_file = os.path.join(work_dir, 'model_devi_decent.xyz')
             if data_format == DataFormat.LAMMPS_OUTPUT_DIR:
                 atoms_list = []
                 for frame_id in decent_df.step:
-                    dump_file = os.path.join(model_devi_out_url, LAMMPS_TRAJ_DIR, f'{frame_id}{LAMMPS_TRAJ_SUFFIX}')
+                    lammps_dump_dir = model_devi_output['attrs'].pop('lammps_dump_dir', LAMMPS_DUMP_DIR)
+                    dump_file = os.path.join(model_devi_dir, lammps_dump_dir, f'{frame_id}{LAMMPS_DUMP_SUFFIX}')
                     atoms_list.extend(ase.io.read(dump_file, ':', format='lammps-dump-text', specorder=type_map))
             elif data_format == DataFormat.LASP_LAMMPS_OUT_DIR:
-                structures_file = os.path.join(model_devi_out_url, 'structures.xyz')
+                structures_file = os.path.join(model_devi_dir, 'structures.xyz')
                 atoms_list = list(itemgetter(*decent_df.step)(ase.io.read(structures_file, ':', format='extxyz')))  # type: ignore
             else:
                 raise ValueError('unknown model_devi_data types')
             ase.io.write(model_devi_decent_file, atoms_list, format='extxyz')
             decent_structures_artifact = {
                 'url': model_devi_decent_file,
                 'format': DataFormat.EXTXYZ,
                 'attrs': {
                     **model_devi_output['attrs'],
-                    'size': len(atoms_list)
                 }
             }
         dump_json([decent_structures_artifact, stats], os.path.join(work_dir, 'output.debug.json'))
         return decent_structures_artifact, stats  # type: ignore
 
     def bulk_select_distinct_structures(candidates: List[ArtifactDict],
                                         descriptor_opt: dict,
@@ -259,41 +265,44 @@
                                    ):
         os.makedirs(work_dir, exist_ok=True)
 
         dump_json(attrs, os.path.join(work_dir, 'attrs.debug.json'))
         # load structures and save it to a tmp file for ASAP to load
         atoms_list = [atoms for _, atoms in artifacts_to_ase_atoms(candidates, type_map=type_map)]
 
-        if len(atoms_list) < max_structures_per_system:
-            ...  # TODO: no need for extra screening
-
-        tmp_structures_file = os.path.join(work_dir, '.tmp-structures.xyz')
-        ase.io.write(tmp_structures_file, atoms_list, format='extxyz')
+        if len(atoms_list) < max(max_structures_per_system, 10):
+            # Nothing to do when the total number of atoms is small
+            # FIXME: there are a lot of potential issue when the number of atoms is small
+            # the root cause is in asaplib, which I guess is not tested with small dataset
+            selected_atoms_list = atoms_list
+        else:
+            tmp_structures_file = os.path.join(work_dir, '.tmp-structures.xyz')
+            ase.io.write(tmp_structures_file, atoms_list, format='extxyz')
 
-        # use asaplib to group structures
-        asapxyz = ASAPXYZ(tmp_structures_file)
+            # use asaplib to group structures
+            asapxyz = ASAPXYZ(tmp_structures_file)
 
-        # group structures
-        path_prefix = os.path.join(work_dir, 'asap')
-        descriptors, _ = get_descriptor(asapxyz, descriptor_opt, path_prefix=path_prefix)
-        reduced_descriptors = reduce_dimension(descriptors, dim_reducer_opt)
-        trainer = get_trainer(reduced_descriptors, cluster_opt)
-        cluster_labels = get_cluster(asapxyz, reduced_descriptors, trainer, path_prefix=path_prefix)
-
-        # if max_structures_per_system is not set
-        # selected at least 1 structure from each group
-        if max_structures_per_system <= 0:
-            max_structures_per_system = len(cluster_labels)
-
-        # unpack clusters into a list and
-        # ensure frames of the same group won't be next to each other
-        # so that we can pick up distinct structures by simply choose the first N frames
-        order_frames = flat_evenly(cluster_labels.values())
-        selected_frames = order_frames[:max_structures_per_system]
-        selected_atoms_list = [atoms_list[i] for i in selected_frames]
+            # group structures
+            path_prefix = os.path.join(work_dir, 'asap')
+            descriptors, _ = get_descriptor(asapxyz, descriptor_opt, path_prefix=path_prefix)
+            reduced_descriptors = reduce_dimension(descriptors, dim_reducer_opt)
+            trainer = get_trainer(reduced_descriptors, cluster_opt)
+            cluster_labels = get_cluster(asapxyz, reduced_descriptors, trainer, path_prefix=path_prefix)
+
+            # if max_structures_per_system is not set
+            # selected at least 1 structure from each group
+            if max_structures_per_system <= 0:
+                max_structures_per_system = len(cluster_labels)
+
+            # unpack clusters into a list and
+            # ensure frames of the same group won't be next to each other
+            # so that we can pick up distinct structures by simply choose the first N frames
+            order_frames = flat_evenly(cluster_labels.values())
+            selected_frames = order_frames[:max_structures_per_system]
+            selected_atoms_list = [atoms_list[i] for i in selected_frames]
 
         # write selected structures to file
         distinct_structures_file = os.path.join(work_dir,  'distinct_structures.xyz')
         ase.io.write(distinct_structures_file, selected_atoms_list, format='extxyz')
 
         output = {
             'url': distinct_structures_file,
```

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/util.py` & `ai2_kit-0.6.0/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/domain/vasp.py` & `ai2_kit-0.6.0/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/main.py` & `ai2_kit-0.6.0/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.5/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.6.0/ai2_kit/workflow/cll_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,22 +196,20 @@
             train_output = await apply_checkpoint(f'{cp_prefix}/train-deepmd')(deepmd.cll_deepmd)(deepmd_input, deepmd_context)
 
         else:
             raise ValueError('No train method is specified')
 
         # explore
         if workflow_config.explore.lammps and context_config.explore.lammps:
-            md_options = lammps.CllLammpsInput.MdOptions(
-                models=train_output.get_mlp_models(),
-            )
             lammps_input = lammps.CllLammpsInput(
                 config=workflow_config.explore.lammps,
                 type_map=type_map,
                 mass_map=mass_map,
-                md_options=md_options,
+                dp_models={'': train_output.get_mlp_models()},
+                preset_template='default',
             )
             lammps_context = lammps.CllLammpsContext(
                 path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
                 config=context_config.explore.lammps,
                 resource_manager=resource_manager,
             )
             explore_output = await apply_checkpoint(f'{cp_prefix}/explore-lammps')(lammps.cll_lammps)(lammps_input, lammps_context)
@@ -234,15 +232,15 @@
             raise ValueError('No explore method is specified')
 
         # select
         if workflow_config.select.model_devi:
             selector_input = selector.CllModelDeviSelectorInput(
                 config=workflow_config.select.model_devi,
                 model_devi_data=explore_output.get_model_devi_dataset(),
-                model_devi_out_filename=const.MODEL_DEVI_OUT,
+                model_devi_file=const.MODEL_DEVI_OUT,
                 type_map=type_map,
             )
             selector_context = selector.CllModelDevSelectorContext(
                 path_prefix=os.path.join(iter_path_prefix, 'selector-model-devi'),
                 resource_manager=resource_manager,
             )
             selector_output = await apply_checkpoint(f'{cp_prefix}/selector-model-devi')(selector.cll_model_devi_selector)(selector_input, selector_context)
```

### Comparing `ai2_kit-0.5.5/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.6.0/ai2_kit/workflow/fep_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,43 +186,44 @@
         )
 
         # explore
         lammps_input = lammps.CllLammpsInput(
             config=workflow_config.lammps,
             type_map=type_map,
             mass_map=mass_map,
-            fep_options=lammps.CllLammpsInput.FepOptions(
-                neu_models=neu_train_output.get_mlp_models(),
-                red_models=red_train_output.get_mlp_models(),
-            ),
+            dp_models={
+                'NEU': neu_train_output.get_mlp_models(),
+                'RED': red_train_output.get_mlp_models(),
+            },
+            preset_template='fep-2m'
         )
         lammps_context = lammps.CllLammpsContext(
             path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
             config=context_config.lammps,
             resource_manager=resource_manager,
         )
         explore_output = await apply_checkpoint(f'{cp_prefix}/lammps')(lammps.cll_lammps)(lammps_input, lammps_context)
 
         # select
         red_selector_input = selector.CllModelDeviSelectorInput(
             config=workflow_config.red.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
-            model_devi_out_filename=const.MODEL_DEVI_RED_OUT,
+            model_devi_file=const.MODEL_DEVI_RED_OUT,
             type_map=type_map,
         )
         red_selector_context = selector.CllModelDevSelectorContext(
             path_prefix=os.path.join(
                 iter_path_prefix, 'red-selector-threshold'),
             resource_manager=resource_manager,
         )
 
         neu_selector_input = selector.CllModelDeviSelectorInput(
             config=workflow_config.neu.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
-            model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
+            model_devi_file=const.MODEL_DEVI_NEU_OUT,
             type_map=type_map,
         )
         neu_selector_context = selector.CllModelDevSelectorContext(
             path_prefix=os.path.join(iter_path_prefix, 'neu-selector-threshold'),
             resource_manager=resource_manager,
         )
```

### Comparing `ai2_kit-0.5.5/pyproject.toml` & `ai2_kit-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.5.5"
+version = "0.6.0"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.5.5/PKG-INFO` & `ai2_kit-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.5.5
+Version: 0.6.0
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/survey_report_generator-0.0.8.tar.gz` & `tmp/survey_report_generator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey_report_generator-0.0.8.tar", max compression
+gzip compressed data, was "survey_report_generator-0.0.9.tar", max compression
```

## Comparing `survey_report_generator-0.0.8.tar` & `survey_report_generator-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-05 05:33:37.736436 survey_report_generator-0.0.8/LICENSE
--rw-r--r--   0        0        0     2834 2023-08-07 10:46:30.714865 survey_report_generator-0.0.8/README.md
--rw-r--r--   0        0        0      931 2023-08-07 11:41:36.526598 survey_report_generator-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      839 2023-08-07 09:58:08.296356 survey_report_generator-0.0.8/survey_report_generator/__init__.py
--rw-r--r--   0        0        0    10617 2023-08-07 09:38:48.380575 survey_report_generator-0.0.8/survey_report_generator/databases.py
--rw-r--r--   0        0        0    12225 2023-08-07 09:38:48.371683 survey_report_generator-0.0.8/survey_report_generator/databases_summary.py
--rw-r--r--   0        0        0     2965 2023-06-29 03:08:24.254071 survey_report_generator-0.0.8/survey_report_generator/date_time.py
--rw-r--r--   0        0        0     4665 2023-08-07 10:42:12.482586 survey_report_generator-0.0.8/survey_report_generator/download_files.py
--rw-r--r--   0        0        0     2646 2023-08-07 09:38:48.352733 survey_report_generator-0.0.8/survey_report_generator/fesm.py
--rw-r--r--   0        0        0     7154 2023-08-02 01:31:26.062606 survey_report_generator-0.0.8/survey_report_generator/figures_utils.py
--rw-r--r--   0        0        0     2925 2023-07-12 23:25:21.640034 survey_report_generator-0.0.8/survey_report_generator/filter_utils.py
--rw-r--r--   0        0        0     3143 2023-06-28 11:49:29.042738 survey_report_generator-0.0.8/survey_report_generator/filter_utils_summary.py
--rw-r--r--   0        0        0     3353 2023-08-07 09:49:11.581585 survey_report_generator-0.0.8/survey_report_generator/g_drive_utils.py
--rw-r--r--   0        0        0     8773 2023-08-07 11:41:36.522534 survey_report_generator-0.0.8/survey_report_generator/generate_report.py
--rw-r--r--   0        0        0     3828 2023-08-07 09:38:48.360972 survey_report_generator-0.0.8/survey_report_generator/koala_habitat.py
--rw-r--r--   0        0        0     2770 2023-08-07 09:38:48.357342 survey_report_generator-0.0.8/survey_report_generator/pct.py
--rw-r--r--   0        0        0  1246571 2023-07-25 04:03:13.364594 survey_report_generator-0.0.8/survey_report_generator/report-template.docx
--rw-r--r--   0        0        0     6630 2023-08-07 09:40:31.415655 survey_report_generator-0.0.8/survey_report_generator/report.py
--rw-r--r--   0        0        0     1275 2023-08-07 09:49:18.984969 survey_report_generator-0.0.8/survey_report_generator/storage.json
--rw-r--r--   0        0        0     2614 2023-06-29 02:22:00.019734 survey_report_generator-0.0.8/survey_report_generator/summary.py
--rw-r--r--   0        0        0    11371 2023-08-07 09:38:48.384945 survey_report_generator-0.0.8/survey_report_generator/tables.py
--rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 survey_report_generator-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-05 05:33:37.736436 survey_report_generator-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2834 2023-08-07 10:46:30.714865 survey_report_generator-0.0.9/README.md
+-rw-r--r--   0        0        0      931 2023-08-08 07:16:51.089281 survey_report_generator-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      839 2023-08-07 09:58:08.296356 survey_report_generator-0.0.9/survey_report_generator/__init__.py
+-rw-r--r--   0        0        0    10617 2023-08-07 09:38:48.380575 survey_report_generator-0.0.9/survey_report_generator/databases.py
+-rw-r--r--   0        0        0    12225 2023-08-07 09:38:48.371683 survey_report_generator-0.0.9/survey_report_generator/databases_summary.py
+-rw-r--r--   0        0        0     2965 2023-06-29 03:08:24.254071 survey_report_generator-0.0.9/survey_report_generator/date_time.py
+-rw-r--r--   0        0        0     4665 2023-08-07 10:42:12.482586 survey_report_generator-0.0.9/survey_report_generator/download_files.py
+-rw-r--r--   0        0        0     2646 2023-08-07 09:38:48.352733 survey_report_generator-0.0.9/survey_report_generator/fesm.py
+-rw-r--r--   0        0        0     7154 2023-08-02 01:31:26.062606 survey_report_generator-0.0.9/survey_report_generator/figures_utils.py
+-rw-r--r--   0        0        0     2925 2023-07-12 23:25:21.640034 survey_report_generator-0.0.9/survey_report_generator/filter_utils.py
+-rw-r--r--   0        0        0     3143 2023-06-28 11:49:29.042738 survey_report_generator-0.0.9/survey_report_generator/filter_utils_summary.py
+-rw-r--r--   0        0        0     3353 2023-08-07 09:49:11.581585 survey_report_generator-0.0.9/survey_report_generator/g_drive_utils.py
+-rw-r--r--   0        0        0     8557 2023-08-08 07:14:59.773052 survey_report_generator-0.0.9/survey_report_generator/generate_report.py
+-rw-r--r--   0        0        0     3828 2023-08-07 09:38:48.360972 survey_report_generator-0.0.9/survey_report_generator/koala_habitat.py
+-rw-r--r--   0        0        0     2770 2023-08-07 09:38:48.357342 survey_report_generator-0.0.9/survey_report_generator/pct.py
+-rw-r--r--   0        0        0  1246571 2023-07-25 04:03:13.364594 survey_report_generator-0.0.9/survey_report_generator/report-template.docx
+-rw-r--r--   0        0        0     6630 2023-08-07 09:40:31.415655 survey_report_generator-0.0.9/survey_report_generator/report.py
+-rw-r--r--   0        0        0     1275 2023-08-07 09:49:18.984969 survey_report_generator-0.0.9/survey_report_generator/storage.json
+-rw-r--r--   0        0        0     2614 2023-06-29 02:22:00.019734 survey_report_generator-0.0.9/survey_report_generator/summary.py
+-rw-r--r--   0        0        0    11371 2023-08-07 09:38:48.384945 survey_report_generator-0.0.9/survey_report_generator/tables.py
+-rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 survey_report_generator-0.0.9/PKG-INFO
```

### Comparing `survey_report_generator-0.0.8/LICENSE` & `survey_report_generator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/README.md` & `survey_report_generator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/pyproject.toml` & `survey_report_generator-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "survey-report-generator"
-version = "0.0.8"
+version = "0.0.9"
 description = "A tool to generate survey reports from collected data"
 authors = ["Oliver Hahn <oliver.a.hahn@gmail.com>"]
 license = "MIT"  # Assuming your project is MIT licensed based on the classifiers
 readme = "README.md"
 homepage = "https://github.com/nsw-wildlife-drone-hub/report-generator"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `survey_report_generator-0.0.8/survey_report_generator/__init__.py` & `survey_report_generator-0.0.9/survey_report_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/databases.py` & `survey_report_generator-0.0.9/survey_report_generator/databases.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/databases_summary.py` & `survey_report_generator-0.0.9/survey_report_generator/databases_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/date_time.py` & `survey_report_generator-0.0.9/survey_report_generator/date_time.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/download_files.py` & `survey_report_generator-0.0.9/survey_report_generator/download_files.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/fesm.py` & `survey_report_generator-0.0.9/survey_report_generator/fesm.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/figures_utils.py` & `survey_report_generator-0.0.9/survey_report_generator/figures_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/filter_utils.py` & `survey_report_generator-0.0.9/survey_report_generator/filter_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/filter_utils_summary.py` & `survey_report_generator-0.0.9/survey_report_generator/filter_utils_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/g_drive_utils.py` & `survey_report_generator-0.0.9/survey_report_generator/g_drive_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/generate_report.py` & `survey_report_generator-0.0.9/survey_report_generator/generate_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,18 @@
 from .fesm import generate_fesm_map
 
 pd.options.mode.chained_assignment = None  # default='warn'
 warnings.filterwarnings("ignore", category=UserWarning, module="numpy", message=".*Intel MKL WARNING.*")
 
 
 def generate_report(report, download_databases=True, report_location='generated-reports'):
-    """
-    Args:
-        report (Report): Holds all variables specific to each report
-        download_databases (bool): If set to true, the relevant databases will be downloaded from Google Drive.
-        report_location (str): The folder, in which, the report should be saved. By default, this is the current
-            working directory.
-    """
     # Import template
-    # template = DocxTemplate('survey_report_generator/report-template.docx')
     with pkg_resources.path('survey_report_generator', 'report-template.docx') as template_path:
         template = DocxTemplate(template_path)
 
-
     report.generate_databases(download_databases)
 
     # The context variable holds all variables to be inserted into the template
     report.context['num_flights'] = len(report.airdata)
     report.context['client'] = 'NSW National Parks'
     add_dates(report)
     if os.path.exists(os.path.join(report.database_location, 'summary')):
@@ -58,34 +49,37 @@
         tables.add_detections_list_summary(report)
         tables.add_species_list_summary(report)
         tables.add_site_details_summary_table(report)
 
     # Add figures
     print("Generating survey site map...")
     figures_utils.generate_figure(report.kmls, report.detections, 'map.png')
-    report.context['figure_1'] = InlineImage(template, 'figures/map.png', Cm(15))
+    with pkg_resources.path('survey_report_generator', 'map.png') as img_path:
+        report.context['figure_1'] = InlineImage(template, img_path, Cm(15))
     print("Generating koala habitat map...")
     generate_koala_habitat_map(report.kmls, report.detections, 'koala-habitat-map.png')
-    report.context['figure_2'] = InlineImage(template, 'figures/koala-habitat-map.png', Cm(15))
+    with pkg_resources.path('survey_report_generator', 'koala-habitat-map.png') as img_path:
+        report.context['figure_2'] = InlineImage(template, img_path, Cm(15))
     print("Generating PCT map...")
     generate_pct_map(report.kmls, report.detections, 'pct-map.png')
-    report.context['figure_3'] = InlineImage(template, 'figures/pct-map.png', Cm(15))
+    with pkg_resources.path('survey_report_generator', 'pct-map.png') as img_path:
+        report.context['figure_3'] = InlineImage(template, img_path, Cm(15))
     print("Generating FESM map...")
     generate_fesm_map(report.kmls, report.detections, 'fesm-map.png')
-    report.context['figure_4'] = InlineImage(template, 'figures/fesm-map.png', Cm(15))
+    with pkg_resources.path('survey_report_generator', 'fesm-map.png') as img_path:
+        report.context['figure_4'] = InlineImage(template, img_path, Cm(15))
 
     if report_location:
         # Render automated report
         template.render(report.context)
         if not os.path.exists(report_location):
             # Create a new directory because it does not exist
             os.makedirs(report_location)
         template.save(os.path.join(report_location, f'{report.location_name}.docx'))
         report.export_dataframes(report.database_location)
-    # report.export_dataframes(os.path.join(report.database_location, 'summary'))
 
 
 def generate_multiple_reports(reports_list, report_location):
     """
     This method produces multiple reports one after the other with the given input parameters.
 
     Args:
```

### Comparing `survey_report_generator-0.0.8/survey_report_generator/koala_habitat.py` & `survey_report_generator-0.0.9/survey_report_generator/koala_habitat.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/pct.py` & `survey_report_generator-0.0.9/survey_report_generator/pct.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/report-template.docx` & `survey_report_generator-0.0.9/survey_report_generator/report-template.docx`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/report.py` & `survey_report_generator-0.0.9/survey_report_generator/report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/storage.json` & `survey_report_generator-0.0.9/survey_report_generator/storage.json`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/summary.py` & `survey_report_generator-0.0.9/survey_report_generator/summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/survey_report_generator/tables.py` & `survey_report_generator-0.0.9/survey_report_generator/tables.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.8/PKG-INFO` & `survey_report_generator-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey-report-generator
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to generate survey reports from collected data
 Home-page: https://github.com/nsw-wildlife-drone-hub/report-generator
 License: MIT
 Author: Oliver Hahn
 Author-email: oliver.a.hahn@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```


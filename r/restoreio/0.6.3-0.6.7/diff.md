# Comparing `tmp/restoreio-0.6.3.tar.gz` & `tmp/restoreio-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.6.3.tar", last modified: Sun Jul  9 08:07:47 2023, max compression
+gzip compressed data, was "restoreio-0.6.7.tar", last modified: Wed Aug  9 03:03:23 2023, max compression
```

## Comparing `restoreio-0.6.3.tar` & `restoreio-0.6.7.tar`

### file list

```diff
@@ -1,206 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-09 08:07:34.000000 restoreio-0.6.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 08:07:34.000000 restoreio-0.6.3/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-09 08:07:34.000000 restoreio-0.6.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-09 08:07:34.000000 restoreio-0.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 08:07:34.000000 restoreio-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-09 08:07:47.080313 restoreio-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-09 08:07:34.000000 restoreio-0.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/cli_restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/cli_scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/generated/restoreio.scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-09 08:07:34.000000 restoreio-0.6.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21771 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/examples/uncertainty_quant/_utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/subset_domain.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17491 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/plot_js_divergence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/restoreio_mwe.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-09 08:07:34.000000 restoreio-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-09 08:07:34.000000 restoreio-0.6.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25367 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_scripts/examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45708 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_scripts/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_server_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_server_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_server_utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_server_utils/terminate_with_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-09 08:07:47.000000 restoreio-0.6.3/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-09 08:07:47.080313 restoreio-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-09 08:07:34.000000 restoreio-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-09 08:07:34.000000 restoreio-0.6.3/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-09 08:07:34.000000 restoreio-0.6.3/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-09 08:07:34.000000 restoreio-0.6.3/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-09 08:07:34.000000 restoreio-0.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.594630 restoreio-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-09 03:03:04.000000 restoreio-0.6.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-09 03:03:04.000000 restoreio-0.6.7/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-09 03:03:04.000000 restoreio-0.6.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-09 03:03:04.000000 restoreio-0.6.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-09 03:03:04.000000 restoreio-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-08-09 03:03:23.594630 restoreio-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-08-09 03:03:04.000000 restoreio-0.6.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.542629 restoreio-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.546629 restoreio-0.6.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/FormData.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.538629 restoreio-0.6.7/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.538629 restoreio-0.6.7/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.546629 restoreio-0.6.7/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.546629 restoreio-0.6.7/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.538629 restoreio-0.6.7/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.550629 restoreio-0.6.7/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.558629 restoreio-0.6.7/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.570629 restoreio-0.6.7/docs/source/_static/images/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)   835046 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/user-guide/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   798215 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/user-guide/grid-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   807105 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/user-guide/grid-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2194491 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/user-guide/velocities.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1888556 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/images/user-guide/velocities.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.574630 restoreio-0.6.7/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.574630 restoreio-0.6.7/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.574630 restoreio-0.6.7/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/cli_restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/cli_scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.574630 restoreio-0.6.7/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/generated/restoreio.scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/recursive_glob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/docs/source/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/user_guide/generating_ensembles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/user_guide/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30963 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/user_guide/input_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/user_guide/output_var.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/user_guide/restore_setting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-09 03:03:04.000000 restoreio-0.6.7/docs/source/user_guide/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-09 03:03:04.000000 restoreio-0.6.7/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.538629 restoreio-0.6.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21771 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/examples/uncertainty_quant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.542629 restoreio-0.6.7/examples/uncertainty_quant/_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/examples/uncertainty_quant/_utils/_load_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_load_variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/examples/uncertainty_quant/_utils/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.578630 restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/subset_domain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17491 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/plot_js_divergence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1198 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/plot_js_divergence.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-08-09 03:03:04.000000 restoreio-0.6.7/examples/uncertainty_quant/restoreio_mwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-09 03:03:04.000000 restoreio-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-09 03:03:04.000000 restoreio-0.6.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.582630 restoreio-0.6.7/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.582630 restoreio-0.6.7/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.582630 restoreio-0.6.7/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.582630 restoreio-0.6.7/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.582630 restoreio-0.6.7/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_input_output/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.586630 restoreio-0.6.7/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.586630 restoreio-0.6.7/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.590630 restoreio-0.6.7/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.590630 restoreio-0.6.7/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.590630 restoreio-0.6.7/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_scripts/examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45759 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_scripts/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.590630 restoreio-0.6.7/restoreio/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.590630 restoreio-0.6.7/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.590630 restoreio-0.6.7/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-08-09 03:03:04.000000 restoreio-0.6.7/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.582630 restoreio-0.6.7/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-09 03:03:23.000000 restoreio-0.6.7/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-09 03:03:23.594630 restoreio-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-09 03:03:04.000000 restoreio-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:03:23.594630 restoreio-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-09 03:03:04.000000 restoreio-0.6.7/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-09 03:03:04.000000 restoreio-0.6.7/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-09 03:03:04.000000 restoreio-0.6.7/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-09 03:03:04.000000 restoreio-0.6.7/tox.ini
```

### Comparing `restoreio-0.6.3/LICENSE.txt` & `restoreio-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/MANIFEST.in` & `restoreio-0.6.7/MANIFEST.in`

 * *Files 7% similar despite different names*

```diff
@@ -19,28 +19,31 @@
 recursive-include docs Makefile
 recursive-include docs *.bib
 recursive-include docs *.in
 recursive-include docs *.txt
 recursive-exclude docs *.html
 recursive-exclude docs *.pdf
 recursive-include docs *.ipynb
+recursive-include docs *.json
 recursive-include docs/source *.html
 
 recursive-include restoreio *.rst
 recursive-include examples *.py
 recursive-include examples *.rst
 recursive-include notebooks *.ipynb
 recursive-include tests *.py
 recursive-include tests *.rst
 recursive-include scripts *.sh
 
 recursive-exclude notebooks *.pdf
 recursive-exclude notebooks *.svg
 recursive-exclude examples *.pdf
 recursive-exclude examples *.svg
+recursive-include examples *.sh
+
 recursive-exclude tests *.svg
 recursive-exclude tests *.nc
 recursive-include tests *.txt
 
 include CHANGELOG.rst
 include README.rst
 include AUTHORS.txt
```

### Comparing `restoreio-0.6.3/PKG-INFO` & `restoreio-0.6.7/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,20 @@
-Metadata-Version: 2.1
-Name: restoreio
-Version: 0.6.3
-Summary: Reconstruct incomplete oceanographic dataset
-Home-page: https://github.com/ameli/restoreio
-Download-URL: https://github.com/ameli/restoreio/archive/main.zip
-Author: Siavash Ameli
-Author-email: sameli@berkeley.edu
-Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
-Project-URL: Source, https://github.com/ameli/restoreio
-Project-URL: Tracker, https://github.com/ameli/restoreio/issues
-Keywords: reconstruct-data oceanographic-data hf-radar
-Platform: Linux
-Platform: OSX
-Platform: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE.txt
-License-File: AUTHORS.txt
-
 ******
 |logo|
 ******
 
-``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset.
-
-``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <https://transport.me.berkeley.edu/restore>`__.
+``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset, with specific focus on ocean surface velocity data. This package can also generate data ensembles and perform statistical analysis, which allows uncertainty qualification of such datasets.
 
 Links
 =====
 
-* `Online Gateway <https://transport.me.berkeley.edu/restore>`_
+* `Online Gateway <https://restoreio.org>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
-* `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
-* `Git Hub <https://github.com/ameli/restoreio>`_
+* `Anaconda Cloud <https://anaconda.org/s-ameli/restoreio>`_
 
 Install
 =======
 
 Install with ``pip``
 --------------------
 
@@ -101,26 +59,75 @@
    :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-macos
 .. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-windows.yml
    :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-windows
 
 Documentation
 =============
 
-|deploy-docs| |binder|
+|deploy-docs|
 
 See `documentation <https://ameli.github.io/restoreio/index.html>`__, including:
 
-* `What This Packages Does? <https://ameli.github.io/restoreio/overview.html>`_
-* `Comprehensive Installation Guide <https://ameli.github.io/restoreio/tutorials/install.html>`_
-* `How to Work with Docker Container? <https://ameli.github.io/restoreio/tutorials/docker.html>`_
-* `How to Deploy on GPU Devices? <https://ameli.github.io/restoreio/tutorials/gpu.html>`_
+* `Installation Guide <https://ameli.github.io/restoreio/install.html>`_
 * `API Reference <https://ameli.github.io/restoreio/api.html>`_
-* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
+* `Examples <https://ameli.github.io/restoreio/examples.html>`_
 * `Publications <https://ameli.github.io/restoreio/cite.html>`_
 
+Interactive Tutorial
+====================
+
+|binder|
+
+Visit this `Jupyter notebook <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`__ for interactive tutorial.
+
+Usage
+=====
+
+An installation of ``restoreio`` can be used in two ways: (1) as an importable python package or (2) as a standalone executable in the command line environment.
+
+As a Python Package
+-------------------
+
+You may import ``restoreio`` in python. The main functions of this package are:
+
+* `restoreio.restore <https://ameli.github.io/restoreio/generated/restoreio.restore.html#restoreio.restore>`__: restores incomplete data, generates ensembles, and performs statistical analysis. You may import this function as
+
+  ::
+
+    from restoreio import restore
+
+* `restoreio.scan <https://ameli.github.io/restoreio/generated/restoreio.scan.html#restoreio.scan>`__: performs a pre-scan of your netcdf dataset. You may import this function as
+
+  ::
+
+    from restoreio import scan
+
+As a Standalone Executable
+--------------------------
+
+Alternatively, you may use ``restoreio`` as a standalone executable (outside of python environment) which can be executed in command line. When ``restoreio`` is installed, the following executables are available:
+
+* `restore <https://ameli.github.io/restoreio/cli_restore.html>`__: This executable is identical to ``restoreio.restore`` function in the Python interface.
+* `restore-scan <https://ameli.github.io/restoreio/cli_scan.html>`__: This executable is identical to ``restoreio.scan`` function in the Python interface.
+
+To use these executables, make sure the ``/bin`` directory of your python installation is set on your ``PATH`` environment variable. For instance, if your python is installed on ``/opt/minicinda3/``, add this path ``/opt/miniconda3/bin`` directory to ``PATH`` by
+
+::
+
+    export PATH=/opt/minicinda/bin:$PATH
+
+You may place the above line in ``~/.bashrc`` to make the above change permanently.
+
+Online Web-Based Interface
+==========================
+
+Alongside ``restoreio`` python package, we have additionally developed a web server to serve as a web-based interface for this software. This platform is available at: `https://restoreio.org <https://restoreio.org>`__.
+
+This online gateway allows users to efficiently process both local and remote datasets. The computational tasks are executed on the server side, leveraging the parallel processing capabilities of a high-performance computing cluster. Moreover, the web-based interface seamlessly integrates an interactive globe map, empowering sophisticated visualization of the results within the online platform.
+
 How to Contribute
 =================
 
 We welcome contributions via `GitHub's pull request <https://github.com/ameli/restoreio/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restoreio/issues>`_.
 
 How to Cite
 ===========
```

### Comparing `restoreio-0.6.3/docs/Makefile` & `restoreio-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/make.bat` & `restoreio-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_inspect.py` & `restoreio-0.6.7/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.6.7/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.6.7/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.6.7/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.6.7/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/css/custom-pydata.css` & `restoreio-0.6.7/docs/source/_static/css/custom-pydata.css`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 /* .copybtn { */
 /*     color: var(--pst-color-text-muted); */
 /* } */
 html[data-theme="dark"] button.copybtn {
     filter: invert(0.88) brightness(1.1);
 }
 
+/* Color of function signature in dark mode */
+html[data-theme="dark"] dt:target, span.highlighted {
+    background-color: #373737;
+}
+
 /* Logo color */
 img.logo__image {
     /* filter: grayscale(1) brightness(1.5); */
     filter: brightness(1.1);
 }
 
 img.logo__image:hover {
```

### Comparing `restoreio-0.6.3/docs/source/_static/css/custom.css` & `restoreio-0.6.7/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.6.7/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.png` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.svg` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.png` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.svg` & `restoreio-0.6.7/docs/source/_static/images/icons/logo-traceflows-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.6.7/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/deviation.png` & `restoreio-0.6.7/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.6.7/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.6.7/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.6.7/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.6.7/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.6.7/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.6.7/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.6.7/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.6.7/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_static/js/custom-pydata.js` & `restoreio-0.6.7/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_templates/autosummary/class.rst` & `restoreio-0.6.7/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_templates/layout.html` & `restoreio-0.6.7/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/_templates/version.html` & `restoreio-0.6.7/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/cite.rst` & `restoreio-0.6.7/docs/source/cite.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 
 Publications
 ************
 
 How to Cite
 ===========
 
+
 If you publish work that uses |project|, please consider citing the following manuscripts.
 
+
+.. _ref1:
 .. [1] Ameli, S., and Shadden. S. C. (2019). A Transport Method for Restoring Incomplete Ocean Current Measurements. *Journal of Geophysical Research: Oceans*, 124, 227-242 |ameli-jgr| |btn-bib-jgr| |btn-view-pdf-jgr|
 
    .. raw:: html
 
         <div class="highlight-BibTeX notranslate collapse" id="collapse-bib-jgr">
         <div class="highlight">
         <pre class="language-bib">
@@ -24,15 +27,16 @@
             pages   = {227-242},
             doi     = {https://doi.org/10.1029/2018JC014254},
             year    = {2019}
         }</code></pre>
         </div>
         </div>
 
-.. [2] Ameli, S., and Shadden. S. C. (2023). tochastic Modeling of HF Radar Data for Uncertainty Quantification and Gap Filling. |ameli-uq| |btn-bib-uq| |btn-view-pdf-uq|
+.. _ref2:
+.. [2] Ameli, S., and Shadden. S. C. (2023). Stochastic Modeling of HF Radar Data for Uncertainty Quantification and Gap Filling. |ameli-uq| |btn-bib-uq| |btn-view-pdf-uq|
 
    .. raw:: html
 
         <div class="highlight-BibTeX notranslate collapse" id="collapse-bib-uq">
         <div class="highlight">
         <pre class="language-bib">
         <code class="language-bib">@article{https://doi.org/10.1029/2018JC014254,
@@ -44,14 +48,15 @@
             pages   = {227-242},
             doi     = {https://doi.org/10.1029/2018JC014254},
             year    = {2019}
         }</code></pre>
         </div>
         </div>
 
+.. _ref3:
 .. [3] Ameli, S. (2022). *RestoreIO, a Python Package to Restore Incomplete Oceanographic Dataset*. |restoreio-zenodo| |btn-bib-restoreio|
 
    .. raw:: html
 
         <div class="highlight-BibTeX notranslate collapse" id="collapse-bib-restore">
         <div class="highlight">
         <pre class="language-bib">
```

### Comparing `restoreio-0.6.3/docs/source/conf.py` & `restoreio-0.6.7/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,20 +140,18 @@
     'sphinx-prompt',
     'sphinx_copybutton',
     'nbsphinx',
    'sphinx_gallery.load_style',
    'sphinxarg.ext',
 ]
 
-# Inner-sphinx to cross-reference imate packahe
-intersphinx_mapping = {
-    'imate': ('https://ameli.github.io/imate', None),
-    'detkit': ('https://ameli.github.io/detkit', None),
-    'special_functions': ('https://ameli.github.io/special_functions', None),
-}
+# Inner-sphinx to cross-reference other packages
+# intersphinx_mapping = {
+#     'traceflows': ('https://ameli.github.io/traceflows', None),
+# }
 
 # Copy button settings
 copybutton_prompt_is_regexp = True
 copybutton_prompt_text = r'>>> |\.\.\. '
 
 # Automatically generate autosummary after each build
 autosummary_generate = True
```

### Comparing `restoreio-0.6.3/docs/source/custom_domain.py` & `restoreio-0.6.7/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/examples.rst` & `restoreio-0.6.7/docs/source/examples.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _examples:
 
 Examples
 ********
 
-The following set of instructions is a step-by-step guide to reproduce the result in [R1]_, which is an example of using |project|.
+The following set of instructions is a step-by-step guide to reproduce the result in :ref:`[2] <ref2>`, which is an example of using |project|.
 
 Dataset
 =======
 
 The paper uses the HF radar dataset from the Monterey Bay region in California, USA. The HF radar can be accessed publicly through the `national HF radar network gateway <http://cordc.ucsd.edu/projects/mapping/>`__ maintained by the Coastal Observing Research and Development Center. Please follow these steps to obtain the data file.
 
 **Dataset Webpage:** The studied data is available through its `OpenDap page <https://hfrnet-tds.ucsd.edu/thredds/dodsC/HFR/USWC/2km/hourly/RTV/HFRADAR_US_West_Coast_2km_Resolution_Hourly_RTV_best.ncd.html>`__. In particular, the **OpenDap URL** of this dataset is
@@ -153,15 +153,9 @@
  :align: left
  :figwidth: 100%
  :width: 70%
  :class: custom-dark
  
  **Figure 10:** *The JS distance between the probability distributions pm(x, ξ) and pn(x, ξ) is shown as a function of m = 0, . . . , n. These two distributions correspond to the ensembles generated by the m-term (truncated) and n-term (complete) KL expansions, respectively. We note that the abscissa of the figure is displayed as the percentage of the ratio m/n where n = 485.*
 
-References
-==========
-
-.. [R1] Ameli, S., Shadden, S. C. (2023). *Stochastic Modeling of HF Radar Data for Uncertainty Quantification and Gap Filling*. `arXiv: 2206.09976 [physics.ao-ph] <https://arxiv.org/abs/2206.09976>`_
-
-
 .. |script_dir| replace:: ``/examples/uncertainty_quant``
 .. _script_dir: https://github.com/ameli/restoreio/blob/main/examples/uncertainty_quant/
```

### Comparing `restoreio-0.6.3/docs/source/index.rst` & `restoreio-0.6.7/docs/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 .. module:: restoreio
 
 |project| Documentation
 ***********************
 
 |deploy-docs|
 
-|project| is a python package to **Restore** **I**\ ncomplete **O**\ ceanographic datasets, with specific focus on ocean surface velocity data. It can also generate data ensembles and perform statistical analysis, enabling uncertainty qualification.
-
-.. .. toctree::
-    :maxdepth: 1
-
-    old/ComputeLogDeterminant.rst
-    old/ComputeTraceOfInverse.rst
-    old/examples.rst
-    old/generate_matrix.rst
-    old/InterpolateTraceOfInverse.rst
-    old/introduction.rst
+|project| is a python package to **Restore** **I**\ ncomplete **O**\ ceanographic datasets, with a specific focus on ocean surface velocity data. This package can also generate data ensembles and perform statistical analysis, which allows uncertainty qualification of such datasets.
 
 .. grid:: 4
 
     .. grid-item-card:: GitHub
         :link: https://github.com/ameli/restoreio
         :text-align: center
         :class-card: custom-card-link
@@ -31,28 +21,28 @@
 
     .. grid-item-card:: Anaconda Cloud
         :link: https://anaconda.org/s-ameli/restoreio
         :text-align: center
         :class-card: custom-card-link
 
     .. grid-item-card:: Online Interface
-        :link: https://transport.me.berkeley.edu/restore
+        :link: https://restoreio.org
         :text-align: center
         :class-card: custom-card-link
 
 .. grid:: 4
 
     .. grid-item-card:: Install
         :link: install
         :link-type: ref
         :text-align: center
         :class-card: custom-card-link
 
-    .. grid-item-card:: Tutorials
-        :link: index_tutorials
+    .. grid-item-card:: User Guide
+        :link: user_guide
         :link-type: ref
         :text-align: center
         :class-card: custom-card-link
 
     .. grid-item-card:: API reference
         :link: api
         :link-type: ref
@@ -61,30 +51,14 @@
 
     .. grid-item-card:: Publications
         :link: index_publications
         :link-type: ref
         :text-align: center
         :class-card: custom-card-link
 
-.. Content for performance are not ready. I cnaged this to Publications temporarily.
-.. .. grid-item-card:: Performance
-..     :link: index_performance
-..     :link-type: ref
-..     :text-align: center
-..     :class-card: custom-card-link
-
-.. Overview
-.. ========
-..
-.. To learn more about |project| functionality, see:
-..
-.. .. toctree::
-..
-..     overview
-
 Supported Platforms
 ===================
 
 Successful installation and tests performed on the following operating systems, architectures, and Python versions:
 
 .. |y| unicode:: U+2714
 .. |n| unicode:: U+2716
@@ -136,60 +110,52 @@
 For complete installation guide, see:
 
 .. toctree::
     :maxdepth: 2
 
     Install <install>
 
-.. _index_tutorials:
-
-Tutorials
-=========
-
-|binder|
+User Guide
+==========
 
 .. toctree::
-    :maxdepth: 1
-
-    Quick Start (jupyter notebook) <notebooks/quick_start.ipynb>
-    Examples <examples>
+    :maxdepth: 2
 
-Launch `online interactive notebook <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_ with Binder.
+    User Guide <user_guide/user_guide>
 
 API Reference
 =============
 
 Check the list of functions, classes, and modules of |project| with their usage, options, and examples.
 
 .. toctree::
-   :maxdepth: 2
+    :maxdepth: 2
    
-   API Reference <api>
+    API Reference <api>
+
+Examples
+========
 
-.. Features
-.. ========
+.. toctree::
+    :maxdepth: 2
+
+    Examples <examples>
 
-.. * **Randomized algorithms** using Hutchinson and stochastic Lanczos quadrature algorithms (see :ref:`Overview <overview>`)
-.. * Novel method to **interpolate** matrix functions. See :ref:`Interpolation of Affine Matrix Functions <interpolation>`.
-.. * Parallel processing both on **shared memory** and CUDA Capable **multi-GPU** devices.
-.. * Sparse covariance
-.. * Mixed covariance model, object
-.. * Automatic Relevance Determination (ARD)
-.. * Jacobian and Hessian based optimization
-.. * Learn hyperparameters in reduced space (profile likelihood)
-.. * Prediction in dual space with with :math:`\mathcal{O}(n)` complexity.
+Online Web-Based Interface
+==========================
+
+Alongside |project| python package, we also offer a online service as a web-based interface for this software. This platform is available at: `https://restoreio.org <https://restoreio.org>`__.
+
+This online gateway allows users to efficiently process both local and remote datasets. The computational tasks are executed on the server side, leveraging the parallel processing capabilities of a high-performance computing cluster. Moreover, the web-based interface seamlessly integrates an interactive globe map, empowering sophisticated visualization of the results within the online platform.
 
 Technical Notes
 ===============
 
 |tokei|
 
-.. Some notable implementation techniques used to develop |project| are:
-
-
 How to Contribute
 =================
 
 We welcome contributions via `GitHub's pull request <https://github.com/ameli/restoreio/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restoreio/issues>`_.
 
 .. _index_publications:
 
@@ -206,39 +172,25 @@
 License
 =======
 
 |license|
 
 This project uses a `BSD 3-clause license <https://github.com/ameli/restoreio/blob/main/LICENSE.txt>`_, in hopes that it will be accessible to most projects. If you require a different license, please raise an `issue <https://github.com/ameli/restoreio/issues>`_ and we will consider a dual license.
 
-.. Related Projects
-.. ================
+.. Companion Applications
+.. ======================
 ..
 .. .. grid:: 3
 ..
-..    .. grid-item-card:: |imate-light| |imate-dark|
-..        :link: https://ameli.github.io/imate/index.html
+..    .. grid-item-card:: |traceflows-light| |traceflows-dark|
+..        :link: https://ameli.github.io/traceflows/index.html
 ..        :text-align: center
 ..        :class-card: custom-card-link
 ..    
-..        A high-performance python package for scalable randomized algorithms for matrix functions in machine learning.
-..
-..    .. grid-item-card:: |detkit-light| |detkit-dark|
-..        :link: https://ameli.github.io/detkit/index.html
-..        :text-align: center
-..        :class-card: custom-card-link
-..
-..        A python package for matrix determinant functions used in machine learning.
-..
-..    .. grid-item-card:: |special-light| |special-dark|
-..       :link: https://ameli.github.io/special_functions/index.html
-..       :text-align: center
-..       :class-card: custom-card-link
-..
-..       A python package providing both Python and Cython interface for special mathematical functions.
+..        An online high-performance computational service for Lagrangian analysis of geophysical flows.
 
 .. |deploy-docs| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/deploy-docs.yml?label=docs
    :target: https://github.com/ameli/restoreio/actions?query=workflow%3Adeploy-docs
 .. |deploy-docker| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/deploy-docker.yml?label=build%20docker
    :target: https://github.com/ameli/restoreio/actions?query=workflow%3Adeploy-docker
 .. |codecov-devel| image:: https://img.shields.io/codecov/c/github/ameli/restoreio
    :target: https://codecov.io/gh/ameli/restoreio
@@ -250,33 +202,21 @@
 .. |pypi| image:: https://img.shields.io/pypi/v/restoreio
 .. |conda| image:: https://anaconda.org/s-ameli/traceinv/badges/installer/conda.svg
    :target: https://anaconda.org/s-ameli/traceinv
 .. |platforms| image:: https://img.shields.io/conda/pn/s-ameli/traceinv?color=orange?label=platforms
    :target: https://anaconda.org/s-ameli/traceinv
 .. |conda-version| image:: https://img.shields.io/conda/v/s-ameli/traceinv
    :target: https://anaconda.org/s-ameli/traceinv
-.. |binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb
 .. |conda-downloads| image:: https://img.shields.io/conda/dn/s-ameli/restoreio
    :target: https://anaconda.org/s-ameli/restoreio
-.. |tokei| image:: https://tokei.rs/b1/github/ameli/restoreio?category=lines
+.. |tokei| image:: https://tokei.ekzhang.com/b1/github/ameli/restoreio?category=lines
    :target: https://github.com/ameli/restoreio
 .. |languages| image:: https://img.shields.io/github/languages/count/ameli/restoreio
    :target: https://github.com/ameli/restoreio
-.. .. |imate-light| image:: _static/images/icons/logo-imate-light.svg
-..    :height: 23
-..    :class: only-light
-.. .. |imate-dark| image:: _static/images/icons/logo-imate-dark.svg
-..    :height: 23
-..    :class: only-dark
-.. .. |detkit-light| image:: _static/images/icons/logo-detkit-light.svg
-..    :height: 27
-..    :class: only-light
-.. .. |detkit-dark| image:: _static/images/icons/logo-detkit-dark.svg
-..    :height: 27
-..    :class: only-dark
-.. .. |special-light| image:: _static/images/icons/logo-special-light.svg
-..    :height: 24
-..    :class: only-light
-.. .. |special-dark| image:: _static/images/icons/logo-special-dark.svg
-..    :height: 24
-..    :class: only-dark
+.. |traceflows-light| image:: _static/images/icons/logo-traceflows-light.svg
+   :height: 23
+   :class: only-light
+.. |traceflows-dark| image:: _static/images/icons/logo-traceflows-dark.svg
+   :height: 23
+   :class: only-dark
+.. .. |binder| image:: https://mybinder.org/badge_logo.svg
+..    :target: https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb
```

### Comparing `restoreio-0.6.3/docs/source/install.rst` & `restoreio-0.6.7/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/docs/source/recursive_glob.py` & `restoreio-0.6.7/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/restore/main_VaryingNumModes.py` & `restoreio-0.6.7/examples/restore/main_VaryingNumModes.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
                     Field_JS_Metric[i, j] = numpy.sqrt(JSD)
         return Field_JS_Metric
 
     # Test
     # import netCDF4 
     # Filename1 = '/home/sia/work/ImageProcessing/HFR-Uncertainty/files/MontereyBay_2km_Output_Full_KL_Expansion.nc'
     # nc_f = netCDF4.Dataset(Filename1)
-    # Mean_f_2 = nc_f.variables['East_vel'][0, :]
-    # Sigma_f_2 = nc_f.variables['East_err'][0, :]
+    # Mean_f_2 = nc_f.variables['east_vel'][0, :]
+    # Sigma_f_2 = nc_f.variables['east_err'][0, :]
 
     JSD = JSDistance(Mean_t, Mean_f, Sigma_t, Sigma_f)
     # JSD = JSDistance(Mean_t, Mean_f_2, Sigma_t, Sigma_f_2)
 
     return JSD
 
 # ==========================
```

### Comparing `restoreio-0.6.3/examples/restore/plot_coverage.py` & `restoreio-0.6.7/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.6.7/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.6.7/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.6.7/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/__init__.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/globals.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_server_utils/globals.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/_array_utilities.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/_array_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/subset_datetime.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/subset_datetime.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/subset_domain.py` & `restoreio-0.6.7/examples/uncertainty_quant/_utils/_subset/subset_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.6.7/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.6.7/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,25 +83,25 @@
     east/north velocities. The JS metric distance is the square root of JS
     distance. Log base 2 is used, hence the output is in range [0, 1].
     """
 
     nc_f = netCDF4.Dataset(filename_1)
     nc_t = netCDF4.Dataset(filename_2)
 
-    east_mean_f = nc_f.variables['East_vel'][0, :]
-    east_mean_t = nc_t.variables['East_vel'][0, :]
-    east_sigma_f = nc_f.variables['East_err'][0, :]
-    east_sigma_t = nc_t.variables['East_err'][0, :]
+    east_mean_f = nc_f.variables['east_vel'][0, :]
+    east_mean_t = nc_t.variables['east_vel'][0, :]
+    east_sigma_f = nc_f.variables['east_err'][0, :]
+    east_sigma_t = nc_t.variables['east_err'][0, :]
     east_jsd = js_distance(east_mean_t, east_mean_f, east_sigma_t,
                            east_sigma_f)
 
-    north_mean_f = nc_f.variables['North_vel'][0, :]
-    north_mean_t = nc_t.variables['North_vel'][0, :]
-    north_sigma_f = nc_f.variables['North_err'][0, :]
-    north_sigma_t = nc_t.variables['North_err'][0, :]
+    north_mean_f = nc_f.variables['north_vel'][0, :]
+    north_mean_t = nc_t.variables['north_vel'][0, :]
+    north_sigma_f = nc_f.variables['north_err'][0, :]
+    north_sigma_t = nc_t.variables['north_err'][0, :]
     north_jsd = js_distance(north_mean_t, north_mean_f, north_sigma_t,
                             north_sigma_f)
 
     return east_jsd, north_jsd
 
 
 # ====
```

### Comparing `restoreio-0.6.3/examples/uncertainty_quant/restoreio_mwe.py` & `restoreio-0.6.7/examples/uncertainty_quant/restoreio_mwe.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/__main__.py` & `restoreio-0.6.7/restoreio/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         scale_error=0.08,
         write_ensembles=False,
         plot=False,
         save=True,
         verbose=False,
         terminate=False):
     """
-    Restore incomplete oceanographic dataset.
+    Restore incomplete oceanographic dataset and generate data ensembles.
 
     Parameters
     ----------
 
     input : str
         Input filename. This can be either the path to a local file or the url
         to a remote dataset. The file extension should be ``.nc`` or ``.ncml``.
@@ -347,14 +347,195 @@
         ``ERROR``. This is useful when this package is executed on a server
         to pass exit signals to a Node application. On the downside, this
         option causes an interactive python environment to both terminate the
         script and the python environment itself. To avoid this, set this
         option to `False`. In this case, upon an error, the ``ValueError`` is
         raised, which cases the script to terminate, however, an interactive
         python environment will not be exited.
+
+    See Also
+    --------
+
+    restoreio.scan
+
+    Notes
+    -----
+
+    **Output File:**
+
+    The output is a NetCDF file in ``.nc`` format containing a selection of the
+    following variables, contingent on the chosen configuration:
+
+    1. Mask
+    2. Reconstructed East and North Velocities
+    3. East and North Velocity Errors
+    4. East and North Velocity Ensembles
+
+    **1. Mask:**
+
+    The mask variable is a three-dimensional array with dimensions for *time*,
+    *longitude*, and *latitude*. This variable is stored under the name
+    ``mask`` in the output file.
+
+    **Interpreting Mask Variable over Segmented Domains:**
+
+    The mask variable includes information about the result of domain
+    segmentation. This array contains integer values ``-1``, ``0``, ``1``, and
+    ``2`` that are interpreted as follows:
+
+    * The value ``-1`` indicates the location is identified to be on the
+      **land** domain :math:`\Omega_l`. In these locations, the output velocity
+      variable is masked.
+    * The value ``0`` indicates the location is identified to be on the
+      **known** domain :math:`\Omega_k`. These locations have velocity data in
+      the input file. The same velocity values are preserved in the output
+      file.
+    * The value ``1`` indicates the location is identified to be on the
+      **missing** domain :math:`\Omega_m`. These locations do not have a
+      velocity data in the input file, but they do have a reconstructed
+      velocity data on the output file.
+    * The value ``2`` indicates the location is identified to be on the
+      **ocean** domain :math:`\Omega_o`. In these locations, the output
+      velocity variable is masked.
+
+    **2. Reconstructed East and North Velocities:**
+
+    The reconstructed east and north velocity variables are stored in the
+    output file under the names ``east_vel`` and ``north_vel``, respectively.
+    These variables are three-dimensional arrays with dimensions for *time*,
+    *longitude*, and *latitude*.
+
+    **Interpreting Velocity Variables over Segmented Domains:**
+
+    The velocity variables on each of the segmented domains are defined as
+    follows:
+
+    * On locations where the ``mask`` value is ``-1`` or ``2``, the output
+      velocity variables are masked.
+    * On locations where the ``mask`` value is ``0``, the output velocity
+      variables have the same values as the corresponding variables in the
+      input file.
+    * On locations where the ``mask`` value is ``1``, the output velocity
+      variables are reconstructed. If the ``uncertainty_quant`` is enabled,
+      these output velocity variables are obtained by the *mean* of the
+      velocity ensembles, where the missing domain of each ensemble is
+      reconstructed.
+
+    **3. East and North Velocity Errors:**
+
+    If the ``uncertainty_quant`` option is enabled, the east and north velocity
+    error variables will be included in the output file under the names
+    ``east_err`` and ``north_err``, respectively. These variables are
+    three-dimensional arrays with dimensions for *time*, *longitude*, and
+    *latitude*.
+
+    **Interpreting Velocity Error Variable over Segmented Domains:**
+
+    The velocity error variables on each of the segmented domains are defined
+    as follows:
+
+    * On locations where the ``mask`` value is ``-1`` or ``2``, the output
+      velocity error variables are masked.
+    * On locations where the ``mask`` value is ``0``, the output velocity error
+      variables are obtained from either the corresponding velocity error or
+      GDOP variables in the input file scaled by the value of ``scale_error``.
+    * On locations where the ``mask`` value is ``1``, the output velocity error
+      variables are obtained from the *standard deviation* of the ensembles,
+      where the missing domain of each ensemble is reconstructed.
+
+    **4. East and North Velocity Ensembles:**
+
+    When you activate the ``uncertainty_quant`` option, a collection of
+    velocity field ensembles is created. Yet, by default, the output file only
+    contains the mean and standard deviation of these ensembles. To incorporate
+    all ensembles into the output file, you should additionally enable the
+    ``write_ensembles`` option. This action saves the east and north velocity
+    ensemble variables in the output file as ``east_vel_ensembles`` and
+    ``north_vel_ensembles``, respectively. These variables are four-dimensional
+    arrays with dimensions for *ensemble*, *time*, *longitude*, and
+    *latitude*.
+
+    The *ensemble* dimension of the array has the size :math:`s+1` where
+    :math:`s` is the number of ensembles specified by ``num_ensembles``
+    argument.. The first ensemble with the index :math:`0` corresponds to the
+    original input dataset. The other ensembles with the indices
+    :math:`1, \dots, s` correspond to the generated ensembles.
+
+    **Interpreting Velocity Ensemble Variables over Segmented Domains:**
+
+    The velocity ensemble variables on each of the segmented domains are
+    defined similar to those presented for velocity velocities. In particular,
+    the missing domain of each ensemble is reconstructed independently.
+
+    **Mean and Standard Deviation of Ensembles:**
+
+    Note that the *mean* and *standard deviation* of the velocity ensemble
+    arrays over the ensemble dimension yield the velocity and velocity error
+    variables, respectively.
+
+    Examples
+    --------
+
+    **Restoring Data:**
+
+    The following code is a minimalistic example of restoring the missing data
+    of an HF radar dataset:
+
+    .. code-block:: python
+
+        >>> # Import package
+        >>> from restoreio import restore
+
+        >>> # OpenDap URL of HF radar data, south side of Martha's Vineyard
+        >>> input = 'https://transport.me.berkeley.edu/thredds/dodsC/' + \\
+        ...         'root/WHOI-HFR/WHOI_HFR_2014_original.nc'
+
+        >>> # Subsetting time
+        >>> min_time = '2014-07-01T20:00:00'
+        >>> max_time = '2014-07-03T20:00:00'
+
+        >>> # Specify output
+        >>> output = 'output.nc'
+
+        >>> # Restore missing velocity data
+        >>> restore(input, output=output, min_time=min_time, max_time=max_time,
+        ...         detect_land=True, fill_coast=False, convex_hull=False,
+        ...         alpha=20, plot=False, verbose=True)
+
+    **Ensemble Generation:**
+
+    The following code is an example of generating ensembles for an HF radar
+    dataset:
+
+    .. code-block:: python
+
+        >>> # Import package
+        >>> from restoreio import restore
+
+        >>> # OpenDap URL of HF radar data, US west coast
+        >>> url = 'http://hfrnet-tds.ucsd.edu/thredds/dodsC/HFR/USWC/2km/' + \\
+        ...       'hourly/RTV/HFRADAR_US_West_Coast_2km_Resolution_Hou' + \\
+        ...       'rly_RTV_best.ncd'
+
+        >>> # Subsetting spatial domain to the Monterey Bay region, California
+        >>> min_lon = -122.344
+        >>> max_lon = -121.781
+        >>> min_lat = 36.507
+        >>> max_lat = 36.992
+
+        >>> # Time subsetting
+        >>> time_point = '2017-01-25T03:00:00'
+
+        >>> # Generate ensembles and reconstruct gaps
+        >>> restore(input=url, output='output.nc', min_lon=min_lon,
+        ...         max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
+        ...         time=time_point, uncertainty_quant=True, plot=False,
+        ...         num_ensembles=2000, ratio_num_modes=1, kernel_width=5,
+        ...         scale_error=0.08, detect_land=True, fill_coast=True,
+        ...         write_ensembles=True, verbose=True) 
     """
 
     # Define global variable for terminate with error
     if terminate:
         globals.terminate = True
     else:
         globals.terminate = False
```

### Comparing `restoreio-0.6.3/restoreio/_file_utilities/__init__.py` & `restoreio-0.6.7/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.6.7/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_geography/__init__.py` & `restoreio-0.6.7/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.6.7/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_geography/create_mask_info.py` & `restoreio-0.6.7/restoreio/_geography/create_mask_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 
     # Missing indices in ocean outside hull
     for i in range(missing_indices_in_ocean_outside_hull.shape[0]):
         mask_info[missing_indices_in_ocean_outside_hull[i, 0],
                   missing_indices_in_ocean_outside_hull[i, 1]] = 2
 
     # Land indices
-    if numpy.any(numpy.isnan(land_indices)) is False:
+    if bool(numpy.any(numpy.isnan(land_indices))) is False:
         for i in range(land_indices.shape[0]):
             mask_info[land_indices[i, 0], land_indices[i, 1]] = -1
 
     return mask_info
```

### Comparing `restoreio-0.6.3/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.6.7/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_geography/locate_missing_data.py` & `restoreio-0.6.7/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_inpaint/_cast_types.py` & `restoreio-0.6.7/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_inpaint/_image.py` & `restoreio-0.6.7/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_inpaint/_plot_image.py` & `restoreio-0.6.7/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_inpaint/inpaint.py` & `restoreio-0.6.7/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_input_output/__init__.py` & `restoreio-0.6.7/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.6.7/restoreio/_input_output/get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_input_output/load_dataset.py` & `restoreio-0.6.7/restoreio/_input_output/load_dataset.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_input_output/load_variables.py` & `restoreio-0.6.7/restoreio/_input_output/load_variables.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,20 +145,20 @@
     north_vel_obj = search_variable(agg, north_vel_names_list,
                                     north_vel_standard_names_list)
     if north_vel_obj is None:
         raise RuntimeError('NorthVelocity object can not be found in ' +
                            'netCDF file.')
 
     # East Velocity Error
-    east_vel_error_names_list = ['east_err', 'dopx']
+    east_vel_error_names_list = ['east_err', 'east_error', 'dopx', 'gdopx']
     east_vel_error_standard_names_list = []
     east_vel_error_obj = search_variable(agg, east_vel_error_names_list,
                                          east_vel_error_standard_names_list)
 
     # North Velocity Error
-    north_vel_error_names_list = ['north_err', 'dopy']
+    north_vel_error_names_list = ['north_err', 'north_error', 'dopy', 'gdopy']
     north_vel_error_standard_names_list = []
     north_vel_error_obj = search_variable(agg, north_vel_error_names_list,
                                           north_vel_error_standard_names_list)
 
     return datetime_obj, lon_obj, lat_obj, east_vel_obj, north_vel_obj, \
         east_vel_error_obj, north_vel_error_obj
```

### Comparing `restoreio-0.6.3/restoreio/_input_output/writer.py` & `restoreio-0.6.7/restoreio/_input_output/writer.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # =======
 
 import os
 import sys
 import netCDF4
 import numpy
 import time
+from .license import License                                       # noqa: E402
 
 __all__ = ['write_output_file']
 
 
 # ====================
 # remove existing file
 # ====================
@@ -102,134 +103,186 @@
     output_latitude.units = 'degree_north'
     output_latitude.standard_name = 'latitude'
     output_latitude.positive = 'up'
     output_latitude._CoordinateAxisType = 'Lat'
     output_latitude.axis = 'Y'
     output_latitude.coordsys = 'geographic'
 
-    # mask Info
+    # Mask
     mask = output_file.createVariable(
             'mask', numpy.dtype('float64').char, ('time', 'lat', 'lon', ),
             fill_value=fill_value, zlib=True)
     mask[:] = mask_info
-    mask.long_name = "Integer values at each points. \n \
-            -1: Indicates points on land. These points are not used. \n \
-             0: Indicates points in ocean with valid velocity data. \n \
-                These points are used for restoration. \n \
-             1: Indicates points in ocean inside convex/concave hull of \n \
-                data domain but with missing velocity data. These points \n \
-                are restored. \n \
-             2: Indicates points in ocean outside convex/concave hull of \n \
-                data domain but with missing velocity data. These points \n \
-                are not used."
     mask.coordinates = 'longitude latitude datetime'
     mask.missing_value = fill_value
     mask.coordsys = "geographic"
+    mask.comment = \
+        "Segmentation of the spatial domain to (1) land, (2) domain " + \
+        "with known velocity, (3) domain with missing velocity, and (4) " + \
+        "ocean. This variable contains integer values of -1, 0, 1, and 2, " + \
+        "representing the following domains: \n " + \
+        "-1: Indicates points that are identified to be on land. These " + \
+        "locations are masked. \n " + \
+        " 0: Indicates points that are identified to be in ocean with " + \
+        "known velocity data in the input dataset. \n" + \
+        " 1: Indicates points that are identified to be in ocean inside " + \
+        "the data domain, but they have missing velocity data in the " + \
+        "input file. These locations are reconstructed. \n" + \
+        " 2: Indicates points that are identified to be in ocean but " + \
+        "outside of the data domain. These locations are masked."
 
     # Velocity U
     output_u = output_file.createVariable(
-            'East_vel', numpy.dtype('float64').char, ('time', 'lat', 'lon', ),
+            'east_vel', numpy.dtype('float64').char, ('time', 'lat', 'lon', ),
             fill_value=fill_value, zlib=True)
     output_u[:] = u_all_times_inpainted
     output_u.units = 'm s-1'
     output_u.standard_name = 'surface_eastward_sea_water_velocity'
     output_u.positive = 'toward east'
     output_u.coordinates = 'longitude latitude datetime'
     output_u.missing_value = fill_value
     output_u.coordsys = "geographic"
+    output_u.comment = \
+        "Reconstructed east component of velocity. In areas where the " + \
+        "'mask' variable holds values of -1 or 2, the velocity variable " + \
+        "is masked. In regions where the 'mask' variable is 0, the " + \
+        "velocity variable in the output file maintains the same values " + \
+        "as the input file. In regions where the 'mask' variable equals " + \
+        "1, the velocity variable undergoes reconstruction."
 
     # Velocity V
     output_v = output_file.createVariable(
-            'North_vel', numpy.dtype('float64').char, ('time', 'lat', 'lon', ),
+            'north_vel', numpy.dtype('float64').char, ('time', 'lat', 'lon', ),
             fill_value=fill_value, zlib=True)
     output_v[:] = v_all_times_inpainted
     output_v.units = 'm s-1'
     output_v.standard_name = 'surface_northward_sea_water_velocity'
     output_v.positive = 'toward north'
     output_v.coordinates = 'longitude latitude datetime'
     output_v.missing_value = fill_value
     output_v.coordsys = "geographic"
+    output_v.comment = \
+        "Reconstructed north component of velocity. In areas where the " + \
+        "'mask' variable holds values of -1 or 2, the velocity variable " + \
+        "is masked. In regions where the 'mask' variable is 0, the " + \
+        "velocity variable in the output file maintains the same values " + \
+        "as the input file. In regions where the 'mask' variable equals " + \
+        "1, the velocity variable undergoes reconstruction."
 
     # Velocity U Error
     if u_all_times_inpainted_error is not None:
         output_u_error = output_file.createVariable(
-                'East_err', numpy.dtype('float64').char,
+                'east_err', numpy.dtype('float64').char,
                 ('time', 'lat', 'lon', ), fill_value=fill_value, zlib=True)
         output_u_error[:] = u_all_times_inpainted_error
         output_u_error.units = 'm s-1'
         output_u_error.positive = 'toward east'
         output_u_error.coordinates = 'longitude latitude datetime'
         output_u_error.missing_value = fill_value
         output_u_error.coordsys = "geographic"
+        output_u_error.comment = \
+            "East component of velocity error. In areas where the 'mask' " + \
+            "variable holds values of -1 or 2, the velocity error " + \
+            "variable is masked. In regions where the 'mask' variable is " + \
+            "0, the velocity error variable is obtained from the " + \
+            "velocity error or GDOP variable from the input file. In " + \
+            "regions where the 'mask' variable equals 1, the velocity " + \
+            "error variable is obtained from the standard deviation of " + \
+            "the velocity ensembles where the missing domain of each " + \
+            "ensemble is reconstructed."
 
     # Velocity V Error
     if v_all_times_inpainted_error is not None:
         output_v_error = output_file.createVariable(
-                'North_err', numpy.dtype('float64').char,
+                'north_err', numpy.dtype('float64').char,
                 ('time', 'lat', 'lon', ), fill_value=fill_value, zlib=True)
         output_v_error[:] = v_all_times_inpainted_error
         output_v_error.units = 'm s-1'
         output_v_error.positive = 'toward north'
         output_v_error.coordinates = 'longitude latitude datetime'
         output_v_error.missing_value = fill_value
         output_v_error.coordsys = "geographic"
+        output_v_error.comment = \
+            "North component of velocity error. In areas where the 'mask' " + \
+            "variable holds values of -1 or 2, the velocity error " + \
+            "variable is masked. In regions where the 'mask' variable is " + \
+            "0, the velocity error variable is obtained from the " + \
+            "velocity error or GDOP variable from the input file. In " + \
+            "regions where the 'mask' variable equals 1, the velocity " + \
+            "error variable is obtained from the standard deviation of " + \
+            "the velocity ensembles where the missing domain of each " + \
+            "ensemble is reconstructed."
 
     # Velocity U Ensembles
     if (write_ensembles is True) and (u_all_ensembles_inpainted is not None):
         output_u_ens = output_file.createVariable(
-                'East_vel_ensembles', numpy.dtype('float64').char,
+                'east_vel_ensembles', numpy.dtype('float64').char,
                 ('ensemble', 'lat', 'lon', ), fill_value=fill_value, zlib=True)
         output_u_ens[:] = u_all_ensembles_inpainted
         output_u_ens.units = 'm s-1'
         output_u_ens.positive = 'toward east'
         output_u_ens.coordinates = 'longitude latitude ensemble'
         output_u_ens.missing_value = fill_value
         output_u_ens.coordsys = "geographic"
+        output_u_ens.comment = \
+            "Ensembles of the east component of velocity. The first " + \
+            "ensemble is identical to the 'east_vel' variable. The rest " + \
+            "of the ensembles are randomly generated correlated " + \
+            "perturbations around the east velocity variable. The mean of " + \
+            "the ensembles is equivalent to the 'east_vel' variable. The " + \
+            "standard deviation of the ensembles is equal to the " + \
+            "'east_err' variable."
 
     # Velocity V Ensembles
     if (write_ensembles is True) and (v_all_ensembles_inpainted is not None):
         output_v_ens = output_file.createVariable(
-                'North_vel_ensembles', numpy.dtype('float64').char,
+                'north_vel_ensembles', numpy.dtype('float64').char,
                 ('ensemble', 'lat', 'lon', ), fill_value=fill_value, zlib=True)
         output_v_ens[:] = v_all_ensembles_inpainted
         output_v_ens.units = 'm s-1'
         output_v_ens.positive = 'toward east'
         output_v_ens.coordinates = 'longitude latitude ensemble'
         output_v_ens.missing_value = fill_value
         output_v_ens.coordsys = "geographic"
+        output_v_ens.comment = \
+            "Ensembles of the north component of velocity. The first " + \
+            "ensemble is identical to the 'north_vel' variable. The rest " + \
+            "of the ensembles are randomly generated correlated " + \
+            "perturbations around the north velocity variable. The mean " + \
+            "of the ensembles is equivalent to the 'north_vel' variable. " + \
+            "The standard deviation of the ensembles is equal to the " + \
+            "'north_err' variable."
 
+    # -----------------
     # Global Attributes
-    output_file.Conventions = 'CF-1.6'
+    # -----------------
+
+    # Author
+    output_file.creator_name = License.author_name
+    output_file.creator_email = License.author_email
+    output_file.creation_date = time.strftime("%x %X %Z")
+    output_file.institution = License.author_institution
+    output_file.title = License.output_file_title
+    output_file.history = License.output_file_history
+    output_file.project = License.output_file_project
+    output_file.acknowledgement = License.output_file_acknowledgement
+    output_file.license = License.output_file_license
+
+    # Data specific
+    output_file.Conventions = 'CF-1.10'
+    output_file.standard_name_vocabulary = 'CF Standard Name Table v30'
     output_file.COORD_SYSTEM = 'GEOGRAPHIC'
-    output_file.contributor_name = 'Siavash Ameli'
-    output_file.contributor_email = 'sameli@berkeley.edu'
-    output_file.contributor_role = 'Post process data to fill missing points.'
-    output_file.institution = 'University of California, Berkeley'
-    output_file.date_modified = time.strftime("%x")
-    output_file.title = 'Restored missing data inside the data domain'
-    output_file.source = 'Surface observation using high frequency radar.'
-    output_file.summary = """The HFR original data contain missing data points
-            both inside and outside the computational domain. The missing
-            points that are inside a convex hull around the domain of available
-            valid data points are filled. This technique uses a PDE based video
-            restoration."""
-    output_file.project = 'Advanced Lagrangian Predictions for Hazards' + \
-        'Assessments (NSF-ALPHA)'
-    output_file.acknowledgement = 'This material is based upon work ' + \
-        'supported by the National Science Foundation Graduate ' + \
-        'Research Fellowship under Grant No. 1520825.'
     output_file.geospatial_lat_min = "%f" % (numpy.min(latitude[:]))
     output_file.geospatial_lat_max = "%f" % (numpy.max(latitude[:]))
     output_file.geospatial_lat_units = 'degree_north'
     output_file.geospatial_lon_min = "%f" % (numpy.min(longitude[:]))
     output_file.geospatial_lon_max = "%f" % (numpy.max(longitude[:]))
     output_file.geospatial_lon_units = 'degree_east'
     output_file.geospatial_vertical_min = '0'
     output_file.geospatial_vertical_max = '0'
-
     output_file.time_coverage_start = \
         "%s" % (netCDF4.num2date(output_datetime[0],
                 units=output_datetime.units,
                 calendar=output_datetime.calendar))
     output_file.time_coverage_end = \
         "%s" % (netCDF4.num2date(output_datetime[-1],
                 units=output_datetime.units,
```

### Comparing `restoreio-0.6.3/restoreio/_parser/examples.py` & `restoreio-0.6.7/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_parser/formatter.py` & `restoreio-0.6.7/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_parser/parse_arguments.py` & `restoreio-0.6.7/restoreio/_parser/parse_arguments.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_display_utilities.py` & `restoreio-0.6.7/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_draw_map.py` & `restoreio-0.6.7/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_plot_grid.py` & `restoreio-0.6.7/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_plot_quiver.py` & `restoreio-0.6.7/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.6.7/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_plot_utilities.py` & `restoreio-0.6.7/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/_plot_velocities.py` & `restoreio-0.6.7/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots/plot_results.py` & `restoreio-0.6.7/restoreio/_plots/plot_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,20 +125,20 @@
             lon, lat, lon_grid, lat_grid, valid_points_coord,
             land_points_coord, all_missing_points_coord,
             missing_points_coord_inside_hull,
             missing_points_coord_outside_hull, U_original, V_original,
             U_inpainted, V_inpainted, save=save, verbose=verbose)
 
     # Plot original and inpainted velocity streamlines
-    plot_streamlines(
-            lon, lat, lon_grid, lat_grid, valid_points_coord,
-            land_points_coord, all_missing_points_coord,
-            missing_points_coord_inside_hull,
-            missing_points_coord_outside_hull, U_original, V_original,
-            U_inpainted, V_inpainted, save=save, verbose=verbose)
+    # plot_streamlines(
+    #         lon, lat, lon_grid, lat_grid, valid_points_coord,
+    #         land_points_coord, all_missing_points_coord,
+    #         missing_points_coord_inside_hull,
+    #         missing_points_coord_outside_hull, U_original, V_original,
+    #         U_inpainted, V_inpainted, save=save, verbose=verbose)
 
     # Plot original and inpainted velocity quiver
     # plot_quiver(
     #         lon, lat, lon_grid, lat_grid, valid_points_coord,
     #         land_points_coord, all_missing_points_coord,
     #         missing_points_coord_inside_hull,
     #         missing_points_coord_outside_hull, U_original, V_original,
```

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/__init__.py` & `restoreio-0.6.7/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.6.7/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.6.7/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,23 +204,23 @@
     east/north velocities. The JS metric distance is the square root of JS
     distance. Log base 2 is used, hence the output is in range [0, 1].
     """
 
     nc_1 = netCDF4.Dataset(filename_1)
     nc_2 = netCDF4.Dataset(filename_2)
 
-    east_mean_1 = nc_1.variables['East_vel'][0, :]
-    east_mean_2 = nc_2.variables['East_vel'][0, :]
-    east_sigma_1 = nc_1.variables['East_err'][0, :]
-    east_sigma_2 = nc_2.variables['East_err'][0, :]
-
-    north_mean_1 = nc_1.variables['North_vel'][0, :]
-    north_mean_2 = nc_2.variables['North_vel'][0, :]
-    north_sigma_1 = nc_1.variables['North_err'][0, :]
-    north_sigma_2 = nc_2.variables['North_err'][0, :]
+    east_mean_1 = nc_1.variables['east_vel'][0, :]
+    east_mean_2 = nc_2.variables['east_vel'][0, :]
+    east_sigma_1 = nc_1.variables['east_err'][0, :]
+    east_sigma_2 = nc_2.variables['east_err'][0, :]
+
+    north_mean_1 = nc_1.variables['north_vel'][0, :]
+    north_mean_2 = nc_2.variables['north_vel'][0, :]
+    north_sigma_1 = nc_1.variables['north_err'][0, :]
+    north_sigma_2 = nc_2.variables['north_err'][0, :]
 
     east_jsd = numpy.ma.masked_all(east_mean_1.shape, dtype=float)
     north_jsd = numpy.ma.masked_all(north_mean_1.shape, dtype=float)
 
     for i in range(east_mean_1.shape[0]):
         for j in range(east_mean_1.shape[1]):
```

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.6.7/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_restore/__init__.py` & `restoreio-0.6.7/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_restore/_make_array_masked.py` & `restoreio-0.6.7/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_restore/refine_grid.py` & `restoreio-0.6.7/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.6.7/restoreio/_restore/restore_generated_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.6.7/restoreio/_restore/restore_main_ensemble.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_scripts/examples.py` & `restoreio-0.6.7/restoreio/_scripts/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_scripts/scan.py` & `restoreio-0.6.7/restoreio/_scripts/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1151,14 +1151,19 @@
 
     Returns
     -------
 
     info : dict
         A dictionary containing information about the netcdf file dataset.
 
+    See Also
+    --------
+
+    restoreio.restore
+
     Notes
     -----
 
     * If the ``scan_velocity`` option (or ``-V`` in command line) is used to
       scan min and max of velocities, we do not find the min and max of
       velocity for all time frames. This is because if the `nc` file is large,
       it takes a long time. Also we do not load the whole velocities like
@@ -1167,16 +1172,16 @@
 
     Examples
     --------
 
     .. code-block:: python
 
         >>> from restoreio import scan
-        >>> input = 'https://transport.me.berkeley.edu/thredds/dodsC/root/' + \
-        ...         'WHOI-HFR/WHOI_HFR_2014_original.nc'
+        >>> input = 'https://transport.me.berkeley.edu/thredds/dodsC/' + \\
+        ...         'root/WHOI-HFR/WHOI_HFR_2014_original.nc'
 
         >>> # Run script
         >>> info = scan(input, scan_velocity=True, terminate=False,
         ...             verbose=True)
         {
             "Scan": {
                 "ScanStatus": true,
@@ -1233,16 +1238,16 @@
                     "MinLatitude": "41.036086627216",
                     "MaxLatitude": "41.388913372784",
                     "MinLongitude": "-70.87033700055551",
                     "MaxLongitude": "-70.3629969994445"
                 }
             },
             "VelocityInfo": {
-                "EastVelocityName": "East_vel",
-                "NorthVelocityName": "North_vel",
+                "EastVelocityName": "east_vel",
+                "NorthVelocityName": "north_vel",
                 "EastVelocityStandardName": "eastward_wind",
                 "NorthVelocityStandardName": "northward_wind",
                 "VelocityStandardName": "wind",
                 "MinEastVelocity": "-0.48760945773342956",
                 "MaxEastVelocity": "0.3507359965788057",
                 "MinNorthVelocity": "-0.36285106142279266",
                 "MaxNorthVelocity": "0.312877327708193",
```

### Comparing `restoreio-0.6.3/restoreio/_server_utils/globals.py` & `restoreio-0.6.7/restoreio/_server_utils/globals.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_server_utils/terminate_with_error.py` & `restoreio-0.6.7/restoreio/_server_utils/terminate_with_error.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_subset/_array_utilities.py` & `restoreio-0.6.7/restoreio/_subset/_array_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_subset/subset_datetime.py` & `restoreio-0.6.7/restoreio/_subset/subset_datetime.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_subset/subset_domain.py` & `restoreio-0.6.7/restoreio/_subset/subset_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.6.7/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.6.7/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.6.7/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.6.7/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.6.7/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.6.7/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/restoreio.egg-info/PKG-INFO` & `restoreio-0.6.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.6.3
+Version: 0.6.7
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
@@ -37,26 +37,23 @@
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 ******
 |logo|
 ******
 
-``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset.
-
-``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <https://transport.me.berkeley.edu/restore>`__.
+``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset, with specific focus on ocean surface velocity data. This package can also generate data ensembles and perform statistical analysis, which allows uncertainty qualification of such datasets.
 
 Links
 =====
 
-* `Online Gateway <https://transport.me.berkeley.edu/restore>`_
+* `Online Gateway <https://restoreio.org>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
-* `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
-* `Git Hub <https://github.com/ameli/restoreio>`_
+* `Anaconda Cloud <https://anaconda.org/s-ameli/restoreio>`_
 
 Install
 =======
 
 Install with ``pip``
 --------------------
 
@@ -101,26 +98,75 @@
    :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-macos
 .. |build-windows| image:: https://img.shields.io/github/actions/workflow/status/ameli/restoreio/build-windows.yml
    :target: https://github.com/ameli/restoreio/actions?query=workflow%3Abuild-windows
 
 Documentation
 =============
 
-|deploy-docs| |binder|
+|deploy-docs|
 
 See `documentation <https://ameli.github.io/restoreio/index.html>`__, including:
 
-* `What This Packages Does? <https://ameli.github.io/restoreio/overview.html>`_
-* `Comprehensive Installation Guide <https://ameli.github.io/restoreio/tutorials/install.html>`_
-* `How to Work with Docker Container? <https://ameli.github.io/restoreio/tutorials/docker.html>`_
-* `How to Deploy on GPU Devices? <https://ameli.github.io/restoreio/tutorials/gpu.html>`_
+* `Installation Guide <https://ameli.github.io/restoreio/install.html>`_
 * `API Reference <https://ameli.github.io/restoreio/api.html>`_
-* `Interactive Notebook Tutorials <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`_
+* `Examples <https://ameli.github.io/restoreio/examples.html>`_
 * `Publications <https://ameli.github.io/restoreio/cite.html>`_
 
+Interactive Tutorial
+====================
+
+|binder|
+
+Visit this `Jupyter notebook <https://mybinder.org/v2/gh/ameli/restoreio/HEAD?filepath=notebooks%2Fquick_start.ipynb>`__ for interactive tutorial.
+
+Usage
+=====
+
+An installation of ``restoreio`` can be used in two ways: (1) as an importable python package or (2) as a standalone executable in the command line environment.
+
+As a Python Package
+-------------------
+
+You may import ``restoreio`` in python. The main functions of this package are:
+
+* `restoreio.restore <https://ameli.github.io/restoreio/generated/restoreio.restore.html#restoreio.restore>`__: restores incomplete data, generates ensembles, and performs statistical analysis. You may import this function as
+
+  ::
+
+    from restoreio import restore
+
+* `restoreio.scan <https://ameli.github.io/restoreio/generated/restoreio.scan.html#restoreio.scan>`__: performs a pre-scan of your netcdf dataset. You may import this function as
+
+  ::
+
+    from restoreio import scan
+
+As a Standalone Executable
+--------------------------
+
+Alternatively, you may use ``restoreio`` as a standalone executable (outside of python environment) which can be executed in command line. When ``restoreio`` is installed, the following executables are available:
+
+* `restore <https://ameli.github.io/restoreio/cli_restore.html>`__: This executable is identical to ``restoreio.restore`` function in the Python interface.
+* `restore-scan <https://ameli.github.io/restoreio/cli_scan.html>`__: This executable is identical to ``restoreio.scan`` function in the Python interface.
+
+To use these executables, make sure the ``/bin`` directory of your python installation is set on your ``PATH`` environment variable. For instance, if your python is installed on ``/opt/minicinda3/``, add this path ``/opt/miniconda3/bin`` directory to ``PATH`` by
+
+::
+
+    export PATH=/opt/minicinda/bin:$PATH
+
+You may place the above line in ``~/.bashrc`` to make the above change permanently.
+
+Online Web-Based Interface
+==========================
+
+Alongside ``restoreio`` python package, we have additionally developed a web server to serve as a web-based interface for this software. This platform is available at: `https://restoreio.org <https://restoreio.org>`__.
+
+This online gateway allows users to efficiently process both local and remote datasets. The computational tasks are executed on the server side, leveraging the parallel processing capabilities of a high-performance computing cluster. Moreover, the web-based interface seamlessly integrates an interactive globe map, empowering sophisticated visualization of the results within the online platform.
+
 How to Contribute
 =================
 
 We welcome contributions via `GitHub's pull request <https://github.com/ameli/restoreio/pulls>`_. If you do not feel comfortable modifying the code, we also welcome feature requests and bug reports as `GitHub issues <https://github.com/ameli/restoreio/issues>`_.
 
 How to Cite
 ===========
```

### Comparing `restoreio-0.6.3/restoreio.egg-info/SOURCES.txt` & `restoreio-0.6.7/restoreio.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/make.bat
 docs/notes.rst
 docs/requirements.txt
+docs/source/FormData.json
 docs/source/_inspect.py
 docs/source/api.rst
 docs/source/cite.rst
 docs/source/cli_restore.rst
 docs/source/cli_scan.rst
 docs/source/conf.py
 docs/source/contents.rst
@@ -53,33 +54,44 @@
 docs/source/_static/images/plots/ensembles_js_distance.png
 docs/source/_static/images/plots/gdop_coverage.png
 docs/source/_static/images/plots/js_distance.png
 docs/source/_static/images/plots/kl_eigenvalues.png
 docs/source/_static/images/plots/kl_eigenvectors.png
 docs/source/_static/images/plots/orig_vel_and_error.png
 docs/source/_static/images/plots/rbf_kernel_2d.png
+docs/source/_static/images/user-guide/ensembles.png
+docs/source/_static/images/user-guide/grid-1.png
+docs/source/_static/images/user-guide/grid-2.png
+docs/source/_static/images/user-guide/velocities.png
+docs/source/_static/images/user-guide/velocities.svg
 docs/source/_static/js/custom-pydata.js
 docs/source/_templates/layout.html
 docs/source/_templates/sidebar-nav-bs.html
 docs/source/_templates/version.html
 docs/source/_templates/autosummary/attribute.rst
 docs/source/_templates/autosummary/class.rst
 docs/source/_templates/autosummary/method.rst
 docs/source/_templates/autosummary/ndarray_subclass.rst
 docs/source/_templates/autosummary/property.rst
 docs/source/generated/restoreio.restore.rst
 docs/source/generated/restoreio.scan.rst
-docs/source/notebooks/quick_start.ipynb
+docs/source/user_guide/generating_ensembles.rst
+docs/source/user_guide/getting_started.rst
+docs/source/user_guide/input_data.rst
+docs/source/user_guide/output_var.rst
+docs/source/user_guide/restore_setting.rst
+docs/source/user_guide/user_guide.rst
 examples/restore/main_VaryingNumModes.py
 examples/restore/plot_coverage.py
 examples/restore/plot_fixed_size_artificial_mask.py
 examples/restore/plot_variable_d_artificial_masks.py
 examples/restore/plot_variable_size_artificial_masks.py
 examples/uncertainty_quant/plot_gdop_coverage.py
 examples/uncertainty_quant/plot_js_divergence.py
+examples/uncertainty_quant/plot_js_divergence.sh
 examples/uncertainty_quant/restoreio_mwe.py
 examples/uncertainty_quant/_utils/_load_variables/__init__.py
 examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py
 examples/uncertainty_quant/_utils/_plot_utils/__init__.py
 examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py
 examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py
 examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py
@@ -110,14 +122,15 @@
 restoreio/_inpaint/__init__.py
 restoreio/_inpaint/_cast_types.py
 restoreio/_inpaint/_image.py
 restoreio/_inpaint/_plot_image.py
 restoreio/_inpaint/inpaint.py
 restoreio/_input_output/__init__.py
 restoreio/_input_output/get_datetime_info.py
+restoreio/_input_output/license.py
 restoreio/_input_output/load_dataset.py
 restoreio/_input_output/load_variables.py
 restoreio/_input_output/writer.py
 restoreio/_parser/__init__.py
 restoreio/_parser/examples.py
 restoreio/_parser/formatter.py
 restoreio/_parser/parse_arguments.py
```

### Comparing `restoreio-0.6.3/setup.py` & `restoreio-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/tests/test_restore_local_data.py` & `restoreio-0.6.7/tests/test_restore_local_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     max_lat = float('nan')
     time = '2017-01-25T03:00:00'
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     input = os.path.join(dir, input)
     output = os.path.join(dir, output)
-    plot = False
+    plot = True
 
     # Check input exists
     if not os.path.exists(input):
         raise RuntimeError('File: %s does not exists.' % input)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
```

### Comparing `restoreio-0.6.3/tests/test_restore_remote_data.py` & `restoreio-0.6.7/tests/test_restore_remote_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     min_lat = 41.2
     max_lat = 41.3
     min_time = '2014-07-01T20:00:00'
     max_time = '2014-07-03T20:00:00'
 
     # Output
     output = 'output_remote_data.nc'
-    plot = True
+    plot = False
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     output = os.path.join(dir, output)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
```

### Comparing `restoreio-0.6.3/tests/test_scan.py` & `restoreio-0.6.7/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.6.3/tox.ini` & `restoreio-0.6.7/tox.ini`

 * *Files identical despite different names*


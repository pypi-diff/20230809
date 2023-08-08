# Comparing `tmp/nirwals-0.0.1.tar.gz` & `tmp/nirwals-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nirwals-0.0.1.tar", last modified: Fri Jun  9 21:43:10 2023, max compression
+gzip compressed data, was "nirwals-0.0.5.tar", last modified: Tue Aug  8 22:06:33 2023, max compression
```

## Comparing `nirwals-0.0.1.tar` & `nirwals-0.0.5.tar`

### file list

```diff
@@ -1,53 +1,26 @@
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.514978 nirwals-0.0.1/
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.510978 nirwals-0.0.1/.github/
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.510978 nirwals-0.0.1/.github/workflows/
--rw-r--r--   0 rkotulla  (1000) users      (100)      947 2023-06-09 21:27:20.000000 nirwals-0.0.1/.github/workflows/release_to_pypi.yml
--rw-r--r--   0 rkotulla  (1000) users      (100)       13 2023-06-09 20:07:19.000000 nirwals-0.0.1/.gitignore
--rw-r--r--   0 rkotulla  (1000) users      (100)      284 2023-06-09 21:43:10.514978 nirwals-0.0.1/PKG-INFO
--rw-r--r--   0 rkotulla  (1000) users      (100)     3378 2023-06-09 20:06:01.000000 nirwals-0.0.1/README.md
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.510978 nirwals-0.0.1/dev/
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     2152 2023-06-09 20:07:00.000000 nirwals-0.0.1/dev/check_variance.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     7080 2023-06-09 20:07:00.000000 nirwals-0.0.1/dev/compare_ramps.py
--rw-r--r--   0 rkotulla  (1000) users      (100)      249 2022-09-16 22:52:20.000000 nirwals-0.0.1/dev/dev__frames2urg.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)      542 2022-12-07 17:57:44.000000 nirwals-0.0.1/dev/dirty_dark_subtract.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)      951 2023-02-16 17:57:25.000000 nirwals-0.0.1/dev/find_naughty_pixels.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)      371 2022-12-01 17:51:43.000000 nirwals-0.0.1/dev/make_pixellist.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     7272 2023-01-19 22:55:02.000000 nirwals-0.0.1/dev/plot_and_fit_curves.py
--rw-r--r--   0 rkotulla  (1000) users      (100)      579 2023-06-09 21:36:34.000000 nirwals-0.0.1/pyproject.toml
--rw-r--r--   0 rkotulla  (1000) users      (100)      107 2023-06-09 21:43:10.514978 nirwals-0.0.1/setup.cfg
--rw-r--r--   0 rkotulla  (1000) users      (100)      513 2023-06-09 21:39:44.000000 nirwals-0.0.1/setup.py
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.510978 nirwals-0.0.1/src/
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.514978 nirwals-0.0.1/src/nirwals/
--rw-r--r--   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:42:50.000000 nirwals-0.0.1/src/nirwals/__init__.py
--rw-r--r--   0 rkotulla  (1000) users      (100)      899 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/dev__cubeinspect.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     2716 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/dev__cubemath.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)      616 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/dev__dummyplot.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)      601 2022-01-10 22:32:50.000000 nirwals-0.0.1/src/nirwals/dev__extract_reference_pixels.py
--rw-r--r--   0 rkotulla  (1000) users      (100)      628 2023-06-09 21:42:29.000000 nirwals-0.0.1/src/nirwals/dev__find_previous_frame.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     5894 2023-06-09 21:42:29.000000 nirwals-0.0.1/src/nirwals/dev__fitpersistencysignal.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     1186 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/dev__fixbiasdips.py
--rw-r--r--   0 rkotulla  (1000) users      (100)      764 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/dev__mptest.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     1807 2022-01-26 21:56:38.000000 nirwals-0.0.1/src/nirwals/dev__pairwise_overscan_subtract.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     1285 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/dev__rowaverage.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     1390 2022-01-10 22:35:46.000000 nirwals-0.0.1/src/nirwals/edge_subtract.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     1831 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/mpfitter.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)    15519 2022-07-12 21:42:50.000000 nirwals-0.0.1/src/nirwals/mplogging.py
--rw-r--r--   0 rkotulla  (1000) users      (100)      517 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/nirwals__fit_nonlinearity.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     2229 2022-09-22 19:42:37.000000 nirwals-0.0.1/src/nirwals/nirwals_cubecombine.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     3229 2023-06-09 21:42:29.000000 nirwals-0.0.1/src/nirwals/nirwals_darkcorrect.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     8960 2023-06-09 21:42:29.000000 nirwals-0.0.1/src/nirwals/nirwals_explorer.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)      501 2022-09-06 21:32:06.000000 nirwals-0.0.1/src/nirwals/nirwals_extractHDU.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     2851 2022-08-26 21:00:56.000000 nirwals-0.0.1/src/nirwals/nirwals_filepicker.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     5866 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/nirwals_makedark.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     1331 2022-09-12 19:23:06.000000 nirwals-0.0.1/src/nirwals/nirwals_makemasterdark.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     2849 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/nirwals_plotpixel.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)    74815 2023-06-09 21:42:29.000000 nirwals-0.0.1/src/nirwals/nirwals_reduce.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     5784 2022-11-16 21:10:16.000000 nirwals-0.0.1/src/nirwals/nirwals_refpixel_calibrate.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     1538 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/plotcube.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)     3845 2022-09-13 22:01:29.000000 nirwals-0.0.1/src/nirwals/provenance.py
--rw-r--r--   0 rkotulla  (1000) users      (100)     4820 2023-06-09 19:44:43.000000 nirwals-0.0.1/src/nirwals/single_pixel_check.py
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2023-06-09 21:43:10.514978 nirwals-0.0.1/src/nirwals.egg-info/
--rw-r--r--   0 rkotulla  (1000) users      (100)      284 2023-06-09 21:43:10.000000 nirwals-0.0.1/src/nirwals.egg-info/PKG-INFO
--rw-r--r--   0 rkotulla  (1000) users      (100)     1327 2023-06-09 21:43:10.000000 nirwals-0.0.1/src/nirwals.egg-info/SOURCES.txt
--rw-r--r--   0 rkotulla  (1000) users      (100)        1 2023-06-09 21:43:10.000000 nirwals-0.0.1/src/nirwals.egg-info/dependency_links.txt
--rw-r--r--   0 rkotulla  (1000) users      (100)        8 2023-06-09 21:43:10.000000 nirwals-0.0.1/src/nirwals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:33.035298 nirwals-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-08 22:06:33.035298 nirwals-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-08-08 22:06:29.000000 nirwals-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 22:06:31.000000 nirwals-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 22:06:33.035298 nirwals-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-08 22:06:31.000000 nirwals-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:33.027298 nirwals-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:33.031298 nirwals-0.0.5/src/nirwals/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/edge_subtract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    90748 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/nirwals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8957 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/nirwals_explorer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/plotcube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/previous_file_picker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/provenance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13035 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/refpixel_calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals/single_pixel_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:33.035298 nirwals-0.0.5/src/nirwals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-08 22:06:33.000000 nirwals-0.0.5/src/nirwals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 22:06:33.000000 nirwals-0.0.5/src/nirwals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:06:33.000000 nirwals-0.0.5/src/nirwals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 22:06:33.000000 nirwals-0.0.5/src/nirwals.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9629 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals_fit_nonlinearity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5847 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals_makedark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals_makemasterdark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7861 2023-08-08 22:06:29.000000 nirwals-0.0.5/src/nirwals_reduce.py
```

### Comparing `nirwals-0.0.1/README.md` & `nirwals-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nirwals-0.0.1/pyproject.toml` & `nirwals-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nirwals"
-version = "0.0.1"
+version = "0.0.5"
 authors = [
   { name="Ralf Kotulla", email="ralf.kotulla@gmail.com" },
 ]
 description = "basic instrument signature removal for the NIRWALS instrument on the SALT telescope"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `nirwals-0.0.1/src/nirwals/dev__fitpersistencysignal.py` & `nirwals-0.0.5/src/nirwals_makedark.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,132 @@
 #!/usr/bin/env python3
 
 import sys
 import os
 import argparse
 import numpy
-import scipy
-import scipy.optimize
-import matplotlib.pyplot as plt
-import time
-
-import multiparlog as mplog
-import logging
 
 import astropy.io.fits as pyfits
 
-import nirwals_reduce
-
+from  nirwals import NIRWALS
 
+from dev__fitpersistencysignal import fit_persistency_plus_signal_pixel
 
 if __name__ == "__main__":
 
-    mplog.setup_logging(debug_filename="../../debug.log",
-                        log_filename="run_analysis.log")
-    mpl_logger = logging.getLogger('matplotlib')
-    mpl_logger.setLevel(logging.WARNING)
-
-    logger = logging.getLogger("RunAnalysis")
-
     cmdline = argparse.ArgumentParser()
     cmdline.add_argument("--maxfiles", dest="max_number_files", default=None, type=int,
                          help="limit number of files to load for processing")
     cmdline.add_argument("--nonlinearity", dest="nonlinearity_fn", type=str, default=None,
                          help="non-linearity correction coefficients (3-d FITS cube)")
     cmdline.add_argument("--output", dest="output_fn", type=str, default=None,
                          help="output filename")
     cmdline.add_argument("--dumps", dest="write_dumps", default=False, action='store_true',
                          help="write intermediate process data [default: NO]")
-    cmdline.add_argument("--refpixel", dest="use_ref_pixels", default=False, action='store_true',
-                         help="use reference pixels [default: NO]")
-    cmdline.add_argument("--previous", dest="previous_frame", type=str, default=None,
-                         help="last frame of previous exposure")
-    cmdline.add_argument("--xy", dest="xy", default=None, type=str,
-                         help="Run on a single pixel only")
-
     cmdline.add_argument("files", nargs="+",
                          help="list of input filenames")
     args = cmdline.parse_args()
 
     if (args.write_dumps):
         print("File-dumping enabled!")
 
     for fn in args.files:
 
-        rss = rss_reduce.RSS(fn, max_number_files=args.max_number_files,
-                   use_reference_pixels=args.use_ref_pixels,
-                   mask_saturated_pixels=True)
+        rss = NIRWALS(fn, max_number_files=args.max_number_files)
 
         if (args.nonlinearity_fn is not None and os.path.isfile(args.nonlinearity_fn)):
             rss.read_nonlinearity_corrections(args.nonlinearity_fn)
         rss.reduce(write_dumps=args.write_dumps,
-                   mask_bad_data=rss_reduce.RSS.mask_SATURATED,
-                   mask_saturated_pixels=True)
+                   mask_bad_data=NIRWALS.mask_SATURATED)
+
+        # count the number of good samples
+        number_good_dark_samples = numpy.sum(~rss.bad_data_mask, axis=0)
+        print("# good samples", number_good_dark_samples.shape)
 
         # Figure out what the incremental exposure time per read is
-        # exptime = rss.first_header['USEREXP'] / 1000. # raw values are in milli-seconds
-        # delta_exptime = exptime / rss.first_header['NGROUPS']
+        exptime = rss.first_header['USEREXP'] / 1000. # raw values are in milli-seconds
+        delta_exptime = exptime / rss.first_header['NGROUPS']
+        integ_exp_time = numpy.arange(rss.image_stack.shape[0]) * delta_exptime
+
+        darkrate = rss.weighted_mean / delta_exptime
+
+        # keep track of what kind of pixel each one is
+        pixeltype = numpy.full_like(darkrate, fill_value=nirwals.darktype_GOOD, dtype=numpy.int)
+
+        # find typical noise levels, so we can identify pixels that may need special treatment
+        good_data = numpy.isfinite(darkrate)
+        for iter in range(3):
+            _stats = numpy.nanpercentile(darkrate[good_data], [16, 50, 84])
+            print(iter, _stats)
+            _median = _stats[1]
+            _sigma = 0.5 * (_stats[2]-_stats[0])
+            good_data = good_data & (darkrate > _median-3*_sigma) & (darkrate < _median+3*_sigma)
+        final_stats = numpy.nanpercentile(darkrate[good_data], [16, 50, 84])
+        print("final image stats: ", final_stats)
+
+        darkrate_cleaned = numpy.copy(darkrate)
+        # darkrate_cleaned[~good_data] = numpy.NaN
+        pyfits.PrimaryHDU(data=darkrate_cleaned).writeto("darkrate_cleaned.fits", overwrite=True)
+
+        # identify pixels we need to have a special treatment for
+
+        negative_pixels = ~good_data & (darkrate < 0)
+        # let's ignore those for now, and set the actual dark-current to 0
+        # TODO: add code here
+        pixeltype[negative_pixels] = nirwals.darktype_COLD
+
+        min_exptime_required = 15. # seconds
+        min_frames = min_exptime_required / (delta_exptime)
+        hot_pixels = ~good_data & (darkrate > 0) & (number_good_dark_samples < min_frames)
+        pixeltype[hot_pixels] = nirwals.darktype_HOT
+
+        warm_pixels = ~good_data & (darkrate > 0) & (number_good_dark_samples >= min_frames)
+        pixeltype[warm_pixels] = nirwals.darktype_WARM
+        iy,ix = numpy.indices(darkrate.shape)
+        ixy = numpy.dstack([ix,iy])
+        print("IXY", ixy.shape)
+        warm_ixy = ixy[warm_pixels]
+        print("warm_ixy:", warm_ixy.shape)
+
+        warm_coefficients = numpy.zeros((3, darkrate.shape[0], darkrate.shape[1]))
+        for i, _xy in enumerate(warm_ixy):
+            x, y = _xy[0], _xy[1]
+            fullseries = rss.linearized_cube[:, y, x]
+            bad = rss.bad_data_mask[:, y, x]
+
+            series = fullseries[~bad]
+            times = integ_exp_time[~bad]
+            bestfit = fit_persistency_plus_signal_pixel(times, series)
+
+            warm_coefficients[:, y,x] = bestfit
+            if ((i%1000) == 0):
+                sys.stdout.write(">")
+                sys.stdout.flush()
 
         # now that we have the dark-rate, apply the correction to the frame to estimate the noise
-        # integ_exp_time = numpy.arange(rss.image_stack.shape[0]) * delta_exptime
+        mean_rate_subtracted = rss.linearized_cube - integ_exp_time.reshape((-1,1,1)) * darkrate.reshape((1, darkrate.shape[0], darkrate.shape[1]))
+        print("mean rate shape:", mean_rate_subtracted.shape)
+
+        dark_hdu = pyfits.HDUList([
+            pyfits.PrimaryHDU(header=rss.first_header),
+            pyfits.ImageHDU(data=darkrate, name='DARKRATE'),
+            pyfits.ImageHDU(data=number_good_dark_samples, name='N_SAMPLES'),
+            pyfits.ImageHDU(data=warm_coefficients, name='WARM_DARK_COEFFS'),
+        ])
+
+        if args.output_fn is None:
+            out_fn = rss.filebase + ".darkrate.fits"
+        else:
+            out_fn = args.output_fn
+        print("Writing darkrate image to %s ..." % (out_fn))
+        dark_hdu.writeto(out_fn, overwrite=True)
+
+        for (x,y) in [(1384,576), (1419,605), (1742,540), (1722,514)]:
+            rss.plot_pixel_curve(x,y,filebase=rss.filebase+"___")
+            rss.dump_pixeldata(x,y,filebase=rss.filebase+"___", extras=[mean_rate_subtracted])
 
-        if (args.xy is not None):
-            xy = [int(x) for x in args.xy.split(",")]
-            x = xy[0]
-            y = xy[1]
-
-            print("Working on a single pixel: x=%d y=%d" % (x,y))
-
-            ret = rss_reduce.persistency_fit_pixel(
-                differential_cube=rss.differential_cube,
-                linearized_cube=rss.linearized_cube,
-                read_times=rss.read_times,
-                x=x-1,
-                y=y-1,
-            )
-
-            bestfit, fit_uncert, good4fit = ret
-            print(bestfit)
-            print(fit_uncert)
-
-            rates = rss.differential_cube[:, y-1, x-1]
-            linear = rss.linearized_cube[:, y-1, x-1]
-            read_times = rss.read_times
-
-            numpy.savetxt("dummy_fit_singlepixel.dmp",
-                          numpy.array([read_times, rates, linear, good4fit]).T)
-
-            continue
-
-        print(args.previous_frame)
-        rss.fit_signal_with_persistency(previous_frame=args.previous_frame)
-
-        out_tmp = pyfits.PrimaryHDU(data=rss.persistency_fit_global)
-        out_tmp.writeto(args.output_fn, overwrite=True)
-
-        continue
-
-        for (x,y) in [(1384,576), (1419,605), (1742,540), (1722,514),
-            (1785,550), (1784,550), (1782,541), (1793,552), (1801,551), (1771,534), (1761,546), (1762,546),
-            (1763,546), (1764,546), (1764,547), (1764,549), (1761,551), (1759,552), (1757,542), (1756,542),
-            (1755,542), (1754,542), (1751,506), (1752,506), (1753,506), (1754,506),
-            ]:
-
-            t1 = time.time()
-            # rss.fit_signal_with_persistency_singlepixel(x, y, debug=True, plot=True)
-            rss.fit_signal_with_persistency_singlepixel(x, y, debug=False, plot=False)
-            t2 = time.time()
-            dt  = t2-t1
-            print("this took %f seconds (%f)" % (dt, dt*4e6))
-
-        # mean_rate_subtracted = rss.linearized_cube - integ_exp_time.reshape((-1,1,1)) * darkrate.reshape((1, darkrate.shape[0], darkrate.shape[1]))
-        # print("mean rate shape:", mean_rate_subtracted.shape)
-        #
-        # dark_hdu = pyfits.HDUList([
-        #     pyfits.PrimaryHDU(header=rss.first_header),
-        #     pyfits.ImageHDU(data=darkrate, name='DARKRATE')
-        # ])
-        #
-        # if args.output_fn is None:
-        #     out_fn = rss.filebase + ".darkrate.fits"
-        # else:
-        #     out_fn = args.output_fn
-        # print("Writing darkrate image to %s ..." % (out_fn))
-        # dark_hdu.writeto(out_fn, overwrite=True)
-
-        # for (x,y) in [(1384,576), (1419,605), (1742,540), (1722,514)]:
-        #     rss.plot_pixel_curve(x,y,filebase=rss.filebase+"___")
-        #     rss.dump_pixeldata(x,y,filebase=rss.filebase+"___", extras=[mean_rate_subtracted])
-        #
 
         # rss.plot_pixel_curve(1384, 576, filebase="darkgood__" + rss.filebase+"__")
         # rss.plot_pixel_curve(1419, 605, filebase="darkgood__" + rss.filebase+"__")
         # rss.plot_pixel_curve(1742, 540, filebase="darkbad__" + rss.filebase+"__")
         # rss.plot_pixel_curve(1722, 514, filebase="darkbad__" + rss.filebase+"__")
```

### Comparing `nirwals-0.0.1/src/nirwals/edge_subtract.py` & `nirwals-0.0.5/src/nirwals/edge_subtract.py`

 * *Files identical despite different names*

### Comparing `nirwals-0.0.1/src/nirwals/nirwals_explorer.py` & `nirwals-0.0.5/src/nirwals/nirwals_explorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import pyds9
 import multiprocessing
 
 import multiparlog as mplog
 import logging
 
 
-import nirwals_reduce
+import nirwals
 
 
 
 
 def ds9_listener(ds9, return_queue):
 
     while(True):
@@ -246,15 +246,15 @@
     ds9 = pyds9.DS9() #target='DS9:RSS_Explorer', start=True)
 
     plt.ion()
     print("Interactive?", plt.isinteractive())
 
     rss = None
     print("Preparing RSS data cube")
-    rss = rss_reduce.RSS(fn=fn, max_number_files=50, use_reference_pixels=True)
+    rss = rss_reduce.NIRWALS(fn=fn, max_number_files=50, use_reference_pixels=True)
     rss.reduce()
     print("Using persistency from %s" % (persistency_fn))
     rss.load_precalculated_results(persistency_fit_fn=persistency_fn)
 
     # load image into ds9
     ds9.set_np2arr(rss.weighted_mean)
```

### Comparing `nirwals-0.0.1/src/nirwals/nirwals_filepicker.py` & `nirwals-0.0.5/src/nirwals/previous_file_picker.py`

 * *Files identical despite different names*

### Comparing `nirwals-0.0.1/src/nirwals/nirwals_makemasterdark.py` & `nirwals-0.0.5/src/nirwals_makemasterdark.py`

 * *Files identical despite different names*

### Comparing `nirwals-0.0.1/src/nirwals/nirwals_reduce.py` & `nirwals-0.0.5/src/nirwals/nirwals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
+import queue
 
 import sys
-print(sys.path)
+# print(sys.path)
 
 import logging
 import os
 
 import multiparlog as mplog
 
 import numpy
@@ -13,22 +14,24 @@
 import matplotlib.pyplot as plt
 import scipy
 import scipy.optimize
 import itertools
 import multiprocessing
 import multiprocessing.shared_memory
 import argparse
+import time
 
 from astropy import log
 log.setLevel('ERROR')
 
 import warnings
 warnings.filterwarnings('ignore')
 
-import provenance
+from .provenance import DataProvenance
+from .refpixel_calibrate import  reference_pixels_to_background_correction
 
 import astropy
 print(astropy.__path__)
 
 
 # def fit_nonlinearity_sequence(pinit, args):
 #     """
@@ -367,15 +370,15 @@
                 linebuffer[n_pars,x] = -99
                 linebuffer[-3,x] = -numpy.sum(unsaturated)
 
                 # if ((x == 385 and row == 81) or (x == 387 and row == 95) or (x == 484 and row == 56)):
             if (x >380 and x<390 and row > 90 and row < 100):
                 print(x,row, full_fit_mask[x], )
                 numpy.savetxt("dump___x=%d_y=%d.txt" % (x,row),
-                      numpy.array([diff_reads, raw_reads, good_data.astype(numpy.int),
+                      numpy.array([diff_reads, raw_reads, good_data.astype(int),
                                    numpy.ones_like(diff_reads)*linebuffer[0,x]]).T)
 
         # end of loop over all pixels in this row
 
         persistency_fit[:, row, :] = linebuffer
 
 
@@ -399,52 +402,375 @@
     'weighted',
     'noise',
     'all',
     'fordark',
     'ngoodpixels',
 ]
 
-class RSS(object):
+
+def fit_pairwise_slope(times, reads, noise, good_reads=None, plot=False, permplot=True, plottitle=None):
+    if (good_reads is None):
+        good_reads = numpy.isfinite(reads) & numpy.isfinite(noise) & numpy.isfinite(times) & (times >= 0)
+
+    times = times[good_reads]
+    reads = reads[good_reads]
+    noise = noise[good_reads]
+
+    # time differences between reads
+    dt = times.reshape((-1, 1)) - times.reshape((1, -1))
+    df = reads.reshape((-1, 1)) - reads.reshape((1, -1))
+    d_noise = noise.reshape((-1, 1)) + noise.reshape((1, -1))
+
+    useful_pairs = (dt > 0) & numpy.isfinite(df)
+    rates = (df / dt)[useful_pairs]
+    noises = d_noise[useful_pairs]
+    #     print(rates.shape)
+
+    try:
+        good = numpy.isfinite(rates)
+
+        for it in range(3):
+            _stats = numpy.nanpercentile(rates[good], [16, 50, 84])
+            _med = _stats[1]
+            _sigma = 0.5 * (_stats[2] - _stats[0])
+            good = good & (rates > _med - 3 * _sigma) & (rates < _med + 3 * _sigma)
+            n_good = numpy.sum(good)
+            if (n_good < 10):
+                break
+
+        weights = 1. / noises
+        weighted = numpy.sum((rates * weights)[good]) / numpy.sum(weights[good])
+    except Exception as e:
+        weighted,_med,_sigma = numpy.NaN, numpy.NaN, numpy.NaN
+
+    if (plot):
+        fig, ax = plt.subplots(tight_layout=True)
+        if (permplot):
+            perm = numpy.random.permutation(rates.shape[0])
+        else:
+            perm = numpy.arange(rates.shape[0])
+        ax.scatter(numpy.arange(rates.shape[0])[perm][good], rates[good], s=0.5, alpha=.2)
+        ax.scatter(numpy.arange(rates.shape[0])[perm][~good], rates[~good], s=0.3, c='red')
+        ax.axhline(y=_med)
+        ax.axhline(y=_med - _sigma, c='grey')
+        ax.axhline(y=_med + _sigma, c='grey')
+        ax.axhline(y=bestfit[0], c='orange')
+        ax.set_ylim((_med - 10 * _sigma, _med + 10 * _sigma))
+        ax.set_title("median/sigma: %.3f +/- %.3f    weighted: %.3f" % (_med, _sigma, weighted))
+        if (plottitle is not None):
+            fig.suptitle(plottitle)
+
+    return dict(
+        weighted=weighted,
+        median=_med,
+        sigma=_sigma
+    )
+
+
+def worker__reference_pixel_correction(
+        shmem_cube_raw, shmem_cube_corrected, cube_shape,
+        refpixel_mode,
+        jobqueue, workername=None,
+):
+    """
+
+    :param shmem_cube_raw: shared memory block with raw input data
+    :param shmem_cube_corrected: shared memory block to hold corrected output file
+    :param cube_shape: shape of data cube
+    :param refpixel_mode: what algorithm to use for corrections. supported options are given in TODO: XXX
+    :param jobqueue: queue to handle workload balancing. By default reference pixels are corrected read by read
+    :param workername: name for worker to use during logging
+    :return: No return value, work is done when the jobqueue is empty
+    """
+
+    logger = logging.getLogger(workername if workername is not None else "RefPixelWorker")
+    logger.debug("Starting worker")
+
+    cube_raw = numpy.ndarray(shape=cube_shape, dtype=numpy.float32,
+                             buffer=shmem_cube_raw.buf)
+    cube_corrected = numpy.ndarray(shape=cube_shape, dtype=numpy.float32,
+                             buffer=shmem_cube_corrected.buf)
+
+    while (True):
+        try:
+            job = jobqueue.get()
+            if (job is None):
+                # this is the termination signal
+                jobqueue.task_done()
+                break
+        except queue.Empty as e:
+            logger.warning("job queue empty (%s)" % (e))
+            break
+
+        slice = job
+        logger.debug("Starting reference pixel correction for slice/read %d" % (slice))
+
+        t1 = time.time()
+        # get correction from data
+        data = cube_raw[slice, :, :]
+        corr_image = reference_pixels_to_background_correction(
+            data=data,
+            edge=1,
+            mode=refpixel_mode,
+            verbose=False, make_plots=False, debug=False)
+
+        # write results to output shared memory
+        cube_corrected[slice, :, :] = data - corr_image
+        t2 = time.time()
+        logger.debug("Correction for read %d done after %.3f seconds" % (slice, t2-t1))
+
+        jobqueue.task_done()
+
+    logger.debug("Shutting down")
+    shmem_cube_corrected.close()
+    shmem_cube_raw.close()
+
+def worker__nonlinearity_correction(
+        shmem_cube_corrected, shmem_corrections, cube_shape, corrections_shape,
+        jobqueue, workername=None,
+):
+    """
+
+    :param shmem_cube_corrected:
+    :param shmem_corrections:
+    :param cube_shape:
+    :param corrections_shape:
+    :param jobqueue:
+    :param workername:
+    :return:
+    """
+
+    logger = logging.getLogger(workername if workername is not None else "NonlinCorrectionWorker")
+    logger.debug("Starting worker")
+
+    cube_corrected = numpy.ndarray(shape=cube_shape, dtype=numpy.float32,
+                             buffer=shmem_cube_corrected.buf)
+    poly_corrections = numpy.ndarray(shape=corrections_shape, dtype=numpy.float32,
+                             buffer=shmem_corrections.buf)
+
+    # derive polynomial degree from number of factors
+    poly_order = poly_corrections.shape[0] - 1
+
+    while (True):
+        try:
+            job = jobqueue.get()
+            if (job is None):
+                # this is the termination signal
+                jobqueue.task_done()
+                break
+        except queue.Empty as e:
+            logger.warning("job queue empty (%s)" % (e))
+            break
+
+        y = job
+        logger.debug("Starting nonlinearity correction for row %d" % (y))
+
+        t1 = time.time()
+        # get correction from data
+
+        linecube = numpy.array(cube_corrected[:,y,:])
+        zero_offset = numpy.min(linecube, axis=0)
+        # print(zero_offset.shape)
+        linecube -= zero_offset
+
+        linefactors = poly_corrections[:,y,:]
+
+        outbuf = numpy.zeros_like(linecube)
+        for p in range(poly_order):
+            # logger.info("poly-order %d (img^%d)" % (p, poly_order-p))
+            outbuf += linefactors[p] * numpy.power(linecube, poly_order-p)
+
+        cube_corrected[:,y,:] = outbuf[:,:]
+
+        t2 = time.time()
+        logger.debug("Correction for row %d done after %.3f seconds" % (y, t2-t1))
+
+        jobqueue.task_done()
+
+    logger.debug("Shutting down")
+    shmem_corrections.close()
+    shmem_cube_corrected.close()
+
+
+def worker__fit_pairwise_slopes(
+        shmem_cube_corrected, shmem_results, cube_shape, results_shape,
+        jobqueue, read_times, speedy=False, workername=None,
+):
+
+    logger = logging.getLogger(workername if workername is not None else "PairSlopesWorker")
+    logger.debug("Starting worker")
+
+    cube_linearized = numpy.ndarray(shape=cube_shape, dtype=numpy.float32,
+                             buffer=shmem_cube_corrected.buf)
+    cube_results = numpy.ndarray(shape=results_shape, dtype=numpy.float32,
+                             buffer=shmem_results.buf)
+
+    while (True):
+        try:
+            job = jobqueue.get()
+            if (job is None):
+                # this is the termination signal
+                jobqueue.task_done()
+                break
+        except queue.Empty as e:
+            logger.warning("job queue empty (%s)" % (e))
+            break
+
+        y = job
+        logger.debug("Starting to fit pairwise slopes for row %d" % (y))
+
+        t1 = time.time()
+        # get correction from data
+
+        for x in range(4, cube_results.shape[2]-4 ):
+
+            reads = cube_linearized[:,y,x]
+            noise = numpy.sqrt(reads) # TODO: THIS NEEDS FIXING
+            times = numpy.array(read_times)
+
+            good_reads = numpy.isfinite(reads) & numpy.isfinite(noise) & numpy.isfinite(times) & (times >= 0)
+            if (numpy.sum(good_reads) < 1):
+                # not enough data to do anything with
+                continue
+
+            times = times[good_reads]
+            reads = reads[good_reads]
+            noise = noise[good_reads]
+
+            max_t = numpy.max(times)
+            n_samples = times.shape[0]
+
+            if (not speedy):
+                # time differences between reads
+                dt = times.reshape((-1, 1)) - times.reshape((1, -1))
+                df = reads.reshape((-1, 1)) - reads.reshape((1, -1))
+                d_noise = noise.reshape((-1, 1)) + noise.reshape((1, -1))
+            else:
+                # let's cut down the number of samples to use for pairwise fitting
+
+                # use all samples
+                n_select_x = numpy.arange(numpy.min([30, n_samples]))
+                n_select_y = numpy.arange(numpy.min([30, n_samples]))
+                pass
+                if (n_samples > 30):
+                    # use first 50, plus every 3rd after wards
+                    n_select_x = numpy.append(n_select_x, numpy.arange(30, numpy.min([150, n_samples, 4])))
+                    n_select_x = numpy.append(n_select_x, numpy.arange(30, numpy.min([151, n_samples, 3])))
+                    pass
+                if (n_samples > 150):
+                    #  use first 50, plus every 5th to 150, then fewer based on prime numbers to make sure we get
+                    #  unique pairings
+                    n_select_x = numpy.append(n_select_x, numpy.arange(150, n_samples, 7))
+                    n_select_x = numpy.append(n_select_x, numpy.arange(152, n_samples, 11))
+                # always include the last sample
+                n_select_x = numpy.append(n_select_x, [-1])
+                n_select_y = numpy.append(n_select_y, [-1])
+
+                dt = times[n_select_x].reshape((-1, 1)) - times[n_select_y].reshape((1, -1))
+                df = reads[n_select_x].reshape((-1, 1)) - reads[n_select_y].reshape((1, -1))
+                d_noise = noise[n_select_x].reshape((-1, 1)) + noise[n_select_y].reshape((1, -1))
+
+            useful_pairs = (dt > 0) & numpy.isfinite(df)
+            n_useful_pairs = numpy.sum(useful_pairs)
+            rates = (df / dt)[useful_pairs]
+            noises = d_noise[useful_pairs]
+            #     print(rates.shape)
+
+            try:
+                good = numpy.isfinite(rates)
+                n_good = numpy.sum(good)
+
+                for it in range(3):
+                    _stats = numpy.nanpercentile(rates[good], [16, 50, 84])
+                    _med = _stats[1]
+                    _sigma = 0.5 * (_stats[2] - _stats[0])
+                    new_good = good & (rates > _med - 3 * _sigma) & (rates < _med + 3 * _sigma)
+                    n_good = numpy.sum(new_good)
+                    if (n_good < 10):
+                        # if after this iteration we are left we too few good results then
+                        # skip this iteration step and use all remaining data
+                        break
+                    else:
+                        good = new_good
+
+                weights = 1. / noises
+                weighted = numpy.sum((rates * weights)[good]) / numpy.sum(weights[good])
+
+                cube_results[:,y,x] = [weighted, _med, _sigma, n_useful_pairs, max_t]
+            except Exception as e:
+                logger.debug("Encountered exception in pairfitting for x=%d, y=%d: %s" % (x,y,str(e)))
+                cube_results[:,y,x] = [numpy.NaN, numpy.NaN, numpy.NaN, n_useful_pairs, max_t]
+
+        t2 = time.time()
+        logger.debug("Fitting pair-slopes for row %d done after %.3f seconds" % (y, t2-t1))
+
+        jobqueue.task_done()
+
+    logger.debug("Shutting down")
+    shmem_results.close()
+    shmem_cube_corrected.close()
+
+
+class NIRWALS(object):
 
     mask_SATURATED = 0x0001
     mask_LOW_RATE = 0x0002
     mask_BAD_DARK = 0x0004
     mask_NEGATIVE = 0x0008
 
+    RESULT_EXTENSIONS = ["SCI", "MEDIAN", "NOISE", "NPAIRS", "MAX_T_EXP"]
+    N_RESULTS = len(RESULT_EXTENSIONS)
+
     def __init__(self, fn, max_number_files=-1,
                  saturation=None,
                  saturation_level=62000,
                  saturation_fraction=0.25, saturation_percentile=95,
-                 use_reference_pixels=True,
-                 mask_saturated_pixels=False):
+                 use_reference_pixels='none',
+                 mask_saturated_pixels=False,
+                 nonlinearity=None,
+                 n_cores=0,
+                 speedy=False,
+                 dumps=None,
+                 logger_name=None):
 
         self.fn = fn
         self.filelist = []
-        self.logger = logging.getLogger("RSS")
+        self.logger = logging.getLogger("Nirwals" if logger_name is None else logger_name)
+
+        self.logger.info("Current working directory: %s" % (os.getcwd()))
 
         self.use_reference_pixels = use_reference_pixels
         self.image_stack_initialized = False
         self.first_read_subtracted = False
         self.first_read = None
         self.first_header = None
         self.saturation_frame = None
 
-        self.nonlin_fn = None
+        self.nonlin_fn = nonlinearity
         self.nonlinearity_cube = None
+        self.nonlinearity_polyorder = -1
 
         self.alloc_persistency = False
 
         # store values we may/will need during reduction
         self.max_number_files = -1 if max_number_files is None else max_number_files
         self.saturation_level = saturation_level
         self.saturation_fraction = saturation_fraction
         self.saturation_percentile = saturation_percentile
         self.mask_saturated_pixels = mask_saturated_pixels
 
-        self.provenance = provenance.DataProvenance(
+        self.shmem_cube_raw = None
+        self.shmem_cube_linearized = None
+        self.shmem_cube_nonlinearity = None
+        self.shmem_cube_results = None
+
+        # Keep track of what intermediate processing steps to save/dump
+        self.write_dumps = dumps
+
+        self.provenance = DataProvenance(
             logger=self.logger,
             track_machine_data=True
         )
 
         if (saturation is not None):
             if (os.path.isfile(saturation)):
                 self.saturation_frame = saturation
@@ -459,47 +785,132 @@
                     self.saturation_level = _sat
                     self.provenance.add("saturation-level", _sat)
                 except:
                     pass
         else:
             self.provenance.add("saturation-level", self.saturation_level)
 
+        self.n_cores = n_cores if (n_cores is not None and n_cores > 0) else multiprocessing.cpu_count()
+        self.logger.info("Using %d CPU cores/threads for parallel processing" % (self.n_cores))
+
         self.read_exposure_setup()
+        self.speedy = speedy
 
         self.get_full_filelist()
 
+        try:
+            self.allocate_shared_memory()
+        except FileExistsError as e:
+            self.logger.critical(
+                "Unable to allocate shared memory -- most likely causes are it is either left from previous aborted run "
+                "(check /dev/shm or the like) or you are running multiple runs in parallel. Clean up files and try again")
+            raise(e)
+
+    def nonlinearity_valid(self):
+        if (self.nonlin_fn is None or not os.path.isfile(self.nonlin_fn)):
+            return False
+        try:
+            hdu = pyfits.open(self.nonlin_fn)
+            data = hdu[0].data
+            if (data is not None and data.ndim == 3 and data.shape[1]==self.ny and data.shape[2]==self.nx):
+                polyorder = hdu[0].data.shape[0] - 1
+                self.logger.info("Found valid non-linearity correction cube, order %d, in %s" % (polyorder, self.nonlin_fn))
+                self.nonlinearity_polyorder = polyorder
+                return True
+        except:
+            pass
+        return False
+
+    def allocate_shared_memory(self):
+        """
+        Pre-allocate shared memory for all datacubes to miniminze RAM footprint as much as possible, while
+        providing optimal performance for parallel data processing.
+        """
+
+        n_groups = numpy.min([self.n_groups, self.max_number_files]) if self.max_number_files > 0 else self.n_groups
+        cube_shape = (n_groups, self.ny, self.nx)
+        n_pixels_in_cube = n_groups * self.ny * self.nx
+        dummy = numpy.array([], dtype=numpy.float32)
+        self.logger.info("Assuming cube dimensions of %s for shared memory (%d bytes/pixel, total %.3f GB per cube)" % (
+            str(cube_shape), dummy.itemsize, n_pixels_in_cube*dummy.itemsize/2**30))
+
+        self.logger.info("Allocating shared memory: raw cube")
+        self.shmem_cube_raw = multiprocessing.shared_memory.SharedMemory(
+            name='raw_datacube', create=True,
+            size=(dummy.itemsize * n_pixels_in_cube),
+        )
+        self.cube_raw = numpy.ndarray(shape=cube_shape, dtype=numpy.float32, buffer=self.shmem_cube_raw.buf)
+
+        # logger.info("Copying datacube to shared memory")
+        # _raw = numpy.ndarray(shape=data_shape, dtype=numpy.float32, buffer=shmem_raw.buf)
+        # _raw[:, :, :] = raw_cube[:, :, :]
+
+        # allocate buffer for corrected data
+        self.logger.info("Allocating shared memory: linearized cube")
+        self.shmem_cube_linearized = multiprocessing.shared_memory.SharedMemory(
+            name='linearized_datacube', create=True,
+            size=(dummy.itemsize * n_pixels_in_cube),
+        )
+        self.cube_linearized = numpy.ndarray(shape=cube_shape, dtype=numpy.float32, buffer=self.shmem_cube_linearized.buf)
+        self.cube_linearized[:, :, :] = 0.
+
+        # Add place-holders for the nonlinearity corrections, to be read later
+        self.shmem_cube_nonlinearity = None
+        self.cube_nonlinearity = None
+        if (self.nonlinearity_valid()):
+            nonlin_shape = (self.nonlinearity_polyorder + 1, self.ny, self.nx)
+            n_pixels_nonlinearity = (self.nonlinearity_polyorder + 1) * self.ny * self.nx
+            self.logger.info("Allocating shared memory: linearized cube")
+            self.shmem_cube_nonlinearity = multiprocessing.shared_memory.SharedMemory(
+                name='nonlinearity_corrections', create=True,
+                size=(dummy.itemsize * n_pixels_nonlinearity),
+            )
+            self.cube_nonlinearity = numpy.ndarray(shape=nonlin_shape, dtype=numpy.float32, buffer=self.shmem_cube_nonlinearity.buf)
+            self.cube_nonlinearity[:, :, :] = 0.
+            self.logger.debug("shared meory for nonlinearity corrections initialized")
+
+        self.n_results_dimension = self.N_RESULTS
+        self.logger.info("Allocating shared memory for results (ndim=%d)" % (self.n_results_dimension))
+        n_pixels_results_cube = self.n_results_dimension * self.nx * self.ny
+        self.shmem_cube_results = multiprocessing.shared_memory.SharedMemory(
+            name='results_datacube', create=True,
+            size=(dummy.itemsize * n_pixels_results_cube),
+        )
+        self.cube_results = numpy.ndarray(
+            shape=(self.n_results_dimension, self.ny, self.nx), dtype=numpy.float32, buffer=self.shmem_cube_results.buf
+        )
+
     def read_exposure_setup(self):
         if (self.fn is None):
             self.logger.critical("Unable to get exposure setup without valid input filename")
 
         # read the input file as reference file
         self.ref_hdulist = pyfits.open(self.fn)
         self.ref_header = self.ref_hdulist[0].header
         self.provenance.add("ref-header", self.fn)
 
         # image dimensions
         self.nx = self.ref_header['XSTOP'] - self.ref_header['XSTART'] + 1
         self.ny = self.ref_header['YSTOP'] - self.ref_header['YSTART'] + 1
 
-        # readout settings
+        # readout settings -- FOR NOW NO MULTIPLE READS/RAMPS SUPPORTED IN A SINGLE SEQUENCE
         self.n_groups = self.ref_header['NGROUPS']
-        self.n_ramps = self.ref_header['NRAMPS']
-        self.n_reads = self.ref_header['NREADS']
+        self.n_ramps = 1 #self.ref_header['NRAMPS']
+        self.n_reads = 1 #self.ref_header['NREADS']
         self.n_outputs = self.ref_header['NOUTPUTS']
         self.gain = self.ref_header['GAIN']
 
         # exposure and other times
         self.exptime = self.ref_header['USEREXP'] / 1000.
         self.diff_exptime = self.exptime / self.n_groups
-
-
     def get_full_filelist(self):
         # get basedir
         fullpath = os.path.abspath(self.fn)
-        print(fullpath)
+        self.logger.info("absolute path of input file: %s" % (fullpath))
+
         self.basedir, _fn = os.path.split(fullpath)
         self.filebase = ".".join(_fn.split(".")[:-2])
         # print(self.basedir, filebase)
 
         for _read in range(1,1000):
             filename = "%s.%d.fits" % (self.filebase, _read)
             full_filename = os.path.join(self.basedir, filename)
@@ -509,25 +920,16 @@
                 break
 
             # print(full_filename, os.path.isfile(full_filename))
 
         self.logger.debug("Loading filelist:\n"+"\n -- ".join(self.filelist))
 
         return
-
     def add_file(self, filename):
         return
-
-    # def store_header_info(self, hdr):
-    #     self.first_header = hdr
-    #
-    #     self.exptime = hdr['USEREXP'] / 1000.
-    #     self.n_groups = hdr['NGROUPS']
-    #     self.diff_exptime = self.exptime / self.n_groups
-
     def load_all_files(self, max_number_files=None, mask_saturated_pixels=True):
 
         if (max_number_files is None):
             max_number_files = self.max_number_files
         if (self.image_stack_initialized):
             self.logger.debug("stack already initialized, skipping repeat try")
             return
@@ -541,20 +943,20 @@
         #     _filelist = _filelist[:max_number_files]
 
         # setup the data-cube to hold all the data
         if (max_number_files is not None and max_number_files > 0 and self.n_groups > max_number_files):
             self.n_groups = max_number_files
             print("Limiting input data to %d read-groups" % (max_number_files))
 
-        self.image_stack_raw = numpy.full(
-            (self.n_reads, self.n_groups, self.ny, self.nx),
-            fill_value=numpy.NaN, dtype=numpy.float32)
-        self.raw_read_times = numpy.full((self.n_reads, self.n_groups), fill_value=numpy.NaN)
+        # self.image_stack_raw = numpy.full(
+        #     (self.n_reads, self.n_groups, self.ny, self.nx),
+        #     fill_value=numpy.NaN, dtype=numpy.float32)
+        self.raw_read_times = numpy.full((self.n_groups), fill_value=numpy.NaN)
 
-        self.logger.debug("raw image cube dimensions: %s" % (str(self.image_stack_raw.shape)))
+        self.logger.debug("raw image cube dimensions: %s" % (str(self.cube_raw.shape)))
 
         # TODO: Add proper handling for combined Fowler and up-the-ramp sampling
         for fn in _filelist:
             try:
                 hdulist = pyfits.open(fn)
                 hdr = hdulist[0].header
                 imgdata = hdulist[0].data.astype(numpy.float32)
@@ -563,17 +965,17 @@
                 continue
 
             # hdulist.info()
 
             img_group = hdr['GROUP']
             img_read = hdr['READ']
             img_exptime = hdr['ACTEXP'] / 1000000. # convert time from raw microseconds to seconds
-            self.logger.info("FN=%s // grp=%d rd=%d exptime=%.4f" % (fn, img_group, img_read, img_exptime))
+            self.logger.debug("FN=%s // grp=%d rd=%d exptime=%.4f" % (fn, img_group, img_read, img_exptime))
 
-            if (max_number_files > 0 and img_group >= max_number_files):
+            if (max_number_files > 0 and img_group > max_number_files):
                 self.logger.debug("img-group > max-number-file --> skipping this file")
                 continue
 
             # track input files for provenance
             self.provenance.add("input", fn)
 
             # mask all saturated pixels if requested
@@ -585,64 +987,69 @@
                 saturation_mask[  :  , -4: ] = False # right
                 saturation_mask[  :4 ,   : ] = False # top
                 saturation_mask[-4:  ,   : ] = False # bottom
                 self.logger.debug("masking out %d saturated pixels" % (
                     numpy.sum(saturation_mask)))
                 imgdata[saturation_mask] = numpy.Inf
 
-
-            self.raw_read_times[img_read-1, img_group-1] = img_exptime
+            self.raw_read_times[img_group-1] = img_exptime
             # self.logger.debug("raw read times: %s" % (str(self.raw_read_times)))
 
-            self.image_stack_raw[img_read-1, img_group-1, :, :] = imgdata
+            # self.image_stack_raw[img_read-1, img_group-1, :, :] = imgdata
 
+            # self.logger.debug("Reading read %d into slice %d" % (img_group, img_group-1))
+            self.cube_raw[img_group-1, :, :] = imgdata
 
 
             # self._image_stack.append(imgdata)
             # if  (self.first_header is None):
             #     self.store_header_info(hdulist[0].header)
 
             # break
 
         # calculate the initial image stack
         self.logger.info("#groups=%d // #ramps=%d // #reads=%d" % (self.n_groups, self.n_ramps, self.n_reads))
         if (self.n_groups == 1 and self.n_reads >= 1):
             # this is a plain fowler mode, so calculate pair-wise differences
-            self.logger.info("Using fowler-sampling strategy")
-            self.image_stack = numpy.diff(self.image_stack_raw, axis=0)
-            print("@@@@@@@@@@@@@", self.image_stack.shape)
-            self.read_times = numpy.nanmean(self.raw_read_times, axis=0)
+            self.logger.critical("FOWLER MODE NOT SUPPORTED, NEED N_GROUPS>1 AND N_READS==1")
+            # self.logger.info("Using fowler-sampling strategy")
+            # self.image_stack = numpy.diff(self.image_stack_raw, axis=0)
+            # print("@@@@@@@@@@@@@", self.image_stack.shape)
+            # self.read_times = numpy.nanmean(self.raw_read_times, axis=0)
+            return
 
         elif (self.n_groups > 1):
             # up-the-ramp sampling.
             self.logger.info("Using up-the-ramp strategy")
-            self.image_stack = numpy.nanmean(self.image_stack_raw, axis=0)
-            print(self.raw_read_times)
-            self.read_times = numpy.nanmean(self.raw_read_times, axis=0)
+            # self.image_stack = numpy.nanmean(self.image_stack_raw, axis=0)
+            # print(self.raw_read_times)
+            self.read_times = self.raw_read_times #numpy.nanmean(self.raw_read_times, axis=0)
 
         else:
             self.logger.critical("No idea what's going here and what to do with this data - HELP!!!!")
             return
 
+        # self.logger.debug("stack before/after: %s --> %s" % (str(self.image_stack_raw.shape), str(self.image_stack.shape)))
+        self.logger.debug("read-times: %s" % (str(self.read_times)))
+        self.logger.debug("stack shape: %s" % (str(self.cube_raw.shape)))
 
-#         self.image_stack = numpy.array(self._image_stack, dtype=numpy.float32)
-
-        # self.image_stack = numpy.diff(self.image_stack_raw, axis=0)
-
-        self.logger.debug("stack before/after: %s --> %s" % (str(self.image_stack_raw.shape), str(self.image_stack.shape)))
-
-        self.logger.info("read-times: %s" % (str(self.read_times)))
+        #
+        # Now also load the nonlinearity corrections from file into shared memory
+        #
+        if (self.nonlinearity_valid()):
+            self.logger.info("Loading nonlinearity correction factors from %s" % (self.nonlin_fn))
+            hdu = pyfits.open(self.nonlin_fn)
+            nonlin = hdu[0].data
+            self.cube_nonlinearity[:,:,:] = nonlin[:,:,:]
 
-        self.logger.debug("stack shape: %s" % (str(self.image_stack.shape)))
 
         # delete raw stack to clean up memory
-        del self.image_stack_raw
+        # del self.image_stack_raw
 
         self.image_stack_initialized = True
-
     def apply_dark_correction(self, dark_fn, dark_mode="differential"):
 
         self.dark_cube = numpy.zeros_like(self.linearized_cube)
         if (dark_fn is None):
             self.logger.warning("No dark correction requested, skipping")
             return
         elif (not os.path.isfile(dark_fn)):
@@ -659,15 +1066,15 @@
                 self.logger.error("error during dark subtraction:\n%s" % (str(e)))
                 return
 
         if (dark_mode == "linearized"):
             # TODO: CHECK THAT THIS IS CORRECT
             # perform a dark subtraction;
             # dark-current = rate [in cts/sec] * frame-# * exposure-time per frame [in sec]
-            self.dark_cube = (numpy.arange(linearized.shape[0], dtype=numpy.float).reshape((-1, 1, 1)) + 1) \
+            self.dark_cube = (numpy.arange(linearized.shape[0], dtype=float).reshape((-1, 1, 1)) + 1) \
                         * self.diff_exptime \
                         * dark.reshape((1, dark.shape[0], dark.shape[1]))
             self.logger.debug("shape of dark cube: %s" % (self.dark_cube.shape))
             self.linearized_cube -= self.dark_cube
 
         elif (dark_mode == "differential"):
             # if (dark.shape[0] == self.differential_cube.shape[0]):
@@ -701,20 +1108,16 @@
                 else:
                     self.logger.debug("Dark correction for read %d from master dark" % (read))
                     self.differential_cube[read, :, :] -= dark[read, :, :]
             # self.differential_cube[:,:,] = self.differential_cube[:,:,:] - dark_correction[:,:,:] # * 1e-6)
             # pyfits.PrimaryHDU(data=self.differential_cube).writeto("darkcorrect_after.fits", overwrite=True)
 
         return
-
-
-
-
     def dump_data(self, data, fn, datatype="?_default_?", extname=None):
-        self.logger.debug("Writing %s to %s" % (datatype, fn))
+        self.logger.info("Writing %s to %s" % (datatype, fn))
 
         # all output gets reference header information
         _ext = [pyfits.PrimaryHDU(header=self.ref_header)]
 
         # add one or all image datasets
         if (type(data) == list):
             for (extname, d) in data:
@@ -727,40 +1130,128 @@
         # add data provenance, just in case
 
         # now write results
         hdulist = pyfits.HDUList(_ext)
         hdulist.writeto(fn, overwrite=True)
 
         return
+    def apply_reference_pixel_corrections(self):
+
+        n_reads = self.cube_raw.shape[0]
+
+        # prepare jobs for each worker
+        self.logger.info("Preparing jobs for ref pixel correction workers")
+        slice_queue = multiprocessing.JoinableQueue()
+        for slice in range(n_reads):
+            slice_queue.put(slice)
+
+        # start workers (as many as requested, but not more than jobs available)
+        self.logger.info("Starting ref pixel workers")
+        n_workers = numpy.min([self.n_cores, n_reads])
+        worker_processes = []
+        for n in range(n_workers):
+            p = multiprocessing.Process(
+                target=worker__reference_pixel_correction,
+                kwargs=dict(
+                    shmem_cube_raw=self.shmem_cube_raw,
+                    shmem_cube_corrected=self.shmem_cube_linearized,
+                    cube_shape=self.cube_raw.shape,
+                    refpixel_mode=self.use_reference_pixels,
+                    jobqueue=slice_queue,
+                    workername='RefPixelWorker_%03d' % (n+1)
+                ),
+                daemon=True
+            )
+            slice_queue.put(None)
+            p.start()
+            worker_processes.append(p)
+
+        # wait for work to be completed
+        self.logger.info("Waiting for ref pixel work to be done")
+        slice_queue.join()
+
+        # make sure all workers are shut down
+        for p in worker_processes:
+            p.join()
 
+        self.logger.info("All ref pixel correction work complete")
 
-    def reduce(self, dark_fn=None, write_dumps=False, mask_bad_data=None, mask_saturated_pixels=False):
+        pass
+
+    def reduce(self, dark_fn=None, mask_bad_data=None, mask_saturated_pixels=False):
 
         self.load_all_files(mask_saturated_pixels=mask_saturated_pixels)
+        self.logger.info("Done loading all files")
+
+        self.logger.info("Typical interval between reads: %.3f seconds" % (
+            numpy.nanmean(numpy.diff(self.read_times[1:-1]))))
 
         # pyfits.PrimaryHDU(data=self.image_stack).writeto("raw_stack_dmp.fits", overwrite=True)
 
-        self.reference_corrections_cube = numpy.full_like(self.image_stack, fill_value=0.)
+        # self.reference_corrections_cube = numpy.full_like(self.image_stack, fill_value=0.)
 
-        reset_frame_subtracted = self.image_stack.copy()
-        if (self.use_reference_pixels):
-            self.logger.info("Applying reference pixel corrections")
-            for frame_id in range(self.image_stack.shape[0]):
-                reference_pixel_correction = rss_refpixel_calibrate.reference_pixels_to_background_correction(
-                    self.image_stack[frame_id], debug=False,
-                )
-                self.reference_corrections_cube[frame_id] = reference_pixel_correction
-                reset_frame_subtracted[frame_id] -= reference_pixel_correction
+        # reset_frame_subtracted = self.image_stack.copy()
+        # if (self.use_reference_pixels != 'none'):
+        # pyfits.PrimaryHDU(data=self.cube_raw).writeto("cube_raw.fits", overwrite=True)
+        self.dump_save(imgtype='raw')
+
+        self.logger.info("Applying reference pixel corrections [%s]" % (self.use_reference_pixels))
+        self.apply_reference_pixel_corrections()
+        self.dump_save(imgtype='refpixcorr')
+
+        if (not self.nonlinearity_valid()):
+            self.logger.warning("No valid non-linearity correction selected or found, this is not good")
         else:
-            self.logger.info("Subtracting first read from stack")
-            # self.subtract_first_read()
-            # apply first-read subtraction
-            self.reset_frame = self.image_stack[0]
-            self.reference_corrections_cube[:] = self.reset_frame.reshape((-1, self.ny, self.nx))
-            # reset_frame_subtracted = self.image_stack - self.reset_frame
+            self.apply_nonlinearity_corrections()
+        self.dump_save(imgtype='linearized')
+
+        # self.logger.info("Dumping corrected datacube to file")
+        # pyfits.PrimaryHDU(data=self.cube_linearized).writeto("dump_cube.fits", overwrite=True)
+
+        self.fit_pairwise_slopes()
+
+    def dump_save(self, imgtype=None):
+
+        if (not self.write_dumps):
+            # no dumps need to be written
+            return
+        elif ('all' in self.write_dumps):
+            pass
+        elif (not imgtype in self.write_dumps):
+            # this dump is not selected
+            return
+
+        bn = self.filebase + "__"
+        self.logger.debug("Dump-file basename: %s" % (bn))
+
+        if (imgtype == 'raw'):
+            self.dump_data(self.cube_raw, bn+"stack_raw.fits", "RAW")
+        elif (imgtype == 'refpixcorr'):
+            self.dump_data(self.cube_linearized, bn + "stack_refpixcorr.fits", "REFPIXCORR")
+        elif (imgtype == 'linearized'):
+            self.dump_data(self.cube_linearized, bn + "stack_linearized.fits", "LINEARIZED")
+        else:
+            logger.info("Dumping of %s not yet implemented" % (imgtype))
+
+        return
+
+        # for frame_id in range(self.image_stack.shape[0]):
+        #     reference_pixel_correction = reference_pixels_to_background_correction(
+        #         self.image_stack[frame_id], debug=False, mode=self.use_reference_pixels,
+        #     )
+        #     self.reference_corrections_cube[frame_id] = reference_pixel_correction
+        #     reset_frame_subtracted[frame_id] -= reference_pixel_correction
+
+        # else:
+        #     self.logger.info("Subtracting first read from stack")
+        #     # self.subtract_first_read()
+        #     # apply first-read subtraction
+        #     self.reset_frame = self.image_stack[0]
+        #     self.reference_corrections_cube[:] = self.reset_frame.reshape((-1, self.ny, self.nx))
+        #     # reset_frame_subtracted = self.image_stack - self.reset_frame
 
         # print(self.read_times)
         self.logger.info("Typical interval between reads: %.3f seconds" % (
             numpy.nanmean(numpy.diff(self.read_times[1:-1]))))
 
         # apply any necessary corrections for nonlinearity and other things
         self.logger.info("Applying non-linearity corrections")
@@ -794,153 +1285,126 @@
             buffer=self.shmem_image_mask.buf
         )
         self.image_mask[:,:] = 0
 
         # TODO: Add flexibility to have darks either in linear or differential mode
         # for now let's simplify things and assume differential mode only
 
-        # allocate shared memory for the differential stack and calculate from
-        # the linearized cube
-        # calculate differential stack
-        self.logger.debug("Allocating shared memory for differential cube")
-        self.shmem_differential_cube = multiprocessing.shared_memory.SharedMemory(
-            create=True, size=self.linearized_cube.nbytes
-        )
-        self.differential_cube = numpy.ndarray(
-            shape=self.linearized_cube.shape, dtype=numpy.float32,
-            buffer=self.shmem_differential_cube.buf,
-        )
-        self.logger.debug("differential cube allocated")
-
-        self.logger.debug("calculating differential cube")
-        self.differential_read_times = numpy.pad(numpy.diff(self.read_times), (1,0))
-        self.differential_cube[:, :, :] = numpy.pad(
-            numpy.diff(linearized, axis=0), ((1,0),(0,0),(0,0))
-        ) / self.differential_read_times.reshape((-1,1,1))
-        self.logger.debug("diff stack: %s" % (str(self.differential_cube.shape)))
-
-        self.logger.info("Next up (maybe): dark correction")
-        self.apply_dark_correction(dark_fn)
-
-        # mask out all saturated and/or otherwise bad samples
-        max_count_rates = -1000 # TODO: FIX THIS numpy.nanpercentile(self.differential_stack, q=self.saturation_percentile, axis=0)
-        # print("max counrates:", max_count_rates.shape)
-
-        # TODO: implement full iterative outlier rejection here
-        if (mask_bad_data is None):
-            mask_bad_data = self.mask_BAD_DARK | self.mask_SATURATED | self.mask_LOW_RATE | self.mask_NEGATIVE
-        self.logger.info("Identifying bad/dead/saturated/negative pixels (0x%02x)" % (mask_bad_data))
-        bad_data = numpy.zeros_like(self.image_stack, dtype=numpy.bool)
-        if (mask_bad_data is not None and (mask_bad_data & self.mask_SATURATED) > 0):
-            bad_data = bad_data | (self.image_stack > self.saturation_level)
-        if (mask_bad_data is not None and (mask_bad_data & self.mask_LOW_RATE) > 0):
-            bad_data = bad_data | (self.differential_cube < self.saturation_fraction * max_count_rates)
-        # if (mask_bad_data is not None and (mask_bad_data & self.mask_BAD_DARK) > 0):
-        #     bad_data = bad_data | (self.dark_cube >= linearized)
-        # if (mask_bad_data is not None and (mask_bad_data & self.mask_NEGATIVE) > 0):
-            bad_data = bad_data | (linearized < 0)
-
-        self.bad_data_mask = bad_data
-
-        # bad_data = (self.image_stack > self.saturation_level) | \
-        #            (self.differential_stack < self.saturation_fraction*max_count_rates) | \
-        #            (dark_cube >= linearized) | \
-        #            (linearized < 0)
-
-        self.logger.info("Cleaning image cube")
-        self.clean_stack = self.differential_cube.copy()
-        self.clean_stack[bad_data] = numpy.NaN
-        self.clean_stack[0, :, :] = numpy.NaN # mask out the first slice, which is just padding
-        # pyfits.PrimaryHDU(data=self.clean_stack).writeto("darkcorrect___cleanstack.fits", overwrite=True)
-
-        # calculate a average countrate image
-        self.logger.info("calculating final image from stack")
-        # image7 = numpy.nanmean(self.clean_stack[:7], axis=0)
-        self.reduced_image_plain = numpy.nanmean(self.clean_stack, axis=0)
-        noise = numpy.sqrt(self.image_stack)
-        # pyfits.PrimaryHDU(data=noise).writeto("darkcorrect___noise.fits", overwrite=True)
-        noise[bad_data] = numpy.NaN
-        noise[0, :, :] = numpy.NaN
-        self.inv_noise = numpy.nansum(1./noise, axis=0)
-        self.weighted_mean = numpy.nanmean(self.clean_stack, axis=0) # numpy.nansum(self.clean_stack / noise, axis=0) / self.inv_noise
-        self.noise_image = 1. / self.inv_noise
-        # print(image.shape)
-
+        # # allocate shared memory for the differential stack and calculate from
+        # # the linearized cube
+        # # calculate differential stack
+        # self.logger.debug("Allocating shared memory for differential cube")
+        # self.shmem_differential_cube = multiprocessing.shared_memory.SharedMemory(
+        #     create=True, size=self.linearized_cube.nbytes
+        # )
+        # self.differential_cube = numpy.ndarray(
+        #     shape=self.linearized_cube.shape, dtype=numpy.float32,
+        #     buffer=self.shmem_differential_cube.buf,
+        # )
+        # self.logger.debug("differential cube allocated")
+        #
+        # self.logger.debug("calculating differential cube")
+        # self.differential_read_times = numpy.pad(numpy.diff(self.read_times), (1,0))
+        # self.differential_cube[:, :, :] = numpy.pad(
+        #     numpy.diff(linearized, axis=0), ((1,0),(0,0),(0,0))
+        # ) / self.differential_read_times.reshape((-1,1,1))
+        # self.logger.debug("diff stack: %s" % (str(self.differential_cube.shape)))
+        #
+        # self.logger.info("Next up (maybe): dark correction")
+        # self.apply_dark_correction(dark_fn)
+        #
+        # # mask out all saturated and/or otherwise bad samples
+        # max_count_rates = -1000 # TODO: FIX THIS numpy.nanpercentile(self.differential_stack, q=self.saturation_percentile, axis=0)
+        # # print("max counrates:", max_count_rates.shape)
+        #
+        # # TODO: implement full iterative outlier rejection here
+        # if (mask_bad_data is None):
+        #     mask_bad_data = self.mask_BAD_DARK | self.mask_SATURATED | self.mask_LOW_RATE | self.mask_NEGATIVE
+        # self.logger.info("Identifying bad/dead/saturated/negative pixels (0x%02x)" % (mask_bad_data))
+        # bad_data = numpy.zeros_like(self.image_stack, dtype=bool)
+        # if (mask_bad_data is not None and (mask_bad_data & self.mask_SATURATED) > 0):
+        #     bad_data = bad_data | (self.image_stack > self.saturation_level)
+        # if (mask_bad_data is not None and (mask_bad_data & self.mask_LOW_RATE) > 0):
+        #     bad_data = bad_data | (self.differential_cube < self.saturation_fraction * max_count_rates)
+        # # if (mask_bad_data is not None and (mask_bad_data & self.mask_BAD_DARK) > 0):
+        # #     bad_data = bad_data | (self.dark_cube >= linearized)
+        # # if (mask_bad_data is not None and (mask_bad_data & self.mask_NEGATIVE) > 0):
+        #     bad_data = bad_data | (linearized < 0)
+        #
+        # self.bad_data_mask = bad_data
+        #
+        # # bad_data = (self.image_stack > self.saturation_level) | \
+        # #            (self.differential_stack < self.saturation_fraction*max_count_rates) | \
+        # #            (dark_cube >= linearized) | \
+        # #            (linearized < 0)
+        #
+        # self.logger.info("Cleaning image cube")
+        # self.clean_stack = self.differential_cube.copy()
+        # self.clean_stack[bad_data] = numpy.NaN
+        # self.clean_stack[0, :, :] = numpy.NaN # mask out the first slice, which is just padding
+        # # pyfits.PrimaryHDU(data=self.clean_stack).writeto("darkcorrect___cleanstack.fits", overwrite=True)
+        #
+        # # calculate a average countrate image
+        # self.logger.info("calculating final image from stack")
+        # # image7 = numpy.nanmean(self.clean_stack[:7], axis=0)
+        # self.reduced_image_plain = numpy.nanmean(self.clean_stack, axis=0)
+        # noise = numpy.sqrt(self.image_stack)
+        # # pyfits.PrimaryHDU(data=noise).writeto("darkcorrect___noise.fits", overwrite=True)
+        # noise[bad_data] = numpy.NaN
+        # noise[0, :, :] = numpy.NaN
+        # self.inv_noise = numpy.nansum(1./noise, axis=0)
+        # self.weighted_mean = numpy.nanmean(self.clean_stack, axis=0) # numpy.nansum(self.clean_stack / noise, axis=0) / self.inv_noise
+        # self.noise_image = 1. / self.inv_noise
+        # # print(image.shape)
+
+        self.weighted_mean = numpy.zeros((2048,2048))
+        self.noise_image = numpy.zeros((2048,2048))
+        self.median_image = numpy.zeros((2048,2048))
+        readnoise = 20
+        for y in range(2048):
+            self.logger.info("Reconstructing image,y=%d" % (y))
+            for x in range(2048):
+                raw_reads = self.linearized_cube[:,y,x]
+                result = fit_pairwise_slope(
+                    times=self.read_times,
+                    reads=raw_reads,
+                    noise=numpy.sqrt(numpy.fabs(raw_reads) + readnoise**2),
+                    good_reads=None,
+                    plot=False
+                )
+                self.weighted_mean[y,x] = result['weighted']
+                self.noise_image[y,x] = result['sigma']
+                self.median_image[y,x] = result['median']
+
+        pyfits.PrimaryHDU(data=self.weighted_mean).writeto("safety__weightedmean.fits", overwrite=True)
+        pyfits.PrimaryHDU(data=self.noise_image).writeto("safety__sigma.fits", overwrite=True)
+        pyfits.PrimaryHDU(data=self.median_image).writeto("safety__median.fits", overwrite=True)
         # ratios = linearized / linearized[3:4, :, :]
 
-        if (write_dumps):
-            self.logger.info("Writing all dumps")
-            bn = self.filebase + "__"
-            self.logger.debug("Dump-file basename: %s" % (bn))
-            if ('rawstack' in write_dumps):
-                self.dump_data(self.image_stack, bn+"stack_raw.fits", "rawstack")
-            if ("zerosubstack" in write_dumps):
-                self.dump_data(data=self.image_stack,
-                               fn=bn+"stack_zerosub.fits",
-                               datatype='zerosubstack')
-            if ('linearstack' in write_dumps or 'fordark' in write_dumps):
-                self.dump_data(data=linearized,
-                               fn=bn+"stack_linearized.fits",
-                               datatype='linearstack')
-            if ('darkstack' in write_dumps):
-                self.dump_data(data=dark_cube,
-                               fn=bn+"stack_darkcube.fits",
-                               datatype='darkstack')
-            if ('diffstack' in write_dumps or 'fordark' in write_dumps):
-                self.dump_data(data=self.differential_cube,
-                               fn=bn + "stack_diff.fits",
-                               datatype='diffstack')
-            if ('cleanstack' in write_dumps):
-                self.dump_data(data=self.clean_stack,
-                               fn=bn+"stack_clean.fits",
-                               datatype='cleanstack')
-            # pyfits.PrimaryHDU(data=ratios).writeto("stack_ratios.fits", overwrite=True)
-            # pyfits.PrimaryHDU(data=self.reduced_image_plain).writeto("final_image.fits", overwrite=True)
-            # pyfits.PrimaryHDU(data=image7).writeto("final_image7.fits", overwrite=True)
-            # pyfits.PrimaryHDU(data=max_count_rates).writeto("max_count_rates.fits", overwrite=True)
-            # pyfits.PrimaryHDU(data=bad_data.astype(numpy.int)).writeto(bn+"bad_data.fits", overwrite=True)
-            if ('weighted' in write_dumps):
-                self.dump_data(data=self.weighted_mean,
-                               fn=bn+"final_image_weighted.fits",
-                               datatype='weighted')
-            if ('noise' in write_dumps):
-                self.dump_data(data=self.inv_noise,
-                               fn=bn+"final_inv_noise.fits",
-                               datatype='noise')
-
-            if ('ngoodpixels' in write_dumps):
-                n_good_pixels = numpy.sum(~bad_data, axis=0)
-                print("#goodpixels", n_good_pixels.shape)
-                self.dump_data(data=n_good_pixels,
-                               fn=bn+"n_good_pixels.fits", overwrite=True)
 
         return
-
     def subtract_first_read(self):
         if (self.first_read_subtracted):
             self.logger.debug("First read already subtracted, skipping")
             return
 
         if (self.first_read is None):
             self.first_read = self.image_stack[0].copy()
 
         self.image_stack -= self.first_read
         self.first_read_subtracted = True
-
     def _nonlinearity_fit_fct(self, p, x):
         y = numpy.zeros(x.shape)
         for i in range(p.shape[0]):
             y += p[i] * x**(i+1)
         return y
-
     def _nonlinearity_fit_err_fct(self, p, x, y):
         yfit = self._nonlinearity_fit_fct(p, x)
         err = numpy.sqrt(y + 10 ** 2)
         return ((y - yfit) / err)
-
     def _fit_nonlinearity_pixel(self, _x, _y):
         # print("fitting", _x.shape, _y.shape)
         # return 1
 
         # define two sub-routines we need for the fitting
 
 
@@ -962,15 +1426,14 @@
             func=self._nonlinearity_fit_err_fct, x0=pinit,
             args=(x, y),
             full_output=1
         )
         pfit = fit[0]
 
         return pfit
-
     def fit_nonlinearity(self, ref_frame_id=10, max_linear=50000, make_plot=False):
 
         # self.subtract_first_read()
         # if (self.first_read_subtracted):
         #     bad_data = (self.image_stack + self.first_read) > max_linear
         # else:
         #     bad_data = self.image_stack > max_linear
@@ -1134,15 +1597,14 @@
             #break
 
         # return
 
         pyfits.PrimaryHDU(data=nonlinearity_fits_3d).writeto("nonlin3d.fits", overwrite=True)
         pyfits.PrimaryHDU(data=nonlinearity_fits_inverse).writeto("nonlin_inverse.fits", overwrite=True)
         return
-
     def read_nonlinearity_corrections(self, nonlin_fn):
 
         self.logger.debug("Reading non-linearity: %s (file exists: %s)" % (
             nonlin_fn, os.path.isfile(nonlin_fn)))
         if (os.path.isfile(nonlin_fn)):
             try:
                 self.logger.info("Reading nonlinearity corrections from %s" % (nonlin_fn))
@@ -1153,70 +1615,139 @@
             except Exception as e:
                 self.logger.error(str(e))
                 return False
 
         self.provenance.add("nonlinearity", nonlin_fn)
         self.nonlin_fn = nonlin_fn
         self.nonlinearity_cube = nonlinearity_cube
+    def apply_nonlinearity_corrections(self, img_cube=None):
 
+        pyfits.PrimaryHDU(data=self.cube_linearized).writeto("cube_before_nonlin.fits", overwrite=True)
 
-    def apply_nonlinearity_corrections(self, img_cube=None):
+        self.logger.info("Starting nonlinearity correction")
+        t1 = time.time()
+        jobqueue = multiprocessing.JoinableQueue()
+        for y in range(2048):
+            jobqueue.put(y)
 
-        if (self.nonlinearity_cube is None):
-            self.logger.warning("No nonlinearity corrections loaded, skipping")
-            return None
+        # setup and start worker processes
+        worker_processes = []
+        n_workers = self.n_cores
+        for n in range(n_workers):
+            p = multiprocessing.Process(
+                target=worker__nonlinearity_correction,
+                kwargs=dict(shmem_cube_corrected=self.shmem_cube_linearized,
+                            shmem_corrections=self.shmem_cube_nonlinearity,
+                            cube_shape=self.cube_raw.shape,
+                            corrections_shape=self.cube_nonlinearity.shape,
+                            jobqueue=jobqueue,
+                            workername="NonLinWorker_%03d" % (n+1),
+                ),
+                daemon=True
+            )
+            jobqueue.put(None)
+            p.start()
+            worker_processes.append(p)
 
-        # self.subtract_first_read()
-        if (img_cube is None):
-            img_cube = self.image_stack
+        # wait for work to be done
+        self.logger.info("Working for all nonlinearity correction jobs to finish")
+        jobqueue.join()
+        for p in worker_processes:
+            p.join()
 
-        self.logger.debug("NONLIN: data=%s   corr=%s" % (str(img_cube.shape), str(self.nonlinearity_cube.shape)))
+        t2 = time.time()
 
-        linearized_cube = \
-            self.nonlinearity_cube[0:1, :, :] * numpy.power(img_cube, 1) + \
-            self.nonlinearity_cube[1:2, :, :] * numpy.power(img_cube, 2) + \
-            self.nonlinearity_cube[2:3, :, :] * numpy.power(img_cube, 3)
+        self.logger.info("Non-linearity correction complete after taking %.3f seconds" % (t2-t1))
+        pyfits.PrimaryHDU(data=self.cube_linearized).writeto("cube_after_nonlin.fits", overwrite=True)
+        return
 
-        return linearized_cube
+    def fit_pairwise_slopes(self):
 
+        self.logger.info("Start of fit pairwise slopes")
+        t1 = time.time()
+        jobqueue = multiprocessing.JoinableQueue()
+        for y in range(4, 2048-4):
+            jobqueue.put(y)
+
+        # setup and start worker processes
+        worker_processes = []
+        n_workers = self.n_cores
+        for n in range(n_workers):
+            p = multiprocessing.Process(
+                target=worker__fit_pairwise_slopes,
+                kwargs=dict(
+                    shmem_cube_corrected=self.shmem_cube_linearized,
+                    shmem_results=self.shmem_cube_results,
+                    cube_shape=self.cube_linearized.shape,
+                    results_shape=self.cube_results.shape,
+                    jobqueue=jobqueue,
+                    workername="PairSlopeWorker_%03d" % (n+1),
+                    read_times=self.read_times,
+                    speedy=self.speedy,
+                ),
+                daemon=True
+            )
+            jobqueue.put(None)
+            p.start()
+            worker_processes.append(p)
+
+        # wait for work to be done
+        self.logger.info("Waiting for all pairwise slope-fitting jobs to finish")
+        jobqueue.join()
+        for p in worker_processes:
+            p.join()
+
+        t2 = time.time()
+
+        self.logger.info("Pairwise slope-fitting complete after taking %.3f seconds" % (t2-t1))
+        # pyfits.PrimaryHDU(data=self.cube_linearized).writeto("cube_after_nonlin.fits", overwrite=True)
+        return
 
     def write_results(self, fn=None, flat4salt=False):
         if (fn is None):
             fn = os.path.join(self.basedir, self.filebase) + ".reduced.fits"
 
         # collect all output results
         _list = [pyfits.PrimaryHDU(header=self.ref_header)]
         if (flat4salt):
+            self.logger.info("Writing flattened version of output")
             # only write the reduced frame and nothing else
             try:
                 img = self.persistency_fit_global[:, :, 0]
                 hdu = pyfits.ImageHDU(data=img, name="SCI")
                 hdr = hdu.header
                 hdr['FIT_PERS'] = (True, "true persistency results")
             except:
                 img = self.weighted_mean
                 hdu = pyfits.ImageHDU(data=img, name="SCI")
                 hdr = hdu.header
                 hdr['FIT_PERS'] = (False, "true persistency results")
             _list.append(hdu)
         else:
-            _list.extend([
-                pyfits.ImageHDU(data=self.weighted_mean, name="SCI"),
-                pyfits.ImageHDU(data=self.noise_image, name='NOISE')
-            ])
-            try:
-                for i,extname in enumerate(persistency_values):
-                    _list.append(
-                        pyfits.ImageHDU(
-                            data=rss.persistency_fit_global[i, :, :],
-                            name=extname)
-                    )
-            except:
-                pass
+            self.logger.info("Writing output in MEF format")
+            for i,name in enumerate(self.RESULT_EXTENSIONS):
+                _list.append(pyfits.ImageHDU(data=self.cube_results[i], name=name))
+            # _list.extend([
+            #     pyfits.ImageHDU(data=self.cube_results[0], name="SCI"),
+            #     pyfits.ImageHDU(data=self.cube_results[2], name='NOISE'),
+            #     pyfits.ImageHDU(data=self.cube_results[1], name='MEDIAN'),
+            # ])
+            # try:
+            #     for i,extname in enumerate(persistency_values):
+            #         self.logger.debug("Adding MEF extension: %s" % (extname))
+            #         _list.append(
+            #             pyfits.ImageHDU(
+            #                 data=self.persistency_fit_global[i, :, :],
+            #                 name=extname)
+            #         )
+            # except Exception as e:
+            #     self.logger.critical(str(e))
+            #     pass
 
+        self.logger.debug("Adding data provenance")
         _list.append(self.provenance.write_as_hdu())
 
         hdulist = pyfits.HDUList(_list)
         self.logger.info("Writing reduced results to %s" % (fn))
         hdulist.writeto(fn, overwrite=True)
         return
 
@@ -1228,21 +1759,15 @@
         )
         self.persistency_fit_global = numpy.ndarray(
             shape=(n_persistency_values, self.ny, self.ny), dtype=numpy.float32,
             buffer=self.shmem_persistency_fit_global.buf,
         )
         self.persistency_fit_global[:,:,:] = numpy.NaN
         self.alloc_persistency = True
-
-    def fit_signal_with_persistency(
-            self,
-            n_workers=0,
-            previous_frame=None,
-            write_test_plots=False
-    ):
+    def fit_signal_with_persistency(self, n_workers=0, previous_frame=None, write_test_plots=False):
 
         # by default use all existing CPU cores for processing
         if (n_workers <= 0):
             n_workers = multiprocessing.cpu_count()
 
         if (not self.alloc_persistency):
             self._alloc_persistency()
@@ -1299,15 +1824,14 @@
             t.join()
 
         # for now write the fit output
         self.logger.debug("dumping fit results")
         out_tmp = pyfits.PrimaryHDU(data=self.persistency_fit_global)
         out_tmp.writeto("persistency_fit_dump.fits", overwrite=True)
         return
-
     def fit_signal_with_persistency_singlepixel(self, x, y, debug=False, plot=False):
 
         _x = x - 1
         _y = y - 1
 
         bad_data = self.bad_data_mask[:, _y, _x]
         rate_series = self.differential_cube[:, _y, _x]
@@ -1378,15 +1902,14 @@
             fig.suptitle("F = %.0f + %.0f x exp(-t/%.3fs)" % (bestfit[0], bestfit[1], bestfit[2]))
             ax.set_xlabel("integration time [seconds]")
             ax.set_ylabel("flux above read #0 [counts]")
             fig.savefig(plot_fn, dpi=200)
             plt.close(fig)
 
         return bestfit, fit_uncert
-
     def plot_pixel_curve(self, x, y, filebase=None,
                          cumulative=True, differential=False,
                          diff_vs_cum=False,
                          show_fits=False, show_errors=False,
                          show_plot=False):
 
         # self.subtract_first_read()
@@ -1479,16 +2002,14 @@
             fig.savefig(plot_fn)
 
             if (show_plot):
                 fig.show()
             else:
                 plt.close(fig)
             # plt.close(fig)
-
-
     def dump_pixeldata(self, x, y, filebase=None, extras=None):
 
         self.logger.debug("dumping pixeldata for pixel @ %d / %d" % (x,y))
 
         _x = x-1
         _y = y-1
         frame_number = numpy.arange(self.image_stack.shape[0])
@@ -1507,16 +2028,14 @@
             except:
                 pass
 
         numpy.savetxt(fn, numpy.array([
             frame_number, raw_series, linearized
             ]+extra_pixels).T
         )
-
-
     def _parallel_worker(self, job_queue, result_queue, execute_function, is_in_class=True):
         self.logger.debug("Worker has started")
         while (True):
             job = job_queue.get()
             if (job is None):
                 job_queue.task_done()
                 self.logger.debug("Worker shutting down")
@@ -1529,16 +2048,14 @@
                 result = execute_function(x, y)
             else:
                 result = execute_function(self, x, y)
 
             result_queue.put((x, y, result))
 
             job_queue.task_done()
-
-
     def parallel_fitter(self, xrange=None, yrange=None,
                         execute_function=None, return_dim=1, is_in_class=True,
                         n_workers=None):
 
         if (xrange is None):
             x1 = 0
             x2 = self.image_stack.shape[2]
@@ -1605,17 +2122,14 @@
         # receive all the results back from the workers
         for j in range(n_jobs):
             result = result_queue.get()
             (x,y,value) = result
             return_results[:, y-y1,x-x1] = value
 
         return return_results
-
-
-
     def fit_2component_persistency_plus_signal(self, x, y):
 
         _x = x-1
         _y = y-1
 
         raw_data = self.image_stack[:, _y, _x]
         bad_data = raw_data > self.saturation_level
@@ -1626,15 +2140,15 @@
             series = self.image_stack[:,_y,_x]
 
         if (numpy.sum(~bad_data) < 5):
             return [numpy.NaN, numpy.NaN, numpy.NaN]
 
         pinit = [1., 0.] #, 1.]
 
-        readout_times = numpy.arange(series.shape[0], dtype=numpy.float) * self.diff_exptime
+        readout_times = numpy.arange(series.shape[0], dtype=float) * self.diff_exptime
         img_time = readout_times[~bad_data]
         img_flux = series[~bad_data]
 
         fit = scipy.optimize.leastsq(
             func=_persistency_plus_signal_fit_err_fct, x0=pinit,
             args=(img_time, img_flux),
             full_output=1
@@ -1642,15 +2156,14 @@
         # print(fit)
         pfit = fit[0]
 
         # bestfit = _fit_persistency_plus_signal_pixel(
         #     integ_exp_time[~bad_data], series[~bad_data])
 
         return pfit #self.image_stack[1, y-1, x-1]
-
     def load_precalculated_results(self, weighted_image_fn=None, persistency_fit_fn=None):
 
         if (weighted_image_fn is not None and os.path.isfile(weighted_image_fn)):
             self.logger.warning("Loading weighted results from file isn't implemented yet")
             pass
 
         if (persistency_fit_fn is not None and os.path.isfile(persistency_fit_fn)):
@@ -1665,166 +2178,41 @@
             )
             hdulist = pyfits.open(persistency_fit_fn)
             self.persistency_fit_global[:,:,:] = hdulist[0].data[:,:,:]
         else:
             self.logger.warning("Unable to load previous persistency results (%s)" % (persistency_fit_fn))
 
             pass
-
     def find_previous_exposure(self, search_dir):
 
         self.logger.debug("Finding previous exposure (%s)" % (search_dir))
 
         dir_index = rss_filepicker.PreviousFilePicker(search_dir)
         prior_fn, delta_seconds = dir_index.find_closest(self.ref_header)
 
         if (prior_fn is None):
             self.logger.warn("Unable to find prior frame as persistency reference")
         else:
             self.logger.info("Found %s, taken %.2f seconds prior to %s" % (prior_fn, delta_seconds, self.ref_header['FILE']))
 
         return prior_fn, delta_seconds
-
-
     def __del__(self):
+        self.logger.info("Releasing shared memory allocations")
         # self.logger.debug("Running destructor and cleaning up shared memory")
         # clean up shared memory
-        try:
-            self.shmem_linearized_cube.close()
-            self.shmem_linearized_cube.unlink()
-        except:
-            pass
-
-        try:
-            self.shmem_differential_cube.close()
-            self.shmem_differential_cube.unlink()
-        except:
-            pass
-
-        try:
-            self.shmem_persistency_fit_global.close()
-            self.shmem_persistency_fit_global.unlink()
-        except:
-            pass
-
-
-if __name__ == "__main__":
-
-    mplog.setup_logging(debug_filename="../../debug.log",
-                        log_filename="run_analysis.log")
-    mpl_logger = logging.getLogger('matplotlib')
-    mpl_logger.setLevel(logging.WARNING)
-
-    logger = logging.getLogger("RunAnalysis")
-
-    cmdline = argparse.ArgumentParser()
-    cmdline.add_argument("--maxfiles", dest="max_number_files", default=None, type=int,
-                         help="limit number of files to load for processing")
-    cmdline.add_argument("--nonlinearity", dest="nonlinearity_fn", type=str, default=None,
-                         help="non-linearity correction coefficients (3-d FITS cube)")
-    cmdline.add_argument("--flat", dest="flatfield_fn", type=str, default=None,
-                         help="calibration flatfield")
-    cmdline.add_argument("--dark", dest="dark_fn", type=str, default=None,
-                         help="calibration dark")
-    cmdline.add_argument("--output", dest="output_postfix", type=str, default="reduced",
-                         help="addition to output filename")
-
-    cmdline.add_argument("--persistency", dest="persistency_mode", type=str, default="quick",
-                         help="persistency mode")
-    cmdline.add_argument("--saturation", dest="saturation", default=62000,
-                         help="saturation value/file")
-
-    # cmdline.add_argument("healpix32", nargs="+", type=int,
-    #                      help="list of input filenames")
-    # cmdline.add_argument("--rerun", type=int, default=6,
-    #                      help="rerun")
-    cmdline.add_argument("--dumps", dest="write_dumps", default=None,
-                         help="write intermediate process data [default: NO]")
-    cmdline.add_argument("--debugpngs", dest="write_debug_pngs", default=False, action='store_true',
-                         help="generate debug plots for all pixels with persistency [default: NO]")
-    cmdline.add_argument("--refpixel", dest="use_ref_pixels", default=False, action='store_true',
-                         help="use reference pixels [default: NO]")
-    cmdline.add_argument("--flat4salt", dest="write_flat_for_salt", default=False, action='store_true',
-                         help="write a flat, 1-extension FITS file for SALT")
-    cmdline.add_argument("files", nargs="+",
-                         help="list of input filenames")
-    args = cmdline.parse_args()
-
-    dumpfiles = []
-    if (args.write_dumps is not None):
-        for di in [x.lower() for x in args.write_dumps.split(",")]:
-            if (di in dump_options):
-                dumpfiles.append(di)
-
-    for fn in args.files:
-        # fn = sys.argv[1]
-
-        rss = RSS(fn, max_number_files=args.max_number_files,
-                  use_reference_pixels=args.use_ref_pixels,
-                  saturation=args.saturation,
-                  )
-
-        if (args.nonlinearity_fn is not None and os.path.isfile(args.nonlinearity_fn)):
-            logger.info("Attempting to load non-linearity from %s" % (args.nonlinearity_fn))
-            rss.read_nonlinearity_corrections(args.nonlinearity_fn)
-        rss.reduce(write_dumps=dumpfiles,
-                   dark_fn=args.dark_fn,
-                   )
-
-        persistency_options = args.persistency_mode.split(":")
-        persistency_mode = persistency_options[0].lower()
-        have_persistency_results = False
-        if (persistency_mode == "none"):
-            logger.info("Nothing to do")
-        elif (persistency_mode == "full"):
-            logger.info("Calculating persistency results for all pixels")
-            rss.fit_signal_with_persistency(previous_frame=None)
-            have_persistency_results = True
-        elif (persistency_mode == "best"):
-            logger.info("Using on-demand persistency fitting")
-            if(len(persistency_options) < 2):
-                logger.info("Insufficient information, defaulting to running on all pixels")
-                rss.fit_signal_with_persistency(previous_frame=None)
-                have_persistency_results = True
-            else:
-                opt = persistency_options[1]
-                if (os.path.isfile(opt)):
-                    logger.info("Using optimized persistency mode (ref-fn: %s)" % (opt))
-                    rss.fit_signal_with_persistency(previous_frame=opt)
-                    have_persistency_results = True
-                elif (os.path.isdir(opt)):
-                    logger.info("Searching for optimal reference frame in --> %s <--" % (opt))
-                    xxx = rss.find_previous_exposure(opt)  #find_previous_frame(rss.ref_header, opt)
-                    # print(xxx)
-                    ref_fn, delta_t = xxx #rss.find_previous_exposure(opt)  #find_previous_frame(rss.ref_header, opt)
-                    if (ref_fn is not None):
-                        logger.info("Using optimized persistency mode using automatic ref-fn: %s (Dt=%.3f)" % (ref_fn, delta_t))
-                        rss.fit_signal_with_persistency(previous_frame=ref_fn,
-                                                        write_test_plots=args.write_debug_pngs)
-                        have_persistency_results = True
-                    else:
-                        logger.warning("No previous frame found, skipping persistency fit")
-                        # rss.fit_signal_with_persistency(previous_frame=ref_fn)
-                        # have_persistency_results = True
-                else:
-                    logger.info("Unknown option to best mode (found: %s), skipping persistency modeling" % (opt))
-        else:
-            logger.info("Unknown persistency request (%s)" % (persistency_mode))
 
-        if (have_persistency_results):
-            out_tmp = pyfits.PrimaryHDU(data=rss.persistency_fit_global)
-            fit_fn = "%s.%s.persistencyfit.fits" % (rss.filebase, args.output_postfix)
-            logger.info("Writing persistency fit to %s ..." % (fit_fn))
-            out_tmp.writeto(fit_fn, overwrite=True)
-
-        red_fn = "%s.%s.fits" % (rss.filebase, args.output_postfix)
-        logger.info("Writing reduction results to %s" % (red_fn))
-        rss.write_results(fn=red_fn, flat4salt=args.write_flat_for_salt)
-
-        rss.provenance.report()
-
-        # rss.plot_pixel_curve(818,1033)
-        # rss.plot_pixel_curve(1700,555)
-        # rss.plot_pixel_curve(505,1660)
+        for shmem in [
+            self.shmem_cube_raw,
+            self.shmem_cube_linearized,
+            self.shmem_cube_results,
+            self.shmem_cube_nonlinearity,
+            ]:
+            if (shmem is None):
+                continue
+            try:
+                shmem.close()
+                shmem.unlink()
+            except Exception as e:
+                self.logger.warning("Error releasing shared memory: %s" % (str(e)))
+                pass
 
-        del rss
-        print("all done!")
+        self.logger.debug("All done releasing shared memory")
```

### Comparing `nirwals-0.0.1/src/nirwals/plotcube.py` & `nirwals-0.0.5/src/nirwals/plotcube.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import os
 import sys
 import numpy
 import astropy.io.fits as pyfits
 
 import matplotlib.pyplot as plt
 
-import nirwals_reduce
+import nirwals
 
 if __name__ == "__main__":
 
     fn = sys.argv[1]
-    rss = rss_reduce.RSS(fn)
+    rss = rss_reduce.NIRWALS(fn)
     rss.load_all_files()
 
     # rss.read_nonlinearity_corrections("nonlin_inverse.fits")
     rss.read_nonlinearity_corrections("nonlin3d.fits")
 
     coord_list_fn = sys.argv[2]
     lines = []
```

### Comparing `nirwals-0.0.1/src/nirwals/provenance.py` & `nirwals-0.0.5/src/nirwals/provenance.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,19 +96,21 @@
 
         tbhdu = pyfits.BinTableHDU.from_columns(coldefs)
         tbhdu.name = "PROVENANCE"
 
         return tbhdu
 
     def report(self):
-        print("\n ==== DATA PROVENANCE INVENTORY ==== ")
+        inv = []
+        inv.append("\n ==== DATA PROVENANCE INVENTORY ==== ")
         for key in self.inventory:
             for fn in self.inventory[key]:
-                print("% 20s: %s" % (key, fn))
-        print(" ==== DATA PROVENANCE INVENTORY END ==== ")
+                inv.append("% 20s: %s" % (key, fn))
+        inv.append(" ==== DATA PROVENANCE INVENTORY END ==== ")
+        self.logger.info("\n".join(inv))
         return
 
 
     def read_from_fits(self, filename, extname='PROVENANCE'):
         hdulist = pyfits.open(filename)
 
         tbhdu = hdulist[extname]
```

### Comparing `nirwals-0.0.1/src/nirwals/single_pixel_check.py` & `nirwals-0.0.5/src/nirwals/single_pixel_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import numpy
 import astropy.io.fits as pyfits
 import matplotlib
 import matplotlib.pyplot as plt
 import argparse
 
-import nirwals_reduce
+import nirwals
 
 
 if __name__ == "__main__":
 
     cmdline = argparse.ArgumentParser()
     cmdline.add_argument("--maxfiles", dest="max_number_files", default=None, type=int,
                          help="limit number of files to load for processing")
@@ -29,15 +29,15 @@
     args = cmdline.parse_args()
 
     if (args.write_dumps):
         print("File-dumping enabled!")
 
     for fn in args.files:
 
-        rss = rss_reduce.RSS(fn)
+        rss = rss_reduce.NIRWALS(fn)
         # rss.reduce(write_dumps=False)
         # rss.write_results()
 
         x = int(sys.argv[2])
         y = int(sys.argv[3])
         _x = x - 1
         _y = y - 1
```

### Comparing `nirwals-0.0.1/src/nirwals.egg-info/SOURCES.txt` & `nirwals-0.0.5/src/nirwals.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,21 @@
-.gitignore
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-.github/workflows/release_to_pypi.yml
-dev/check_variance.py
-dev/compare_ramps.py
-dev/dev__frames2urg.py
-dev/dirty_dark_subtract.py
-dev/find_naughty_pixels.py
-dev/make_pixellist.py
-dev/plot_and_fit_curves.py
+src/nirwals_fit_nonlinearity.py
+src/nirwals_makedark.py
+src/nirwals_makemasterdark.py
+src/nirwals_reduce.py
 src/nirwals/__init__.py
-src/nirwals/dev__cubeinspect.py
-src/nirwals/dev__cubemath.py
-src/nirwals/dev__dummyplot.py
-src/nirwals/dev__extract_reference_pixels.py
-src/nirwals/dev__find_previous_frame.py
-src/nirwals/dev__fitpersistencysignal.py
-src/nirwals/dev__fixbiasdips.py
-src/nirwals/dev__mptest.py
-src/nirwals/dev__pairwise_overscan_subtract.py
-src/nirwals/dev__rowaverage.py
 src/nirwals/edge_subtract.py
-src/nirwals/mpfitter.py
-src/nirwals/mplogging.py
-src/nirwals/nirwals__fit_nonlinearity.py
-src/nirwals/nirwals_cubecombine.py
-src/nirwals/nirwals_darkcorrect.py
+src/nirwals/nirwals.py
 src/nirwals/nirwals_explorer.py
-src/nirwals/nirwals_extractHDU.py
-src/nirwals/nirwals_filepicker.py
-src/nirwals/nirwals_makedark.py
-src/nirwals/nirwals_makemasterdark.py
-src/nirwals/nirwals_plotpixel.py
-src/nirwals/nirwals_reduce.py
-src/nirwals/nirwals_refpixel_calibrate.py
 src/nirwals/plotcube.py
+src/nirwals/previous_file_picker.py
 src/nirwals/provenance.py
+src/nirwals/refpixel_calibrate.py
 src/nirwals/single_pixel_check.py
 src/nirwals.egg-info/PKG-INFO
 src/nirwals.egg-info/SOURCES.txt
 src/nirwals.egg-info/dependency_links.txt
 src/nirwals.egg-info/top_level.txt
```


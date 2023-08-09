# Comparing `tmp/cvxpy-1.3.1.tar.gz` & `tmp/cvxpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpy-1.3.1.tar", last modified: Sat Mar 18 20:40:24 2023, max compression
+gzip compressed data, was "cvxpy-1.3.2.tar", last modified: Tue Jun 27 08:01:18 2023, max compression
```

## Comparing `cvxpy-1.3.1.tar` & `cvxpy-1.3.2.tar`

### file list

```diff
@@ -1,783 +1,783 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.491191 cvxpy-1.3.1/
--rw-r--r--   0 runner     (501) staff       (20)    11344 2023-03-18 20:33:39.000000 cvxpy-1.3.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      102 2023-03-18 20:33:39.000000 cvxpy-1.3.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     9055 2023-03-18 20:40:24.491523 cvxpy-1.3.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6949 2023-03-18 20:33:39.000000 cvxpy-1.3.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.627422 cvxpy-1.3.1/cvxpy/
--rw-r--r--   0 runner     (501) staff       (20)     2160 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.698100 cvxpy-1.3.1/cvxpy/atoms/
--rw-r--r--   0 runner     (501) staff       (20)     5256 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.713510 cvxpy-1.3.1/cvxpy/atoms/affine/
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3967 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/add_expr.py
--rw-r--r--   0 runner     (501) staff       (20)     5719 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/affine_atom.py
--rw-r--r--   0 runner     (501) staff       (20)    14584 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/binary_operators.py
--rw-r--r--   0 runner     (501) staff       (20)     1137 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/bmat.py
--rw-r--r--   0 runner     (501) staff       (20)     2313 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/conj.py
--rw-r--r--   0 runner     (501) staff       (20)     3469 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/conv.py
--rw-r--r--   0 runner     (501) staff       (20)     4371 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/cumsum.py
--rw-r--r--   0 runner     (501) staff       (20)     4741 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/diag.py
--rw-r--r--   0 runner     (501) staff       (20)     1644 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/diff.py
--rw-r--r--   0 runner     (501) staff       (20)     2977 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/hstack.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/imag.py
--rw-r--r--   0 runner     (501) staff       (20)     6401 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/index.py
--rw-r--r--   0 runner     (501) staff       (20)     4379 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/kron.py
--rw-r--r--   0 runner     (501) staff       (20)     3312 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/partial_trace.py
--rw-r--r--   0 runner     (501) staff       (20)     3365 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/partial_transpose.py
--rw-r--r--   0 runner     (501) staff       (20)     3204 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/promote.py
--rw-r--r--   0 runner     (501) staff       (20)     1486 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/real.py
--rw-r--r--   0 runner     (501) staff       (20)     4440 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/reshape.py
--rw-r--r--   0 runner     (501) staff       (20)     3553 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/sum.py
--rw-r--r--   0 runner     (501) staff       (20)     2937 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/trace.py
--rw-r--r--   0 runner     (501) staff       (20)     2872 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/transpose.py
--rw-r--r--   0 runner     (501) staff       (20)     2752 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/unary_operators.py
--rw-r--r--   0 runner     (501) staff       (20)     4346 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/upper_tri.py
--rw-r--r--   0 runner     (501) staff       (20)     1108 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/vec.py
--rw-r--r--   0 runner     (501) staff       (20)     3033 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/vstack.py
--rw-r--r--   0 runner     (501) staff       (20)     3746 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/affine/wraps.py
--rw-r--r--   0 runner     (501) staff       (20)    16154 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/atom.py
--rw-r--r--   0 runner     (501) staff       (20)     4313 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/axis_atom.py
--rw-r--r--   0 runner     (501) staff       (20)     3132 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/condition_number.py
--rw-r--r--   0 runner     (501) staff       (20)     2943 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/cummax.py
--rw-r--r--   0 runner     (501) staff       (20)     2423 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/dist_ratio.py
--rw-r--r--   0 runner     (501) staff       (20)     4928 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/dotsort.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.727699 cvxpy-1.3.1/cvxpy/atoms/elementwise/
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2457 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/abs.py
--rw-r--r--   0 runner     (501) staff       (20)     4790 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/ceil.py
--rw-r--r--   0 runner     (501) staff       (20)     2414 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/elementwise.py
--rw-r--r--   0 runner     (501) staff       (20)     2746 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/entr.py
--rw-r--r--   0 runner     (501) staff       (20)     2358 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/exp.py
--rw-r--r--   0 runner     (501) staff       (20)     3520 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/huber.py
--rw-r--r--   0 runner     (501) staff       (20)      703 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/inv_pos.py
--rw-r--r--   0 runner     (501) staff       (20)     3009 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/kl_div.py
--rw-r--r--   0 runner     (501) staff       (20)     2757 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/log.py
--rw-r--r--   0 runner     (501) staff       (20)     2046 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/log1p.py
--rw-r--r--   0 runner     (501) staff       (20)     2052 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/log_normcdf.py
--rw-r--r--   0 runner     (501) staff       (20)     1419 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/loggamma.py
--rw-r--r--   0 runner     (501) staff       (20)     2345 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/logistic.py
--rw-r--r--   0 runner     (501) staff       (20)     3519 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/maximum.py
--rw-r--r--   0 runner     (501) staff       (20)     3222 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/minimum.py
--rw-r--r--   0 runner     (501) staff       (20)      699 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/neg.py
--rw-r--r--   0 runner     (501) staff       (20)      696 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/pos.py
--rw-r--r--   0 runner     (501) staff       (20)    14794 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/power.py
--rw-r--r--   0 runner     (501) staff       (20)     2988 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/rel_entr.py
--rw-r--r--   0 runner     (501) staff       (20)      779 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/scalene.py
--rw-r--r--   0 runner     (501) staff       (20)      739 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/sqrt.py
--rw-r--r--   0 runner     (501) staff       (20)      691 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/square.py
--rw-r--r--   0 runner     (501) staff       (20)     2682 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/elementwise/xexp.py
--rw-r--r--   0 runner     (501) staff       (20)     3300 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/eye_minus_inv.py
--rw-r--r--   0 runner     (501) staff       (20)     3518 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/gen_lambda_max.py
--rw-r--r--   0 runner     (501) staff       (20)    11946 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/geo_mean.py
--rw-r--r--   0 runner     (501) staff       (20)     4909 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/gmatmul.py
--rw-r--r--   0 runner     (501) staff       (20)     1292 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/harmonic_mean.py
--rw-r--r--   0 runner     (501) staff       (20)     1197 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/inv_prod.py
--rw-r--r--   0 runner     (501) staff       (20)     3291 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/lambda_max.py
--rw-r--r--   0 runner     (501) staff       (20)      811 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/lambda_min.py
--rw-r--r--   0 runner     (501) staff       (20)     2318 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/lambda_sum_largest.py
--rw-r--r--   0 runner     (501) staff       (20)      834 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/lambda_sum_smallest.py
--rw-r--r--   0 runner     (501) staff       (20)     2282 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/length.py
--rw-r--r--   0 runner     (501) staff       (20)     3645 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/log_det.py
--rw-r--r--   0 runner     (501) staff       (20)     2690 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/log_sum_exp.py
--rw-r--r--   0 runner     (501) staff       (20)     4538 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/matrix_frac.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/max.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/min.py
--rw-r--r--   0 runner     (501) staff       (20)     1304 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/mixed_norm.py
--rw-r--r--   0 runner     (501) staff       (20)     3098 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/norm.py
--rw-r--r--   0 runner     (501) staff       (20)     3212 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/norm1.py
--rw-r--r--   0 runner     (501) staff       (20)     3376 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/norm_inf.py
--rw-r--r--   0 runner     (501) staff       (20)     2271 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/norm_nuc.py
--rw-r--r--   0 runner     (501) staff       (20)     2801 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/one_minus_pos.py
--rw-r--r--   0 runner     (501) staff       (20)     4220 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/perspective.py
--rw-r--r--   0 runner     (501) staff       (20)     2694 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/pf_eigenvalue.py
--rw-r--r--   0 runner     (501) staff       (20)     8451 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/pnorm.py
--rw-r--r--   0 runner     (501) staff       (20)     4180 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/prod.py
--rw-r--r--   0 runner     (501) staff       (20)     7827 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/quad_form.py
--rw-r--r--   0 runner     (501) staff       (20)     4351 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/quad_over_lin.py
--rw-r--r--   0 runner     (501) staff       (20)     2381 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/sigma_max.py
--rw-r--r--   0 runner     (501) staff       (20)     2121 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/sign.py
--rw-r--r--   0 runner     (501) staff       (20)     2979 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/sum_largest.py
--rw-r--r--   0 runner     (501) staff       (20)      802 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/sum_smallest.py
--rw-r--r--   0 runner     (501) staff       (20)      930 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/sum_squares.py
--rw-r--r--   0 runner     (501) staff       (20)     4048 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/suppfunc.py
--rw-r--r--   0 runner     (501) staff       (20)     2101 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/total_variation.py
--rw-r--r--   0 runner     (501) staff       (20)     3832 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/tr_inv.py
--rw-r--r--   0 runner     (501) staff       (20)     3821 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/atoms/von_neumann_entr.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.733792 cvxpy-1.3.1/cvxpy/constraints/
--rw-r--r--   0 runner     (501) staff       (20)     1081 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7254 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/constraint.py
--rw-r--r--   0 runner     (501) staff       (20)    13162 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/exponential.py
--rw-r--r--   0 runner     (501) staff       (20)     4073 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/finite_set.py
--rw-r--r--   0 runner     (501) staff       (20)     7113 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/nonpos.py
--rw-r--r--   0 runner     (501) staff       (20)     9261 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/power.py
--rw-r--r--   0 runner     (501) staff       (20)     2706 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/psd.py
--rw-r--r--   0 runner     (501) staff       (20)     5430 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/second_order.py
--rw-r--r--   0 runner     (501) staff       (20)     3831 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/utilities.py
--rw-r--r--   0 runner     (501) staff       (20)     5264 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/constraints/zero.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.734345 cvxpy-1.3.1/cvxpy/cvxcore/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.600408 cvxpy-1.3.1/cvxpy/cvxcore/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.752430 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/
--rw-r--r--   0 runner     (501) staff       (20)      694 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1206 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Cholesky
--rw-r--r--   0 runner     (501) staff       (20)     1900 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/CholmodSupport
--rw-r--r--   0 runner     (501) staff       (20)    18103 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Core
--rw-r--r--   0 runner     (501) staff       (20)      122 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Dense
--rw-r--r--   0 runner     (501) staff       (20)       35 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Eigen
--rw-r--r--   0 runner     (501) staff       (20)     1822 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Eigenvalues
--rw-r--r--   0 runner     (501) staff       (20)     2050 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Geometry
--rw-r--r--   0 runner     (501) staff       (20)      874 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Householder
--rw-r--r--   0 runner     (501) staff       (20)     2083 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner     (501) staff       (20)      939 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Jacobi
--rw-r--r--   0 runner     (501) staff       (20)     1433 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/LU
--rw-r--r--   0 runner     (501) staff       (20)      991 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/MetisSupport
--rw-r--r--   0 runner     (501) staff       (20)     2483 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/OrderingMethods
--rw-r--r--   0 runner     (501) staff       (20)     1676 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner     (501) staff       (20)     1116 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/PardisoSupport
--rw-r--r--   0 runner     (501) staff       (20)     1317 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/QR
--rw-r--r--   0 runner     (501) staff       (20)      945 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner     (501) staff       (20)     1162 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SPQRSupport
--rw-r--r--   0 runner     (501) staff       (20)     1629 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SVD
--rw-r--r--   0 runner     (501) staff       (20)      919 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Sparse
--rw-r--r--   0 runner     (501) staff       (20)     1371 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseCholesky
--rw-r--r--   0 runner     (501) staff       (20)     2240 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseCore
--rw-r--r--   0 runner     (501) staff       (20)     1713 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseLU
--rw-r--r--   0 runner     (501) staff       (20)     1195 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseQR
--rw-r--r--   0 runner     (501) staff       (20)      797 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/StdDeque
--rw-r--r--   0 runner     (501) staff       (20)      726 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/StdList
--rw-r--r--   0 runner     (501) staff       (20)      803 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/StdVector
--rw-r--r--   0 runner     (501) staff       (20)     2243 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SuperLUSupport
--rw-r--r--   0 runner     (501) staff       (20)     1382 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.612606 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.754337 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/
--rw-r--r--   0 runner     (501) staff       (20)    24480 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner     (501) staff       (20)    18395 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner     (501) staff       (20)     3974 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.754901 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner     (501) staff       (20)    22307 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.796947 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/
--rw-r--r--   0 runner     (501) staff       (20)    12115 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Array.h
--rw-r--r--   0 runner     (501) staff       (20)     8237 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner     (501) staff       (20)     6775 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner     (501) staff       (20)     2720 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner     (501) staff       (20)    38153 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner     (501) staff       (20)    12479 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner     (501) staff       (20)    13910 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    18064 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Block.h
--rw-r--r--   0 runner     (501) staff       (20)     4249 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner     (501) staff       (20)     5689 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner     (501) staff       (20)     6990 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner     (501) staff       (20)    62197 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner     (501) staff       (20)     4525 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner     (501) staff       (20)     7593 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)    31424 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     8256 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     3877 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     5366 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner     (501) staff       (20)    27551 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner     (501) staff       (20)    24212 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner     (501) staff       (20)    22205 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner     (501) staff       (20)     9597 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner     (501) staff       (20)    12666 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)      970 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner     (501) staff       (20)    11507 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner     (501) staff       (20)     5619 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner     (501) staff       (20)     4769 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner     (501) staff       (20)     5705 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner     (501) staff       (20)    21123 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner     (501) staff       (20)    22069 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)    10222 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)     7076 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/IO.h
--rw-r--r--   0 runner     (501) staff       (20)     3519 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner     (501) staff       (20)     7239 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Map.h
--rw-r--r--   0 runner     (501) staff       (20)    11212 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner     (501) staff       (20)    41000 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)     3369 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner     (501) staff       (20)    19067 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner     (501) staff       (20)    23276 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner     (501) staff       (20)     3400 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner     (501) staff       (20)     3582 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner     (501) staff       (20)     9234 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner     (501) staff       (20)    20694 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    45354 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7235 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Product.h
--rw-r--r--   0 runner     (501) staff       (20)    51070 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner     (501) staff       (20)     6379 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Random.h
--rw-r--r--   0 runner     (501) staff       (20)    17852 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner     (501) staff       (20)    12844 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner     (501) staff       (20)     5595 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner     (501) staff       (20)     4200 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner     (501) staff       (20)     7073 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner     (501) staff       (20)     6020 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Select.h
--rw-r--r--   0 runner     (501) staff       (20)    14245 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner     (501) staff       (20)     1697 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     6795 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner     (501) staff       (20)     9208 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner     (501) staff       (20)     4365 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7692 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner     (501) staff       (20)     3865 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner     (501) staff       (20)     2683 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner     (501) staff       (20)    14856 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner     (501) staff       (20)    13092 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner     (501) staff       (20)    37304 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     3462 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner     (501) staff       (20)    29441 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner     (501) staff       (20)     8074 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.604072 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.799607 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner     (501) staff       (20)    18037 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    17776 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    27841 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     1194 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.800925 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner     (501) staff       (20)    15528 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    50865 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.802881 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner     (501) staff       (20)    16443 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    10797 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner     (501) staff       (20)    37671 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.806784 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner     (501) staff       (20)     4240 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    23547 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner     (501) staff       (20)     2387 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    10744 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)    35476 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner     (501) staff       (20)     5509 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.807901 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner     (501) staff       (20)     1989 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner     (501) staff       (20)     1746 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.809702 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner     (501) staff       (20)    17706 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     2846 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    28726 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.812464 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner     (501) staff       (20)    19426 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    18888 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner     (501) staff       (20)    35843 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     1759 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.814229 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner     (501) staff       (20)    15366 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     4418 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner     (501) staff       (20)    32283 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.818122 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/
--rw-r--r--   0 runner     (501) staff       (20)     6284 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)    18263 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)     8229 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)     4400 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)      607 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)    27946 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.860226 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/
--rw-r--r--   0 runner     (501) staff       (20)    81646 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner     (501) staff       (20)    18887 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    15898 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner     (501) staff       (20)     6937 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     5106 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)    26808 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner     (501) staff       (20)     6368 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     4934 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner     (501) staff       (20)    20103 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    11570 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     9901 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner     (501) staff       (20)     5209 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     6162 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     4066 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner     (501) staff       (20)    20879 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    13867 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)    14722 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner     (501) staff       (20)    10571 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)    14540 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     6707 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     5741 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.042332 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/
--rwxr-xr-x   0 runner     (501) staff       (20)    19307 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner     (501) staff       (20)    21579 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner     (501) staff       (20)     4360 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner     (501) staff       (20)    14094 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner     (501) staff       (20)     4026 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner     (501) staff       (20)    38322 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner     (501) staff       (20)    40579 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner     (501) staff       (20)    21356 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner     (501) staff       (20)       85 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner     (501) staff       (20)     1024 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner     (501) staff       (20)    10518 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner     (501) staff       (20)    34903 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.051889 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner     (501) staff       (20)    12558 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)    17273 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner     (501) staff       (20)     4178 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    22944 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)    17176 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)     9715 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)    14351 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner     (501) staff       (20)     5539 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner     (501) staff       (20)    23586 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner     (501) staff       (20)    20749 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner     (501) staff       (20)     3650 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    33705 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)     4104 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    22444 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.066124 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/
--rw-r--r--   0 runner     (501) staff       (20)    14815 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner     (501) staff       (20)     8423 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner     (501) staff       (20)     3639 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner     (501) staff       (20)    20539 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner     (501) staff       (20)    11961 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner     (501) staff       (20)     8949 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner     (501) staff       (20)     8308 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner     (501) staff       (20)    32704 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner     (501) staff       (20)     6877 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner     (501) staff       (20)     8063 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner     (501) staff       (20)     6331 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner     (501) staff       (20)    60555 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner     (501) staff       (20)     7664 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner     (501) staff       (20)     6190 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.066867 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner     (501) staff       (20)     5387 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.068886 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/
--rw-r--r--   0 runner     (501) staff       (20)     4481 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner     (501) staff       (20)     5345 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner     (501) staff       (20)    20603 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.082376 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner     (501) staff       (20)     6755 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner     (501) staff       (20)     7253 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner     (501) staff       (20)     9289 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner     (501) staff       (20)    15062 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner     (501) staff       (20)    15234 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner     (501) staff       (20)    11527 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7762 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner     (501) staff       (20)     4158 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.082972 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Jacobi/
--rw-r--r--   0 runner     (501) staff       (20)    15902 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.086512 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/
--rw-r--r--   0 runner     (501) staff       (20)     3057 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner     (501) staff       (20)    32803 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner     (501) staff       (20)    15064 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner     (501) staff       (20)    21538 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner     (501) staff       (20)     3555 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.087087 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/arch/
--rw-r--r--   0 runner     (501) staff       (20)    13662 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.087826 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/MetisSupport/
--rw-r--r--   0 runner     (501) staff       (20)     4588 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.089763 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner     (501) staff       (20)    16396 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner     (501) staff       (20)    62266 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner     (501) staff       (20)     5229 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.090520 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner     (501) staff       (20)    22248 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.091255 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner     (501) staff       (20)    20060 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.099906 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/
--rw-r--r--   0 runner     (501) staff       (20)    24881 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner     (501) staff       (20)     4662 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    20805 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner     (501) staff       (20)    25478 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner     (501) staff       (20)    14022 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner     (501) staff       (20)     2993 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.100529 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner     (501) staff       (20)    11405 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.104179 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/
--rw-r--r--   0 runner     (501) staff       (20)    49870 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner     (501) staff       (20)    32949 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner     (501) staff       (20)     5099 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    12752 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner     (501) staff       (20)    15957 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.105663 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner     (501) staff       (20)    24017 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner     (501) staff       (20)     6912 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.142761 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/
--rw-r--r--   0 runner     (501) staff       (20)    10670 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner     (501) staff       (20)     8164 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner     (501) staff       (20)    13178 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     2191 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     8080 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner     (501) staff       (20)    25592 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner     (501) staff       (20)     6485 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner     (501) staff       (20)    12720 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner     (501) staff       (20)    25840 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     4737 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)    12487 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     5808 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     3080 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner     (501) staff       (20)     1107 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner     (501) staff       (20)    12589 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner     (501) staff       (20)    52401 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    17923 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7329 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner     (501) staff       (20)     7049 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     1699 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner     (501) staff       (20)    15492 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner     (501) staff       (20)    25721 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner     (501) staff       (20)     4424 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner     (501) staff       (20)     8704 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner     (501) staff       (20)     3175 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner     (501) staff       (20)     6437 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner     (501) staff       (20)     6602 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner     (501) staff       (20)    14831 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner     (501) staff       (20)     8127 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner     (501) staff       (20)     9657 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.159960 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/
--rw-r--r--   0 runner     (501) staff       (20)    27844 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner     (501) staff       (20)     4303 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner     (501) staff       (20)     7601 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner     (501) staff       (20)     4974 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner     (501) staff       (20)    10022 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     2049 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner     (501) staff       (20)     6712 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner     (501) staff       (20)     6582 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner     (501) staff       (20)     3681 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner     (501) staff       (20)    10216 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner     (501) staff       (20)     4181 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner     (501) staff       (20)     5723 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner     (501) staff       (20)     8486 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner     (501) staff       (20)     9028 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner     (501) staff       (20)     4979 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner     (501) staff       (20)     4545 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner     (501) staff       (20)     2889 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.160635 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseQR/
--rw-r--r--   0 runner     (501) staff       (20)    28373 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.163172 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/
--rw-r--r--   0 runner     (501) staff       (20)     5279 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner     (501) staff       (20)     4147 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner     (501) staff       (20)     5330 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner     (501) staff       (20)     2809 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.163735 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner     (501) staff       (20)    34345 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.164435 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner     (501) staff       (20)    17202 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.174718 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/
--rw-r--r--   0 runner     (501) staff       (20)     2913 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/Image.h
--rw-r--r--   0 runner     (501) staff       (20)     2742 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner     (501) staff       (20)     1748 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner     (501) staff       (20)    30560 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/blas.h
--rw-r--r--   0 runner     (501) staff       (20)     7834 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner     (501) staff       (20)  1058368 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner     (501) staff       (20)      474 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.179753 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/
--rw-r--r--   0 runner     (501) staff       (20)    13166 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)    16929 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)    37403 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner     (501) staff       (20)     4828 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)     5621 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)     6375 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)     2937 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.190317 cvxpy-1.3.1/cvxpy/cvxcore/python/
--rw-r--r--   0 runner     (501) staff       (20)      139 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/python/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    20191 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/python/canonInterface.py
--rw-r--r--   0 runner     (501) staff       (20)     2403 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/python/cvxcore.i
--rw-r--r--   0 runner     (501) staff       (20)    38475 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/python/cvxcore.py
--rw-r--r--   0 runner     (501) staff       (20)   885382 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/python/cvxcore_wrap.cxx
--rw-r--r--   0 runner     (501) staff       (20)    54061 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/python/numpy.i
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.211834 cvxpy-1.3.1/cvxpy/cvxcore/src/
--rw-r--r--   0 runner     (501) staff       (20)       24 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/.keep
--rw-r--r--   0 runner     (501) staff       (20)     4970 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/LinOp.hpp
--rw-r--r--   0 runner     (501) staff       (20)    39092 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/LinOpOperations.cpp
--rw-r--r--   0 runner     (501) staff       (20)      844 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/LinOpOperations.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3365 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/ProblemData.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5057 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/Utils.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1454 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/Utils.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8098 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/cvxcore.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1328 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/cvxcore/src/cvxcore.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1299 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/error.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.214754 cvxpy-1.3.1/cvxpy/expressions/
--rw-r--r--   0 runner     (501) staff       (20)      590 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.217693 cvxpy-1.3.1/cvxpy/expressions/constants/
--rw-r--r--   0 runner     (501) staff       (20)      670 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/constants/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1071 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/constants/callback_param.py
--rw-r--r--   0 runner     (501) staff       (20)     7756 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/constants/constant.py
--rw-r--r--   0 runner     (501) staff       (20)     3737 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/constants/parameter.py
--rw-r--r--   0 runner     (501) staff       (20)     3421 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/cvxtypes.py
--rw-r--r--   0 runner     (501) staff       (20)    24786 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    16470 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/leaf.py
--rw-r--r--   0 runner     (501) staff       (20)     4288 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/expressions/variable.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.220382 cvxpy-1.3.1/cvxpy/interface/
--rw-r--r--   0 runner     (501) staff       (20)      611 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5171 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/base_matrix_interface.py
--rw-r--r--   0 runner     (501) staff       (20)    10920 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/matrix_utilities.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.226484 cvxpy-1.3.1/cvxpy/interface/numpy_interface/
--rw-r--r--   0 runner     (501) staff       (20)      818 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/numpy_interface/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2058 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/numpy_interface/matrix_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     2423 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/numpy_interface/ndarray_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     3446 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/numpy_interface/sparse_matrix_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     1181 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/interface/scipy_wrapper.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.230662 cvxpy-1.3.1/cvxpy/lin_ops/
--rw-r--r--   0 runner     (501) staff       (20)      684 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/lin_ops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    38309 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/lin_ops/canon_backend.py
--rw-r--r--   0 runner     (501) staff       (20)     1126 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/lin_ops/lin_constraints.py
--rw-r--r--   0 runner     (501) staff       (20)     3370 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/lin_ops/lin_op.py
--rw-r--r--   0 runner     (501) staff       (20)    18564 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/lin_ops/lin_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    12097 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/lin_ops/tree_mat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.234579 cvxpy-1.3.1/cvxpy/problems/
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/problems/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4958 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/problems/iterative.py
--rw-r--r--   0 runner     (501) staff       (20)     7339 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/problems/objective.py
--rw-r--r--   0 runner     (501) staff       (20)     1615 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/problems/param_prob.py
--rw-r--r--   0 runner     (501) staff       (20)    62517 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/problems/problem.py
--rw-r--r--   0 runner     (501) staff       (20)     2921 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/problems/xpress_problem.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/py.typed
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.245133 cvxpy-1.3.1/cvxpy/reductions/
--rw-r--r--   0 runner     (501) staff       (20)     1452 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4850 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/canonicalization.py
--rw-r--r--   0 runner     (501) staff       (20)     2667 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/chain.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.246456 cvxpy-1.3.1/cvxpy/reductions/complex2real/
--rw-r--r--   0 runner     (501) staff       (20)      566 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.273236 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     4612 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1058 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     3462 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      912 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1780 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2240 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     7495 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      860 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/param_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      815 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1042 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1554 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1720 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     8307 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/complex2real/complex2real.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.275759 cvxpy-1.3.1/cvxpy/reductions/cone2cone/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/cone2cone/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    17759 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/cone2cone/affine2direct.py
--rw-r--r--   0 runner     (501) staff       (20)     7063 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/cone2cone/approximations.py
--rw-r--r--   0 runner     (501) staff       (20)     3035 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/cone2cone/exotic2common.py
--rw-r--r--   0 runner     (501) staff       (20)     5848 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/cvx_attr2constr.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.277669 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/
--rw-r--r--   0 runner     (501) staff       (20)      564 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.312689 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     4264 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1091 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/entr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      965 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/exp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1067 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/geo_mean_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1512 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/huber_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/indicator_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      937 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/kl_div_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1194 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_max_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1494 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_sum_largest_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      705 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log1p_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1049 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_det_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1690 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_sum_exp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1118 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/logistic_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1220 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/matrix_frac_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1211 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/mul_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1310 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/normNuc_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     3661 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/perspective_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2402 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/pnorm_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1427 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/power_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1281 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_form_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1185 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_over_lin_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      938 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/rel_entr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1124 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/sigma_max_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2133 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/suppfunc_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1683 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/tr_inv_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1971 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/von_neumann_entr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1162 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/xexp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)    16825 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py
--rw-r--r--   0 runner     (501) staff       (20)     5440 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dcp2cone/dcp2cone.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.314322 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.358776 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     5713 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      995 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/add_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      732 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/constant_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      101 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/div_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/exp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1442 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/eye_minus_inv_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      152 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/geo_mean_canon.py
--rw-r--r--   0 runner     (501) staff       (20)       63 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/gmatmul_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      101 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/log_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      126 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/mul_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/mulexpression_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/nonpos_constr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      258 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/norm1_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      268 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/norm_inf_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      173 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/one_minus_pos_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/parameter_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      693 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pf_eigenvalue_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      697 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pnorm_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      122 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/power_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      154 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/prod_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      326 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/quad_form_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      295 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/quad_over_lin_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      709 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/sum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      293 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/trace_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      125 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/xexp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      161 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/zero_constr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     3289 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/dgp2dcp.py
--rw-r--r--   0 runner     (501) staff       (20)      273 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.360071 cvxpy-1.3.1/cvxpy/reductions/discrete2mixedint/
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/discrete2mixedint/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2750 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.363123 cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/
--rw-r--r--   0 runner     (501) staff       (20)      562 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9534 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py
--rw-r--r--   0 runner     (501) staff       (20)     3453 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/inverse.py
--rw-r--r--   0 runner     (501) staff       (20)     5154 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/sets.py
--rw-r--r--   0 runner     (501) staff       (20)     1154 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/tighten.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.364651 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/
--rw-r--r--   0 runner     (501) staff       (20)      566 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.379284 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     2079 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      748 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/abs_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1106 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cummax_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1133 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cumsum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1380 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/dotsort_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1333 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/max_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      765 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/maximum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      882 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/min_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      879 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/minimum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1186 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm1_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1329 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm_inf_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/sum_largest_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1464 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py
--rw-r--r--   0 runner     (501) staff       (20)     2689 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/eval_params.py
--rw-r--r--   0 runner     (501) staff       (20)     2051 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/flip_objective.py
--rw-r--r--   0 runner     (501) staff       (20)     1944 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/inverse_data.py
--rw-r--r--   0 runner     (501) staff       (20)     2597 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/matrix_stuffing.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.383289 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/
--rw-r--r--   0 runner     (501) staff       (20)      564 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.393503 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     2097 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1492 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/huber_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1431 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/power_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      967 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_form_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1298 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_over_lin_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2392 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py
--rw-r--r--   0 runner     (501) staff       (20)    11970 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py
--rw-r--r--   0 runner     (501) staff       (20)     5050 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/reduction.py
--rw-r--r--   0 runner     (501) staff       (20)     3020 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solution.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.399543 cvxpy-1.3.1/cvxpy/reductions/solvers/
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7382 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/bisection.py
--rw-r--r--   0 runner     (501) staff       (20)     3636 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/compr_matrix.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.423697 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/
--rw-r--r--   0 runner     (501) staff       (20)     1145 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6917 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     6988 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    14223 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/conic_solver.py
--rw-r--r--   0 runner     (501) staff       (20)    12800 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/copt_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    18667 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    13312 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     6715 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     5053 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     6672 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     8924 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/glop_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     3953 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     4477 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    14167 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    28459 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     9608 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/nag_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     9580 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    14954 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/scip_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    10042 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    13214 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/scs_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     9046 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    15315 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     1085 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/constant_solver.py
--rw-r--r--   0 runner     (501) staff       (20)     5244 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/defines.py
--rw-r--r--   0 runner     (501) staff       (20)     4177 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/intermediate_chain.py
--rw-r--r--   0 runner     (501) staff       (20)     4372 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/kktsolver.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.424623 cvxpy-1.3.1/cvxpy/reductions/solvers/lp_solvers/
--rw-r--r--   0 runner     (501) staff       (20)      566 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/lp_solvers/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.429682 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5907 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     5757 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     9848 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     4222 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     5723 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     3609 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/qp_solver.py
--rw-r--r--   0 runner     (501) staff       (20)     9432 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     2495 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/solver.py
--rw-r--r--   0 runner     (501) staff       (20)    16777 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/solving_chain.py
--rw-r--r--   0 runner     (501) staff       (20)     2830 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/solvers/utilities.py
--rw-r--r--   0 runner     (501) staff       (20)     6122 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/reductions/utilities.py
--rw-r--r--   0 runner     (501) staff       (20)     5120 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/settings.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.471612 cvxpy-1.3.1/cvxpy/tests/
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1497 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/base_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1963 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/ram_limited.py
--rw-r--r--   0 runner     (501) staff       (20)    41065 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/solver_test_helpers.py
--rw-r--r--   0 runner     (501) staff       (20)    65672 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_atoms.py
--rw-r--r--   0 runner     (501) staff       (20)     9823 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_benchmarks.py
--rw-r--r--   0 runner     (501) staff       (20)    29018 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_complex.py
--rw-r--r--   0 runner     (501) staff       (20)    29812 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_cone2cone.py
--rw-r--r--   0 runner     (501) staff       (20)    76805 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_conic_solvers.py
--rw-r--r--   0 runner     (501) staff       (20)     1005 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_constant.py
--rw-r--r--   0 runner     (501) staff       (20)    19098 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_constant_atoms.py
--rw-r--r--   0 runner     (501) staff       (20)    13747 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_constraints.py
--rw-r--r--   0 runner     (501) staff       (20)     4310 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_convolution.py
--rw-r--r--   0 runner     (501) staff       (20)     2983 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_copy.py
--rw-r--r--   0 runner     (501) staff       (20)     3491 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_curvature.py
--rw-r--r--   0 runner     (501) staff       (20)     3939 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_custom_solver.py
--rw-r--r--   0 runner     (501) staff       (20)    25483 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_derivative.py
--rw-r--r--   0 runner     (501) staff       (20)     7749 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_dgp.py
--rw-r--r--   0 runner     (501) staff       (20)    27269 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_dgp2dcp.py
--rw-r--r--   0 runner     (501) staff       (20)     7197 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_domain.py
--rw-r--r--   0 runner     (501) staff       (20)    32192 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_dpp.py
--rw-r--r--   0 runner     (501) staff       (20)    25997 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_dqcp.py
--rw-r--r--   0 runner     (501) staff       (20)    21420 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_examples.py
--rw-r--r--   0 runner     (501) staff       (20)    52582 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_expressions.py
--rw-r--r--   0 runner     (501) staff       (20)    32554 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_grad.py
--rw-r--r--   0 runner     (501) staff       (20)     1570 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_gurobi_write.py
--rw-r--r--   0 runner     (501) staff       (20)     7545 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_interfaces.py
--rw-r--r--   0 runner     (501) staff       (20)     7671 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_kron_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     4989 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_lin_ops.py
--rw-r--r--   0 runner     (501) staff       (20)    16619 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_linear_cone.py
--rw-r--r--   0 runner     (501) staff       (20)     5135 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_matrices.py
--rw-r--r--   0 runner     (501) staff       (20)     4098 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_mip_vars.py
--rw-r--r--   0 runner     (501) staff       (20)     2993 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_monotonicity.py
--rw-r--r--   0 runner     (501) staff       (20)     6616 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_nonlinear_atoms.py
--rw-r--r--   0 runner     (501) staff       (20)     3726 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_numpy.py
--rw-r--r--   0 runner     (501) staff       (20)     4985 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_objectives.py
--rw-r--r--   0 runner     (501) staff       (20)     4260 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_param_cone_prog.py
--rw-r--r--   0 runner     (501) staff       (20)     4223 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_param_quad_prog.py
--rw-r--r--   0 runner     (501) staff       (20)    12777 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_perspective.py
--rw-r--r--   0 runner     (501) staff       (20)     4337 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_power_tools.py
--rw-r--r--   0 runner     (501) staff       (20)    81573 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_problem.py
--rw-r--r--   0 runner     (501) staff       (20)    43565 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_python_backends.py
--rw-r--r--   0 runner     (501) staff       (20)    22381 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_qp_solvers.py
--rw-r--r--   0 runner     (501) staff       (20)     7895 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_quad_form.py
--rw-r--r--   0 runner     (501) staff       (20)     6631 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_quadratic.py
--rw-r--r--   0 runner     (501) staff       (20)     3247 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_semidefinite_vars.py
--rw-r--r--   0 runner     (501) staff       (20)     3992 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_shape.py
--rw-r--r--   0 runner     (501) staff       (20)     2694 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_sign.py
--rw-r--r--   0 runner     (501) staff       (20)     7775 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_suppfunc.py
--rw-r--r--   0 runner     (501) staff       (20)    11072 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_valinvec2mixedint.py
--rw-r--r--   0 runner     (501) staff       (20)     1901 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_versioning.py
--rw-r--r--   0 runner     (501) staff       (20)     9116 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/tests/test_von_neumann_entr.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.478174 cvxpy-1.3.1/cvxpy/transforms/
--rw-r--r--   0 runner     (501) staff       (20)      996 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/transforms/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3672 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/transforms/indicator.py
--rw-r--r--   0 runner     (501) staff       (20)     2088 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/transforms/linearize.py
--rw-r--r--   0 runner     (501) staff       (20)    10918 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/transforms/partial_optimize.py
--rw-r--r--   0 runner     (501) staff       (20)     4306 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/transforms/scalarize.py
--rw-r--r--   0 runner     (501) staff       (20)     6782 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/transforms/suppfunc.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:24.490701 cvxpy-1.3.1/cvxpy/utilities/
--rw-r--r--   0 runner     (501) staff       (20)      629 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5446 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/canonical.py
--rw-r--r--   0 runner     (501) staff       (20)    12257 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/coeff_extractor.py
--rw-r--r--   0 runner     (501) staff       (20)     2968 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/cvxpy_upgrade.py
--rw-r--r--   0 runner     (501) staff       (20)     3264 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/debug_tools.py
--rw-r--r--   0 runner     (501) staff       (20)      245 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/deterministic.py
--rw-r--r--   0 runner     (501) staff       (20)     1424 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/grad.py
--rw-r--r--   0 runner     (501) staff       (20)     6226 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/key_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4911 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/linalg.py
--rw-r--r--   0 runner     (501) staff       (20)     2437 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/performance_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2178 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/perspective_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    19336 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/power_tools.py
--rw-r--r--   0 runner     (501) staff       (20)     1552 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/replace_quad_forms.py
--rw-r--r--   0 runner     (501) staff       (20)     1400 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/scopes.py
--rw-r--r--   0 runner     (501) staff       (20)     4983 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/shape.py
--rw-r--r--   0 runner     (501) staff       (20)     1968 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/sign.py
--rw-r--r--   0 runner     (501) staff       (20)     1825 2023-03-18 20:33:39.000000 cvxpy-1.3.1/cvxpy/utilities/versioning.py
--rw-r--r--   0 runner     (501) staff       (20)      213 2023-03-18 20:40:08.000000 cvxpy-1.3.1/cvxpy/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-18 20:40:23.630990 cvxpy-1.3.1/cvxpy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9055 2023-03-18 20:40:14.000000 cvxpy-1.3.1/cvxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    32903 2023-03-18 20:40:23.000000 cvxpy-1.3.1/cvxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-03-18 20:40:14.000000 cvxpy-1.3.1/cvxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-03-18 20:36:29.000000 cvxpy-1.3.1/cvxpy.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      412 2023-03-18 20:40:14.000000 cvxpy-1.3.1/cvxpy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       15 2023-03-18 20:40:14.000000 cvxpy-1.3.1/cvxpy.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1276 2023-03-18 20:33:40.000000 cvxpy-1.3.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      476 2023-03-18 20:40:24.497853 cvxpy-1.3.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     8455 2023-03-18 20:33:40.000000 cvxpy-1.3.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.149116 cvxpy-1.3.2/
+-rw-r--r--   0 runner     (501) staff       (20)    11344 2023-06-27 07:55:55.000000 cvxpy-1.3.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      102 2023-06-27 07:55:55.000000 cvxpy-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     9055 2023-06-27 08:01:18.149510 cvxpy-1.3.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6949 2023-06-27 07:55:55.000000 cvxpy-1.3.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.812705 cvxpy-1.3.2/cvxpy/
+-rw-r--r--   0 runner     (501) staff       (20)     2160 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.834573 cvxpy-1.3.2/cvxpy/atoms/
+-rw-r--r--   0 runner     (501) staff       (20)     5266 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.847473 cvxpy-1.3.2/cvxpy/atoms/affine/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3967 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/add_expr.py
+-rw-r--r--   0 runner     (501) staff       (20)     5719 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/affine_atom.py
+-rw-r--r--   0 runner     (501) staff       (20)    14543 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/binary_operators.py
+-rw-r--r--   0 runner     (501) staff       (20)     1137 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/bmat.py
+-rw-r--r--   0 runner     (501) staff       (20)     2313 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/conj.py
+-rw-r--r--   0 runner     (501) staff       (20)     6168 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     4371 2023-06-27 07:55:55.000000 cvxpy-1.3.2/cvxpy/atoms/affine/cumsum.py
+-rw-r--r--   0 runner     (501) staff       (20)     4741 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/diag.py
+-rw-r--r--   0 runner     (501) staff       (20)     1644 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/diff.py
+-rw-r--r--   0 runner     (501) staff       (20)     2977 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/hstack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/imag.py
+-rw-r--r--   0 runner     (501) staff       (20)     6401 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/index.py
+-rw-r--r--   0 runner     (501) staff       (20)     4379 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/kron.py
+-rw-r--r--   0 runner     (501) staff       (20)     3310 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/partial_trace.py
+-rw-r--r--   0 runner     (501) staff       (20)     3365 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/partial_transpose.py
+-rw-r--r--   0 runner     (501) staff       (20)     3204 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/promote.py
+-rw-r--r--   0 runner     (501) staff       (20)     1486 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/real.py
+-rw-r--r--   0 runner     (501) staff       (20)     4440 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/reshape.py
+-rw-r--r--   0 runner     (501) staff       (20)     3553 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/sum.py
+-rw-r--r--   0 runner     (501) staff       (20)     2937 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/trace.py
+-rw-r--r--   0 runner     (501) staff       (20)     2872 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/transpose.py
+-rw-r--r--   0 runner     (501) staff       (20)     2752 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/unary_operators.py
+-rw-r--r--   0 runner     (501) staff       (20)     4346 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/upper_tri.py
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/vec.py
+-rw-r--r--   0 runner     (501) staff       (20)     3033 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/vstack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3746 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/affine/wraps.py
+-rw-r--r--   0 runner     (501) staff       (20)    16154 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/atom.py
+-rw-r--r--   0 runner     (501) staff       (20)     4313 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/axis_atom.py
+-rw-r--r--   0 runner     (501) staff       (20)     3132 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/condition_number.py
+-rw-r--r--   0 runner     (501) staff       (20)     2943 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/cummax.py
+-rw-r--r--   0 runner     (501) staff       (20)     2423 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/dist_ratio.py
+-rw-r--r--   0 runner     (501) staff       (20)     4928 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/dotsort.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.857920 cvxpy-1.3.2/cvxpy/atoms/elementwise/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2457 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/abs.py
+-rw-r--r--   0 runner     (501) staff       (20)     4790 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/ceil.py
+-rw-r--r--   0 runner     (501) staff       (20)     2414 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/elementwise.py
+-rw-r--r--   0 runner     (501) staff       (20)     2746 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/entr.py
+-rw-r--r--   0 runner     (501) staff       (20)     2358 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/exp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3520 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/huber.py
+-rw-r--r--   0 runner     (501) staff       (20)      703 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/inv_pos.py
+-rw-r--r--   0 runner     (501) staff       (20)     3009 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/kl_div.py
+-rw-r--r--   0 runner     (501) staff       (20)     2757 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/log.py
+-rw-r--r--   0 runner     (501) staff       (20)     2046 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/log1p.py
+-rw-r--r--   0 runner     (501) staff       (20)     2036 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/log_normcdf.py
+-rw-r--r--   0 runner     (501) staff       (20)     1417 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/loggamma.py
+-rw-r--r--   0 runner     (501) staff       (20)     2345 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/logistic.py
+-rw-r--r--   0 runner     (501) staff       (20)     3519 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/maximum.py
+-rw-r--r--   0 runner     (501) staff       (20)     3222 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/minimum.py
+-rw-r--r--   0 runner     (501) staff       (20)      699 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/neg.py
+-rw-r--r--   0 runner     (501) staff       (20)      696 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/pos.py
+-rw-r--r--   0 runner     (501) staff       (20)    14794 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     2988 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/rel_entr.py
+-rw-r--r--   0 runner     (501) staff       (20)      779 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/scalene.py
+-rw-r--r--   0 runner     (501) staff       (20)      739 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/sqrt.py
+-rw-r--r--   0 runner     (501) staff       (20)      691 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/square.py
+-rw-r--r--   0 runner     (501) staff       (20)     2682 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/elementwise/xexp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/eye_minus_inv.py
+-rw-r--r--   0 runner     (501) staff       (20)     3518 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/gen_lambda_max.py
+-rw-r--r--   0 runner     (501) staff       (20)    11931 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/geo_mean.py
+-rw-r--r--   0 runner     (501) staff       (20)     4909 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/gmatmul.py
+-rw-r--r--   0 runner     (501) staff       (20)     1292 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/harmonic_mean.py
+-rw-r--r--   0 runner     (501) staff       (20)     1197 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/inv_prod.py
+-rw-r--r--   0 runner     (501) staff       (20)     3291 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/lambda_max.py
+-rw-r--r--   0 runner     (501) staff       (20)      811 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/lambda_min.py
+-rw-r--r--   0 runner     (501) staff       (20)     2318 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/lambda_sum_largest.py
+-rw-r--r--   0 runner     (501) staff       (20)      834 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/lambda_sum_smallest.py
+-rw-r--r--   0 runner     (501) staff       (20)     2282 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/length.py
+-rw-r--r--   0 runner     (501) staff       (20)     3645 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/log_det.py
+-rw-r--r--   0 runner     (501) staff       (20)     2690 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/log_sum_exp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4538 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/matrix_frac.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/max.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/min.py
+-rw-r--r--   0 runner     (501) staff       (20)     1304 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/mixed_norm.py
+-rw-r--r--   0 runner     (501) staff       (20)     3098 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/norm.py
+-rw-r--r--   0 runner     (501) staff       (20)     3212 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/norm1.py
+-rw-r--r--   0 runner     (501) staff       (20)     3376 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/norm_inf.py
+-rw-r--r--   0 runner     (501) staff       (20)     2271 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/norm_nuc.py
+-rw-r--r--   0 runner     (501) staff       (20)     2801 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/one_minus_pos.py
+-rw-r--r--   0 runner     (501) staff       (20)     4220 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/perspective.py
+-rw-r--r--   0 runner     (501) staff       (20)     2694 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/pf_eigenvalue.py
+-rw-r--r--   0 runner     (501) staff       (20)     8451 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/pnorm.py
+-rw-r--r--   0 runner     (501) staff       (20)     4180 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/prod.py
+-rw-r--r--   0 runner     (501) staff       (20)     7827 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/quad_form.py
+-rw-r--r--   0 runner     (501) staff       (20)     4351 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/quad_over_lin.py
+-rw-r--r--   0 runner     (501) staff       (20)     2381 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/sigma_max.py
+-rw-r--r--   0 runner     (501) staff       (20)     2121 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/sign.py
+-rw-r--r--   0 runner     (501) staff       (20)     2979 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/sum_largest.py
+-rw-r--r--   0 runner     (501) staff       (20)      802 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/sum_smallest.py
+-rw-r--r--   0 runner     (501) staff       (20)      930 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/sum_squares.py
+-rw-r--r--   0 runner     (501) staff       (20)     4048 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/suppfunc.py
+-rw-r--r--   0 runner     (501) staff       (20)     2101 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/total_variation.py
+-rw-r--r--   0 runner     (501) staff       (20)     3832 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/tr_inv.py
+-rw-r--r--   0 runner     (501) staff       (20)     3821 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/atoms/von_neumann_entr.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.862365 cvxpy-1.3.2/cvxpy/constraints/
+-rw-r--r--   0 runner     (501) staff       (20)     1081 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7254 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/constraint.py
+-rw-r--r--   0 runner     (501) staff       (20)    13162 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/exponential.py
+-rw-r--r--   0 runner     (501) staff       (20)     4073 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/finite_set.py
+-rw-r--r--   0 runner     (501) staff       (20)     7113 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/nonpos.py
+-rw-r--r--   0 runner     (501) staff       (20)     9275 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     2706 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/psd.py
+-rw-r--r--   0 runner     (501) staff       (20)     5430 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/second_order.py
+-rw-r--r--   0 runner     (501) staff       (20)     3831 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)     5264 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/constraints/zero.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.862781 cvxpy-1.3.2/cvxpy/cvxcore/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.792620 cvxpy-1.3.2/cvxpy/cvxcore/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.876325 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/
+-rw-r--r--   0 runner     (501) staff       (20)      694 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Cholesky
+-rw-r--r--   0 runner     (501) staff       (20)     1900 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/CholmodSupport
+-rw-r--r--   0 runner     (501) staff       (20)    18103 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Core
+-rw-r--r--   0 runner     (501) staff       (20)      122 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Dense
+-rw-r--r--   0 runner     (501) staff       (20)       35 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Eigen
+-rw-r--r--   0 runner     (501) staff       (20)     1822 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Eigenvalues
+-rw-r--r--   0 runner     (501) staff       (20)     2050 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Geometry
+-rw-r--r--   0 runner     (501) staff       (20)      874 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Householder
+-rw-r--r--   0 runner     (501) staff       (20)     2083 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner     (501) staff       (20)      939 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Jacobi
+-rw-r--r--   0 runner     (501) staff       (20)     1433 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/LU
+-rw-r--r--   0 runner     (501) staff       (20)      991 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/MetisSupport
+-rw-r--r--   0 runner     (501) staff       (20)     2483 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/OrderingMethods
+-rw-r--r--   0 runner     (501) staff       (20)     1676 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/PaStiXSupport
+-rwxr-xr-x   0 runner     (501) staff       (20)     1116 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/PardisoSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1317 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/QR
+-rw-r--r--   0 runner     (501) staff       (20)      945 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner     (501) staff       (20)     1162 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SPQRSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1629 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SVD
+-rw-r--r--   0 runner     (501) staff       (20)      919 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Sparse
+-rw-r--r--   0 runner     (501) staff       (20)     1371 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseCholesky
+-rw-r--r--   0 runner     (501) staff       (20)     2240 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseCore
+-rw-r--r--   0 runner     (501) staff       (20)     1713 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseLU
+-rw-r--r--   0 runner     (501) staff       (20)     1195 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseQR
+-rw-r--r--   0 runner     (501) staff       (20)      797 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/StdDeque
+-rw-r--r--   0 runner     (501) staff       (20)      726 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/StdList
+-rw-r--r--   0 runner     (501) staff       (20)      803 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/StdVector
+-rw-r--r--   0 runner     (501) staff       (20)     2243 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SuperLUSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1382 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.801897 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.877740 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/
+-rw-r--r--   0 runner     (501) staff       (20)    24480 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner     (501) staff       (20)    18395 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner     (501) staff       (20)     3974 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.878260 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    22307 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.910243 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/
+-rw-r--r--   0 runner     (501) staff       (20)    12115 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner     (501) staff       (20)     8237 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     6775 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner     (501) staff       (20)     2720 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner     (501) staff       (20)    38153 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    12479 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner     (501) staff       (20)    13910 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    18064 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner     (501) staff       (20)     4249 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner     (501) staff       (20)     5689 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner     (501) staff       (20)     6990 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner     (501) staff       (20)    62197 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner     (501) staff       (20)     4525 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner     (501) staff       (20)     7593 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    31424 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     8256 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     3877 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     5366 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner     (501) staff       (20)    27551 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    24212 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    22205 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner     (501) staff       (20)     9597 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner     (501) staff       (20)    12666 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)      970 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)    11507 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner     (501) staff       (20)     5619 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     4769 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner     (501) staff       (20)     5705 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner     (501) staff       (20)    21123 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)    22069 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    10222 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     7076 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner     (501) staff       (20)     3519 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner     (501) staff       (20)     7239 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner     (501) staff       (20)    11212 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    41000 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     3369 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    19067 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    23276 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     3400 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner     (501) staff       (20)     3582 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner     (501) staff       (20)     9234 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner     (501) staff       (20)    20694 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    45354 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7235 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner     (501) staff       (20)    51070 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner     (501) staff       (20)     6379 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner     (501) staff       (20)    17852 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner     (501) staff       (20)    12844 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner     (501) staff       (20)     5595 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner     (501) staff       (20)     4200 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner     (501) staff       (20)     7073 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner     (501) staff       (20)     6020 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner     (501) staff       (20)    14245 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner     (501) staff       (20)     1697 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     6795 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner     (501) staff       (20)     9208 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner     (501) staff       (20)     4365 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7692 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner     (501) staff       (20)     3865 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner     (501) staff       (20)     2683 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner     (501) staff       (20)    14856 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner     (501) staff       (20)    13092 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner     (501) staff       (20)    37304 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     3462 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner     (501) staff       (20)    29441 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     8074 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.795605 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.912268 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner     (501) staff       (20)    18037 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    17776 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    27841 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.913193 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner     (501) staff       (20)    15528 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    50865 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.914701 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner     (501) staff       (20)    16443 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    10797 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    37671 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.917878 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner     (501) staff       (20)     4240 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    23547 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner     (501) staff       (20)     2387 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    10744 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    35476 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner     (501) staff       (20)     5509 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.918733 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner     (501) staff       (20)     1989 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)     1746 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.920239 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner     (501) staff       (20)    17706 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     2846 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    28726 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.922411 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner     (501) staff       (20)    19426 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    18888 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    35843 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     1759 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.923803 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner     (501) staff       (20)    15366 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     4418 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    32283 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.926679 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/
+-rw-r--r--   0 runner     (501) staff       (20)     6284 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)    18263 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)     8229 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)     4400 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)      607 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)    27946 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.937054 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/
+-rw-r--r--   0 runner     (501) staff       (20)    81646 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner     (501) staff       (20)    18887 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    15898 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner     (501) staff       (20)     6937 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5106 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    26808 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     6368 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     4934 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner     (501) staff       (20)    20103 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    11570 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     9901 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     6162 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     4066 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner     (501) staff       (20)    20879 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    13867 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    14722 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)    10571 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    14540 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     6707 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5741 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.942942 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner     (501) staff       (20)    19307 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner     (501) staff       (20)    21579 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     4360 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner     (501) staff       (20)    14094 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     4026 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner     (501) staff       (20)    38322 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner     (501) staff       (20)    40579 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    21356 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner     (501) staff       (20)       85 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner     (501) staff       (20)    10518 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner     (501) staff       (20)    34903 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.949852 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner     (501) staff       (20)    12558 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    17273 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner     (501) staff       (20)     4178 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    22944 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    17176 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     9715 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    14351 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner     (501) staff       (20)     5539 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner     (501) staff       (20)    23586 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner     (501) staff       (20)    20749 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    33705 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     4104 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    22444 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.956318 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/
+-rw-r--r--   0 runner     (501) staff       (20)    14815 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner     (501) staff       (20)     8423 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner     (501) staff       (20)     3639 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner     (501) staff       (20)    20539 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner     (501) staff       (20)    11961 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner     (501) staff       (20)     8949 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     8308 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner     (501) staff       (20)    32704 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner     (501) staff       (20)     6877 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner     (501) staff       (20)     8063 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     6331 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner     (501) staff       (20)    60555 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner     (501) staff       (20)     7664 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner     (501) staff       (20)     6190 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.956756 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner     (501) staff       (20)     5387 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.958048 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/
+-rw-r--r--   0 runner     (501) staff       (20)     4481 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner     (501) staff       (20)     5345 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner     (501) staff       (20)    20603 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.961903 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner     (501) staff       (20)     6755 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner     (501) staff       (20)     7253 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner     (501) staff       (20)     9289 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner     (501) staff       (20)    15062 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner     (501) staff       (20)    15234 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner     (501) staff       (20)    11527 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7762 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner     (501) staff       (20)     4158 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.962390 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Jacobi/
+-rw-r--r--   0 runner     (501) staff       (20)    15902 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.964841 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/
+-rw-r--r--   0 runner     (501) staff       (20)     3057 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner     (501) staff       (20)    32803 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner     (501) staff       (20)    15064 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    21538 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner     (501) staff       (20)     3555 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.965276 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/
+-rw-r--r--   0 runner     (501) staff       (20)    13662 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.965716 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner     (501) staff       (20)     4588 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.967319 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner     (501) staff       (20)    16396 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner     (501) staff       (20)    62266 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner     (501) staff       (20)     5229 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.967748 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    22248 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.968275 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    20060 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.971384 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/
+-rw-r--r--   0 runner     (501) staff       (20)    24881 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)     4662 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    20805 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner     (501) staff       (20)    25478 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)    14022 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)     2993 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.971818 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    11405 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.974532 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/
+-rw-r--r--   0 runner     (501) staff       (20)    49870 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner     (501) staff       (20)    32949 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner     (501) staff       (20)     5099 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    12752 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    15957 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.975616 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner     (501) staff       (20)    24017 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner     (501) staff       (20)     6912 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.990954 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/
+-rw-r--r--   0 runner     (501) staff       (20)    10670 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     8164 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner     (501) staff       (20)    13178 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     2191 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     8080 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner     (501) staff       (20)    25592 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner     (501) staff       (20)     6485 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner     (501) staff       (20)    12720 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    25840 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     4737 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    12487 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     5808 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     3080 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner     (501) staff       (20)     1107 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner     (501) staff       (20)    12589 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner     (501) staff       (20)    52401 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    17923 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7329 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner     (501) staff       (20)     7049 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     1699 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner     (501) staff       (20)    15492 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner     (501) staff       (20)    25721 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner     (501) staff       (20)     4424 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     8704 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner     (501) staff       (20)     3175 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner     (501) staff       (20)     6437 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner     (501) staff       (20)     6602 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner     (501) staff       (20)    14831 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     8127 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner     (501) staff       (20)     9657 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.999141 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/
+-rw-r--r--   0 runner     (501) staff       (20)    27844 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner     (501) staff       (20)     4303 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)     7601 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner     (501) staff       (20)    10022 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     2049 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner     (501) staff       (20)     6712 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     6582 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner     (501) staff       (20)     3681 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner     (501) staff       (20)    10216 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     4181 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner     (501) staff       (20)     5723 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     8486 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     9028 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner     (501) staff       (20)     4979 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner     (501) staff       (20)     4545 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.999562 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseQR/
+-rw-r--r--   0 runner     (501) staff       (20)    28373 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.001496 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/
+-rw-r--r--   0 runner     (501) staff       (20)     5279 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner     (501) staff       (20)     4147 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner     (501) staff       (20)     5330 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     2809 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.001916 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    34345 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.002464 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    17202 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.007956 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/
+-rw-r--r--   0 runner     (501) staff       (20)     2913 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner     (501) staff       (20)     2742 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     1748 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner     (501) staff       (20)    30560 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner     (501) staff       (20)     7834 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner     (501) staff       (20)  1058368 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner     (501) staff       (20)      474 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.011364 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/
+-rw-r--r--   0 runner     (501) staff       (20)    13166 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    16929 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    37403 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     4828 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     5621 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     6375 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     2937 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.015975 cvxpy-1.3.2/cvxpy/cvxcore/python/
+-rw-r--r--   0 runner     (501) staff       (20)      139 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/python/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    20191 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/python/canonInterface.py
+-rw-r--r--   0 runner     (501) staff       (20)     2403 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/python/cvxcore.i
+-rw-r--r--   0 runner     (501) staff       (20)    38475 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/python/cvxcore.py
+-rw-r--r--   0 runner     (501) staff       (20)   885382 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/python/cvxcore_wrap.cxx
+-rw-r--r--   0 runner     (501) staff       (20)    54061 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/python/numpy.i
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.020217 cvxpy-1.3.2/cvxpy/cvxcore/src/
+-rw-r--r--   0 runner     (501) staff       (20)       24 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/.keep
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/LinOp.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    39092 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/LinOpOperations.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      844 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/LinOpOperations.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3365 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/ProblemData.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5057 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/Utils.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1454 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/Utils.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8098 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/cvxcore.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1328 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/cvxcore/src/cvxcore.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/error.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.022521 cvxpy-1.3.2/cvxpy/expressions/
+-rw-r--r--   0 runner     (501) staff       (20)      590 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.024251 cvxpy-1.3.2/cvxpy/expressions/constants/
+-rw-r--r--   0 runner     (501) staff       (20)      670 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/constants/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1071 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/constants/callback_param.py
+-rw-r--r--   0 runner     (501) staff       (20)     7756 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/constants/constant.py
+-rw-r--r--   0 runner     (501) staff       (20)     3737 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/constants/parameter.py
+-rw-r--r--   0 runner     (501) staff       (20)     3421 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/cvxtypes.py
+-rw-r--r--   0 runner     (501) staff       (20)    24786 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    16456 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/leaf.py
+-rw-r--r--   0 runner     (501) staff       (20)     4288 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/expressions/variable.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.026053 cvxpy-1.3.2/cvxpy/interface/
+-rw-r--r--   0 runner     (501) staff       (20)      611 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5171 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/base_matrix_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    10920 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/matrix_utilities.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.027985 cvxpy-1.3.2/cvxpy/interface/numpy_interface/
+-rw-r--r--   0 runner     (501) staff       (20)      818 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/numpy_interface/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2058 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/numpy_interface/matrix_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     2423 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/numpy_interface/ndarray_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     3446 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/numpy_interface/sparse_matrix_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     1405 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/interface/scipy_wrapper.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.030809 cvxpy-1.3.2/cvxpy/lin_ops/
+-rw-r--r--   0 runner     (501) staff       (20)      684 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/lin_ops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    38309 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/lin_ops/canon_backend.py
+-rw-r--r--   0 runner     (501) staff       (20)     1126 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/lin_ops/lin_constraints.py
+-rw-r--r--   0 runner     (501) staff       (20)     3370 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/lin_ops/lin_op.py
+-rw-r--r--   0 runner     (501) staff       (20)    18564 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/lin_ops/lin_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    12097 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/lin_ops/tree_mat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.033606 cvxpy-1.3.2/cvxpy/problems/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/problems/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4958 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/problems/iterative.py
+-rw-r--r--   0 runner     (501) staff       (20)     7339 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/problems/objective.py
+-rw-r--r--   0 runner     (501) staff       (20)     1615 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/problems/param_prob.py
+-rw-r--r--   0 runner     (501) staff       (20)    62475 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/problems/problem.py
+-rw-r--r--   0 runner     (501) staff       (20)     2921 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/problems/xpress_problem.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/py.typed
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.038389 cvxpy-1.3.2/cvxpy/reductions/
+-rw-r--r--   0 runner     (501) staff       (20)     1452 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4850 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/canonicalization.py
+-rw-r--r--   0 runner     (501) staff       (20)     2667 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/chain.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.039224 cvxpy-1.3.2/cvxpy/reductions/complex2real/
+-rw-r--r--   0 runner     (501) staff       (20)      566 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.045138 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     4612 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1058 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     3462 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      912 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1780 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2240 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     7500 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      860 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/param_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      815 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1042 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1554 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1720 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     8302 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/complex2real/complex2real.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.046970 cvxpy-1.3.2/cvxpy/reductions/cone2cone/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/cone2cone/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    17759 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/cone2cone/affine2direct.py
+-rw-r--r--   0 runner     (501) staff       (20)     7035 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/cone2cone/approximations.py
+-rw-r--r--   0 runner     (501) staff       (20)     3035 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/cone2cone/exotic2common.py
+-rw-r--r--   0 runner     (501) staff       (20)     5848 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/cvx_attr2constr.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.048271 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/
+-rw-r--r--   0 runner     (501) staff       (20)      564 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.062329 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     4264 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/entr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      965 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/exp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1067 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/geo_mean_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1514 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/huber_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/indicator_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      937 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/kl_div_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_max_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1495 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_sum_largest_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      705 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log1p_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1049 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_det_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1690 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_sum_exp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1118 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/logistic_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/matrix_frac_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1211 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/mul_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1310 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/normNuc_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     3661 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/perspective_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2403 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/pnorm_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1427 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/power_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1282 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_form_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1185 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_over_lin_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      938 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/rel_entr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1124 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/sigma_max_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2134 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/suppfunc_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1683 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/tr_inv_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1972 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/von_neumann_entr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1163 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/xexp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)    16778 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py
+-rw-r--r--   0 runner     (501) staff       (20)     5442 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dcp2cone/dcp2cone.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.063679 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.076039 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     5713 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      995 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/add_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      732 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/constant_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      101 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/div_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/exp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1444 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/eye_minus_inv_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      152 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/geo_mean_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)       63 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/gmatmul_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      101 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/log_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      126 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/mul_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/mulexpression_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/nonpos_constr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      258 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/norm1_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      269 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/norm_inf_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      173 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/one_minus_pos_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/parameter_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      694 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pf_eigenvalue_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      697 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pnorm_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      122 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/power_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      154 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/prod_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      326 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/quad_form_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      295 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/quad_over_lin_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      709 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/sum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      293 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/trace_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      125 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/xexp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      161 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/zero_constr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     3289 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/dgp2dcp.py
+-rw-r--r--   0 runner     (501) staff       (20)      273 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.077090 cvxpy-1.3.2/cvxpy/reductions/discrete2mixedint/
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/discrete2mixedint/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2750 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.079680 cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/
+-rw-r--r--   0 runner     (501) staff       (20)      562 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9534 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3453 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/inverse.py
+-rw-r--r--   0 runner     (501) staff       (20)     5154 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/sets.py
+-rw-r--r--   0 runner     (501) staff       (20)     1154 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/tighten.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.080798 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/
+-rw-r--r--   0 runner     (501) staff       (20)      566 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.086930 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     2079 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      748 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/abs_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1106 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cummax_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1133 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cumsum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1380 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/dotsort_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1333 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/max_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      765 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/maximum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      883 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/min_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      880 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/minimum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1187 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm1_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1329 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm_inf_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/sum_largest_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1465 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py
+-rw-r--r--   0 runner     (501) staff       (20)     2689 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/eval_params.py
+-rw-r--r--   0 runner     (501) staff       (20)     2051 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/flip_objective.py
+-rw-r--r--   0 runner     (501) staff       (20)     1944 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/inverse_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     2597 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/matrix_stuffing.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.088259 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/
+-rw-r--r--   0 runner     (501) staff       (20)      564 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.090786 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     2097 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1494 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/huber_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1431 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/power_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      967 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_form_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1298 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_over_lin_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2393 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py
+-rw-r--r--   0 runner     (501) staff       (20)    11911 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py
+-rw-r--r--   0 runner     (501) staff       (20)     5050 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/reduction.py
+-rw-r--r--   0 runner     (501) staff       (20)     3020 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solution.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.095864 cvxpy-1.3.2/cvxpy/reductions/solvers/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7382 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/bisection.py
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/compr_matrix.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.106538 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/
+-rw-r--r--   0 runner     (501) staff       (20)     1145 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7745 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     6970 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    14223 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/conic_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)    12853 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/copt_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    18657 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    13569 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     6715 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     5058 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     6658 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     8903 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/glop_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     3939 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     4477 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    14154 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    28743 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     9595 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/nag_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     9572 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    15715 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/scip_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    10342 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    13211 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/scs_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     9031 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    15320 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/constant_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)     5166 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/defines.py
+-rw-r--r--   0 runner     (501) staff       (20)     4177 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/intermediate_chain.py
+-rw-r--r--   0 runner     (501) staff       (20)     4372 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/kktsolver.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.106998 cvxpy-1.3.2/cvxpy/reductions/solvers/lp_solvers/
+-rw-r--r--   0 runner     (501) staff       (20)      566 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/lp_solvers/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.111617 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5955 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     5766 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     9848 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     4222 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     5723 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     3557 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/qp_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)     9408 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     2495 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/solver.py
+-rw-r--r--   0 runner     (501) staff       (20)    16745 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/solving_chain.py
+-rw-r--r--   0 runner     (501) staff       (20)     2830 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/solvers/utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)     6122 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/reductions/utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)     5120 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/settings.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.137310 cvxpy-1.3.2/cvxpy/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1497 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/base_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1963 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/ram_limited.py
+-rw-r--r--   0 runner     (501) staff       (20)    45230 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/solver_test_helpers.py
+-rw-r--r--   0 runner     (501) staff       (20)    66346 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_atoms.py
+-rw-r--r--   0 runner     (501) staff       (20)     9823 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_benchmarks.py
+-rw-r--r--   0 runner     (501) staff       (20)    29018 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_complex.py
+-rw-r--r--   0 runner     (501) staff       (20)    29804 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_cone2cone.py
+-rw-r--r--   0 runner     (501) staff       (20)    80205 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_conic_solvers.py
+-rw-r--r--   0 runner     (501) staff       (20)     1005 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_constant.py
+-rw-r--r--   0 runner     (501) staff       (20)    19098 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_constant_atoms.py
+-rw-r--r--   0 runner     (501) staff       (20)    13743 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_constraints.py
+-rw-r--r--   0 runner     (501) staff       (20)     7343 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_convolution.py
+-rw-r--r--   0 runner     (501) staff       (20)     2983 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     3491 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_curvature.py
+-rw-r--r--   0 runner     (501) staff       (20)     3939 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_custom_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)    25483 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_derivative.py
+-rw-r--r--   0 runner     (501) staff       (20)     7749 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_dgp.py
+-rw-r--r--   0 runner     (501) staff       (20)    27269 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_dgp2dcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     7197 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_domain.py
+-rw-r--r--   0 runner     (501) staff       (20)    32192 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_dpp.py
+-rw-r--r--   0 runner     (501) staff       (20)    25997 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_dqcp.py
+-rw-r--r--   0 runner     (501) staff       (20)    21420 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_examples.py
+-rw-r--r--   0 runner     (501) staff       (20)    52582 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_expressions.py
+-rw-r--r--   0 runner     (501) staff       (20)    32554 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_grad.py
+-rw-r--r--   0 runner     (501) staff       (20)     1570 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_gurobi_write.py
+-rw-r--r--   0 runner     (501) staff       (20)     7545 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_interfaces.py
+-rw-r--r--   0 runner     (501) staff       (20)     7671 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_kron_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     4949 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_lin_ops.py
+-rw-r--r--   0 runner     (501) staff       (20)    16619 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_linear_cone.py
+-rw-r--r--   0 runner     (501) staff       (20)     5135 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_matrices.py
+-rw-r--r--   0 runner     (501) staff       (20)     4090 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_mip_vars.py
+-rw-r--r--   0 runner     (501) staff       (20)     2993 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_monotonicity.py
+-rw-r--r--   0 runner     (501) staff       (20)     6616 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_nonlinear_atoms.py
+-rw-r--r--   0 runner     (501) staff       (20)     3694 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_numpy.py
+-rw-r--r--   0 runner     (501) staff       (20)     4985 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_objectives.py
+-rw-r--r--   0 runner     (501) staff       (20)     4260 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_param_cone_prog.py
+-rw-r--r--   0 runner     (501) staff       (20)     4223 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_param_quad_prog.py
+-rw-r--r--   0 runner     (501) staff       (20)    12777 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_perspective.py
+-rw-r--r--   0 runner     (501) staff       (20)     4337 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_power_tools.py
+-rw-r--r--   0 runner     (501) staff       (20)    81538 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_problem.py
+-rw-r--r--   0 runner     (501) staff       (20)    43578 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_python_backends.py
+-rw-r--r--   0 runner     (501) staff       (20)    22394 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_qp_solvers.py
+-rw-r--r--   0 runner     (501) staff       (20)     7895 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_quad_form.py
+-rw-r--r--   0 runner     (501) staff       (20)     6631 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_quadratic.py
+-rw-r--r--   0 runner     (501) staff       (20)     3247 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_semidefinite_vars.py
+-rw-r--r--   0 runner     (501) staff       (20)     3992 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_shape.py
+-rw-r--r--   0 runner     (501) staff       (20)     2694 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_sign.py
+-rw-r--r--   0 runner     (501) staff       (20)     7775 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_suppfunc.py
+-rw-r--r--   0 runner     (501) staff       (20)    11072 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_valinvec2mixedint.py
+-rw-r--r--   0 runner     (501) staff       (20)     1901 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_versioning.py
+-rw-r--r--   0 runner     (501) staff       (20)     9116 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/tests/test_von_neumann_entr.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.140012 cvxpy-1.3.2/cvxpy/transforms/
+-rw-r--r--   0 runner     (501) staff       (20)      996 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/transforms/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3672 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/transforms/indicator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2088 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/transforms/linearize.py
+-rw-r--r--   0 runner     (501) staff       (20)    10918 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/transforms/partial_optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)     4306 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/transforms/scalarize.py
+-rw-r--r--   0 runner     (501) staff       (20)     6761 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/transforms/suppfunc.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:18.148585 cvxpy-1.3.2/cvxpy/utilities/
+-rw-r--r--   0 runner     (501) staff       (20)      629 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5446 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/canonical.py
+-rw-r--r--   0 runner     (501) staff       (20)    12219 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/coeff_extractor.py
+-rw-r--r--   0 runner     (501) staff       (20)     2968 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/cvxpy_upgrade.py
+-rw-r--r--   0 runner     (501) staff       (20)     3264 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/debug_tools.py
+-rw-r--r--   0 runner     (501) staff       (20)      245 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/deterministic.py
+-rw-r--r--   0 runner     (501) staff       (20)     1424 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/grad.py
+-rw-r--r--   0 runner     (501) staff       (20)     6226 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/key_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5897 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/linalg.py
+-rw-r--r--   0 runner     (501) staff       (20)     2437 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/performance_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2178 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/perspective_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    19336 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/power_tools.py
+-rw-r--r--   0 runner     (501) staff       (20)     1552 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/replace_quad_forms.py
+-rw-r--r--   0 runner     (501) staff       (20)     1399 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/scopes.py
+-rw-r--r--   0 runner     (501) staff       (20)     4983 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/shape.py
+-rw-r--r--   0 runner     (501) staff       (20)     1968 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/sign.py
+-rw-r--r--   0 runner     (501) staff       (20)     1825 2023-06-27 07:55:56.000000 cvxpy-1.3.2/cvxpy/utilities/versioning.py
+-rw-r--r--   0 runner     (501) staff       (20)      213 2023-06-27 08:01:06.000000 cvxpy-1.3.2/cvxpy/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-27 08:01:17.815392 cvxpy-1.3.2/cvxpy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     9055 2023-06-27 08:01:10.000000 cvxpy-1.3.2/cvxpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    32903 2023-06-27 08:01:17.000000 cvxpy-1.3.2/cvxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-27 08:01:10.000000 cvxpy-1.3.2/cvxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-27 07:58:08.000000 cvxpy-1.3.2/cvxpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      412 2023-06-27 08:01:10.000000 cvxpy-1.3.2/cvxpy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       15 2023-06-27 08:01:10.000000 cvxpy-1.3.2/cvxpy.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1297 2023-06-27 07:55:56.000000 cvxpy-1.3.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      386 2023-06-27 08:01:18.154707 cvxpy-1.3.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     8455 2023-06-27 07:55:56.000000 cvxpy-1.3.2/setup.py
```

### Comparing `cvxpy-1.3.1/LICENSE` & `cvxpy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/PKG-INFO` & `cvxpy-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A domain-specific language for modeling convex optimization problems in Python.
 Home-page: https://github.com/cvxpy/cvxpy
 Author: Steven Diamond, Eric Chu, Stephen Boyd
 Author-email: stevend2@stanford.edu, akshayka@cs.stanford.edu, echu508@stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Description: CVXPY
         =====================
```

### Comparing `cvxpy-1.3.1/README.md` & `cvxpy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/__init__.py` & `cvxpy-1.3.2/cvxpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/__init__.py` & `cvxpy-1.3.2/cvxpy/atoms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 limitations under the License.
 """
 
 from cvxpy.atoms.affine.binary_operators import (matmul, multiply,
                                                  scalar_product,)
 from cvxpy.atoms.affine.bmat import bmat
 from cvxpy.atoms.affine.conj import conj
-from cvxpy.atoms.affine.conv import conv
+from cvxpy.atoms.affine.conv import conv, convolve
 from cvxpy.atoms.affine.cumsum import cumsum
 from cvxpy.atoms.affine.diag import diag
 from cvxpy.atoms.affine.diff import diff
 from cvxpy.atoms.affine.hstack import hstack
 from cvxpy.atoms.affine.imag import imag
 from cvxpy.atoms.affine.kron import kron
 from cvxpy.atoms.affine.partial_trace import partial_trace
@@ -112,15 +112,14 @@
     power,
     huber,
 ]
 
 EXP_ATOMS = [
     log_sum_exp,
     log_det,
-    tr_inv,
     entr,
     exp,
     kl_div,
     rel_entr,
     von_neumann_entr,
     log,
     log1p,
@@ -132,14 +131,15 @@
     lambda_max,
     lambda_sum_largest,
     condition_number,
     log_det,
     MatrixFrac,
     normNuc,
     sigma_max,
+    tr_inv,
 ]
 
 NONPOS_ATOMS = [
     norm1,
     abs,
     huber,
 ]
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/__init__.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/add_expr.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/add_expr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/affine_atom.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/affine_atom.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/binary_operators.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/binary_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 from cvxpy.atoms.affine.add_expr import AddExpression
 from cvxpy.atoms.affine.affine_atom import AffAtom
 from cvxpy.atoms.affine.conj import conj
 from cvxpy.atoms.affine.reshape import deep_flatten
 from cvxpy.atoms.affine.sum import sum as cvxpy_sum
 from cvxpy.constraints.constraint import Constraint
 from cvxpy.error import DCPError
-from cvxpy.expressions.constants.parameter import (is_param_affine,
-                                                   is_param_free,)
+from cvxpy.expressions.constants.parameter import (
+    is_param_affine,
+    is_param_free,
+)
 
 
 class BinaryOperator(AffAtom):
     """
     Base class for expressions involving binary operators. (other than addition)
 
     """
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/bmat.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/bmat.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/conj.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/conj.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/conv.py` & `cvxpy-1.3.2/cvxpy/atoms/von_neumann_entr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,127 @@
 """
-Copyright 2013 Steven Diamond
+Copyright 2022, the CVXPY authors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 from typing import List, Tuple
 
 import numpy as np
+from scipy import linalg as LA
+from scipy.special import entr
 
-import cvxpy.interface as intf
-import cvxpy.lin_ops.lin_op as lo
-import cvxpy.lin_ops.lin_utils as lu
-import cvxpy.utilities as u
-from cvxpy.atoms.affine.affine_atom import AffAtom
+from cvxpy.atoms.atom import Atom
 from cvxpy.constraints.constraint import Constraint
 
 
-class conv(AffAtom):
-    """ 1D discrete convolution of two vectors.
+class von_neumann_entr(Atom):
+    """
+    Computes the Von Neumann Entropy of the positive-definite matrix
+    :math:`X\\in\\mathbb{S}^n_{+}`
+
+        .. math::
+            -\\operatorname{tr}(X \\operatorname{logm}(X))
 
-    The discrete convolution :math:`c` of vectors :math:`a` and :math:`b` of
-    lengths :math:`n` and :math:`m`, respectively, is a length-:math:`(n+m-1)`
-    vector where
+    where :math:`\\operatorname{tr}` is the trace and
+    :math:`\\operatorname{logm}` is the matrix logarithm
 
-    .. math::
+    | May alternatively be expressed as:
 
-        c_k = \\sum_{i+j=k} a_ib_j, \\quad k=0, \\ldots, n+m-2.
+        .. math::
+            \\texttt{von_neumann_entr}(X) = -\\textstyle\\sum_{i=1}^n \\lambda_i \\log \\lambda_i
+
+    | where :math:`\\lambda_{i}` are the eigenvalues of :math:`X`
+    This atom does not enforce :math:`\\operatorname{tr}(X) = 1`
+    as is expected in applications from quantum mechanics.
 
     Parameters
     ----------
-    lh_expr : Constant
-        A constant 1D vector or a 2D column vector.
-    rh_expr : Expression
-        A 1D vector or a 2D column vector.
+    X : Expression or numeric
+        A PSD matrix
     """
-    # TODO work with right hand constant.
-    # TODO(akshayka): make DGP-compatible
 
-    def __init__(self, lh_expr, rh_expr) -> None:
-        super(conv, self).__init__(lh_expr, rh_expr)
+    def __init__(self, X, quad_approx: Tuple[int, int] = ()) -> None:
+        # TODO: add a check that N is symmetric/Hermitian.
+        self.quad_approx = quad_approx
+        super(von_neumann_entr, self).__init__(X)
 
-    @AffAtom.numpy_numeric
     def numeric(self, values):
-        """Convolve the two values.
-        """
-        # Convert values to 1D.
-        values = list(map(intf.from_2D_to_1D, values))
-        return np.convolve(values[0], values[1])
+        N = values[0]
+        if hasattr(N, 'value'):
+            N = N.value  # assume this is an ndarray
+        w = LA.eigvalsh(N)
+        val = np.sum(entr(w))
+        return val
 
     def validate_arguments(self) -> None:
-        """Checks that both arguments are vectors, and the first is constant.
+        """Verify that the argument A is PSD.
         """
-        if not self.args[0].is_vector() or not self.args[1].is_vector():
-            raise ValueError("The arguments to conv must resolve to vectors.")
-        if not self.args[0].is_constant():
-            raise ValueError("The first argument to conv must be constant.")
-
-    def shape_from_args(self) -> Tuple[int, int]:
-        """The sum of the argument dimensions - 1.
-        """
-        lh_length = self.args[0].shape[0]
-        rh_length = self.args[1].shape[0]
-        return (lh_length + rh_length - 1, 1)
+        N = self.args[0]
+        if N.size > 1:
+            if N.ndim != 2 or N.shape[0] != N.shape[1]:
+                raise ValueError('Argument must be a square matrix.')
 
     def sign_from_args(self) -> Tuple[bool, bool]:
-        """Same as times.
+        """Returns sign (is positive, is negative) of the expression.
+        """
+        return (False, False)
+
+    def is_atom_convex(self) -> bool:
+        """Is the atom convex?
+        """
+        return False
+
+    def shape_from_args(self) -> Tuple[int, ...]:
+        """Returns the shape of the expression.
         """
-        return u.sign.mul_sign(self.args[0], self.args[1])
+        return tuple()
+
+    def is_atom_concave(self) -> bool:
+        """Is the atom concave?
+        """
+        return True
 
     def is_incr(self, idx) -> bool:
         """Is the composition non-decreasing in argument idx?
         """
-        return self.args[0].is_nonneg()
+        return False
 
     def is_decr(self, idx) -> bool:
         """Is the composition non-increasing in argument idx?
         """
-        return self.args[0].is_nonpos()
+        return False
+
+    def get_data(self):
+        return [self.quad_approx]
+
+    def _grad(self, values):
+        """Gives the (sub/super)gradient of the atom w.r.t. each argument.
+
+        Matrix expressions are vectorized, so the gradient is a matrix.
+
+        Args:
+            values: A list of numeric values for the arguments.
+
+        Returns:
+            A list of SciPy CSC sparse matrices or None.
+        """
+        # N = values[0]
+        # L = cholesky(N)
+        # derivative = 2*(L + L * logm(np.dot(L.T, L)))
+        # TODO: have to wrap derivative around scipy CSC sparse matrices
+        #  compare to log_det atom.
+        raise ValueError()
 
-    def graph_implementation(
-        self, arg_objs, shape: Tuple[int, ...], data=None
-    ) -> Tuple[lo.LinOp, List[Constraint]]:
-        """Convolve two vectors.
-
-        Parameters
-        ----------
-        arg_objs : list
-            LinExpr for each argument.
-        shape : tuple
-            The shape of the resulting expression.
-        data :
-            Additional data required by the atom.
-
-        Returns
-        -------
-        tuple
-            (LinOp for objective, list of constraints)
+    def _domain(self) -> List[Constraint]:
+        """Returns constraints describing the domain of the node.
         """
-        return (lu.conv(arg_objs[0], arg_objs[1], shape), [])
+        return [self.args[0] >> 0]
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/cumsum.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/cumsum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/diag.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/diag.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/diff.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/diff.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/hstack.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/hstack.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/imag.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/imag.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/index.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/index.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/kron.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/kron.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/partial_trace.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/partial_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         else:
             eye_mat = sp.eye(dim)
             a = sp.kron(a, eye_mat)
             b = sp.kron(b, eye_mat)
     return a @ expr @ b
 
 
-# flake8: noqa: E501
+# ruff: noqa: E501
 def partial_trace(expr, dims: Tuple[int], axis: Optional[int] = 0):
     """
     Assumes :math:`\\texttt{expr} = X_1 \\otimes \\cdots \\otimes X_n` is a 2D Kronecker
     product composed of :math:`n = \\texttt{len(dims)}` implicit subsystems.
     Letting :math:`k = \\texttt{axis}`, the returned expression represents
     the *partial trace* of :math:`\\texttt{expr}` along its :math:`k^{\\text{th}}` implicit subsystem:
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/partial_transpose.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/partial_transpose.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/promote.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/promote.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/real.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/real.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/reshape.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/reshape.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/sum.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/sum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/trace.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/trace.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/transpose.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/transpose.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/unary_operators.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/unary_operators.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/upper_tri.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/upper_tri.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/vec.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/vec.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/vstack.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/vstack.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/affine/wraps.py` & `cvxpy-1.3.2/cvxpy/atoms/affine/wraps.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/atom.py` & `cvxpy-1.3.2/cvxpy/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/axis_atom.py` & `cvxpy-1.3.2/cvxpy/atoms/axis_atom.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/condition_number.py` & `cvxpy-1.3.2/cvxpy/atoms/condition_number.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/cummax.py` & `cvxpy-1.3.2/cvxpy/atoms/cummax.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/dist_ratio.py` & `cvxpy-1.3.2/cvxpy/atoms/dist_ratio.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/dotsort.py` & `cvxpy-1.3.2/cvxpy/atoms/dotsort.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/__init__.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/abs.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/abs.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/ceil.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/ceil.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/elementwise.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/elementwise.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/entr.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/exp.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/exp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/huber.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/huber.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/inv_pos.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/inv_pos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/kl_div.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/kl_div.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/log.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/log.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/log1p.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/log1p.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/log_normcdf.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/log_normcdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 from cvxpy.atoms.affine.reshape import reshape
 from cvxpy.atoms.affine.sum import sum as sum_
 from cvxpy.atoms.elementwise.maximum import maximum
 from cvxpy.expressions.expression import Expression
 
 
-# flake8: noqa: E501
-def log_normcdf(x):  # noqa: E501
+# ruff: noqa: E501
+def log_normcdf(x):
     """Elementwise log of the cumulative distribution function of a standard normal random variable.
 
     The implementation is a quadratic approximation with modest accuracy over [-4, 4].
     For details on the nature of the approximation, refer to
     `CVXPY GitHub PR #1224 <https://github.com/cvxpy/cvxpy/pull/1224#issue-793221374>`_.
 
     .. note::
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/loggamma.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/loggamma.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 from cvxpy.atoms.elementwise.entr import entr
 from cvxpy.atoms.elementwise.log import log
 from cvxpy.atoms.elementwise.maximum import maximum
 
 
-# flake8: noqa: E501
+# ruff: noqa: E501
 def loggamma(x):
     """Elementwise log of the gamma function.
 
     Implementation has modest accuracy over the full range, approaching perfect
     accuracy as x goes to infinity. For details on the nature of the approximation,
     refer to `CVXPY GitHub Issue #228 <https://github.com/cvxpy/cvxpy/issues/228#issuecomment-544281906>`_.
     """
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/logistic.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/logistic.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/maximum.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/maximum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/minimum.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/minimum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/neg.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/neg.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/pos.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/pos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/power.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/power.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/rel_entr.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/rel_entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/scalene.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/scalene.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/sqrt.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/sqrt.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/square.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/square.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/elementwise/xexp.py` & `cvxpy-1.3.2/cvxpy/atoms/elementwise/xexp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/eye_minus_inv.py` & `cvxpy-1.3.2/cvxpy/atoms/eye_minus_inv.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/gen_lambda_max.py` & `cvxpy-1.3.2/cvxpy/atoms/gen_lambda_max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/geo_mean.py` & `cvxpy-1.3.2/cvxpy/atoms/geo_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,22 @@
 
 import numpy as np
 import scipy.sparse as sp
 
 from cvxpy.atoms.atom import Atom
 from cvxpy.constraints.constraint import Constraint
 from cvxpy.expressions import cvxtypes
-from cvxpy.utilities.power_tools import (approx_error, decompose, fracify,
-                                         lower_bound, over_bound, prettydict,)
+from cvxpy.utilities.power_tools import (
+    approx_error,
+    decompose,
+    fracify,
+    lower_bound,
+    over_bound,
+    prettydict,
+)
 
 
 class geo_mean(Atom):
     """ The (weighted) geometric mean of vector ``x``, with optional powers given by ``p``:
 
     .. math::
```

### Comparing `cvxpy-1.3.1/cvxpy/atoms/gmatmul.py` & `cvxpy-1.3.2/cvxpy/atoms/gmatmul.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/harmonic_mean.py` & `cvxpy-1.3.2/cvxpy/atoms/harmonic_mean.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/inv_prod.py` & `cvxpy-1.3.2/cvxpy/atoms/inv_prod.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/lambda_max.py` & `cvxpy-1.3.2/cvxpy/atoms/lambda_max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/lambda_min.py` & `cvxpy-1.3.2/cvxpy/atoms/lambda_min.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/lambda_sum_largest.py` & `cvxpy-1.3.2/cvxpy/atoms/lambda_sum_largest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/lambda_sum_smallest.py` & `cvxpy-1.3.2/cvxpy/atoms/lambda_sum_smallest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/length.py` & `cvxpy-1.3.2/cvxpy/atoms/length.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/log_det.py` & `cvxpy-1.3.2/cvxpy/atoms/log_det.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/log_sum_exp.py` & `cvxpy-1.3.2/cvxpy/atoms/log_sum_exp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/matrix_frac.py` & `cvxpy-1.3.2/cvxpy/atoms/matrix_frac.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/max.py` & `cvxpy-1.3.2/cvxpy/atoms/max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/min.py` & `cvxpy-1.3.2/cvxpy/atoms/min.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/mixed_norm.py` & `cvxpy-1.3.2/cvxpy/atoms/mixed_norm.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/norm.py` & `cvxpy-1.3.2/cvxpy/atoms/norm.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/norm1.py` & `cvxpy-1.3.2/cvxpy/atoms/norm1.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/norm_inf.py` & `cvxpy-1.3.2/cvxpy/atoms/norm_inf.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/norm_nuc.py` & `cvxpy-1.3.2/cvxpy/atoms/norm_nuc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/one_minus_pos.py` & `cvxpy-1.3.2/cvxpy/atoms/one_minus_pos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/perspective.py` & `cvxpy-1.3.2/cvxpy/atoms/perspective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/pf_eigenvalue.py` & `cvxpy-1.3.2/cvxpy/atoms/pf_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/pnorm.py` & `cvxpy-1.3.2/cvxpy/atoms/pnorm.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/prod.py` & `cvxpy-1.3.2/cvxpy/atoms/prod.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/quad_form.py` & `cvxpy-1.3.2/cvxpy/atoms/quad_form.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/quad_over_lin.py` & `cvxpy-1.3.2/cvxpy/atoms/quad_over_lin.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/sigma_max.py` & `cvxpy-1.3.2/cvxpy/atoms/sigma_max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/sign.py` & `cvxpy-1.3.2/cvxpy/atoms/sign.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/sum_largest.py` & `cvxpy-1.3.2/cvxpy/atoms/sum_largest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/sum_smallest.py` & `cvxpy-1.3.2/cvxpy/atoms/sum_smallest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/sum_squares.py` & `cvxpy-1.3.2/cvxpy/atoms/sum_squares.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/suppfunc.py` & `cvxpy-1.3.2/cvxpy/atoms/suppfunc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/total_variation.py` & `cvxpy-1.3.2/cvxpy/atoms/total_variation.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/atoms/tr_inv.py` & `cvxpy-1.3.2/cvxpy/atoms/tr_inv.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/__init__.py` & `cvxpy-1.3.2/cvxpy/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/constraint.py` & `cvxpy-1.3.2/cvxpy/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/exponential.py` & `cvxpy-1.3.2/cvxpy/constraints/exponential.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/finite_set.py` & `cvxpy-1.3.2/cvxpy/constraints/finite_set.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/nonpos.py` & `cvxpy-1.3.2/cvxpy/constraints/nonpos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/power.py` & `cvxpy-1.3.2/cvxpy/constraints/power.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             raise ValueError(msg)
         super(PowCone3D, self).__init__([self.x, self.y, self.z],
                                         constr_id)
 
     def __str__(self) -> str:
         return "Pow3D(%s, %s, %s; %s)" % (self.x, self.y, self.z, self.alpha)
 
+    @property
     def residual(self):
         # TODO: The projection should be implemented directly.
         from cvxpy import Minimize, Problem, Variable, hstack, norm2
         if self.x.value is None or self.y.value is None or self.z.value is None:
             return None
         x = Variable(self.x.shape)
         y = Variable(self.y.shape)
```

### Comparing `cvxpy-1.3.1/cvxpy/constraints/psd.py` & `cvxpy-1.3.2/cvxpy/constraints/psd.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/second_order.py` & `cvxpy-1.3.2/cvxpy/constraints/second_order.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/utilities.py` & `cvxpy-1.3.2/cvxpy/constraints/utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/constraints/zero.py` & `cvxpy-1.3.2/cvxpy/constraints/zero.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/CMakeLists.txt` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Cholesky` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/CholmodSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Core` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Eigenvalues` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Geometry` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Householder` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Jacobi` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/LU` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/MetisSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/OrderingMethods` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/PaStiXSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/PardisoSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/QR` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SPQRSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SVD` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/Sparse` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseCholesky` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseCore` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseLU` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SparseQR` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/StdDeque` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/StdList` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/StdVector` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/SuperLUSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/UmfPackSupport` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Array.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Block.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/IO.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Map.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Product.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Random.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Select.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/Image.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/blas.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `cvxpy-1.3.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/python/canonInterface.py` & `cvxpy-1.3.2/cvxpy/cvxcore/python/canonInterface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/python/cvxcore.i` & `cvxpy-1.3.2/cvxpy/cvxcore/python/cvxcore.i`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/python/cvxcore.py` & `cvxpy-1.3.2/cvxpy/cvxcore/python/cvxcore.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/python/cvxcore_wrap.cxx` & `cvxpy-1.3.2/cvxpy/cvxcore/python/cvxcore_wrap.cxx`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/python/numpy.i` & `cvxpy-1.3.2/cvxpy/cvxcore/python/numpy.i`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/LinOp.hpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/LinOp.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/LinOpOperations.cpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/LinOpOperations.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/LinOpOperations.hpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/LinOpOperations.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/ProblemData.hpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/ProblemData.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/Utils.cpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/Utils.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/Utils.hpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/Utils.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/cvxcore.cpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/cvxcore.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/cvxcore/src/cvxcore.hpp` & `cvxpy-1.3.2/cvxpy/cvxcore/src/cvxcore.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/error.py` & `cvxpy-1.3.2/cvxpy/error.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/__init__.py` & `cvxpy-1.3.2/cvxpy/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/constants/__init__.py` & `cvxpy-1.3.2/cvxpy/expressions/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/constants/callback_param.py` & `cvxpy-1.3.2/cvxpy/expressions/constants/callback_param.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/constants/constant.py` & `cvxpy-1.3.2/cvxpy/expressions/constants/constant.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/constants/parameter.py` & `cvxpy-1.3.2/cvxpy/expressions/constants/parameter.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/cvxtypes.py` & `cvxpy-1.3.2/cvxpy/expressions/cvxtypes.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/expression.py` & `cvxpy-1.3.2/cvxpy/expressions/expression.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/expressions/leaf.py` & `cvxpy-1.3.2/cvxpy/expressions/leaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,19 @@
 import numpy as np
 import numpy.linalg as LA
 import scipy.sparse as sp
 
 import cvxpy.interface as intf
 from cvxpy.constraints.constraint import Constraint
 from cvxpy.expressions import expression
-from cvxpy.settings import (GENERAL_PROJECTION_TOL, PSD_NSD_PROJECTION_TOL,
-                            SPARSE_PROJECTION_TOL,)
+from cvxpy.settings import (
+    GENERAL_PROJECTION_TOL,
+    PSD_NSD_PROJECTION_TOL,
+    SPARSE_PROJECTION_TOL,
+)
 
 
 class Leaf(expression.Expression):
     """
     A leaf node of an expression tree; i.e., a Variable, Constant, or Parameter.
 
     A leaf may carry *attributes* that constrain the set values permissible
```

### Comparing `cvxpy-1.3.1/cvxpy/expressions/variable.py` & `cvxpy-1.3.2/cvxpy/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/__init__.py` & `cvxpy-1.3.2/cvxpy/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/base_matrix_interface.py` & `cvxpy-1.3.2/cvxpy/interface/base_matrix_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/matrix_utilities.py` & `cvxpy-1.3.2/cvxpy/interface/matrix_utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/numpy_interface/__init__.py` & `cvxpy-1.3.2/cvxpy/interface/numpy_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/numpy_interface/matrix_interface.py` & `cvxpy-1.3.2/cvxpy/interface/numpy_interface/matrix_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/numpy_interface/ndarray_interface.py` & `cvxpy-1.3.2/cvxpy/interface/numpy_interface/ndarray_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/numpy_interface/sparse_matrix_interface.py` & `cvxpy-1.3.2/cvxpy/interface/numpy_interface/sparse_matrix_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/interface/scipy_wrapper.py` & `cvxpy-1.3.2/cvxpy/interface/scipy_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,39 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from scipy.sparse import spmatrix
+from scipy import sparse
 
 from cvxpy.expressions import expression as exp
 
+SPARSE_MATRIX_CLASSES = [
+    sparse.csc_matrix, 
+    sparse.csr_matrix, 
+    sparse.coo_matrix, 
+    sparse.bsr_matrix, 
+    sparse.lil_matrix, 
+    sparse.dia_matrix,
+    sparse.dok_matrix,
+]
 BIN_OPS = ["__div__", "__mul__", "__add__", "__sub__",
            "__le__", "__eq__", "__lt__", "__gt__"]
 
 
 def wrap_bin_op(method):
     """Factory for wrapping binary operators.
     """
     def new_method(self, other):
         if isinstance(other, exp.Expression):
             return NotImplemented
         else:
             return method(self, other)
     return new_method
 
-
-for method_name in BIN_OPS:
-    method = getattr(spmatrix, method_name)
-    new_method = wrap_bin_op(method)
-    setattr(spmatrix, method_name, new_method)
+for cls in SPARSE_MATRIX_CLASSES:
+    for method_name in BIN_OPS:
+        method = getattr(cls, method_name)
+        new_method = wrap_bin_op(method)
+        setattr(cls, method_name, new_method)
```

### Comparing `cvxpy-1.3.1/cvxpy/lin_ops/__init__.py` & `cvxpy-1.3.2/cvxpy/lin_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/lin_ops/canon_backend.py` & `cvxpy-1.3.2/cvxpy/lin_ops/canon_backend.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/lin_ops/lin_constraints.py` & `cvxpy-1.3.2/cvxpy/lin_ops/lin_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/lin_ops/lin_op.py` & `cvxpy-1.3.2/cvxpy/lin_ops/lin_op.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/lin_ops/lin_utils.py` & `cvxpy-1.3.2/cvxpy/lin_ops/lin_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/lin_ops/tree_mat.py` & `cvxpy-1.3.2/cvxpy/lin_ops/tree_mat.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/problems/__init__.py` & `cvxpy-1.3.2/cvxpy/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/problems/iterative.py` & `cvxpy-1.3.2/cvxpy/problems/iterative.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/problems/objective.py` & `cvxpy-1.3.2/cvxpy/problems/objective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/problems/param_prob.py` & `cvxpy-1.3.2/cvxpy/problems/param_prob.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/problems/problem.py` & `cvxpy-1.3.2/cvxpy/problems/problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 from cvxpy.reductions.solution import INF_OR_UNB_MESSAGE
 from cvxpy.reductions.solvers import bisection
 from cvxpy.reductions.solvers import defines as slv_def
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import ConicSolver
 from cvxpy.reductions.solvers.defines import SOLVER_MAP_CONIC, SOLVER_MAP_QP
 from cvxpy.reductions.solvers.qp_solvers.qp_solver import QpSolver
 from cvxpy.reductions.solvers.solver import Solver
-from cvxpy.reductions.solvers.solving_chain import (SolvingChain,
-                                                    construct_solving_chain,)
+from cvxpy.reductions.solvers.solving_chain import (
+    SolvingChain,
+    construct_solving_chain,
+)
 from cvxpy.settings import SOLVERS
 from cvxpy.utilities import debug_tools
 from cvxpy.utilities.deterministic import unique_list
 
 SolveResult = namedtuple(
     'SolveResult',
     ['opt_value', 'status', 'primal_values', 'dual_values'])
```

### Comparing `cvxpy-1.3.1/cvxpy/problems/xpress_problem.py` & `cvxpy-1.3.2/cvxpy/problems/xpress_problem.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/canonicalization.py` & `cvxpy-1.3.2/cvxpy/reductions/canonicalization.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/chain.py` & `cvxpy-1.3.2/cvxpy/reductions/chain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,23 @@
 limitations under the License.
 """
 
 from typing import List, Optional, Union
 
 import numpy as np
 
-from cvxpy.atoms import (bmat, lambda_sum_largest, normNuc, reshape,
-                         symmetric_wrap, von_neumann_entr, vstack,)
+from cvxpy.atoms import (
+    bmat,
+    lambda_sum_largest,
+    normNuc,
+    reshape,
+    symmetric_wrap,
+    von_neumann_entr,
+    vstack,
+)
 from cvxpy.atoms.affine.wraps import psd_wrap
 from cvxpy.constraints.exponential import OpRelEntrConeQuad
 from cvxpy.expressions.constants.constant import Constant
 from cvxpy.expressions.expression import Expression
 
 
 def expand_complex(real_part: Optional[Expression],
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/param_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/param_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/complex2real/complex2real.py` & `cvxpy-1.3.2/cvxpy/reductions/complex2real/complex2real.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,29 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from cvxpy import problems
 from cvxpy import settings as s
 from cvxpy.atoms.affine.upper_tri import vec_to_upper_tri
-from cvxpy.constraints import (PSD, SOC, Equality, Inequality, NonNeg, NonPos,
-                               OpRelEntrConeQuad, Zero,)
+from cvxpy.constraints import (
+    PSD,
+    SOC,
+    Equality,
+    Inequality,
+    NonNeg,
+    NonPos,
+    OpRelEntrConeQuad,
+    Zero,
+)
 from cvxpy.constraints.constraint import Constraint
 from cvxpy.expressions import cvxtypes
 from cvxpy.lin_ops import lin_utils as lu
 from cvxpy.reductions import InverseData, Solution
-from cvxpy.reductions.complex2real.canonicalizers import (
-    CANON_METHODS as elim_cplx_methods,)
+from cvxpy.reductions.complex2real.canonicalizers import CANON_METHODS as elim_cplx_methods
 from cvxpy.reductions.reduction import Reduction
 
 
 def accepts(problem) -> bool:
     leaves = problem.variables() + problem.parameters() + problem.constants()
     return any(leaf.is_complex() for leaf in leaves)
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/cone2cone/affine2direct.py` & `cvxpy-1.3.2/cvxpy/reductions/cone2cone/affine2direct.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/cone2cone/approximations.py` & `cvxpy-1.3.2/cvxpy/reductions/cone2cone/approximations.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,25 @@
 from typing import List, Tuple
 
 import numpy as np
 
 import cvxpy as cp
 from cvxpy.atoms.affine.upper_tri import upper_tri
 from cvxpy.constraints.constraint import Constraint
-from cvxpy.constraints.exponential import (ExpCone, OpRelEntrConeQuad,
-                                           RelEntrConeQuad,)
+from cvxpy.constraints.exponential import (
+    ExpCone,
+    OpRelEntrConeQuad,
+    RelEntrConeQuad,
+)
 from cvxpy.constraints.zero import Zero
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.canonicalization import Canonicalization
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.von_neumann_entr_canon import (
-    von_neumann_entr_canon,)
+    von_neumann_entr_canon,
+)
 
 APPROX_CONES = {
     RelEntrConeQuad: {cp.SOC},
     OpRelEntrConeQuad: {cp.PSD}
 }
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/cone2cone/exotic2common.py` & `cvxpy-1.3.2/cvxpy/reductions/cone2cone/exotic2common.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/cvx_attr2constr.py` & `cvxpy-1.3.2/cvxpy/reductions/cvx_attr2constr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/entr_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/entr_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/exp_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/exp_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/geo_mean_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/geo_mean_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/huber_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/huber_canon.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 limitations under the License.
 """
 
 from cvxpy.atoms.elementwise.abs import abs
 from cvxpy.atoms.elementwise.power import power
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.power_canon import (
-    power_canon,)
+    power_canon,
+)
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers.abs_canon import (
-    abs_canon,)
+    abs_canon,
+)
 
 
 def huber_canon(expr, args):
     M = expr.M
     x = args[0]
     shape = expr.shape
     n = Variable(shape)
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/indicator_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/indicator_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/kl_div_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/kl_div_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_max_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_max_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_sum_largest_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/lambda_sum_largest_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from cvxpy.atoms import trace
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.lambda_max_canon import (
-    lambda_max_canon,)
+    lambda_max_canon,
+)
 
 
 def lambda_sum_largest_canon(expr, args):
     """
     S_k(X) denotes lambda_sum_largest(X, k)
     t >= k S_k(X - Z) + trace(Z), Z is PSD
     implies
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log1p_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log1p_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_det_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_det_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_sum_exp_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/log_sum_exp_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/logistic_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/logistic_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/matrix_frac_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/matrix_frac_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/mul_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/mul_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/normNuc_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/normNuc_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/perspective_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/perspective_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/pnorm_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/pnorm_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from cvxpy.atoms.affine.sum import sum
 from cvxpy.atoms.affine.vec import vec
 from cvxpy.atoms.elementwise.abs import abs
 from cvxpy.constraints.second_order import SOC
 from cvxpy.expressions.constants import Constant
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers.abs_canon import (
-    abs_canon,)
+    abs_canon,
+)
 from cvxpy.utilities.power_tools import gm_constrs
 
 
 def pnorm_canon(expr, args):
     x = args[0]
     p = expr.p
     axis = expr.axis
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/power_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/power_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_form_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_form_canon.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 limitations under the License.
 """
 
 from cvxpy.atoms import sum_squares
 from cvxpy.atoms.quad_form import decomp_quad
 from cvxpy.expressions.constants import Constant
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.quad_over_lin_canon import (
-    quad_over_lin_canon,)
+    quad_over_lin_canon,
+)
 
 
 def quad_form_canon(expr, args):
     # TODO this doesn't work with parameters!
     scale, M1, M2 = decomp_quad(args[1].value)
     # Special case where P == 0.
     if M1.size == M2.size == 0:
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_over_lin_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/quad_over_lin_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/rel_entr_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/rel_entr_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/sigma_max_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/sigma_max_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/suppfunc_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/suppfunc_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
 from cvxpy import SOC, Variable, hstack
 from cvxpy.constraints.exponential import ExpCone
 from cvxpy.reductions.solvers.conic_solvers.scs_conif import (
-    scs_psdvec_to_psdmat,)
+    scs_psdvec_to_psdmat,
+)
 
 
 def suppfunc_canon(expr, args):
     y = args[0].flatten()
     # ^ That's the user-supplied argument to the support function.
     parent = expr._parent
     A, b, K_sels = parent.conic_repr_of_set()
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/tr_inv_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/tr_inv_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/von_neumann_entr_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/von_neumann_entr_canon.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 """
 from cvxpy import Variable, lambda_sum_largest, trace
 from cvxpy.atoms.affine.sum import sum
 from cvxpy.constraints.nonpos import NonPos
 from cvxpy.constraints.zero import Zero
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.entr_canon import entr_canon
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.lambda_sum_largest_canon import (
-    lambda_sum_largest_canon,)
+    lambda_sum_largest_canon,
+)
 
 
 def von_neumann_entr_canon(expr, args):
     N = args[0]
     assert N.is_real()
     n = N.shape[0]
     x = Variable(shape=(n,))
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/atom_canonicalizers/xexp_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/atom_canonicalizers/xexp_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 limitations under the License.
 """
 
 from cvxpy.atoms.elementwise.power import power
 from cvxpy.constraints.exponential import ExpCone
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.dcp2cone.atom_canonicalizers.power_canon import (
-    power_canon,)
+    power_canon,
+)
 
 
 def xexp_canon(expr, args):
     x = args[0]
     u = Variable(expr.shape, nonneg=True)
     t = Variable(expr.shape, nonneg=True)
     power_expr = power(x, 2)
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,39 @@
 """
 from __future__ import annotations
 
 import numpy as np
 import scipy.sparse as sp
 
 import cvxpy.settings as s
-from cvxpy.constraints import (PSD, SOC, Equality, ExpCone, Inequality, NonNeg,
-                               NonPos, PowCone3D, Zero,)
+from cvxpy.constraints import (
+    PSD,
+    SOC,
+    Equality,
+    ExpCone,
+    Inequality,
+    NonNeg,
+    NonPos,
+    PowCone3D,
+    Zero,
+)
 from cvxpy.cvxcore.python import canonInterface
 from cvxpy.expressions.variable import Variable
 from cvxpy.problems.objective import Minimize
 from cvxpy.problems.param_prob import ParamProb
 from cvxpy.reductions import InverseData, Solution, cvx_attr2constr
 from cvxpy.reductions.matrix_stuffing import MatrixStuffing, extract_mip_idx
-from cvxpy.reductions.utilities import (ReducedMat, are_args_affine,
-                                        group_constraints, lower_equality,
-                                        lower_ineq_to_nonneg, nonpos2nonneg,)
+from cvxpy.reductions.utilities import (
+    ReducedMat,
+    are_args_affine,
+    group_constraints,
+    lower_equality,
+    lower_ineq_to_nonneg,
+    nonpos2nonneg,
+)
 from cvxpy.utilities.coeff_extractor import CoeffExtractor
 
 
 class ConeDims:
     """Summary of cone dimensions present in constraints.
 
     Constraints must be formatted as dictionary that maps from
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dcp2cone/dcp2cone.py` & `cvxpy-1.3.2/cvxpy/reductions/dcp2cone/dcp2cone.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 
 from cvxpy import problems
 from cvxpy.expressions import cvxtypes
 from cvxpy.expressions.expression import Expression
 from cvxpy.problems.objective import Minimize
 from cvxpy.reductions.canonicalization import Canonicalization
 from cvxpy.reductions.dcp2cone.atom_canonicalizers import (
-    CANON_METHODS as cone_canon_methods,)
+    CANON_METHODS as cone_canon_methods,
+)
 from cvxpy.reductions.inverse_data import InverseData
 from cvxpy.reductions.qp2quad_form.atom_canonicalizers import (
-    QUAD_CANON_METHODS as quad_canon_methods,)
+    QUAD_CANON_METHODS as quad_canon_methods,
+)
 
 
 class Dcp2Cone(Canonicalization):
     """Reduce DCP problems to a conic form.
 
     This reduction takes as input (minimization) DCP problems and converts
     them into problems with affine or quadratic objectives and conic
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/add_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/add_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/constant_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/constant_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/eye_minus_inv_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/eye_minus_inv_canon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from cvxpy.atoms.affine.binary_operators import matmul
 from cvxpy.atoms.affine.diag import diag
 from cvxpy.atoms.one_minus_pos import one_minus_pos
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.dgp2dcp.atom_canonicalizers.mulexpression_canon import (
-    mulexpression_canon,)
+    mulexpression_canon,
+)
 from cvxpy.reductions.dgp2dcp.atom_canonicalizers.one_minus_pos_canon import (
-    one_minus_pos_canon,)
+    one_minus_pos_canon,
+)
 
 
 def eye_minus_inv_canon(expr, args):
     X = args[0]
 
     # (I - X)^{-1} \leq T iff there exists 0 <= Y <= T s.t.  YX + I <= Y
     #
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/mulexpression_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/mulexpression_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/parameter_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/parameter_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pf_eigenvalue_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pf_eigenvalue_canon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from cvxpy.atoms.affine.binary_operators import matmul
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.dgp2dcp.atom_canonicalizers.mul_canon import mul_canon
 from cvxpy.reductions.dgp2dcp.atom_canonicalizers.mulexpression_canon import (
-    mulexpression_canon,)
+    mulexpression_canon,
+)
 
 
 def pf_eigenvalue_canon(expr, args):
     X = args[0]
     # rho(X) \leq lambda iff there exists v s.t. Xv \leq lambda v
     # v and lambd represent log variables, hence no positivity constraints
     lambd = Variable()
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pnorm_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/pnorm_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/atom_canonicalizers/sum_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/atom_canonicalizers/sum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dgp2dcp/dgp2dcp.py` & `cvxpy-1.3.2/cvxpy/reductions/dgp2dcp/dgp2dcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py` & `cvxpy-1.3.2/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py` & `cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/inverse.py` & `cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/inverse.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/sets.py` & `cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/sets.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/dqcp2dcp/tighten.py` & `cvxpy-1.3.2/cvxpy/reductions/dqcp2dcp/tighten.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/abs_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/abs_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cummax_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cummax_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cumsum_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/cumsum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/dotsort_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/dotsort_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/max_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/max_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/maximum_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/maximum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/min_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/min_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from cvxpy.atoms.max import max
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers.max_canon import (
-    max_canon,)
+    max_canon,
+)
 
 
 def min_canon(expr, args):
     axis = expr.axis
     del expr
     assert len(args) == 1
     tmp = max(-args[0], axis=axis)
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/minimum_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/minimum_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from cvxpy.atoms.elementwise.maximum import maximum
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers.maximum_canon import (
-    maximum_canon,)
+    maximum_canon,
+)
 
 
 def minimum_canon(expr, args):
     del expr
     tmp = maximum(*[-arg for arg in args])
     canon, constr = maximum_canon(tmp, tmp.args)
     return -canon, constr
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm1_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm1_canon.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from cvxpy.atoms.affine.sum import sum
 from cvxpy.atoms.elementwise.abs import abs
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers.abs_canon import (
-    abs_canon,)
+    abs_canon,
+)
 
 
 def norm1_canon(expr, args):
     x = args[0]
     axis = expr.axis
 
     # we need an absolute value constraint for the symmetric convex branches
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm_inf_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/norm_inf_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/sum_largest_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/atom_canonicalizers/sum_largest_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py` & `cvxpy-1.3.2/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from cvxpy.atoms import abs, max, maximum, norm1, norm_inf, sum_largest
 from cvxpy.reductions.canonicalization import Canonicalization
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers import (
-    CANON_METHODS as elim_pwl_methods,)
+    CANON_METHODS as elim_pwl_methods,
+)
 
 
 class EliminatePwl(Canonicalization):
     """Eliminates piecewise linear atoms."""
 
     def __init__(self, problem=None) -> None:
         super(EliminatePwl, self).__init__(
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/eval_params.py` & `cvxpy-1.3.2/cvxpy/reductions/eval_params.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/flip_objective.py` & `cvxpy-1.3.2/cvxpy/reductions/flip_objective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/inverse_data.py` & `cvxpy-1.3.2/cvxpy/reductions/inverse_data.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/matrix_stuffing.py` & `cvxpy-1.3.2/cvxpy/reductions/matrix_stuffing.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/huber_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/huber_canon.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 limitations under the License.
 """
 
 from cvxpy.atoms.elementwise.abs import abs
 from cvxpy.atoms.elementwise.power import power
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.eliminate_pwl.atom_canonicalizers.abs_canon import (
-    abs_canon,)
+    abs_canon,
+)
 from cvxpy.reductions.qp2quad_form.atom_canonicalizers.power_canon import (
-    power_canon,)
+    power_canon,
+)
 
 
 def huber_canon(expr, args):
     M = expr.M
     x = args[0]
     shape = expr.shape
     n = Variable(shape)
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/power_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/power_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_form_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_form_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_over_lin_canon.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/atom_canonicalizers/quad_over_lin_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 limitations under the License.
 """
 
 from cvxpy.constraints import Equality, Inequality, NonNeg, NonPos, Zero
 from cvxpy.reductions.canonicalization import Canonicalization
 from cvxpy.reductions.cvx_attr2constr import convex_attributes
 from cvxpy.reductions.qp2quad_form.atom_canonicalizers import (
-    CANON_METHODS as qp_canon_methods,)
+    CANON_METHODS as qp_canon_methods,
+)
 from cvxpy.reductions.utilities import are_args_affine
 
 
 def accepts(problem):
     """
     Problems with quadratic, piecewise affine objectives,
     piecewise-linear constraints inequality constraints, and
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py` & `cvxpy-1.3.2/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,37 @@
 limitations under the License.
 """
 from __future__ import annotations
 
 import numpy as np
 
 import cvxpy.settings as s
-from cvxpy.constraints import (PSD, SOC, Equality, ExpCone, Inequality, NonPos,
-                               Zero,)
+from cvxpy.constraints import (
+    PSD,
+    SOC,
+    Equality,
+    ExpCone,
+    Inequality,
+    NonPos,
+    Zero,
+)
 from cvxpy.cvxcore.python import canonInterface
 from cvxpy.expressions.variable import Variable
 from cvxpy.problems.objective import Minimize
 from cvxpy.problems.param_prob import ParamProb
 from cvxpy.reductions import InverseData, Solution
 from cvxpy.reductions.cvx_attr2constr import convex_attributes
 from cvxpy.reductions.matrix_stuffing import MatrixStuffing, extract_mip_idx
-from cvxpy.reductions.utilities import (ReducedMat, are_args_affine,
-                                        group_constraints, lower_equality,
-                                        lower_ineq_to_nonpos,)
+from cvxpy.reductions.utilities import (
+    ReducedMat,
+    are_args_affine,
+    group_constraints,
+    lower_equality,
+    lower_ineq_to_nonpos,
+)
 from cvxpy.utilities.coeff_extractor import CoeffExtractor
 
 
 class ConeDims:
     """Summary of cone dimensions present in constraints.
 
     Constraints must be formatted as dictionary that maps from
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/reduction.py` & `cvxpy-1.3.2/cvxpy/reductions/reduction.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solution.py` & `cvxpy-1.3.2/cvxpy/reductions/solution.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/bisection.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/bisection.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/compr_matrix.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/compr_matrix.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 """
 
 import numpy as np
 
 import cvxpy.settings as s
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    ConicSolver, dims_to_solver_dict,)
+    ConicSolver,
+    dims_to_solver_dict,
+)
 
 
 class CBC(ConicSolver):
     """ An interface to the CBC solver
     """
 
     # Solver capabilities.
@@ -55,16 +57,15 @@
         """The name of the solver.
         """
         return s.CBC
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        from cylp.cy import CyClpSimplex
-        CyClpSimplex  # For flake8
+        from cylp.cy import CyClpSimplex  # noqa F401
 
     def accepts(self, problem) -> bool:
         """Can Cbc solve the problem?
         """
         # TODO check if is matrix stuffed.
         if not problem.objective.args[0].is_affine():
             return False
@@ -156,35 +157,51 @@
 
         # Verbosity Clp
         if not verbose:
             model.logLevel = 0
 
         # Build model & solve
         status = None
+        clp_model_options = {"dualTolerance", "primalTolerance",
+                             "maxNumIteration", "logLevel", "automaticScaling",
+                             "scaling", "infeasibilityCost", "optimizationDirection"}
+        clp_solve_options = {"presolve"}
+        # all the above keys except logLevel apply only to models solved with CLP
+        non_cbc_options = (clp_model_options | clp_solve_options) - {"logLevel"}
+        for key in solver_opts:
+            if key in clp_model_options:
+                setattr(model, key, solver_opts[key])
         if data[s.BOOL_IDX] or data[s.INT_IDX]:
             # Convert model
             cbcModel = model.getCbcModel()
-            for key, value in solver_opts.items():
-                setattr(cbcModel, key, value)
 
             # Verbosity Cbc
             if not verbose:
                 cbcModel.logLevel = 0
+            # Other Solver options
+            for key, value in solver_opts.items():
+                if key in non_cbc_options:
+                    continue
+                setattr(cbcModel, key, value)
 
             # cylp: /cylp/cy/CyCbcModel.pyx#L134
             # Call CbcMain. Solve the problem using the same parameters used by
             # CbcSolver. Equivalent to solving the model from the command line
             # using cbc's binary.
             cbcModel.solve()
             status = cbcModel.status
         else:
             # cylp: /cylp/cy/CyClpSimplex.pyx
             # Run CLP's initialSolve. It does a presolve and uses primal or dual
             # Simplex to solve a problem.
-            status = model.initialSolve()
+            solve_args = {}
+            for key in clp_solve_options:
+                if key in solver_opts:
+                    solve_args[key] = solver_opts[key]
+            status = model.initialSolve(**solve_args)
 
         solution = {}
         if data[s.BOOL_IDX] or data[s.INT_IDX]:
             solution["status"] = self.STATUS_MAP_MIP[status]
             solution["primal"] = cbcModel.primalVariableSolution['x']
             solution["value"] = cbcModel.objectiveValue
         else:
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,15 @@
         """The name of the solver.
         """
         return 'CLARABEL'
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        import clarabel
-        clarabel  # For flake8
+        import clarabel  # noqa F401
 
     def supports_quad_obj(self) -> bool:
         """Clarabel supports quadratic objective with any combination of conic constraints.
         """
         return True
 
     @staticmethod
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/conic_solver.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/conic_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/copt_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/copt_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import scipy.sparse as sp
 
 import cvxpy.settings as s
 from cvxpy.constraints import PSD, SOC
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers import utilities
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    ConicSolver, dims_to_solver_dict,)
+    ConicSolver,
+    dims_to_solver_dict,
+)
 
 
 def tri_to_full(lower_tri, n):
     """
     Expands n*(n+1)//2 lower triangular to full matrix
 
     Parameters
@@ -47,38 +49,37 @@
     REQUIRES_CONSTR = True
 
     # Only supports MI LPs
     MI_SUPPORTED_CONSTRAINTS = ConicSolver.SUPPORTED_CONSTRAINTS
 
     # Map between COPT status and CVXPY status
     STATUS_MAP = {
-                  1: s.OPTIMAL,       # optimal
-                  2: s.INFEASIBLE,    # infeasible
-                  3: s.UNBOUNDED,     # unbounded
-                  4: s.INF_OR_UNB,    # infeasible or unbounded
-                  5: s.SOLVER_ERROR,  # numerical
-                  6: s.USER_LIMIT,    # node limit
-                  7: s.SOLVER_ERROR,  # error
-                  8: s.USER_LIMIT,    # time out
-                  9: s.SOLVER_ERROR,  # unfinished
-                  10: s.USER_LIMIT    # interrupted
+                  1: s.OPTIMAL,             # optimal
+                  2: s.INFEASIBLE,          # infeasible
+                  3: s.UNBOUNDED,           # unbounded
+                  4: s.INF_OR_UNB,          # infeasible or unbounded
+                  5: s.SOLVER_ERROR,        # numerical
+                  6: s.USER_LIMIT,          # node limit
+                  7: s.OPTIMAL_INACCURATE,  # imprecise
+                  8: s.USER_LIMIT,          # time out
+                  9: s.SOLVER_ERROR,        # unfinished
+                  10: s.USER_LIMIT          # interrupted
                  }
 
     def name(self):
         """
         The name of solver.
         """
         return 'COPT'
 
     def import_solver(self):
         """
         Imports the solver.
         """
-        import coptpy
-        coptpy  # For flake8
+        import coptpy  # noqa F401
 
     def accepts(self, problem):
         """
         Can COPT solve the problem?
         """
         if not problem.objective.args[0].is_affine():
             return False
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from scipy.sparse import dok_matrix
 
 import cvxpy.settings as s
 from cvxpy.constraints import SOC
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers import utilities
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    ConicSolver, dims_to_solver_dict,)
+    ConicSolver,
+    dims_to_solver_dict,
+)
 
 # Values used to distinguish between linear and quadratic constraints.
 _LIN, _QUAD = 0, 1
 # For internal bookkeeping, we have to separate linear indices from
 # quadratic indices. The "cpx_constrs" member of the solution will
 # contain namedtuples of (constr_type, index) where constr_type is either
 # _LIN or _QUAD.
@@ -212,16 +214,15 @@
 
     def name(self):
         """The name of the solver. """
         return s.CPLEX
 
     def import_solver(self) -> None:
         """Imports the solver."""
-        import cplex
-        cplex  # For flake8
+        import cplex  # noqa F401
 
     def accepts(self, problem) -> bool:
         """Can CPLEX solve the problem?
         """
         # TODO check if is matrix stuffed.
         if not problem.objective.args[0].is_affine():
             return False
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,15 @@
         """The name of the solver.
         """
         return s.CVXOPT
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        import cvxopt
-        cvxopt  # For flake8
+        import cvxopt  # noqa F401
 
     def accepts(self, problem) -> bool:
         """Can CVXOPT solve the problem?
         """
         # TODO check if is matrix stuffed.
         if not problem.objective.args[0].is_affine():
             return False
@@ -279,15 +278,21 @@
                 return s.OPTIMAL
             elif not b.item() == 0.0:
                 return s.INFEASIBLE
             else:
                 data[s.A] = None
                 data[s.B] = None
                 return s.OPTIMAL
-        eig = eigsh(gram, k=1, which='SM', return_eigenvectors=False)
+        if hasattr(np.random, 'default_rng'):
+            g = np.random.default_rng(123)
+        else:  # fallback to legacy RandomState
+            g = np.random.RandomState(123)
+        n = gram.shape[0]
+        rand_v0 = g.normal(loc=0.0, scale=1.0, size=n)
+        eig = eigsh(gram, k=1, which='SM', v0=rand_v0, return_eigenvectors=False)
         if eig > TOL:
             return s.OPTIMAL
         #
         # Redundant constraints exist, up to numerical tolerance;
         # reformulate equality constraints to remove this redundancy.
         #
         Q, R, P = scipy.linalg.qr(A.todense(), pivoting=True)  # pivoting helps robustness
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 import cvxpy.interface as intf
 import cvxpy.settings as s
 from cvxpy.constraints import ExpCone
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers import utilities
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import ConicSolver
 from cvxpy.reductions.solvers.conic_solvers.ecos_conif import (
-    ECOS, dims_to_solver_dict,)
+    ECOS,
+    dims_to_solver_dict,
+)
 
 
 class ECOS_BB(ECOS):
     """An interface for the ECOS BB solver.
     """
 
     # Solver capabilities.
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,15 @@
 
     # Order of exponential cone arguments for solver.
     EXP_CONE_ORDER = [0, 2, 1]
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        import ecos
-        ecos  # For flake8
+        import ecos  # noqa F401
 
     def name(self):
         """The name of the solver.
         """
         return s.ECOS
 
     def apply(self, problem):
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/glop_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/glop_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,24 @@
 
     def name(self) -> str:
         """The name of the solver."""
         return 'GLOP'
 
     def import_solver(self) -> None:
         """Imports the solver."""
-        import google.protobuf
-        import ortools
+        import google.protobuf  # noqa F401
+        import ortools  # noqa F401
         if Version(ortools.__version__) < Version('9.3.0'):
             raise RuntimeError(f'Version of ortools ({ortools.__version__}) '
                                f'is too old. Expected >= 9.3.0.')
         if Version(ortools.__version__) >= Version('9.5.0'):
             raise RuntimeError('Unrecognized new version of ortools '
                                f'({ortools.__version__}). Expected < 9.5.0.'
                                'Please open a feature request on cvxpy to '
                                'enable support for this version.')
-        ortools, google.protobuf  # For flake8
 
     def apply(self, problem: ParamConeProg) -> Tuple[Dict, Dict]:
         """Returns a new problem and data for inverting the new solution."""
         from ortools.linear_solver import linear_solver_pb2
 
         # Create data and inv_data objects
         data = {}
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         """The name of the solver.
         """
         return s.GLPK
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        from cvxopt import glpk
-        glpk  # For flake8
+        from cvxopt import glpk  # noqa F401
 
     def invert(self, solution, inverse_data):
         """Returns the solution to the original problem given the inverse_data.
         """
         return super(GLPK, self).invert(solution, inverse_data)
 
     def solve_via_data(self, data, warm_start: bool, verbose: bool, solver_opts, solver_cache=None):
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 import scipy.sparse as sp
 
 import cvxpy.settings as s
 from cvxpy.constraints import SOC
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers import utilities
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    ConicSolver, dims_to_solver_dict,)
+    ConicSolver,
+    dims_to_solver_dict,
+)
 
 
 class GUROBI(ConicSolver):
     """
     An interface for the Gurobi solver.
     """
 
@@ -55,16 +57,15 @@
         """The name of the solver.
         """
         return s.GUROBI
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        import gurobipy
-        gurobipy  # For flake8
+        import gurobipy  # noqa F401
 
     def accepts(self, problem) -> bool:
         """Can Gurobi solve the problem?
         """
         # TODO check if is matrix stuffed.
         if not problem.objective.args[0].is_affine():
             return False
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,16 @@
         K_e = closure{(x,y,z) | x >= y * exp(z/y), x,y >= 0}.
     with this convention, EXP_CONE_ORDER should be should be [2, 1, 0].
     """
 
     def import_solver(self) -> None:
         """Imports the solver (updates the set of supported constraints, if applicable).
         """
-        import mosek
-        mosek  # For flake8
+        import mosek  # noqa F401
+
         if hasattr(mosek.conetype, 'pexp') and ExpCone not in MOSEK.SUPPORTED_CONSTRAINTS:
             MOSEK.SUPPORTED_CONSTRAINTS.append(ExpCone)
             MOSEK.SUPPORTED_CONSTRAINTS.append(PowCone3D)
             MOSEK.MI_SUPPORTED_CONSTRAINTS.append(ExpCone)
             MOSEK.MI_SUPPORTED_CONSTRAINTS.append(PowCone3D)
 
     def name(self):
@@ -241,15 +241,15 @@
             A, c, K = data[s.A], data[s.C], data['K_dir']
             num_psd = len(K[a2d.PSD])
             if num_psd > 0:
                 idx = K[a2d.FREE] + K[a2d.NONNEG] + sum(K[a2d.SOC])
                 total_psd = sum([d * (d+1) // 2 for d in K[a2d.PSD]])
                 A_psd = A[:, idx:idx+total_psd]
                 c_psd = c[idx:idx+total_psd]
-                if K[a2d.DUAL_EXP] == 0:
+                if (K[a2d.DUAL_EXP] == 0) and (K[a2d.DUAL_POW3D] == 0):
                     data[s.A] = A[:, :idx]
                     data[s.C] = c[:idx]
                 else:
                     data[s.A] = sp.sparse.hstack([A[:, :idx], A[:, idx+total_psd:]])
                     data[s.C] = np.concatenate([c[:idx], c[idx+total_psd:]])
                 A_bar_data, c_bar_data = MOSEK.bar_data(A_psd, c_psd, K)
                 data['A_bar_data'] = A_bar_data
@@ -476,18 +476,24 @@
             STATUS_MAP[mosek.solsta.near_prim_infeas_cer] = s.INFEASIBLE_INACCURATE
             STATUS_MAP[mosek.solsta.near_dual_infeas_cer] = s.UNBOUNDED_INACCURATE
         STATUS_MAP = defaultdict(lambda: s.SOLVER_ERROR, STATUS_MAP)
 
         env = solver_output['env']
         task = solver_output['task']
         solver_opts = solver_output['solver_options']
+        simplex_algs = [
+            mosek.optimizertype.primal_simplex,
+            mosek.optimizertype.dual_simplex,
+        ]
+        current_optimizer = task.getintparam(mosek.iparam.optimizer)
+        bfs_active = "bfs" in solver_opts and solver_opts["bfs"] and task.getnumcone() == 0
 
         if task.getnumintvar() > 0:
             sol_type = mosek.soltype.itg
-        elif 'bfs' in solver_opts and solver_opts['bfs'] and task.getnumcone() == 0:
+        elif current_optimizer in simplex_algs or bfs_active:
             sol_type = mosek.soltype.bas  # the basic feasible solution
         else:
             sol_type = mosek.soltype.itr  # the solution found via interior point method
 
         prim_vars = None
         dual_vars = None
         problem_status = task.getprosta(sol_type)
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/nag_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/nag_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
                   50: s.OPTIMAL_INACCURATE,
                   51: s.INFEASIBLE,
                   52: s.UNBOUNDED}
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        from naginterfaces.library import opt
-        opt  # For flake8
+        from naginterfaces.library import opt  # noqa F401
 
     def name(self):
         """The name of the solver.
         """
         return s.NAG
 
     def accepts(self, problem) -> bool:
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,24 @@
 
     def name(self) -> str:
         """The name of the solver."""
         return 'PDLP'
 
     def import_solver(self) -> None:
         """Imports the solver."""
-        import google.protobuf
-        import ortools
+        import google.protobuf  # noqa F401
+        import ortools  # noqa F401
         if Version(ortools.__version__) < Version('9.3.0'):
             raise RuntimeError(f'Version of ortools ({ortools.__version__}) '
                                f'is too old. Expected >= 9.3.0.')
         if Version(ortools.__version__) >= Version('9.5.0'):
             raise RuntimeError('Unrecognized new version of ortools '
                                f'({ortools.__version__}). Expected < 9.5.0.'
                                'Please open a feature request on cvxpy to '
                                'enable support for this version.')
-        ortools, google.protobuf  # For flake8
 
     def apply(self, problem: ParamConeProg) -> Tuple[Dict, Dict]:
         """Returns a new problem and data for inverting the new solution."""
         from ortools.linear_solver import linear_solver_pb2
 
         # Create data and inv_data objects
         data = {}
@@ -164,15 +163,16 @@
             parameters.MergeFrom(proto)
         if "time_limit_sec" in solver_opts:
             request.solver_time_limit_seconds = float(solver_opts["time_limit_sec"])
 
         request.solver_specific_parameters = text_format.MessageToString(parameters)
         if Version(ortools.__version__) >= Version('9.4.0'):
             from ortools.model_builder.python import (
-                pywrap_model_builder_helper,)
+                pywrap_model_builder_helper,
+            )
             solver = pywrap_model_builder_helper.ModelSolverHelper("pdlp")
             response_str = solver.solve_serialized_request(request.SerializeToString())
             response = linear_solver_pb2.MPSolutionResponse.FromString(response_str)
         else:
             # Version 9.3
             from ortools.model_builder.python import model_builder_helper
             solver = model_builder_helper.ModelSolverHelper()
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/scip_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/scip_conif.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
 from typing import Any, Dict, Generic, Iterator, List, Optional, Tuple, Union
 
-from numpy import array, ndarray
+import numpy as np
 from scipy.sparse import dok_matrix
 
 import cvxpy.settings as s
 from cvxpy import Zero
 from cvxpy.constraints import SOC, ExpCone, NonNeg
 from cvxpy.reductions.dcp2cone.cone_matrix_stuffing import ParamConeProg
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers import utilities
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    ConicSolver, dims_to_solver_dict,)
+    ConicSolver,
+    dims_to_solver_dict,
+)
 
 log = logging.getLogger(__name__)
 
 try:
     # Try to import SCIP model for typing
     from pyscipopt.scip import Model as ScipModel
 except ModuleNotFoundError:
@@ -184,15 +186,15 @@
         b = data[s.B]
         A = dok_matrix(data[s.A])
         # Save the dok_matrix.
         data[s.A] = A
         dims = dims_to_solver_dict(data[s.DIMS])
         return A, b, c, dims
 
-    def _create_variables(self, model: ScipModel, data: Dict[str, Any], c: ndarray) -> List:
+    def _create_variables(self, model: ScipModel, data: Dict[str, Any], c: np.ndarray) -> List:
         """Create a list of variables."""
         variables = []
         for n, obj in enumerate(c):
             var_type = get_variable_type(n=n, data=data)
             variables.append(
                 model.addVar(
                     obj=obj,
@@ -205,15 +207,15 @@
         return variables
 
     def _add_constraints(
             self,
             model: ScipModel,
             variables: List,
             A: dok_matrix,
-            b: ndarray,
+            b: np.ndarray,
             dims: Dict[str, Union[int, List]],
     ) -> List:
         """Create a list of constraints."""
 
         # Equal constraints
         equal_constraints = self.add_model_lin_constr(
             model=model,
@@ -318,17 +320,25 @@
             model.optimize()
         except Exception as e:
             log.warning("Error encountered when optimising %s: %s", model, e)
 
         solution = {}
 
         if max(model.getNSols(), model.getNCountedSols()) > 0:
-            solution["value"] = model.getObjVal()
             sol = model.getBestSol()
-            solution["primal"] = array([sol[v] for v in variables])
+            solution["primal"] = np.array([sol[v] for v in variables])
+
+            # HACK can't get objective value directly if stopped due to time limit.
+            if model.getStatus() == 'timelimit':
+                # the solution value is not actually necessary
+                # since CVXPY calculates it by evaluating the objective
+                # at the solution.
+                solution["value"] = np.nan
+            else:
+                solution["value"] = model.getObjVal()
 
             is_mip = data[s.BOOL_IDX] or data[s.INT_IDX]
             has_soc_constr = len(dims[s.SOC_DIM]) > 1
             if not (is_mip or has_soc_constr):
                 # Not the following code calculating the dual values does not
                 # always return the correct values, see tests `test_scip_lp_2`
                 # and `test_scip_socp_1`.
@@ -336,33 +346,43 @@
 
                 # Get linear duals.
                 for lc in constraints:
                     if lc is not None and lc.isLinear():
                         dual = model.getDualsolLinear(lc)
                         vals.append(dual)
 
-                solution["y"] = -array(vals)
+                solution["y"] = -np.array(vals)
                 solution[s.EQ_DUAL] = solution["y"][0:dims[s.EQ_DIM]]
                 solution[s.INEQ_DUAL] = solution["y"][dims[s.EQ_DIM]:]
 
         solution[s.SOLVE_TIME] = model.getSolvingTime()
         solution["status"] = STATUS_MAP[model.getStatus()]
         if solution["status"] == s.SOLVER_ERROR and model.getNCountedSols() > 0:
             solution["status"] = s.OPTIMAL_INACCURATE
 
+        if model.getStatus() == 'timelimit' \
+                and model.getNCountedSols() == 0 \
+                and model.getNSols() == 0:
+            solution["status"] = s.SOLVER_ERROR
+
+        if model.getStatus() == 'timelimit' \
+                and (model.getNSols() > 0 \
+                or model.getNCountedSols() > 0):
+            solution["status"] = s.OPTIMAL_INACCURATE
+
         return solution
 
     def add_model_lin_constr(
         self,
         model: ScipModel,
         variables: List,
         rows: Iterator,
         ctype: str,
         A: dok_matrix,
-        b: ndarray,
+        b: np.ndarray,
     ) -> List:
         """Adds EQ/LEQ constraints to the model using the data from mat and vec.
 
         Return list contains constraints.
         """
         from pyscipopt.scip import quicksum
 
@@ -392,15 +412,15 @@
 
     def add_model_soc_constr(
         self,
         model: ScipModel,
         variables: List,
         rows: Iterator,
         A: dok_matrix,
-        b: ndarray,
+        b: np.ndarray,
     ) -> Tuple:
         """Adds SOC constraint to the model using the data from mat and vec.
 
         Return tuple contains (QConstr, list of Constr, and list of variables).
         """
         from pyscipopt.scip import quicksum
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,25 +38,24 @@
         MIP_CAPABLE = False
     else:
         MIP_CAPABLE = True
         MI_SUPPORTED_CONSTRAINTS = SUPPORTED_CONSTRAINTS
 
     # Map of SciPy linprog status
     STATUS_MAP = {0: s.OPTIMAL,  # Optimal
-                  1: s.SOLVER_ERROR,  # Iteration limit reached
+                  1: s.OPTIMAL_INACCURATE,  # Iteration/time limit reached
                   2: s.INFEASIBLE,  # Infeasible
                   3: s.UNBOUNDED,  # Unbounded
                   4: s.SOLVER_ERROR  # Numerical difficulties encountered
                   }
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        from scipy import optimize as opt
-        opt  # For flake8
+        from scipy import optimize as opt  # noqa F401
 
     def name(self):
         """The name of the solver.
         """
         return s.SCIPY
 
     def apply(self, problem):
@@ -214,15 +213,20 @@
                       "which requires a SciPy version >= 1.6.1."
                       "\n\nThe default method '{}' will be"
                       " used in this case.\n".format(meth))
 
     def invert(self, solution, inverse_data):
         """Returns the solution to the original problem given the inverse_data.
         """
-        status = self.STATUS_MAP[solution['status']]
+        status = self.STATUS_MAP[solution["status"]]
+
+        # Sometimes when the solver's time limit is reached, the solver doesn't return a solution.
+        # In these situations we correct the status from s.OPTIMAL_INACCURATE to s.SOLVER_ERROR
+        if (status == s.OPTIMAL_INACCURATE) and (solution.x is None):
+            status = s.SOLVER_ERROR
 
         primal_vars = None
         dual_vars = None
         if status in s.SOLUTION_PRESENT:
             primal_val = solution['fun']
             opt_val = primal_val + inverse_data[s.OFFSET]
             primal_vars = {inverse_data[self.VAR_ID]: solution['x']}
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/scs_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/scs_conif.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 import scipy.sparse as sp
 
 import cvxpy.settings as s
 from cvxpy.constraints import PSD, SOC, ExpCone, PowCone3D
 from cvxpy.expressions.expression import Expression
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers import utilities
-from cvxpy.reductions.solvers.conic_solvers.conic_solver import ConicSolver
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    dims_to_solver_dict as dims_to_solver_dict_default,)
+    ConicSolver,
+)
+from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
+    dims_to_solver_dict as dims_to_solver_dict_default,
+)
 from cvxpy.utilities.versioning import Version
 
 
 def dims_to_solver_dict(cone_dims):
     cones = dims_to_solver_dict_default(cone_dims)
 
     import scs
@@ -151,16 +154,15 @@
         """The name of the solver.
         """
         return s.SCS
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        import scs
-        scs  # For flake8
+        import scs  # noqa F401
 
     def supports_quad_obj(self) -> bool:
         """SCS >= 3.0.0 supports a quadratic objective.
         """
         import scs
         return Version(scs.__version__) >= Version('3.0.0')
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,15 @@
         """The name of the solver.
         """
         return s.SDPA
 
     def import_solver(self) -> None:
         """Imports the solver.
         """
-        import sdpap
-        sdpap  # For flake8
+        import sdpap  # noqa F401
 
     def accepts(self, problem) -> bool:
         """Can SDPA solve the problem?
         """
         if not problem.objective.args[0].is_affine():
             return False
         for constr in problem.constraints:
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 import numpy as np
 
 import cvxpy.settings as s
 from cvxpy.constraints import SOC
 from cvxpy.reductions.solution import Solution
 from cvxpy.reductions.solvers import utilities
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import (
-    ConicSolver, dims_to_solver_dict,)
+    ConicSolver,
+    dims_to_solver_dict,
+)
 
 
 def makeMstart(A, n, ifCol: int = 1):
     mstart = np.bincount(A.nonzero()[ifCol])
     mstart = np.concatenate((np.array([0], dtype=np.int64),
                              mstart,
                              np.array([0] * (n - len(mstart)), dtype=np.int64)))
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/constant_solver.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/constant_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/defines.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/defines.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,47 +15,39 @@
 """
 
 import numpy as np
 import scipy  # For version checks
 
 import cvxpy.settings as s
 from cvxpy.reductions.solvers.conic_solvers.cbc_conif import CBC as CBC_con
-from cvxpy.reductions.solvers.conic_solvers.clarabel_conif import (
-    CLARABEL as CLARABEL_con,)
+from cvxpy.reductions.solvers.conic_solvers.clarabel_conif import CLARABEL as CLARABEL_con
 from cvxpy.reductions.solvers.conic_solvers.copt_conif import COPT as COPT_con
-from cvxpy.reductions.solvers.conic_solvers.cplex_conif import (
-    CPLEX as CPLEX_con,)
-from cvxpy.reductions.solvers.conic_solvers.cvxopt_conif import (
-    CVXOPT as CVXOPT_con,)
+from cvxpy.reductions.solvers.conic_solvers.cplex_conif import CPLEX as CPLEX_con
+from cvxpy.reductions.solvers.conic_solvers.cvxopt_conif import CVXOPT as CVXOPT_con
+
 # Conic interfaces
-from cvxpy.reductions.solvers.conic_solvers.diffcp_conif import (
-    DIFFCP as DIFFCP_con,)
-from cvxpy.reductions.solvers.conic_solvers.ecos_bb_conif import (
-    ECOS_BB as ECOS_BB_con,)
+from cvxpy.reductions.solvers.conic_solvers.diffcp_conif import DIFFCP as DIFFCP_con
+from cvxpy.reductions.solvers.conic_solvers.ecos_bb_conif import ECOS_BB as ECOS_BB_con
 from cvxpy.reductions.solvers.conic_solvers.ecos_conif import ECOS as ECOS_con
 from cvxpy.reductions.solvers.conic_solvers.glop_conif import GLOP as GLOP_con
 from cvxpy.reductions.solvers.conic_solvers.glpk_conif import GLPK as GLPK_con
-from cvxpy.reductions.solvers.conic_solvers.glpk_mi_conif import (
-    GLPK_MI as GLPK_MI_con,)
-from cvxpy.reductions.solvers.conic_solvers.gurobi_conif import (
-    GUROBI as GUROBI_con,)
-from cvxpy.reductions.solvers.conic_solvers.mosek_conif import (
-    MOSEK as MOSEK_con,)
+from cvxpy.reductions.solvers.conic_solvers.glpk_mi_conif import GLPK_MI as GLPK_MI_con
+from cvxpy.reductions.solvers.conic_solvers.gurobi_conif import GUROBI as GUROBI_con
+from cvxpy.reductions.solvers.conic_solvers.mosek_conif import MOSEK as MOSEK_con
 from cvxpy.reductions.solvers.conic_solvers.nag_conif import NAG as NAG_con
 from cvxpy.reductions.solvers.conic_solvers.pdlp_conif import PDLP as PDLP_con
 from cvxpy.reductions.solvers.conic_solvers.scip_conif import SCIP as SCIP_con
-from cvxpy.reductions.solvers.conic_solvers.scipy_conif import (
-    SCIPY as SCIPY_con,)
+from cvxpy.reductions.solvers.conic_solvers.scipy_conif import SCIPY as SCIPY_con
 from cvxpy.reductions.solvers.conic_solvers.scs_conif import SCS as SCS_con
 from cvxpy.reductions.solvers.conic_solvers.sdpa_conif import SDPA as SDPA_con
-from cvxpy.reductions.solvers.conic_solvers.xpress_conif import (
-    XPRESS as XPRESS_con,)
+from cvxpy.reductions.solvers.conic_solvers.xpress_conif import XPRESS as XPRESS_con
 from cvxpy.reductions.solvers.qp_solvers.copt_qpif import COPT as COPT_qp
 from cvxpy.reductions.solvers.qp_solvers.cplex_qpif import CPLEX as CPLEX_qp
 from cvxpy.reductions.solvers.qp_solvers.gurobi_qpif import GUROBI as GUROBI_qp
+
 # QP interfaces
 from cvxpy.reductions.solvers.qp_solvers.osqp_qpif import OSQP as OSQP_qp
 from cvxpy.reductions.solvers.qp_solvers.proxqp_qpif import PROXQP as PROXQP_qp
 from cvxpy.reductions.solvers.qp_solvers.xpress_qpif import XPRESS as XPRESS_qp
 from cvxpy.utilities.versioning import Version
 
 solver_conic_intf = [DIFFCP_con(), ECOS_con(),
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/intermediate_chain.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/intermediate_chain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/kktsolver.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/kktsolver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/lp_solvers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/lp_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/__init__.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,38 +14,37 @@
     QP interface for the COPT solver
     """
     # Solve capabilities
     MIP_CAPABLE = True
 
     # Map between COPT status and CVXPY status
     STATUS_MAP = {
-                  1: s.OPTIMAL,       # optimal
-                  2: s.INFEASIBLE,    # infeasible
-                  3: s.UNBOUNDED,     # unbounded
-                  4: s.INF_OR_UNB,    # infeasible or unbounded
-                  5: s.SOLVER_ERROR,  # numerical
-                  6: s.USER_LIMIT,    # node limit
-                  7: s.SOLVER_ERROR,  # error
-                  8: s.USER_LIMIT,    # time out
-                  9: s.SOLVER_ERROR,  # unfinished
-                  10: s.USER_LIMIT    # interrupted
+                  1: s.OPTIMAL,             # optimal
+                  2: s.INFEASIBLE,          # infeasible
+                  3: s.UNBOUNDED,           # unbounded
+                  4: s.INF_OR_UNB,          # infeasible or unbounded
+                  5: s.SOLVER_ERROR,        # numerical
+                  6: s.USER_LIMIT,          # node limit
+                  7: s.OPTIMAL_INACCURATE,  # imprecise
+                  8: s.USER_LIMIT,          # time out
+                  9: s.SOLVER_ERROR,        # unfinished
+                  10: s.USER_LIMIT          # interrupted
                  }
 
     def name(self):
         """
         The name of solver.
         """
         return 'COPT'
 
     def import_solver(self):
         """
         Imports the solver.
         """
-        import coptpy
-        coptpy  # For flake8
+        import coptpy  # noqa F401
 
     def invert(self, solution, inverse_data):
         """
         Returns the solution to the original problem given the inverse_data.
         """
         status = solution[s.STATUS]
         attr = {s.SOLVE_TIME: solution[s.SOLVE_TIME],
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 
 import cvxpy.interface as intf
 import cvxpy.settings as s
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers.conic_solvers.cplex_conif import (
-    get_status, hide_solver_output, set_parameters,)
+    get_status,
+    hide_solver_output,
+    set_parameters,
+)
 from cvxpy.reductions.solvers.qp_solvers.qp_solver import QpSolver
 
 
 def constrain_cplex_infty(v) -> None:
     '''
     Limit values of vector v between +/- infinity as
     defined in the CPLEX package
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/qp_solver.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/qp_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 import numpy as np
 import scipy.sparse as sp
 
 import cvxpy.settings as s
 from cvxpy.constraints import NonPos, Zero
 from cvxpy.reductions.cvx_attr2constr import convex_attributes
-from cvxpy.reductions.qp2quad_form.qp_matrix_stuffing import (ConeDims,
-                                                              ParamQuadProg,)
+from cvxpy.reductions.qp2quad_form.qp_matrix_stuffing import (
+    ConeDims,
+    ParamQuadProg,
+)
 from cvxpy.reductions.solvers.solver import Solver
 from cvxpy.reductions.utilities import group_constraints
 
 
 class QpSolver(Solver):
     """
     A QP solver interface.
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 
 import cvxpy.interface as intf
 import cvxpy.settings as s
 from cvxpy.reductions.solution import Solution, failure_solution
 from cvxpy.reductions.solvers.conic_solvers.xpress_conif import (
-    get_status_maps, makeMstart,)
+    get_status_maps,
+    makeMstart,
+)
 from cvxpy.reductions.solvers.qp_solvers.qp_solver import QpSolver
 
 
 class XPRESS(QpSolver):
 
     """Quadratic interface for the FICO Xpress solver"""
 
@@ -18,16 +20,15 @@
         self.prob_ = None
 
     def name(self):
         return s.XPRESS
 
     def import_solver(self) -> None:
 
-        import xpress
-        xpress  # Prevents flake8 warning
+        import xpress  # noqa F401
 
     def apply(self, problem):
         """Returns a new problem and data for inverting the new solution.
 
         Returns
         -------
         tuple
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/solver.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/solving_chain.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/solving_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,43 @@
 
 import warnings
 from typing import List, Optional
 
 import numpy as np
 
 from cvxpy.atoms import EXP_ATOMS, NONPOS_ATOMS, PSD_ATOMS, SOC_ATOMS
-from cvxpy.constraints import (PSD, SOC, Equality, ExpCone, FiniteSet,
-                               Inequality, NonNeg, NonPos, PowCone3D, Zero,)
+from cvxpy.constraints import (
+    PSD,
+    SOC,
+    Equality,
+    ExpCone,
+    FiniteSet,
+    Inequality,
+    NonNeg,
+    NonPos,
+    PowCone3D,
+    Zero,
+)
 from cvxpy.constraints.exponential import OpRelEntrConeQuad, RelEntrConeQuad
 from cvxpy.error import DCPError, DGPError, DPPError, SolverError
 from cvxpy.problems.objective import Maximize
 from cvxpy.reductions.chain import Chain
 from cvxpy.reductions.complex2real import complex2real
 from cvxpy.reductions.cone2cone.approximations import APPROX_CONES, QuadApprox
-from cvxpy.reductions.cone2cone.exotic2common import (EXOTIC_CONES,
-                                                      Exotic2Common,)
+from cvxpy.reductions.cone2cone.exotic2common import (
+    EXOTIC_CONES,
+    Exotic2Common,
+)
 from cvxpy.reductions.cvx_attr2constr import CvxAttr2Constr
 from cvxpy.reductions.dcp2cone.cone_matrix_stuffing import ConeMatrixStuffing
 from cvxpy.reductions.dcp2cone.dcp2cone import Dcp2Cone
 from cvxpy.reductions.dgp2dcp.dgp2dcp import Dgp2Dcp
 from cvxpy.reductions.discrete2mixedint.valinvec2mixedint import (
-    Valinvec2mixedint,)
+    Valinvec2mixedint,
+)
 from cvxpy.reductions.eval_params import EvalParams
 from cvxpy.reductions.flip_objective import FlipObjective
 from cvxpy.reductions.qp2quad_form import qp2symbolic_qp
 from cvxpy.reductions.qp2quad_form.qp_matrix_stuffing import QpMatrixStuffing
 from cvxpy.reductions.reduction import Reduction
 from cvxpy.reductions.solvers import defines as slv_def
 from cvxpy.reductions.solvers.constant_solver import ConstantSolver
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/solvers/utilities.py` & `cvxpy-1.3.2/cvxpy/reductions/solvers/utilities.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Any, Dict
-
 """
 Copyright 2013 Steven Diamond
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -12,14 +10,16 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from typing import Any, Dict
+
 import numpy as np
 
 import cvxpy.interface as intf
 
 
 def stack_vals(variables: list, default: float, order: str = "F") -> np.ndarray:
     """Stacks the values of the given variables.
```

### Comparing `cvxpy-1.3.1/cvxpy/reductions/utilities.py` & `cvxpy-1.3.2/cvxpy/reductions/utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/settings.py` & `cvxpy-1.3.2/cvxpy/settings.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/__init__.py` & `cvxpy-1.3.2/cvxpy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/base_test.py` & `cvxpy-1.3.2/cvxpy/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/ram_limited.py` & `cvxpy-1.3.2/cvxpy/tests/ram_limited.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/solver_test_helpers.py` & `cvxpy-1.3.2/cvxpy/tests/solver_test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -482,14 +482,58 @@
                 np.array([1.30190, 1.38082, 2.67496])]
          )
     ]
     sth = SolverTestHelper(obj_pair, var_pairs, con_pairs)
     return sth
 
 
+def sdp_pcp_1() -> SolverTestHelper:
+    """
+    Example sdp and power cone.
+    """
+    Sigma = np.array([[ 0.4787481 , -0.96924914],
+                      [-0.96924914,  2.77788598]])
+
+    x = cp.Variable(shape=(2,1))
+    y = cp.Variable(shape=(2,1))
+    X = cp.Variable(shape=(2,2), symmetric=True)
+    M1 = cp.vstack([X, x.T])
+    M2 = cp.vstack([x, np.ones((1, 1))])
+    M3 = cp.hstack([M1, M2])
+
+    var_pairs = [
+        (x, np.array([[0.72128204],
+                      [0.27871796]])),
+        (y, np.array([[0.01],
+                      [0.01]])),
+        (X, np.array([[0.52024779, 0.20103426],
+                      [0.20103426, 0.0776837 ]])),        
+    ]
+    con_pairs = [
+        (cp.sum(x) == 1, -0.1503204799112807),
+        (x >= 0, np.array([[-0.],
+                           [-0.]])),
+        (y >= 0.01, np.array([[0.70705506],
+                               [0.70715844]])),
+        (M3 >> 0, np.array([[ 0.4787481 , -0.96924914, -0.07516024],
+                            [-0.96924914,  2.77788598, -0.07516024],
+                            [-0.07516024, -0.07516024,  0.07516094]])),
+        (cp.PowCone3D(x, np.ones((2,1)), y, 0.9), [np.array([[1.17878172e-09],
+                                                             [3.05162243e-09]]),
+                                                   np.array([[9.20157640e-10],
+                                                             [9.40823207e-10]]),
+                                                   np.array([[2.41053358e-10],
+                                                             [7.43432462e-10]])]),
+        ]
+    obj_expr = cp.Minimize(cp.trace(Sigma @ X) + cp.norm(y, p=2))
+    obj_pair = (obj_expr, 0.089301671322676)
+    sth = SolverTestHelper(obj_pair, var_pairs, con_pairs)
+    return sth
+
+
 def pcp_1() -> SolverTestHelper:
     """
     Use a 3D power cone formulation for
 
     min 3 * x[0] + 2 * x[1] + x[2]
     s.t. norm(x,2) <= y
          x[0] + x[1] + 3*x[2] >= 1.0
@@ -748,14 +792,82 @@
     obj = cp.Minimize(0)
     obj_pair = (obj, np.inf)
     con_pairs = [(c, None) for c in constraints]
     var_pairs = [(z, None)]
     sth = SolverTestHelper(obj_pair, var_pairs, con_pairs)
     return sth
 
+def mi_lp_6() -> SolverTestHelper:
+    "Test MILP for timelimit and no feasible solution"
+    n = 70
+    m = 70
+    x = cp.Variable((n,), boolean=True, name="x")
+    y = cp.Variable((n,), name="y")
+    z = cp.Variable((m,), pos=True, name="z")
+    A = np.random.rand(m, n)
+    b = np.random.rand(m)
+    objective = cp.Maximize(cp.sum(y))
+    constraints = [
+        A @ y <= b,
+        y <= 1,
+        cp.sum(x) >= 10,
+        cp.sum(x) <= 20,
+        z[0] + z[1] + z[2] >= 10,
+        z[3] + z[4] + z[5] >= 5,
+        z[6] + z[7] + z[8] >= 7,
+        z[9] + z[10] >= 8,
+        z[11] + z[12] >= 6,
+        z[13] + z[14] >= 3,
+        z[15] + z[16] >= 2,
+        z[17] + z[18] >= 1,
+        z[19] >= 2,
+        z[20] >= 1,
+        z[21] >= 1,
+        z[22] >= 1,
+        z[23] >= 1,
+        z[24] >= 1,
+        z[25] >= 1,
+        z[26] >= 1,
+        z[27] >= 1,
+        z[28] >= 1,
+        z[29] >= 1,
+    ]
+    return SolverTestHelper(
+        (objective, None),
+        [(x, None), (y, None), (z, None)],
+        [(con, None) for con in constraints]
+    )
+
+
+
+def mi_lp_7() -> SolverTestHelper:
+    """Problem that takes significant time to solve - for testing time/iteration limits"""
+    np.random.seed(0)
+    n = 24 * 8
+    c = cp.Variable((n,), pos=True)
+    d = cp.Variable((n,), pos=True)
+    c_or_d = cp.Variable((n,), boolean=True)
+    big = 1e3
+    s = cp.cumsum(c * 0.9 - d)
+    p = np.random.random(n)
+    objective = cp.Maximize(p @ (d - c))
+    constraints = [
+        d <= 1,
+        c <= 1,
+        s >= 0,
+        s <= 1,
+        c <= c_or_d * big,
+        d <= (1 - c_or_d) * big,
+    ]
+    return SolverTestHelper(
+        (objective, None),
+        [(c, None,), (d, None), (c_or_d, None)],
+        [(con, None) for con in constraints]
+    )
+
 
 def mi_socp_1() -> SolverTestHelper:
     """
     Formulate the following mixed-integer SOCP with cvxpy
         min 3 * x[0] + 2 * x[1] + x[2] +  y[0] + 2 * y[1]
         s.t. norm(x,2) <= y[0]
              norm(x,2) <= y[1]
@@ -1097,49 +1209,65 @@
         sth.verify_objective(places)
         sth.verify_primal_values(places)
         if duals:
             sth.check_complementarity(places)
             sth.verify_dual_values(places)
         return sth
 
+    @staticmethod
+    def test_sdp_pcp_1(solver, places: int = 3, duals: bool = False, **kwargs) -> SolverTestHelper:
+        sth = sdp_pcp_1()
+        sth.solve(solver, **kwargs)
+        sth.verify_objective(places)
+        sth.check_primal_feasibility(places)
+        sth.verify_primal_values(places)
+        if duals:
+            sth.check_complementarity(places)
+            sth.check_dual_domains(places)
+        return sth
 
+    
 class StandardTestPCPs:
 
     @staticmethod
     def test_pcp_1(solver, places: int = 3, duals: bool = True, **kwargs) -> SolverTestHelper:
         sth = pcp_1()
         sth.solve(solver, **kwargs)
         sth.verify_objective(places)
+        sth.check_primal_feasibility(places)
         sth.verify_primal_values(places)
         if duals:
             sth.check_complementarity(places)
             sth.verify_dual_values(places)
         return sth
 
     @staticmethod
     def test_pcp_2(solver, places: int = 3, duals: bool = True, **kwargs) -> SolverTestHelper:
         sth = pcp_2()
         sth.solve(solver, **kwargs)
         sth.verify_objective(places)
+        sth.check_primal_feasibility(places)
         sth.verify_primal_values(places)
         if duals:
             sth.check_complementarity(places)
             sth.verify_dual_values(places)
         return sth
 
     @staticmethod
     def test_pcp_3(solver, places: int = 3, duals: bool = True, **kwargs) -> SolverTestHelper:
         sth = pcp_3()
         sth.solve(solver, **kwargs)
         sth.verify_objective(places)
+        sth.check_primal_feasibility(places)
         sth.verify_primal_values(places)
         if duals:
             sth.check_complementarity(places)
             sth.verify_dual_values(places)
 
     @staticmethod
     def test_mi_pcp_0(solver, places: int = 3, **kwargs) -> SolverTestHelper:
         sth = mi_pcp_0()
         sth.solve(solver, **kwargs)
         sth.verify_objective(places)
+        sth.check_primal_feasibility(places)
         sth.verify_primal_values(places)
         return sth
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_atoms.py` & `cvxpy-1.3.2/cvxpy/tests/test_atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,14 +870,32 @@
         expr = cp.kron(a, b)
         assert expr.is_nonpos()
         with self.assertRaises(Exception) as cm:
             cp.kron(self.x, self.x)
         self.assertEqual(str(cm.exception),
                          "At least one argument to kron must be constant.")
 
+    def test_convolve(self) -> None:
+        """Test the convolve atom.
+        """
+        a = np.ones((3,))
+        b = Parameter(2, nonneg=True)
+        expr = cp.convolve(a, b)
+        assert expr.is_nonneg()
+        self.assertEqual(expr.shape, (4,))
+        b = Parameter(2, nonpos=True)
+        expr = cp.convolve(a, b)
+        assert expr.is_nonpos()
+        with self.assertRaises(Exception) as cm:
+            cp.convolve(self.x, -1)
+        self.assertEqual(str(cm.exception),
+                         "The first argument to conv must be constant.")
+        with pytest.raises(ValueError, match="scalar or 1D"):
+            cp.convolve([[0, 1], [0, 1]], self.x)
+
     def test_partial_optimize_dcp(self) -> None:
         """Test DCP properties of partial optimize.
         """
         # Evaluate the 1-norm in the usual way (i.e., in epigraph form).
         dims = 3
         x, t = Variable(dims), Variable(dims)
         p2 = Problem(cp.Minimize(cp.sum(t)), [-t <= x, x <= t])
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_benchmarks.py` & `cvxpy-1.3.2/cvxpy/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_complex.py` & `cvxpy-1.3.2/cvxpy/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_cone2cone.py` & `cvxpy-1.3.2/cvxpy/tests/test_cone2cone.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 from cvxpy.constraints.second_order import SOC
 from cvxpy.reductions.chain import Chain
 from cvxpy.reductions.cone2cone import affine2direct as a2d
 from cvxpy.reductions.cvx_attr2constr import CvxAttr2Constr
 from cvxpy.reductions.dcp2cone.cone_matrix_stuffing import ConeMatrixStuffing
 from cvxpy.reductions.dcp2cone.dcp2cone import Dcp2Cone
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import ConicSolver
-from cvxpy.reductions.solvers.defines import (
-    INSTALLED_MI_SOLVERS as INSTALLED_MI,)
+from cvxpy.reductions.solvers.defines import INSTALLED_MI_SOLVERS as INSTALLED_MI
 from cvxpy.reductions.solvers.defines import MI_SOCP_SOLVERS as MI_SOCP
 from cvxpy.tests import solver_test_helpers as STH
 from cvxpy.tests.base_test import BaseTest
 
 
 class TestDualize(BaseTest):
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_conic_solvers.py` & `cvxpy-1.3.2/cvxpy/tests/test_conic_solvers.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,29 @@
 import numpy as np
 import pytest
 import scipy.linalg as la
 import scipy.stats as st
 
 import cvxpy as cp
 import cvxpy.tests.solver_test_helpers as sths
-from cvxpy.reductions.solvers.defines import (INSTALLED_MI_SOLVERS,
-                                              INSTALLED_SOLVERS,)
+from cvxpy import SolverError
+from cvxpy.reductions.solvers.defines import (
+    INSTALLED_MI_SOLVERS,
+    INSTALLED_SOLVERS,
+)
 from cvxpy.tests.base_test import BaseTest
-from cvxpy.tests.solver_test_helpers import (StandardTestECPs, StandardTestLPs,
-                                             StandardTestMixedCPs,
-                                             StandardTestPCPs, StandardTestQPs,
-                                             StandardTestSDPs,
-                                             StandardTestSOCPs,)
+from cvxpy.tests.solver_test_helpers import (
+    StandardTestECPs,
+    StandardTestLPs,
+    StandardTestMixedCPs,
+    StandardTestPCPs,
+    StandardTestQPs,
+    StandardTestSDPs,
+    StandardTestSOCPs,
+)
 from cvxpy.utilities.versioning import Version
 
 
 class TestECOS(BaseTest):
 
     def setUp(self) -> None:
         self.a = cp.Variable(name='a')
@@ -396,14 +403,17 @@
 
     def test_scs_expcone_1(self) -> None:
         StandardTestECPs.test_expcone_1(solver='SCS', eps=1e-5)
 
     def test_scs_exp_soc_1(self) -> None:
         StandardTestMixedCPs.test_exp_soc_1(solver='SCS', eps=1e-5)
 
+    def test_scs_sdp_pcp_1(self):
+        StandardTestMixedCPs.test_sdp_pcp_1(solver='SCS')
+        
     def test_scs_pcp_1(self) -> None:
         StandardTestPCPs.test_pcp_1(solver='SCS')
 
     def test_scs_pcp_2(self) -> None:
         StandardTestPCPs.test_pcp_2(solver='SCS')
 
     def test_scs_pcp_3(self) -> None:
@@ -597,14 +607,36 @@
                 "MSK_IPAR_PRESOLVE_USE": "MSK_PRESOLVE_MODE_OFF",
                 "MSK_DPAR_INTPNT_CO_TOL_DFEAS": 1e-9,
                 "MSK_DPAR_INTPNT_CO_TOL_PFEAS": "1e-9"
             }
             with pytest.warns():
                 problem.solve(solver=cp.MOSEK, mosek_params=mosek_params)
 
+    def test_mosek_simplex(self) -> None:
+        n = 10
+        m = 4
+        np.random.seed(0)
+        A = np.random.randn(m, n)
+        x = np.random.randn(n)
+        y = A.dot(x)
+
+        # Solve a simple basis pursuit problem for testing purposes.
+        z = cp.Variable(n)
+        objective = cp.Minimize(cp.norm1(z))
+        constraints = [A @ z == y]
+        problem = cp.Problem(objective, constraints)
+        problem.solve(
+            solver=cp.MOSEK, 
+            mosek_params={"MSK_IPAR_OPTIMIZER": "MSK_OPTIMIZER_DUAL_SIMPLEX"}
+        )
+
+    def test_mosek_sdp_power(self) -> None:
+        """Test the problem in issue #2128"""
+        StandardTestMixedCPs.test_sdp_pcp_1(solver='MOSEK')
+        
     def test_power_portfolio(self) -> None:
         """Test the portfolio problem in issue #2042"""
         T, N = 200, 10
 
         rs = np.random.RandomState(123)
         mean = np.zeros(N) + 1/1000
         cov = rs.rand(N, N) * 1.5 - 0.5
@@ -775,59 +807,39 @@
         # maximization
         StandardTestSDPs.test_sdp_1max(solver='SDPA')
 
     def test_sdpa_sdp_2(self) -> None:
         StandardTestSDPs.test_sdp_2(solver='SDPA')
 
 
-@unittest.skipUnless('CBC' in INSTALLED_SOLVERS, 'CBC is not installed.')
-class TestCBC(BaseTest):
-
-    def setUp(self) -> None:
-        self.a = cp.Variable(name='a')
-        self.b = cp.Variable(name='b')
-        self.c = cp.Variable(name='c')
-
-        self.x = cp.Variable(2, name='x')
-        self.y = cp.Variable(3, name='y')
-        self.z = cp.Variable(2, name='z')
-
-        self.A = cp.Variable((2, 2), name='A')
-        self.B = cp.Variable((2, 2), name='B')
-        self.C = cp.Variable((3, 2), name='C')
+def fflush() -> None:
+    """
+    C code in some solvers uses libc buffering; if we want to capture log output from
+    those solvers to use in tests, we must flush the libc buffers before trying to read
+    the log contents from python.
+    https://github.com/pytest-dev/pytest/issues/8753
+    """
+    import ctypes
+    libc = ctypes.CDLL(None)
+    libc.fflush(None)
+
+
+# We can't inherit from unittest.TestCase since we access some advanced pytest features.
+# As a result, we use the pytest skipif decorator instead of unittest.skipUnless.
+@pytest.mark.skipif('CBC' not in INSTALLED_SOLVERS, reason='CBC is not installed.')
+class TestCBC:
 
     def _cylp_checks_isProvenInfeasible():
         try:
             # https://github.com/coin-or/CyLP/pull/150
             from cylp.cy.CyCbcModel import problemStatus
             return problemStatus[0] == 'search completed'
         except ImportError:
             return False
 
-    def test_options(self) -> None:
-        """Test that all the cvx.CBC solver options work.
-        """
-        prob = cp.Problem(cp.Minimize(cp.norm(self.x, 1)),
-                          [self.x == cp.Variable(2, boolean=True)])
-        if cp.CBC in INSTALLED_SOLVERS:
-            for i in range(2):
-                # Some cut-generators seem to be buggy for now -> set to false
-                # prob.solve(solver=cvx.CBC, verbose=True, GomoryCuts=True, MIRCuts=True,
-                #            MIRCuts2=True, TwoMIRCuts=True, ResidualCapacityCuts=True,
-                #            KnapsackCuts=True, FlowCoverCuts=True, CliqueCuts=True,
-                #            LiftProjectCuts=True, AllDifferentCuts=False, OddHoleCuts=True,
-                #            RedSplitCuts=False, LandPCuts=False, PreProcessCuts=False,
-                #            ProbingCuts=True, SimpleRoundingCuts=True)
-                prob.solve(solver=cp.CBC, verbose=True, maximumSeconds=100)
-            self.assertItemsAlmostEqual(self.x.value, [0, 0])
-        else:
-            with self.assertRaises(Exception) as cm:
-                prob.solve(solver=cp.CBC)
-                self.assertEqual(str(cm.exception), "The solver %s is not installed." % cp.CBC)
-
     def test_cbc_lp_0(self) -> None:
         StandardTestLPs.test_lp_0(solver='CBC', duals=False)
 
     def test_cbc_lp_1(self) -> None:
         StandardTestLPs.test_lp_1(solver='CBC', duals=False)
 
     def test_cbc_lp_2(self) -> None:
@@ -850,19 +862,86 @@
 
     def test_cbc_mi_lp_2(self) -> None:
         StandardTestLPs.test_mi_lp_2(solver='CBC')
 
     def test_cbc_mi_lp_3(self) -> None:
         StandardTestLPs.test_mi_lp_3(solver='CBC')
 
-    @unittest.skipUnless(_cylp_checks_isProvenInfeasible(),
-                         'CyLP <= 0.91.4 has no working integer infeasibility detection')
+    @pytest.mark.skipif(not _cylp_checks_isProvenInfeasible(),
+                        reason='CyLP <= 0.91.4 has no working integer infeasibility detection')
     def test_cbc_mi_lp_5(self) -> None:
         StandardTestLPs.test_mi_lp_5(solver='CBC')
 
+    @pytest.mark.parametrize(
+        "opts",
+        [
+            pytest.param(opts, id=next(iter(opts.keys())))
+            for opts in [
+                {"dualTolerance": 1.0},
+                {"primalTolerance": 1.0},
+                {"maxNumIteration": 1},
+                {"scaling": 0},
+                # {"automaticScaling": True},  # Doesn't work
+                # {"infeasibilityCost": 0.000001},  # Doesn't work
+                {"optimizationDirection": "max"},
+                {"presolve": "off"},
+            ]
+        ]
+    )
+    def test_cbc_lp_options(self, opts: dict, capfd: pytest.LogCaptureFixture) -> None:
+        """
+        Validate that cylp is actually using each option.
+
+        Tentative approach: run model with verbose output with or without the specified
+        option; verbose output should be different each way.
+        """
+        # start by making sure capture buffer is empty to ensure valid results
+        fflush()
+        capfd.readouterr()
+        # run the solver with verbose logging without this option and capture output
+        sth = sths.lp_4()
+        sth.solve(solver='CBC', logLevel=2)
+        fflush()
+        base = capfd.readouterr()
+        # run the solver with verbose logging *with* the option under test
+        try:
+            sth.solve(solver='CBC', logLevel=2, **opts)
+        except Exception:
+            # if setting the option caused the case to fail, that's a pass
+            pass
+        else:
+            # if the case still passes, we at least look for change in the log outputs
+            fflush()
+            with_opt = capfd.readouterr()
+            assert base != with_opt
+
+    def test_cbc_lp_logging(self, capfd: pytest.LogCaptureFixture) -> None:
+        """Validate that logLevel parameter is passed to solver"""
+        # start by making sure capture buffer is empty to ensure valid results
+        fflush()
+        capfd.readouterr()
+
+        # for linear problems
+        StandardTestLPs.test_lp_0(solver='CBC', duals=False, logLevel=0)
+        fflush()
+        quiet_output = capfd.readouterr()
+        StandardTestLPs.test_lp_0(solver='CBC', duals=False, logLevel=5)
+        fflush()
+        verbose_output = capfd.readouterr()
+        assert len(verbose_output.out) > len(quiet_output.out)
+
+        # for mixed integer problems
+        StandardTestLPs.test_mi_lp_0(solver='CBC', logLevel=0)
+        fflush()
+        quiet_output = capfd.readouterr()
+        StandardTestLPs.test_mi_lp_0(solver='CBC', logLevel=5)
+        fflush()
+        verbose_output = capfd.readouterr()
+        assert len(verbose_output.out) > len(quiet_output.out)
+
 
 @unittest.skipUnless('GLPK' in INSTALLED_SOLVERS, 'GLPK is not installed.')
 class TestGLPK(unittest.TestCase):
 
     def test_glpk_lp_0(self) -> None:
         StandardTestLPs.test_lp_0(solver='GLPK')
 
@@ -1803,14 +1882,30 @@
         # Since an invalid SCIP param is passed, an error is expected
         # to be raised when calling solve.
         with pytest.raises(KeyError) as ke:
             prob.solve(solver="SCIP", scip_params={"a": "what?"})
             exc = "One or more scip params in ['a'] are not valid: 'Not a valid parameter name'"
             assert ke.exception == exc
 
+    def test_scip_time_limit_reached(self) -> None:
+        sth = sths.mi_lp_7()
+
+        # TODO doesn't work on windows.
+        # run without enough time to find optimum
+        # sth.solve(solver="SCIP", scip_params={"limits/time": 0.01})
+        # assert sth.prob.status == cp.OPTIMAL_INACCURATE
+        # assert all([v.value is not None for v in sth.prob.variables()])
+
+        # run without enough time to do anything
+        with pytest.raises(cp.error.SolverError) as se:
+            sth.solve(solver="SCIP", scip_params={"limits/time": 0.0})
+            exc = "Solver 'SCIP' failed. " \
+                  "Try another solver, or solve with verbose=True for more information."
+            assert str(se.value) == exc
+
 
 class TestAllSolvers(BaseTest):
 
     def setUp(self) -> None:
         self.a = cp.Variable(name='a')
         self.b = cp.Variable(name='b')
         self.c = cp.Variable(name='c')
@@ -1822,17 +1917,19 @@
         self.A = cp.Variable((2, 2), name='A')
         self.B = cp.Variable((2, 2), name='B')
         self.C = cp.Variable((3, 2), name='C')
 
     def test_installed_solvers(self) -> None:
         """Test the list of installed solvers.
         """
-        from cvxpy.reductions.solvers.defines import (INSTALLED_SOLVERS,
-                                                      SOLVER_MAP_CONIC,
-                                                      SOLVER_MAP_QP,)
+        from cvxpy.reductions.solvers.defines import (
+            INSTALLED_SOLVERS,
+            SOLVER_MAP_CONIC,
+            SOLVER_MAP_QP,
+        )
         prob = cp.Problem(cp.Minimize(cp.norm(self.x, 1) + 1.0), [self.x == 0])
         for solver in SOLVER_MAP_CONIC.keys():
             if solver in INSTALLED_SOLVERS:
                 prob.solve(solver=solver)
                 self.assertAlmostEqual(prob.value, 1.0)
                 self.assertItemsAlmostEqual(self.x.value, [0, 0])
             else:
@@ -1982,14 +2079,27 @@
     def test_scipy_mi_lp_4(self) -> None:
         StandardTestLPs.test_mi_lp_4(solver='SCIPY')
 
     @unittest.skipUnless('SCIPY' in INSTALLED_MI_SOLVERS, 'SCIPY version cannot solve MILPs')
     def test_scipy_mi_lp_5(self) -> None:
         StandardTestLPs.test_mi_lp_5(solver='SCIPY')
 
+    @unittest.skipUnless('SCIPY' in INSTALLED_MI_SOLVERS, 'SCIPY version cannot solve MILPs')
+    def test_scipy_mi_time_limit_reached(self) -> None:
+        sth = sths.mi_lp_7()
+
+        # run without enough time to find optimum
+        sth.solve(solver='SCIPY', scipy_options={"time_limit": 0.01})
+        assert sth.prob.status == cp.OPTIMAL_INACCURATE
+        assert sth.objective.value > 0
+
+        # run without enough time to do anything
+        with pytest.raises(SolverError):
+            sth.solve(solver='SCIPY', scipy_options={"time_limit": 0.})
+
 
 @unittest.skipUnless('COPT' in INSTALLED_SOLVERS, 'COPT is not installed.')
 class TestCOPT(unittest.TestCase):
 
     def test_copt_lp_0(self) -> None:
         StandardTestLPs.test_lp_0(solver='COPT')
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_constant.py` & `cvxpy-1.3.2/cvxpy/tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_constant_atoms.py` & `cvxpy-1.3.2/cvxpy/tests/test_constant_atoms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_constraints.py` & `cvxpy-1.3.2/cvxpy/tests/test_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,21 +279,21 @@
         x, y, z = Variable(n), Variable(n), Variable(n)
         con = PowCone3D(x, y, z, alpha)
         # check violation against feasible values
         x0, y0 = 0.1 + np.random.rand(n), 0.1 + np.random.rand(n)
         z0 = x0**alpha * y0**(1-alpha)
         z0[1] *= -1
         x.value, y.value, z.value = x0, y0, z0
-        viol = con.residual()
+        viol = con.residual
         self.assertLessEqual(viol, 1e-7)
         # check violation against infeasible values
         x1 = x0.copy()
         x1[0] *= -0.9
         x.value = x1
-        viol = con.residual()
+        viol = con.residual
         self.assertGreaterEqual(viol, 0.99*abs(x1[0]))
         # check invalid constraint data
         with self.assertRaises(ValueError):
             con = PowCone3D(x, y, z, 1.001)
         with self.assertRaises(ValueError):
             con = PowCone3D(x, y, z, -0.00001)
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_copy.py` & `cvxpy-1.3.2/cvxpy/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_curvature.py` & `cvxpy-1.3.2/cvxpy/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_custom_solver.py` & `cvxpy-1.3.2/cvxpy/tests/test_custom_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_derivative.py` & `cvxpy-1.3.2/cvxpy/tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_dgp.py` & `cvxpy-1.3.2/cvxpy/tests/test_dgp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_dgp2dcp.py` & `cvxpy-1.3.2/cvxpy/tests/test_dgp2dcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_domain.py` & `cvxpy-1.3.2/cvxpy/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_dpp.py` & `cvxpy-1.3.2/cvxpy/tests/test_dpp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_dqcp.py` & `cvxpy-1.3.2/cvxpy/tests/test_dqcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_examples.py` & `cvxpy-1.3.2/cvxpy/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_expressions.py` & `cvxpy-1.3.2/cvxpy/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_grad.py` & `cvxpy-1.3.2/cvxpy/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_gurobi_write.py` & `cvxpy-1.3.2/cvxpy/tests/test_gurobi_write.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_interfaces.py` & `cvxpy-1.3.2/cvxpy/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_kron_canon.py` & `cvxpy-1.3.2/cvxpy/tests/test_kron_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_lin_ops.py` & `cvxpy-1.3.2/cvxpy/tests/test_lin_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,34 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import numpy as np
 import scipy.sparse as sp
 
-from cvxpy.lin_ops.lin_op import (DENSE_CONST, NEG, PARAM, SCALAR_CONST,
-                                  SPARSE_CONST, SUM_ENTRIES, VARIABLE,)
-from cvxpy.lin_ops.lin_utils import (create_const, create_eq, create_leq,
-                                     create_param, create_var, get_expr_vars,
-                                     neg_expr, sum_entries, sum_expr,)
+from cvxpy.lin_ops.lin_op import (
+    DENSE_CONST,
+    NEG,
+    PARAM,
+    SCALAR_CONST,
+    SPARSE_CONST,
+    SUM_ENTRIES,
+    VARIABLE,
+)
+from cvxpy.lin_ops.lin_utils import (
+    create_const,
+    create_eq,
+    create_leq,
+    create_param,
+    create_var,
+    get_expr_vars,
+    neg_expr,
+    sum_entries,
+    sum_expr,
+)
 from cvxpy.tests.base_test import BaseTest
 
 
 class test_lin_ops(BaseTest):
     """ Unit tests for the lin_ops module. """
 
     def test_variables(self) -> None:
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_linear_cone.py` & `cvxpy-1.3.2/cvxpy/tests/test_linear_cone.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_matrices.py` & `cvxpy-1.3.2/cvxpy/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_mip_vars.py` & `cvxpy-1.3.2/cvxpy/tests/test_mip_vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 """
 import unittest
 
 import numpy as np
 
 import cvxpy as cp
 import cvxpy.settings as s
-from cvxpy.reductions.solvers.defines import (
-    INSTALLED_MI_SOLVERS as MIP_SOLVERS,)
+from cvxpy.reductions.solvers.defines import INSTALLED_MI_SOLVERS as MIP_SOLVERS
 from cvxpy.tests.base_test import BaseTest
 
 
 @unittest.skipUnless(len(MIP_SOLVERS) > 0, 'No mixed-integer solver is installed.')
 class TestMIPVariable(BaseTest):
     """ Unit tests for the expressions/shape module. """
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_monotonicity.py` & `cvxpy-1.3.2/cvxpy/tests/test_monotonicity.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_nonlinear_atoms.py` & `cvxpy-1.3.2/cvxpy/tests/test_nonlinear_atoms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_numpy.py` & `cvxpy-1.3.2/cvxpy/tests/test_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 """
 
 
 import numpy as np
 import pytest
 
 import cvxpy as cp
-from cvxpy.expressions.expression import (__BINARY_EXPRESSION_UFUNCS__,
-                                          __NUMPY_UFUNC_ERROR__,)
+from cvxpy.expressions.expression import (
+    __BINARY_EXPRESSION_UFUNCS__,
+    __NUMPY_UFUNC_ERROR__,
+)
 from cvxpy.tests.base_test import BaseTest
 
 
 class TestNumpy(BaseTest):
     """ Unit tests for using NumPy ufuncs on CVXPY objects should cause errors. """
 
     def setUp(self) -> None:
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_objectives.py` & `cvxpy-1.3.2/cvxpy/tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_param_cone_prog.py` & `cvxpy-1.3.2/cvxpy/tests/test_param_cone_prog.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_param_quad_prog.py` & `cvxpy-1.3.2/cvxpy/tests/test_param_quad_prog.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_perspective.py` & `cvxpy-1.3.2/cvxpy/tests/test_perspective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_power_tools.py` & `cvxpy-1.3.2/cvxpy/tests/test_power_tools.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_problem.py` & `cvxpy-1.3.2/cvxpy/tests/test_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,30 +21,33 @@
 from fractions import Fraction
 from io import StringIO
 
 import ecos
 import numpy
 import numpy as np
 import scipy.sparse as sp
+
 # Solvers.
 import scs
 from numpy import linalg as LA
 
 import cvxpy as cp
 import cvxpy.interface as intf
 import cvxpy.settings as s
 from cvxpy.constraints import PSD, ExpCone, NonPos, Zero
 from cvxpy.error import DCPError, ParameterError, SolverError
 from cvxpy.expressions.constants import Constant, Parameter
 from cvxpy.expressions.variable import Variable
 from cvxpy.problems.problem import Problem
 from cvxpy.reductions.solvers.conic_solvers import ecos_conif, scs_conif
 from cvxpy.reductions.solvers.conic_solvers.conic_solver import ConicSolver
-from cvxpy.reductions.solvers.defines import (INSTALLED_SOLVERS,
-                                              SOLVER_MAP_CONIC,)
+from cvxpy.reductions.solvers.defines import (
+    INSTALLED_SOLVERS,
+    SOLVER_MAP_CONIC,
+)
 from cvxpy.tests.base_test import BaseTest
 
 
 class TestProblem(BaseTest):
     """Unit tests for the expression/expression module.
     """
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_python_backends.py` & `cvxpy-1.3.2/cvxpy/tests/test_python_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 
 import numpy as np
 import pytest
 import scipy.sparse as sp
 
 import cvxpy.settings as s
 from cvxpy.lin_ops.canon_backend import (
-    CanonBackend, ScipyCanonBackend, ScipyTensorView, TensorRepresentation,)
+    CanonBackend,
+    ScipyCanonBackend,
+    ScipyTensorView,
+    TensorRepresentation,
+)
 
 
 @dataclass
 class linOpHelper:
     """
     Helper class that allows to access properties of linOps without
     needing to create a full linOps instance
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_qp_solvers.py` & `cvxpy-1.3.2/cvxpy/tests/test_qp_solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,25 @@
 
 import numpy as np
 import scipy.sparse as sp
 from scipy.linalg import lstsq
 
 import cvxpy as cp
 from cvxpy import Maximize, Minimize, Parameter, Problem
-from cvxpy.atoms import (QuadForm, abs, huber, matrix_frac, norm, power,
-                         quad_over_lin, sum, sum_squares,)
+from cvxpy.atoms import (
+    QuadForm,
+    abs,
+    huber,
+    matrix_frac,
+    norm,
+    power,
+    quad_over_lin,
+    sum,
+    sum_squares,
+)
 from cvxpy.expressions.variable import Variable
 from cvxpy.reductions.solvers.defines import INSTALLED_SOLVERS, QP_SOLVERS
 from cvxpy.tests.base_test import BaseTest
 from cvxpy.tests.solver_test_helpers import StandardTestLPs
 
 
 class TestQp(BaseTest):
```

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_quad_form.py` & `cvxpy-1.3.2/cvxpy/tests/test_quad_form.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_quadratic.py` & `cvxpy-1.3.2/cvxpy/tests/test_quadratic.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_semidefinite_vars.py` & `cvxpy-1.3.2/cvxpy/tests/test_semidefinite_vars.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_shape.py` & `cvxpy-1.3.2/cvxpy/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_sign.py` & `cvxpy-1.3.2/cvxpy/tests/test_sign.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_suppfunc.py` & `cvxpy-1.3.2/cvxpy/tests/test_suppfunc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_valinvec2mixedint.py` & `cvxpy-1.3.2/cvxpy/tests/test_valinvec2mixedint.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_versioning.py` & `cvxpy-1.3.2/cvxpy/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/tests/test_von_neumann_entr.py` & `cvxpy-1.3.2/cvxpy/tests/test_von_neumann_entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/transforms/__init__.py` & `cvxpy-1.3.2/cvxpy/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/transforms/indicator.py` & `cvxpy-1.3.2/cvxpy/transforms/indicator.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/transforms/linearize.py` & `cvxpy-1.3.2/cvxpy/transforms/linearize.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/transforms/partial_optimize.py` & `cvxpy-1.3.2/cvxpy/transforms/partial_optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,19 @@
     if opt_vars is None and dont_opt_vars is None:
         raise ValueError(
             "partial_optimize called with neither opt_vars nor dont_opt_vars."
         )
     # If opt_vars is not specified, it's the complement of dont_opt_vars.
     elif opt_vars is None:
         ids = [id(var) for var in dont_opt_vars]
-        opt_vars = [var for var in prob.variables() if not id(var) in ids]
+        opt_vars = [var for var in prob.variables() if id(var) not in ids]
     # If dont_opt_vars is not specified, it's the complement of opt_vars.
     elif dont_opt_vars is None:
         ids = [id(var) for var in opt_vars]
-        dont_opt_vars = [var for var in prob.variables() if not id(var) in ids]
+        dont_opt_vars = [var for var in prob.variables() if id(var) not in ids]
     elif opt_vars is not None and dont_opt_vars is not None:
         ids = [id(var) for var in opt_vars + dont_opt_vars]
         for var in prob.variables():
             if id(var) not in ids:
                 raise ValueError(
                     ("If opt_vars and new_opt_vars are both specified, "
                      "they must contain all variables in the problem.")
```

### Comparing `cvxpy-1.3.1/cvxpy/transforms/scalarize.py` & `cvxpy-1.3.2/cvxpy/transforms/scalarize.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/transforms/suppfunc.py` & `cvxpy-1.3.2/cvxpy/transforms/suppfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         'exp': exp_idxs,
         'soc': soc_idxs,
         'psd': psd_idxs
     }
     return selectors
 
 
-# flake8: noqa: E501
 class SuppFunc:
     """
     Given a list of CVXPY Constraint objects :math:`\\texttt{constraints}`
     involving a real CVXPY Variable :math:`\\texttt{x}`, consider the convex set
 
     .. math::
```

### Comparing `cvxpy-1.3.1/cvxpy/utilities/__init__.py` & `cvxpy-1.3.2/cvxpy/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/canonical.py` & `cvxpy-1.3.2/cvxpy/utilities/canonical.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/coeff_extractor.py` & `cvxpy-1.3.2/cvxpy/utilities/coeff_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
 import numpy as np
 import scipy.sparse as sp
 
 from cvxpy.cvxcore.python import canonInterface
 from cvxpy.lin_ops.lin_op import NO_OP, LinOp
 from cvxpy.reductions.inverse_data import InverseData
-from cvxpy.utilities.replace_quad_forms import (replace_quad_forms,
-                                                restore_quad_forms,)
+from cvxpy.utilities.replace_quad_forms import (
+    replace_quad_forms,
+    restore_quad_forms,
+)
 
 
 # TODO find best format for sparse matrices: csr, csc, dok, lil, ...
 class CoeffExtractor:
 
     def __init__(self, inverse_data, canon_backend: str | None) -> None:
         self.id_map = inverse_data.var_offsets
```

### Comparing `cvxpy-1.3.1/cvxpy/utilities/cvxpy_upgrade.py` & `cvxpy-1.3.2/cvxpy/utilities/cvxpy_upgrade.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/debug_tools.py` & `cvxpy-1.3.2/cvxpy/utilities/debug_tools.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/grad.py` & `cvxpy-1.3.2/cvxpy/utilities/grad.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/key_utils.py` & `cvxpy-1.3.2/cvxpy/utilities/key_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/linalg.py` & `cvxpy-1.3.2/cvxpy/utilities/linalg.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import scipy.linalg as la
 import scipy.sparse as spar
 import scipy.sparse.linalg as sparla
+from scipy.sparse import csc_matrix
 
 
 def orth(V, tol=1e-12):
     """Return a matrix whose columns are an orthonormal basis for range(V)"""
     Q, R, p = la.qr(V, mode='economic', pivoting=True)
     # ^ V[:, p] == Q @ R.
     rank = np.count_nonzero(np.sum(np.abs(R) > tol, axis=1))
@@ -28,14 +29,26 @@
         P = np.eye(n) - Q1 @ Q1.conj().T
     else:
         P = np.eye(n) - Q1 @ Q1.T
     Q2 = orth(P)
     return Q2
 
 
+def is_diagonal(A):
+    if isinstance(A, spar.spmatrix):
+        off_diagonal_elements = A - spar.diags(A.diagonal())
+        off_diagonal_elements = off_diagonal_elements.toarray()
+    elif isinstance(A, np.ndarray):
+        off_diagonal_elements = A - np.diag(np.diag(A))
+    else:
+        raise ValueError("Unsupported matrix type.")
+
+    return np.allclose(off_diagonal_elements, 0)
+
+
 def is_psd_within_tol(A, tol):
     """
     Return True if we can certify that A is PSD (up to tolerance "tol").
 
     First we check if A is PSD according to the Gershgorin Circle Theorem.
 
     If Gershgorin is inconclusive, then we use an iterative method (from ARPACK,
@@ -57,16 +70,34 @@
     tol : float
         Nonnegative. Something very small, like 1e-10.
     """
 
     if gershgorin_psd_check(A, tol):
         return True
 
+    if is_diagonal(A):
+        if isinstance(A, csc_matrix):
+            return np.all(A.data >= -tol)
+        else:
+            min_diag_entry = np.min(np.diag(A))
+            return min_diag_entry >= -tol
+
     def SA_eigsh(sigma):
-        return sparla.eigsh(A, k=1, sigma=sigma, which='SA', return_eigenvectors=False)
+
+        # Check for default_rng in np.random module (new API)
+        if hasattr(np.random, 'default_rng'):
+            g = np.random.default_rng(123)
+        else:  # fallback to legacy RandomState
+            g = np.random.RandomState(123)
+
+        n = A.shape[0]
+        v0 = g.normal(loc=0.0, scale=1.0, size=n)
+
+        return sparla.eigsh(A, k=1, sigma=sigma, which='SA', v0=v0,
+                            return_eigenvectors=False)
         # Returns the eigenvalue w[i] of A where 1/(w[i] - sigma) is minimized.
         #
         # If A - sigma*I is PSD, then w[i] should be equal to the largest
         # eigenvalue of A.
         #
         # If A - sigma*I is not PSD, then w[i] should be the largest eigenvalue
         # of A where w[i] - sigma < 0.
```

### Comparing `cvxpy-1.3.1/cvxpy/utilities/performance_utils.py` & `cvxpy-1.3.2/cvxpy/utilities/performance_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/perspective_utils.py` & `cvxpy-1.3.2/cvxpy/utilities/perspective_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/power_tools.py` & `cvxpy-1.3.2/cvxpy/utilities/power_tools.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/replace_quad_forms.py` & `cvxpy-1.3.2/cvxpy/utilities/replace_quad_forms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/scopes.py` & `cvxpy-1.3.2/cvxpy/utilities/scopes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Generator
-
 """
 Copyright, the CVXPY authors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -12,14 +10,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import contextlib
+from typing import Generator
 
 _dpp_scope_active = False
 
 
 @contextlib.contextmanager
 def dpp_scope() -> Generator[None, None, None]:
     """Context manager for DPP curvature analysis
```

### Comparing `cvxpy-1.3.1/cvxpy/utilities/shape.py` & `cvxpy-1.3.2/cvxpy/utilities/shape.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/sign.py` & `cvxpy-1.3.2/cvxpy/utilities/sign.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy/utilities/versioning.py` & `cvxpy-1.3.2/cvxpy/utilities/versioning.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/cvxpy.egg-info/PKG-INFO` & `cvxpy-1.3.2/cvxpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A domain-specific language for modeling convex optimization problems in Python.
 Home-page: https://github.com/cvxpy/cvxpy
 Author: Steven Diamond, Eric Chu, Stephen Boyd
 Author-email: stevend2@stanford.edu, akshayka@cs.stanford.edu, echu508@stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Description: CVXPY
         =====================
```

### Comparing `cvxpy-1.3.1/cvxpy.egg-info/SOURCES.txt` & `cvxpy-1.3.2/cvxpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxpy-1.3.1/pyproject.toml` & `cvxpy-1.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-[tool.isort]
-include_trailing_comma = true
-use_parentheses = true
-extend_skip = [
-    "cvxpy/__init__.py",
-    "cvxpy/reductions/__init__.py",
-    "cvxpy/reductions/dcp2cone/atom_canonicalizers/__init__.py"
+[tool.ruff]
+select = ["E", "F", "I"]
+line-length = 100
+exclude = [
+    "build",
+    "examples",
+    "doc",
+    "cvxpy/cvxcore/*",
+    "*__init__.py"
 ]
+# The minimum Python version that should be supported
+target-version = "py37"
+
 
 [tool.pytest.ini_options]
 testpaths = [
     "cvxpy/tests/"
 ]
 
 [build-system]
```

### Comparing `cvxpy-1.3.1/setup.py` & `cvxpy-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #   snippets. We have mostly left those comments in-place, but we sometimes preface
 #   them with the following remark:
 #      "The comment below is from the SciPy code which we repurposed for cvxpy."
 #
 
 MAJOR = 1
 MINOR = 3
-MICRO = 1
+MICRO = 2
 IS_RELEASED = True
 IS_RELEASE_BRANCH = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 
 # Return the git revision as a string
 def git_version():
```


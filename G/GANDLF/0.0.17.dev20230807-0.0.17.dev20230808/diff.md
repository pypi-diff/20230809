# Comparing `tmp/GANDLF-0.0.17.dev20230807.tar.gz` & `tmp/GANDLF-0.0.17.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230807.tar", last modified: Mon Aug  7 03:13:11 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230808.tar", last modified: Tue Aug  8 03:12:20 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230807.tar` & `GANDLF-0.0.17.dev20230808.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.942073 GANDLF-0.0.17.dev20230807/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.890072 GANDLF-0.0.17.dev20230807/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.890072 GANDLF-0.0.17.dev20230807/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.894073 GANDLF-0.0.17.dev20230807/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.898073 GANDLF-0.0.17.dev20230807/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.898073 GANDLF-0.0.17.dev20230807/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.902073 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/hed_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.902073 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.902073 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.906073 GANDLF-0.0.17.dev20230807/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.906073 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.910073 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.910073 GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.914073 GANDLF-0.0.17.dev20230807/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.918073 GANDLF-0.0.17.dev20230807/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/metrics/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/metrics/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.926073 GANDLF-0.0.17.dev20230807/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.934073 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.934073 GANDLF-0.0.17.dev20230807/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.934073 GANDLF-0.0.17.dev20230807/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.942073 GANDLF-0.0.17.dev20230807/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 03:13:04.000000 GANDLF-0.0.17.dev20230807/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:13:11.890072 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-07 03:13:11.000000 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-07 03:13:11.000000 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:13:11.000000 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:10:28.000000 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-07 03:13:11.000000 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 03:13:11.000000 GANDLF-0.0.17.dev20230807/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-07 03:13:11.942073 GANDLF-0.0.17.dev20230807/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 03:13:11.942073 GANDLF-0.0.17.dev20230807/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-07 03:10:04.000000 GANDLF-0.0.17.dev20230807/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.655629 GANDLF-0.0.17.dev20230808/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.615628 GANDLF-0.0.17.dev20230808/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.619628 GANDLF-0.0.17.dev20230808/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.619628 GANDLF-0.0.17.dev20230808/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.623628 GANDLF-0.0.17.dev20230808/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.623628 GANDLF-0.0.17.dev20230808/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.627628 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/hed_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.627628 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.627628 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.631628 GANDLF-0.0.17.dev20230808/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.631628 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.635629 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.635629 GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.635629 GANDLF-0.0.17.dev20230808/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.639629 GANDLF-0.0.17.dev20230808/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.647629 GANDLF-0.0.17.dev20230808/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.651629 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.651629 GANDLF-0.0.17.dev20230808/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.651629 GANDLF-0.0.17.dev20230808/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.655629 GANDLF-0.0.17.dev20230808/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 03:12:14.000000 GANDLF-0.0.17.dev20230808/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:12:20.615628 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-08 03:12:20.000000 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-08 03:12:20.000000 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 03:12:20.000000 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 03:10:11.000000 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 03:12:20.000000 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 03:12:20.000000 GANDLF-0.0.17.dev20230808/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-08 03:12:20.655629 GANDLF-0.0.17.dev20230808/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 03:12:20.655629 GANDLF-0.0.17.dev20230808/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-08 03:09:56.000000 GANDLF-0.0.17.dev20230808/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230807/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230808/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230808/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230808/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230808/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230808/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230808/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/generate_metrics.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230808/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230808/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230808/GANDLF/compute/generic.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,17 @@
 
         # Calculate the weights here
         (
             parameters["weights"],
             parameters["class_weights"],
         ) = get_class_imbalance_weights(parameters["training_data"], parameters)
 
+        print("Class weights  : ", parameters["class_weights"])
+        print("Penalty weights: ", parameters["weights"])
+
     else:
         scheduler = None
 
     # these keys contain generators, and are not needed beyond this point in params
     generator_keys_to_remove = ["optimizer_object", "model_parameters"]
     for key in generator_keys_to_remove:
         parameters.pop(key, None)
```

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230808/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230808/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230808/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230808/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/hed_augs.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/hed_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230808/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230808/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230808/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230808/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230808/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230808/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230808/GANDLF/losses/segmentation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 import torch
 
 
 # Dice scores and dice losses
-def dice(predicted, target) -> torch.Tensor:
+def dice(predicted: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
     """
     This function computes a dice score between two tensors.
 
     Args:
-        predicted (_type_): Predicted value by the network.
-        target (_type_): Required target label to match the predicted with
+        predicted (torch.Tensor): Predicted value by the network.
+        target (torch.Tensor): Required target label to match the predicted with
 
     Returns:
         torch.Tensor: The computed dice score.
     """
     predicted_flat = predicted.flatten()
     label_flat = target.flatten()
     intersection = (predicted_flat * label_flat).sum()
@@ -21,84 +21,205 @@
     dice_score = (2.0 * intersection + sys.float_info.min) / (
         predicted_flat.sum() + label_flat.sum() + sys.float_info.min
     )
 
     return dice_score
 
 
-def MCD(predicted, target, num_class, weights=None, ignore_class=None, loss_type=0):
+def mcc(predictions: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+    """
+    This function computes the Matthews Correlation Coefficient (MCC) between two tensors. Adapted from https://github.com/kakumarabhishek/MCC-Loss/blob/main/loss.py.
+
+    Args:
+        predictions (torch.Tensor): The predicted value by the network.
+        targets (torch.Tensor): Required target label to match the predicted with
+
+    Returns:
+        torch.Tensor: The computed MCC score.
+    """
+    tp = torch.sum(torch.mul(predictions, targets))
+    tn = torch.sum(torch.mul((1 - predictions), (1 - targets)))
+    fp = torch.sum(torch.mul(predictions, (1 - targets)))
+    fn = torch.sum(torch.mul((1 - predictions), targets))
+
+    numerator = torch.mul(tp, tn) - torch.mul(fp, fn)
+    # Adding epsilon to the denominator to avoid divide-by-zero errors.
+    denominator = (
+        torch.sqrt(
+            torch.add(tp, 1, fp)
+            * torch.add(tp, 1, fn)
+            * torch.add(tn, 1, fp)
+            * torch.add(tn, 1, fn)
+        )
+        + torch.finfo(torch.float32).eps
+    )
+
+    return torch.div(numerator.sum(), denominator.sum())
+
+
+def generic_loss_calculator(
+    predicted: torch.Tensor,
+    target: torch.Tensor,
+    num_class: int,
+    loss_criteria,
+    weights: list = None,
+    ignore_class: int = None,
+    loss_type: int = 0,
+) -> torch.Tensor:
     """
     This function computes the mean class dice score between two tensors
 
     Args:
         predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         num_class (int): Number of classes (including the background class)
+        loss_criteria (function): Loss function to use
         weights (list, optional): Dice weights for each class (excluding the background class), defaults to None
         ignore_class (int, optional): Class to ignore, defaults to None
-        loss_type (int, optional): Type of loss to compute, defaults to 0
+        loss_type (int, optional): Type of loss to compute, defaults to 0. The options are:
             0: no loss, normal dice calculation
             1: dice loss, (1-dice)
             2: log dice, -log(dice)
 
     Returns:
         torch.Tensor: Mean Class Dice score
     """
+    accumulated_loss = 0
+    # default to a ridiculous value so that it is ignored by default
+    ignore_class = -1e10 if ignore_class is None else ignore_class
+
+    for class_index in range(num_class):
+        if class_index != ignore_class:
+            current_loss = loss_criteria(
+                predicted[:, class_index, ...], target[:, class_index, ...]
+            )
+
+            # subtract from 1 because this is supposed to be a loss
+            default_loss = 1 - current_loss
+            if loss_type == 2 or loss_type == "log":
+                # negative because we want positive losses, and add epsilon to avoid infinities
+                current_loss = -torch.log(current_loss + torch.finfo(torch.float32).eps)
+            else:
+                current_loss = default_loss
+
+            # multiply by appropriate weight if provided
+            if weights is not None:
+                current_loss = current_loss * weights[class_index]
 
-    acc_dice = 0
+            accumulated_loss += current_loss
 
-    for i in range(num_class):  # 0 is background
-        currentDice = dice(predicted[:, i, ...], target[:, i, ...])
+    if weights is None:
+        accumulated_loss /= num_class
 
-        if loss_type == 1:
-            currentDice = 1 - currentDice  # subtract from 1 because this is a loss
-        elif loss_type == 2:
-            # negative because we want positive losses
-            currentDice = -torch.log(currentDice + torch.finfo(torch.float32).eps)
+    return accumulated_loss
 
-        if weights is not None:
-            currentDice = currentDice * weights[i]  # multiply by weight
 
-        acc_dice += currentDice
+def MCD_loss(
+    predicted: torch.Tensor, target: torch.Tensor, params: dict
+) -> torch.Tensor:
+    """
+    This function computes the Dice loss between two tensors. These weights should be the penalty weights, not dice weights.
 
-    if weights is None:
-        acc_dice /= num_class  # we should not be considering 0
+    Args:
+        predicted (torch.Tensor): The predicted value by the network.
+        target (torch.Tensor): Required target label to match the predicted with
+        params (dict): Dictionary of parameters
 
-    return acc_dice
+    Returns:
+        torch.Tensor: The computed MCC loss.
+    """
+    return generic_loss_calculator(
+        predicted,
+        target,
+        len(params["model"]["class_list"]),
+        dice,
+        params["weights"],
+        None,
+        1,
+    )
 
 
-def MCD_loss(predicted, target, params):
+def MCD_log_loss(
+    predicted: torch.Tensor, target: torch.Tensor, params: dict
+) -> torch.Tensor:
     """
-    These weights should be the penalty weights, not dice weights
+    This function computes the Dice loss between two tensors with log. These weights should be the penalty weights, not dice weights.
+
+    Args:
+        predicted (torch.Tensor): The predicted value by the network.
+        target (torch.Tensor): Required target label to match the predicted with
+        params (dict): Dictionary of parameters
+
+    Returns:
+        torch.Tensor: The computed MCC loss.
     """
-    return MCD(
+    return generic_loss_calculator(
         predicted,
         target,
         len(params["model"]["class_list"]),
+        dice,
+        params["weights"],
+        None,
+        2,
+    )
+
+
+def MCC_loss(
+    predicted: torch.Tensor, target: torch.Tensor, params: dict
+) -> torch.Tensor:
+    """
+    This function computes the Matthews Correlation Coefficient (MCC) loss between two tensors. These weights should be the penalty weights, not dice weights.
+
+    Args:
+        predicted (torch.Tensor): The predicted value by the network.
+        target (torch.Tensor): Required target label to match the predicted with
+        params (dict): Dictionary of parameters
+
+    Returns:
+        torch.Tensor: The computed MCC loss.
+    """
+    return generic_loss_calculator(
+        predicted,
+        target,
+        len(params["model"]["class_list"]),
+        mcc,
         params["weights"],
         None,
         1,
     )
 
 
-def MCD_log_loss(predicted, target, params):
+def MCC_log_loss(
+    predicted: torch.Tensor, target: torch.Tensor, params: dict
+) -> torch.Tensor:
     """
-    These weights should be the penalty weights, not dice weights
+    This function computes the Matthews Correlation Coefficient (MCC) loss between two tensors with log. These weights should be the penalty weights, not dice weights.
+
+    Args:
+        predicted (torch.Tensor): The predicted value by the network.
+        target (torch.Tensor): Required target label to match the predicted with
+        params (dict): Dictionary of parameters
+
+    Returns:
+        torch.Tensor: The computed MCC loss.
     """
-    return MCD(
+    return generic_loss_calculator(
         predicted,
         target,
         len(params["model"]["class_list"]),
+        mcc,
         params["weights"],
         None,
         2,
     )
 
 
-def tversky_loss(predicted, target, alpha=0.5, beta=0.5):
+def tversky_loss(
+    predicted: torch.Tensor, target: torch.Tensor, alpha: float = 0.5, beta: float = 0.5
+) -> torch.Tensor:
     """
     This function calculates the Tversky loss between two tensors.
 
     Args:
         predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         alpha (float, optional): Weight of false positives. Defaults to 0.5.
@@ -123,15 +244,17 @@
     denominator = true_positives + alpha * false_positives + beta * false_negatives
     score = (numerator + sys.float_info.min) / (denominator + sys.float_info.min)
 
     loss = 1 - score
     return loss
 
 
-def MCT_loss(predicted, target, params=None):
+def MCT_loss(
+    predicted: torch.Tensor, target: torch.Tensor, params: dict = None
+) -> torch.Tensor:
     """
     This function calculates the Multi-Class Tversky loss between two tensors.
 
     Args:
         predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         params (dict, optional): Additional parameters for computing loss function, including weights for each class
@@ -167,15 +290,17 @@
     Returns:
         torch.Tensor: The computed Kullback-Leibler divergence
     """
     loss = -0.5 * torch.sum(1 + logvar - mu.pow(2) - logvar.exp(), dim=-1)
     return loss.mean()
 
 
-def FocalLoss(predicted, target, params=None):
+def FocalLoss(
+    predicted: torch.Tensor, target: torch.Tensor, params: dict = None
+) -> torch.Tensor:
     """
     This function calculates the Focal loss between two tensors.
 
     Args:
         predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         params (dict, optional): Additional parameters for computing loss function, including weights for each class
@@ -187,15 +312,15 @@
     size_average = True
     if isinstance(params["loss_function"], dict):
         gamma = params["loss_function"].get("gamma", 2.0)
         size_average = params["loss_function"].get("size_average", True)
 
     def _focal_loss(preds, target, gamma, size_average=True):
         """
-        Internal helper function to calcualte focal loss for a single class.
+        Internal helper function to calculate focal loss for a single class.
 
         Args:
             preds (torch.Tensor): predicted generally by the network
             target (torch.Tensor): Required target label to match the predicted with
             gamma (float): The gamma value for focal loss
             size_average (bool, optional): Whether to average the loss across the batch. Defaults to True.
```

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230808/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230808/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230808/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230808/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/metrics/synthesis.py` & `GANDLF-0.0.17.dev20230808/GANDLF/metrics/synthesis.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230808/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230808/GANDLF/optimizers/wrap_torch.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         optimizer (torch.optim.SGD): A Stochastic Gradient Descent optimizer.
 
     """
     # Create the optimizer using the input parameters
     optimizer = SGD(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
-        momentum=parameters["optimizer"].get("momentum", 0.9),
-        weight_decay=parameters["optimizer"].get("weight_decay", 0),
+        momentum=parameters["optimizer"].get("momentum", 0.99),
+        weight_decay=parameters["optimizer"].get("weight_decay", 3e-05),
         dampening=parameters["optimizer"].get("dampening", 0),
-        nesterov=parameters["optimizer"].get("Nesterov", False),
+        nesterov=parameters["optimizer"].get("nesterov", True),
     )
 
     return optimizer
 
 
 def asgd(parameters):
     """
@@ -51,15 +51,15 @@
     # Create the optimizer using the input parameters
     return ASGD(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
         alpha=parameters["optimizer"].get("alpha", 0.75),
         t0=parameters["optimizer"].get("t0", 1e6),
         lambd=parameters["optimizer"].get("lambd", 1e-4),
-        weight_decay=parameters["optimizer"].get("weight_decay", 0),
+        weight_decay=parameters["optimizer"].get("weight_decay", 3e-05),
     )
 
 
 def adam(parameters, opt_type="normal"):
     """
     Creates an Adam or AdamW optimizer from the PyTorch `torch.optim` module using the input parameters.
 
@@ -173,15 +173,15 @@
     """
     # Create the optimizer using the input parameters
     return Adadelta(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
         rho=parameters["optimizer"].get("rho", 0.9),
         eps=parameters["optimizer"].get("eps", 1e-6),
-        weight_decay=parameters["optimizer"].get("weight_decay", 0),
+        weight_decay=parameters["optimizer"].get("weight_decay", 3e-05),
     )
 
 
 def adagrad(parameters):
     """
     Creates an Adagrad optimizer from the PyTorch `torch.optim` module using the input parameters.
 
@@ -195,15 +195,15 @@
 
     # Create the optimizer using the input parameters
     return Adagrad(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
         lr_decay=parameters["optimizer"].get("lr_decay", 0),
         eps=parameters["optimizer"].get("eps", 1e-6),
-        weight_decay=parameters["optimizer"].get("weight_decay", 0),
+        weight_decay=parameters["optimizer"].get("weight_decay", 3e-05),
     )
 
 
 def rmsprop(parameters):
     """
     Creates an RMSprop optimizer from the PyTorch `torch.optim` module using the input parameters.
 
@@ -218,15 +218,15 @@
     return RMSprop(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
         alpha=parameters["optimizer"].get("alpha", 0.99),
         eps=parameters["optimizer"].get("eps", 1e-8),
         centered=parameters["optimizer"].get("centered", False),
         momentum=parameters["optimizer"].get("momentum", 0),
-        weight_decay=parameters["optimizer"].get("weight_decay", 0),
+        weight_decay=parameters["optimizer"].get("weight_decay", 3e-05),
     )
 
 
 def radam(parameters):
     """
     Creates a RAdam optimizer from the PyTorch `torch.optim` module using the input parameters.
 
@@ -238,10 +238,10 @@
     """
     # Create the optimizer using the input parameters
     return RAdam(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
         betas=parameters["optimizer"].get("betas", (0.9, 0.999)),
         eps=parameters["optimizer"].get("eps", 1e-8),
-        weight_decay=parameters["optimizer"].get("weight_decay", 0),
+        weight_decay=parameters["optimizer"].get("weight_decay", 3e-05),
         foreach=parameters["optimizer"].get("foreach", None),
     )
```

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230808/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230808/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230808/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/modelio.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,26 +83,25 @@
                     onnx_path,
                     opset_version=11,
                     export_params=True,
                     verbose=True,
                     input_names=["input"],
                     output_names=["output"],
                 )
-
-            ov_output_dir = os.path.dirname(os.path.abspath(path))
         except RuntimeWarning:
             print("WARNING: Cannot export to ONNX model.")
             return
 
         # Check if OpenVINO is present and try to convert the ONNX model
         openvino_present = False
         try:
             import openvino as ov
             from openvino.tools.mo import convert_model
             from openvino.runtime import get_version
+
             openvino_present = False
             # check for the correct openvino version to prevent inadvertent api breaks
             if "2023.0.1" in get_version():
                 openvino_present = True
         except ImportError:
             print("WARNING: OpenVINO is not present.")
```

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230808/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230808/GANDLF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230807
+Version: 0.0.17.dev20230808
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230807 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230808 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230807/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230808/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/LICENSE` & `GANDLF-0.0.17.dev20230808/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/PKG-INFO` & `GANDLF-0.0.17.dev20230808/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230807
+Version: 0.0.17.dev20230808
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230807 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230808 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230807/README.md` & `GANDLF-0.0.17.dev20230808/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/SECURITY.md` & `GANDLF-0.0.17.dev20230808/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230808/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_collectStats` & `GANDLF-0.0.17.dev20230808/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230808/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230808/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_deploy` & `GANDLF-0.0.17.dev20230808/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230808/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230808/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230808/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_preprocess` & `GANDLF-0.0.17.dev20230808/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230808/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_run` & `GANDLF-0.0.17.dev20230808/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230808/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230807/setup.py` & `GANDLF-0.0.17.dev20230808/setup.py`

 * *Files identical despite different names*


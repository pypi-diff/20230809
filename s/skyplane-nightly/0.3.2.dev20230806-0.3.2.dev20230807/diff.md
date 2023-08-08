# Comparing `tmp/skyplane_nightly-0.3.2.dev20230806.tar.gz` & `tmp/skyplane_nightly-0.3.2.dev20230807.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyplane_nightly-0.3.2.dev20230806.tar", max compression
+gzip compressed data, was "skyplane_nightly-0.3.2.dev20230807.tar", max compression
```

## Comparing `skyplane_nightly-0.3.2.dev20230806.tar` & `skyplane_nightly-0.3.2.dev20230807.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0    11357 2023-08-06 23:44:25.264016 skyplane_nightly-0.3.2.dev20230806/LICENSE
--rw-r--r--   0        0        0     7468 2023-08-06 23:44:25.264016 skyplane_nightly-0.3.2.dev20230806/README.md
--rw-r--r--   0        0        0     3669 2023-08-06 23:45:15.389284 skyplane_nightly-0.3.2.dev20230806/pyproject.toml
--rw-r--r--   0        0        0      649 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/__init__.py
--rw-r--r--   0        0        0     4331 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/client.py
--rw-r--r--   0        0        0     3040 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/config.py
--rw-r--r--   0        0        0    14841 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/dataplane.py
--rw-r--r--   0        0        0     2081 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/obj_store.py
--rw-r--r--   0        0        0     7117 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/pipeline.py
--rw-r--r--   0        0        0    15091 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/provisioner.py
--rw-r--r--   0        0        0    17597 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/tracker.py
--rw-r--r--   0        0        0    38945 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/transfer_job.py
--rw-r--r--   0        0        0    14790 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/api/usage.py
--rw-r--r--   0        0        0     6120 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/chunk.py
--rw-r--r--   0        0        0     3317 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli.py
--rw-r--r--   0        0        0    18045 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_cloud.py
--rw-r--r--   0        0        0     1678 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_config.py
--rw-r--r--   0        0        0    27030 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_init.py
--rw-r--r--   0        0        0    24587 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_transfer.py
--rw-r--r--   0        0        0      461 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/__init__.py
--rw-r--r--   0        0        0    23462 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/cli_profile.py
--rw-r--r--   0        0        0     1757 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/cli_query.py
--rw-r--r--   0        0        0     9215 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/provision.py
--rw-r--r--   0        0        0     3100 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/impl/common.py
--rw-r--r--   0        0        0     4678 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/impl/cp_replicate_fallback.py
--rw-r--r--   0        0        0     3071 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/cli/impl/progress_bar.py
--rw-r--r--   0        0        0     1247 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/__init__.py
--rw-r--r--   0        0        0     5908 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_auth.py
--rw-r--r--   0        0        0    11591 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_cloud_provider.py
--rw-r--r--   0        0        0     4315 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_key_manager.py
--rw-r--r--   0        0        0    11509 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_network.py
--rw-r--r--   0        0        0     1606 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_pricing.py
--rw-r--r--   0        0        0     6294 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_server.py
--rw-r--r--   0        0        0     9526 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/azure/azure_auth.py
--rw-r--r--   0        0        0    20681 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/azure/azure_cloud_provider.py
--rw-r--r--   0        0        0     7503 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/azure/azure_server.py
--rw-r--r--   0        0        0     3564 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/cloud_provider.py
--rw-r--r--   0        0        0     2883 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/const_cmds.py
--rw-r--r--   0        0        0    12043 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_auth.py
--rw-r--r--   0        0        0     9355 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_cloud_provider.py
--rw-r--r--   0        0        0     2462 2023-08-06 23:44:25.280016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_key_manager.py
--rw-r--r--   0        0        0     6288 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_network.py
--rw-r--r--   0        0        0     2786 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_pricing.py
--rw-r--r--   0        0        0     5151 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_server.py
--rw-r--r--   0        0        0      211 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
--rw-r--r--   0        0        0        0 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
--rw-r--r--   0        0        0     2242 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/config.py
--rw-r--r--   0        0        0      877 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/constants.py
--rw-r--r--   0        0        0     5353 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
--rw-r--r--   0        0        0      710 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/utils.py
--rw-r--r--   0        0        0    40464 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
--rw-r--r--   0        0        0     5320 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibmcloud_auth.py
--rw-r--r--   0        0        0     2851 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibmcloud_provider.py
--rw-r--r--   0        0        0     3522 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibmcloud_server.py
--rw-r--r--   0        0        0      937 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/key_utils.py
--rw-r--r--   0        0        0    17426 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/compute/server.py
--rw-r--r--   0        0        0    13473 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/config.py
--rw-r--r--   0        0        0     1229 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/config_paths.py
--rw-r--r--   0        0        0        0 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/data/__init__.py
--rw-r--r--   0        0        0    19636 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/data/aws_transfer_costs.csv
--rw-r--r--   0        0        0      617 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/data/vcpu_info.csv
--rw-r--r--   0        0        0     3078 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/exceptions.py
--rw-r--r--   0        0        0      811 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/cert.py
--rw-r--r--   0        0        0     4349 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/chunk_store.py
--rw-r--r--   0        0        0    15655 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_daemon.py
--rw-r--r--   0        0        0    16570 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_daemon_api.py
--rw-r--r--   0        0        0      718 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_onprem.py
--rw-r--r--   0        0        0     5149 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_program.py
--rw-r--r--   0        0        0     1732 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_queue.py
--rw-r--r--   0        0        0        0 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/operators/__init__.py
--rw-r--r--   0        0        0    25487 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/operators/gateway_operator.py
--rw-r--r--   0        0        0    10552 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/operators/gateway_receiver.py
--rw-r--r--   0        0        0       37 2023-08-06 23:45:15.385284 skyplane_nightly-0.3.2.dev20230806/skyplane/gateway_version.py
--rw-r--r--   0        0        0    13101 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/azure_blob_interface.py
--rw-r--r--   0        0        0     2887 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/azure_storage_account_interface.py
--rw-r--r--   0        0        0    10871 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/cos_interface.py
--rw-r--r--   0        0        0     2010 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/file_system_interface.py
--rw-r--r--   0        0        0    12754 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/gcs_interface.py
--rw-r--r--   0        0        0     5963 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/hdfs_interface.py
--rw-r--r--   0        0        0     3287 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/object_store_interface.py
--rw-r--r--   0        0        0     5644 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/posix_file_interface.py
--rw-r--r--   0        0        0     3606 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/r2_interface.py
--rw-r--r--   0        0        0    11595 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/s3_interface.py
--rw-r--r--   0        0        0     2569 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/storage_interface.py
--rw-r--r--   0        0        0    23858 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/planner/planner.py
--rw-r--r--   0        0        0    18157 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/planner/solver.py
--rw-r--r--   0        0        0     6467 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/planner/solver_ilp.py
--rw-r--r--   0        0        0     1996 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/planner/solver_ron.py
--rw-r--r--   0        0        0     7920 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/planner/topology.py
--rw-r--r--   0        0        0      846 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/cache.py
--rw-r--r--   0        0        0      617 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/definitions.py
--rw-r--r--   0        0        0     2494 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/fn.py
--rw-r--r--   0        0        0     1881 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/generator.py
--rw-r--r--   0        0        0     1386 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/imports.py
--rw-r--r--   0        0        0     2131 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/logger.py
--rw-r--r--   0        0        0     1447 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/networking_tools.py
--rw-r--r--   0        0        0     3162 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/path.py
--rw-r--r--   0        0        0     1160 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/retry.py
--rw-r--r--   0        0        0      612 2023-08-06 23:44:25.284016 skyplane_nightly-0.3.2.dev20230806/skyplane/utils/timer.py
--rw-r--r--   0        0        0    10740 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230806/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 23:44:12.791315 skyplane_nightly-0.3.2.dev20230807/LICENSE
+-rw-r--r--   0        0        0     7468 2023-08-07 23:44:12.791315 skyplane_nightly-0.3.2.dev20230807/README.md
+-rw-r--r--   0        0        0     3669 2023-08-07 23:45:00.052533 skyplane_nightly-0.3.2.dev20230807/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-08-07 23:44:12.803316 skyplane_nightly-0.3.2.dev20230807/skyplane/__init__.py
+-rw-r--r--   0        0        0     4108 2023-08-07 23:44:12.803316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/client.py
+-rw-r--r--   0        0        0     3034 2023-08-07 23:44:12.803316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/config.py
+-rw-r--r--   0        0        0    14809 2023-08-07 23:44:12.803316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/dataplane.py
+-rw-r--r--   0        0        0     2081 2023-08-07 23:44:12.803316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/obj_store.py
+-rw-r--r--   0        0        0     6873 2023-08-07 23:44:12.803316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/pipeline.py
+-rw-r--r--   0        0        0    15091 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/provisioner.py
+-rw-r--r--   0        0        0    17530 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/tracker.py
+-rw-r--r--   0        0        0    38891 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/transfer_job.py
+-rw-r--r--   0        0        0    14790 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/api/usage.py
+-rw-r--r--   0        0        0     6120 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/chunk.py
+-rw-r--r--   0        0        0     3317 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli.py
+-rw-r--r--   0        0        0    18045 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_cloud.py
+-rw-r--r--   0        0        0     1678 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_config.py
+-rw-r--r--   0        0        0    27030 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_init.py
+-rw-r--r--   0        0        0    24492 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_transfer.py
+-rw-r--r--   0        0        0      461 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/__init__.py
+-rw-r--r--   0        0        0    23462 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/cli_profile.py
+-rw-r--r--   0        0        0     1757 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/cli_query.py
+-rw-r--r--   0        0        0     9215 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/provision.py
+-rw-r--r--   0        0        0     3100 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/impl/common.py
+-rw-r--r--   0        0        0     4678 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/impl/cp_replicate_fallback.py
+-rw-r--r--   0        0        0     3048 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/cli/impl/progress_bar.py
+-rw-r--r--   0        0        0     1247 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/__init__.py
+-rw-r--r--   0        0        0     5908 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_auth.py
+-rw-r--r--   0        0        0    11591 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_cloud_provider.py
+-rw-r--r--   0        0        0     4315 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_key_manager.py
+-rw-r--r--   0        0        0    11509 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_network.py
+-rw-r--r--   0        0        0     1606 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_pricing.py
+-rw-r--r--   0        0        0     6294 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_server.py
+-rw-r--r--   0        0        0     9516 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/azure/azure_auth.py
+-rw-r--r--   0        0        0    20681 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/azure/azure_cloud_provider.py
+-rw-r--r--   0        0        0     7503 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/azure/azure_server.py
+-rw-r--r--   0        0        0     3564 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/cloud_provider.py
+-rw-r--r--   0        0        0     2883 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/const_cmds.py
+-rw-r--r--   0        0        0    12043 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_auth.py
+-rw-r--r--   0        0        0     9355 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_cloud_provider.py
+-rw-r--r--   0        0        0     2462 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_key_manager.py
+-rw-r--r--   0        0        0     6288 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_network.py
+-rw-r--r--   0        0        0     2786 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_pricing.py
+-rw-r--r--   0        0        0     5151 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_server.py
+-rw-r--r--   0        0        0      211 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
+-rw-r--r--   0        0        0        0 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
+-rw-r--r--   0        0        0     2242 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/config.py
+-rw-r--r--   0        0        0      877 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/constants.py
+-rw-r--r--   0        0        0     5353 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
+-rw-r--r--   0        0        0      710 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/utils.py
+-rw-r--r--   0        0        0    40464 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
+-rw-r--r--   0        0        0     5320 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibmcloud_auth.py
+-rw-r--r--   0        0        0     2851 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibmcloud_provider.py
+-rw-r--r--   0        0        0     3522 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibmcloud_server.py
+-rw-r--r--   0        0        0      937 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/key_utils.py
+-rw-r--r--   0        0        0    17282 2023-08-07 23:44:12.807316 skyplane_nightly-0.3.2.dev20230807/skyplane/compute/server.py
+-rw-r--r--   0        0        0    13473 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/config.py
+-rw-r--r--   0        0        0     1229 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/config_paths.py
+-rw-r--r--   0        0        0        0 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/data/__init__.py
+-rw-r--r--   0        0        0    19636 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/data/aws_transfer_costs.csv
+-rw-r--r--   0        0        0      617 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/data/vcpu_info.csv
+-rw-r--r--   0        0        0     3078 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/exceptions.py
+-rw-r--r--   0        0        0      811 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/cert.py
+-rw-r--r--   0        0        0     4349 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/chunk_store.py
+-rw-r--r--   0        0        0    15645 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_daemon.py
+-rw-r--r--   0        0        0    16548 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_daemon_api.py
+-rw-r--r--   0        0        0      667 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_onprem.py
+-rw-r--r--   0        0        0     5142 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_program.py
+-rw-r--r--   0        0        0     1732 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_queue.py
+-rw-r--r--   0        0        0        0 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/operators/__init__.py
+-rw-r--r--   0        0        0    25487 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/operators/gateway_operator.py
+-rw-r--r--   0        0        0    10552 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/operators/gateway_receiver.py
+-rw-r--r--   0        0        0       37 2023-08-07 23:45:00.048533 skyplane_nightly-0.3.2.dev20230807/skyplane/gateway_version.py
+-rw-r--r--   0        0        0    13053 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/azure_blob_interface.py
+-rw-r--r--   0        0        0     2887 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/azure_storage_account_interface.py
+-rw-r--r--   0        0        0    10871 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/cos_interface.py
+-rw-r--r--   0        0        0     2000 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/file_system_interface.py
+-rw-r--r--   0        0        0    12754 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/gcs_interface.py
+-rw-r--r--   0        0        0     5963 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/hdfs_interface.py
+-rw-r--r--   0        0        0     3243 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/object_store_interface.py
+-rw-r--r--   0        0        0     5644 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/posix_file_interface.py
+-rw-r--r--   0        0        0     3322 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/r2_interface.py
+-rw-r--r--   0        0        0    11595 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/s3_interface.py
+-rw-r--r--   0        0        0     2569 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/storage_interface.py
+-rw-r--r--   0        0        0    23828 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/planner/planner.py
+-rw-r--r--   0        0        0    18157 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/planner/solver.py
+-rw-r--r--   0        0        0     6467 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/planner/solver_ilp.py
+-rw-r--r--   0        0        0     1996 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/planner/solver_ron.py
+-rw-r--r--   0        0        0     7920 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/planner/topology.py
+-rw-r--r--   0        0        0      846 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/cache.py
+-rw-r--r--   0        0        0      617 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/definitions.py
+-rw-r--r--   0        0        0     2494 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/fn.py
+-rw-r--r--   0        0        0     1881 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/generator.py
+-rw-r--r--   0        0        0     1386 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/imports.py
+-rw-r--r--   0        0        0     2131 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/logger.py
+-rw-r--r--   0        0        0     1897 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/networking_tools.py
+-rw-r--r--   0        0        0     3162 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/path.py
+-rw-r--r--   0        0        0     1160 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/retry.py
+-rw-r--r--   0        0        0      612 2023-08-07 23:44:12.811316 skyplane_nightly-0.3.2.dev20230807/skyplane/utils/timer.py
+-rw-r--r--   0        0        0    10740 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230807/PKG-INFO
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/LICENSE` & `skyplane_nightly-0.3.2.dev20230807/LICENSE`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/README.md` & `skyplane_nightly-0.3.2.dev20230807/README.md`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/pyproject.toml` & `skyplane_nightly-0.3.2.dev20230807/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "skyplane-nightly"
 packages = [{ include = "skyplane" }]
-version = "0.3.2.dev20230806"
+version = "0.3.2.dev20230807"
 description = "Skyplane efficiently transports data between cloud regions and providers."
 authors = ["Skyplane authors <skyplaneproject@gmail.com>"]
 license = "Apache-2.0"
 homepage = "https://skyplane.org/"
 repository = "https://github.com/skyplane-project/skyplane"
 documentation = "https://skyplane.org/"
 readme = "README.md"
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/__init__.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/__init__.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/client.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import uuid
 import typer
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 
 from skyplane.api.config import TransferConfig
-from skyplane.api.dataplane import Dataplane
 from skyplane.api.provisioner import Provisioner
 from skyplane.api.obj_store import ObjectStore
 from skyplane.api.usage import get_clientid
-from skyplane.obj_store.object_store_interface import ObjectStoreInterface
-from skyplane.planner.planner import MulticastDirectPlanner
 from skyplane.utils import logger
 from skyplane.utils.definitions import tmp_log_dir
-from skyplane.utils.path import parse_path
 
 from skyplane.api.pipeline import Pipeline
 
 if TYPE_CHECKING:
     from skyplane.api.config import AWSConfig, AzureConfig, GCPConfig, TransferConfig, IBMCloudConfig
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/config.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 
-from typing import Optional, List
+from typing import Optional
 
 from skyplane import compute
 
 from skyplane.config_paths import aws_quota_path, gcp_quota_path, azure_standardDv5_quota_path
 from pathlib import Path
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/dataplane.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/dataplane.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import os
 import threading
-from collections import defaultdict, Counter
+from collections import defaultdict
 from datetime import datetime
 from functools import partial
 from datetime import datetime
 
 import nacl.secret
 import nacl.utils
 import urllib3
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from skyplane import compute
 from skyplane.exceptions import GatewayContainerStartException
 from skyplane.api.tracker import TransferProgressTracker, TransferHook
-from skyplane.api.transfer_job import CopyJob, SyncJob, TransferJob
+from skyplane.api.transfer_job import TransferJob
 from skyplane.api.config import TransferConfig
 from skyplane.planner.topology import TopologyPlan, TopologyPlanGateway
 from skyplane.utils import logger
 from skyplane.utils.definitions import gateway_docker_image, tmp_log_dir
 from skyplane.utils.fn import PathLike, do_parallel
 
 if TYPE_CHECKING:
@@ -219,15 +219,15 @@
         for node, server in gateway_bound_nodes.items():
             jobs.append(
                 partial(self._start_gateway, gateway_docker_image, node, server, gateway_program_dir, authorize_ssh_pub_key, e2ee_key_bytes)
             )
         logger.fs.debug(f"[Dataplane.provision] Starting gateways on {len(jobs)} servers")
         try:
             do_parallel(lambda fn: fn(), jobs, n=-1, spinner=spinner, spinner_persist=spinner, desc="Starting gateway container on VMs")
-        except Exception as e:
+        except Exception:
             self.copy_gateway_logs()
             raise GatewayContainerStartException(f"Error starting gateways. Please check gateway logs {self.transfer_dir}")
 
     def copy_gateway_logs(self):
         # copy logs from all gateways in parallel
         def copy_log(instance):
             out_file = self.transfer_dir / f"gateway_{instance.uuid()}.stdout"
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/obj_store.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/obj_store.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/pipeline.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-import json
-import time
-import os
 import threading
-from collections import defaultdict, Counter
 from datetime import datetime
-from functools import partial
 from datetime import datetime
 
-import nacl.secret
-import nacl.utils
 import urllib3
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from skyplane import compute
-from skyplane.api.tracker import TransferProgressTracker, TransferHook
+from skyplane.api.tracker import TransferProgressTracker
 from skyplane.api.transfer_job import CopyJob, SyncJob, TransferJob
 from skyplane.api.config import TransferConfig
 
 from skyplane.planner.planner import MulticastDirectPlanner, DirectPlannerSourceOneSided, DirectPlannerDestOneSided
 from skyplane.planner.topology import TopologyPlanGateway
 from skyplane.utils import logger
-from skyplane.utils.definitions import gateway_docker_image, tmp_log_dir
-from skyplane.utils.fn import PathLike, do_parallel
+from skyplane.utils.definitions import tmp_log_dir
 
 from skyplane.api.dataplane import Dataplane
 
 if TYPE_CHECKING:
     from skyplane.api.provisioner import Provisioner
 
 
@@ -114,28 +106,28 @@
 
             # wait for job to finish
             tracker.join()
 
             # copy gateway logs
             if debug:
                 dp.copy_gateway_logs()
-        except Exception as e:
+        except Exception:
             dp.copy_gateway_logs()
         dp.deprovision(spinner=True)
         return dp
 
     def start_async(self, debug=False):
         dp = self.create_dataplane(debug)
         try:
             dp.provision(spinner=False)
             tracker = dp.run_async(self.jobs_to_dispatch)
             if debug:
                 dp.copy_gateway_logs()
             return tracker
-        except Exception as e:
+        except Exception:
             dp.copy_gateway_logs()
             return
 
     def queue_copy(
         self,
         src: str,
         dst: str or List[str],
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/provisioner.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/provisioner.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/tracker.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import functools
-from pprint import pprint
 import json
 import time
 from abc import ABC
 from datetime import datetime
 from threading import Thread
 
 import urllib3
@@ -217,30 +215,30 @@
             e2e_end_time = time.time()
             transfer_stats = {
                 "total_runtime_s": e2e_end_time - e2e_start_time,
                 "throughput_gbits": self.query_bytes_dispatched() / (e2e_end_time - e2e_start_time) / GB * 8,
             }
             self.hooks.on_transfer_end()
 
-            start_time = int(time.time())
+            int(time.time())
             try:
                 for job in self.jobs.values():
                     logger.fs.debug(f"[TransferProgressTracker] Finalizing job {job.uuid}")
                     job.finalize()
             except Exception as e:
                 UsageClient.log_exception(
                     "finalize job",
                     e,
                     args,
                     self.dataplane.topology.src_region_tag,
                     self.dataplane.topology.dest_region_tags[0],
                     session_start_timestamp_ms,
                 )
                 raise e
-            end_time = int(time.time())
+            int(time.time())
 
             # verify transfer
             try:
                 for job in self.jobs.values():
                     logger.fs.debug(f"[TransferProgressTracker] Verifying job {job.uuid}")
                     job.verify()
             except Exception as e:
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/transfer_job.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/transfer_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 import time
 import uuid
 from abc import ABC
 from collections import defaultdict
 from dataclasses import dataclass, field
 from queue import Queue
 
-from abc import ABC, abstractmethod
+from abc import ABC
 from typing import TYPE_CHECKING, Callable, Generator, List, Optional, Tuple, TypeVar, Dict
 
-from abc import ABC, abstractmethod
+from abc import ABC
 
 import urllib3
 from rich import print as rprint
 from functools import partial
 
 from skyplane import exceptions
 from skyplane.api.config import TransferConfig
-from skyplane.chunk import Chunk, ChunkRequest
+from skyplane.chunk import Chunk
 from skyplane.obj_store.storage_interface import StorageInterface
 from skyplane.obj_store.object_store_interface import ObjectStoreObject, ObjectStoreInterface
 from skyplane.utils import logger
 from skyplane.utils.definitions import MB
 from skyplane.utils.fn import do_parallel
 from skyplane.utils.path import parse_path
 from skyplane.utils.retry import retry_backoff
@@ -620,15 +620,15 @@
             chunker.prefetch_generator(chunks, buffer_size=dispatch_batch_size * 32), batch_size=dispatch_batch_size
         )
 
         # dispatch chunk requests
         src_gateways = dataplane.source_gateways()
         queue_size = [0] * len(src_gateways)
         n_multiparts = 0
-        start = time.time()
+        time.time()
 
         for batch in batches:
             # send upload_id mappings to sink gateways
             upload_id_batch = [cr for cr in batch if cr.upload_id_mapping is not None]
             region_dst_gateways = dataplane.sink_gateways()
             for region_tag, dst_gateways in region_dst_gateways.items():
                 for dst_gateway in dst_gateways:
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/api/usage.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/api/usage.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/chunk.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/chunk.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_cloud.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_cloud.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_config.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_init.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_init.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/cli_transfer.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/cli_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
     replicate_small_cp_cmd,
     replicate_small_sync_cmd,
 )
 from skyplane.cli.impl.common import print_header, console, print_stats_completed, register_exception_handler
 from skyplane.api.usage import UsageClient
 from skyplane.config import SkyplaneConfig
 from skyplane.config_paths import cloud_config, config_path
-from skyplane.obj_store.object_store_interface import ObjectStoreInterface, StorageInterface
-from skyplane.obj_store.file_system_interface import FileSystemInterface
+from skyplane.obj_store.object_store_interface import StorageInterface
 from skyplane.cli.impl.progress_bar import ProgressBarTransferHook
 from skyplane.utils import logger
 from skyplane.utils.definitions import GB, format_bytes
 from skyplane.utils.path import parse_path
 
 
 @dataclass
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/cli_profile.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/cli_profile.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/cli_query.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/cli_query.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/experiments/provision.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/experiments/provision.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/impl/common.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/impl/common.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/impl/cp_replicate_fallback.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/impl/cp_replicate_fallback.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/cli/impl/progress_bar.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/cli/impl/progress_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 from collections import defaultdict
 from rich.progress import Progress, SpinnerColumn, TextColumn, BarColumn, DownloadColumn, TransferSpeedColumn, TimeRemainingColumn
 from skyplane import exceptions
 from skyplane.chunk import Chunk
-from skyplane.cli.impl.common import console, print_stats_completed
+from skyplane.cli.impl.common import console
 from skyplane.utils.definitions import format_bytes
 from skyplane.api.tracker import TransferHook
 
 
 class ProgressBarTransferHook(TransferHook):
     """Transfer hook for multi-destination transfers."""
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/__init__.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_auth.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_key_manager.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_network.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_network.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_pricing.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/aws/aws_server.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/aws/aws_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/azure/azure_auth.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/azure/azure_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import os
 import subprocess
-import re
 
 from typing import Dict, List, Optional
 
 from skyplane.compute.const_cmds import query_which_cloud
 from skyplane.config import SkyplaneConfig
 from skyplane.config_paths import config_path, azure_config_path, azure_sku_path, azure_quota_path, azure_standardDv5_quota_path
 from skyplane.utils import imports, logger
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/azure/azure_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/azure/azure_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/azure/azure_server.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/azure/azure_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/const_cmds.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/const_cmds.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_auth.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_key_manager.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_network.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_network.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_pricing.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/gcp/gcp_server.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/gcp/gcp_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/config.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/constants.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/constants.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/utils.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/utils.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibmcloud_auth.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibmcloud_auth.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibmcloud_provider.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibmcloud_provider.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/ibmcloud/ibmcloud_server.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/ibmcloud/ibmcloud_server.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/key_utils.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/key_utils.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/compute/server.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/compute/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import json
 import logging
-from pprint import pprint
 import os
 import socket
 from contextlib import closing
 from enum import Enum, auto
 from functools import partial
 from pathlib import Path
 
 import urllib3
 from typing import Dict, Optional, Tuple
 
 from skyplane import compute
 from skyplane.compute.const_cmds import make_autoshutdown_script, make_dozzle_command, make_sysctl_tcp_tuning_command
 from skyplane.config_paths import config_path, cloud_config, __config_root__
-from skyplane.gateway.gateway_program import GatewayProgram
 from skyplane.utils import logger
 from skyplane.utils.fn import PathLike, wait_for
 from skyplane.utils.retry import retry_backoff
 from skyplane.utils.timer import Timer
-from skyplane.planner.topology import TopologyPlanGateway
 
 tmp_log_dir = Path("/tmp/skyplane")
 
 
 class ServerState(Enum):
     PENDING = auto()
     RUNNING = auto()
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/config.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/config.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/config_paths.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/config_paths.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/data/aws_transfer_costs.csv` & `skyplane_nightly-0.3.2.dev20230807/skyplane/data/aws_transfer_costs.csv`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/data/vcpu_info.csv` & `skyplane_nightly-0.3.2.dev20230807/skyplane/data/vcpu_info.csv`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/exceptions.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/cert.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/cert.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/chunk_store.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/chunk_store.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_daemon.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import os
 import signal
 import sys
 from multiprocessing import Event, Queue
 from os import PathLike
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Dict, List
 
 from skyplane.utils import logger
 
 from skyplane.gateway.gateway_queue import GatewayQueue, GatewayANDQueue
 from skyplane.gateway.chunk_store import ChunkStore
 from skyplane.gateway.gateway_daemon_api import GatewayDaemonAPI
 from skyplane.gateway.operators.gateway_operator import (
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_daemon_api.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_daemon_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import logging.handlers
 import os
 import threading
 from multiprocessing import Queue
 from multiprocessing.managers import DictProxy
 from queue import Empty
 from traceback import TracebackException
-from typing import Dict, List, Tuple, Optional
-import json
+from typing import Dict, List, Tuple
 from flask import Flask, jsonify, request
 from werkzeug.serving import make_server
 
 from skyplane.chunk import ChunkRequest, ChunkState
 from skyplane.gateway.chunk_store import ChunkStore
 from skyplane.gateway.operators.gateway_receiver import GatewayReceiver
 from skyplane.utils import logger
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_program.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_program.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, Tuple
+from typing import Optional, List
 import json
 from collections import defaultdict
 
 
 class GatewayOperator:
     def __init__(self, op_type):
         self.op_type = op_type
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/gateway_queue.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/gateway_queue.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/operators/gateway_operator.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/operators/gateway_operator.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/gateway/operators/gateway_receiver.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/gateway/operators/gateway_receiver.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/azure_blob_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/azure_blob_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Any, Iterator, List, Optional, Tuple
 
 from skyplane import exceptions, compute
 from skyplane.exceptions import NoSuchObjectException
 from skyplane.obj_store.azure_storage_account_interface import AzureStorageAccountInterface
 from skyplane.obj_store.object_store_interface import ObjectStoreInterface, ObjectStoreObject
 from skyplane.utils import logger, imports
-from azure.storage.blob import ContentSettings
 
 
 MAX_BLOCK_DIGITS = 5
 
 
 class AzureBlobObject(ObjectStoreObject):
     def full_path(self):
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/azure_storage_account_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/azure_storage_account_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/cos_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/cos_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/file_system_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/file_system_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass
 from typing import Any, Iterator, List, Optional
 from skyplane.obj_store.storage_interface import StorageInterface
-import os
 
 
 @dataclass
 class LocalFile:
     """Defines file on local node."""
 
     path: str
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/gcs_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/gcs_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/hdfs_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/hdfs_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/object_store_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/object_store_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass
 
-from typing import Any, Iterator, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple
 
 from skyplane.obj_store.storage_interface import StorageInterface
-from skyplane.utils import logger
 
 
 @dataclass
 class ObjectStoreObject:
     """Defines object in object store."""
 
     key: str
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/posix_file_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/posix_file_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/r2_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/r2_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-import base64
-import hashlib
 import os
 import boto3
-from functools import lru_cache
 
-from typing import Iterator, List, Optional, Tuple
+from typing import Iterator
 
-from skyplane import exceptions, compute
-from skyplane.exceptions import NoSuchObjectException
 from skyplane.obj_store.s3_interface import S3Object, S3Interface
-from skyplane.config_paths import cloud_config
 from skyplane.utils import logger, imports
-from skyplane.utils.generator import batch_generator
 
 from skyplane.config_paths import config_path
 from skyplane.config import SkyplaneConfig
 
 
 class R2Object(S3Object):
     def full_path(self):
@@ -31,15 +24,15 @@
             self.s3_client = boto3.client(
                 "s3",
                 endpoint_url=self.endpoint_url,
                 aws_access_key_id=self.config.cloudflare_access_key_id,
                 aws_secret_access_key=self.config.cloudflare_secret_access_key,
                 region_name="auto",  # explicity set region, otherwise may be read from AWS boto3 env
             )
-        except Exception as e:
+        except Exception:
             raise ValueError("Error with connecting to {self.endpoint_url}: {e}")
         self.requester_pays = False
         self.bucket_name = bucket_name
         self.account_id = account_id
 
     @property
     def provider(self):
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/s3_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/s3_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/obj_store/storage_interface.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/obj_store/storage_interface.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/planner/planner.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/planner/planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
             mux_and = src_program.add_operator(GatewayMuxAnd(), parent_handle=obj_store_read, partition_id=partition_id)
             dst_prefixes = job.dst_prefixes
             for i in range(len(job.dst_ifaces)):
                 dst_iface = job.dst_ifaces[i]
                 dst_prefix = dst_prefixes[i]
                 dst_region_tag = dst_iface.region_tag()
                 dst_bucket = dst_iface.bucket()
-                dst_gateways = plan.get_region_gateways(dst_region_tag)
+                plan.get_region_gateways(dst_region_tag)
 
                 # special case where destination is same region as source
                 src_program.add_operator(
                     GatewayWriteObjectStore(dst_bucket, dst_region_tag, self.n_connections, key_prefix=dst_prefix),
                     parent_handle=mux_and,
                     partition_id=partition_id,
                 )
@@ -472,15 +472,15 @@
             # send to all destination
             dst_prefixes = job.dst_prefixes
             for i in range(len(job.dst_ifaces)):
                 dst_iface = job.dst_ifaces[i]
                 dst_prefix = dst_prefixes[i]
                 dst_region_tag = dst_iface.region_tag()
                 dst_bucket = dst_iface.bucket()
-                dst_gateways = plan.get_region_gateways(dst_region_tag)
+                plan.get_region_gateways(dst_region_tag)
 
                 # source region gateway program
                 obj_store_read = dst_program[dst_region_tag].add_operator(
                     GatewayReadObjectStore(src_bucket, src_region_tag, self.n_connections), partition_id=partition_id
                 )
 
                 dst_program[dst_region_tag].add_operator(
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/planner/solver.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/planner/solver.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/planner/solver_ilp.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/planner/solver_ilp.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/planner/solver_ron.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/planner/solver_ron.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/planner/topology.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/planner/topology.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/cache.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/cache.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/definitions.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/fn.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/fn.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/generator.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/generator.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/imports.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/imports.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/logger.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/logger.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/networking_tools.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/networking_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,23 @@
     try:
         if provider == "aws":
             region = requests.get(f"https://ip-ranges.amazonaws.com/ip-ranges.json").json()
             for prefix in region["prefixes"]:
                 if re.match(prefix["ip_prefix"], ip):
                     return prefix["region"]
         elif provider == "azure":
-            region = requests.get(f"https://www.microsoft.com/en-us/download/confirmation.aspx?id=56519").json()
+            user_agent = {
+                "User-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95"
+            }
+            body = requests.get(f"https://www.microsoft.com/en-us/download/confirmation.aspx?id=56519", headers=user_agent).content
+            matches = re.search(b'downloadretry" href="([^"]*)"', body)
+            if matches is None:
+                return default_region[provider]
+            region_url = matches.groups(0)[0]
+            region = requests.get(region_url).json()
             for prefix in region["values"]:
                 if re.match(prefix["properties"]["addressPrefix"], ip):
                     return prefix["properties"]["region"]
         elif provider == "gcp":
             region = requests.get(f"https://www.gstatic.com/ipranges/cloud.json").json()
             for prefix in region["prefixes"]:
                 if re.match(prefix["ipv4Prefix"], ip):
```

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/path.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/path.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/retry.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/retry.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/skyplane/utils/timer.py` & `skyplane_nightly-0.3.2.dev20230807/skyplane/utils/timer.py`

 * *Files identical despite different names*

### Comparing `skyplane_nightly-0.3.2.dev20230806/PKG-INFO` & `skyplane_nightly-0.3.2.dev20230807/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyplane-nightly
-Version: 0.3.2.dev20230806
+Version: 0.3.2.dev20230807
 Summary: Skyplane efficiently transports data between cloud regions and providers.
 Home-page: https://skyplane.org/
 License: Apache-2.0
 Author: Skyplane authors
 Author-email: skyplaneproject@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skyplane-nightly Version: 0.3.2.dev20230806
+Metadata-Version: 2.1 Name: skyplane-nightly Version: 0.3.2.dev20230807
 Summary: Skyplane efficiently transports data between cloud regions and
 providers. Home-page: https://skyplane.org/ License: Apache-2.0 Author:
 Skyplane authors Author-email: skyplaneproject@gmail.com Requires-Python:
 >=3.7.1,<3.12 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```


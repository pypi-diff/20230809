# Comparing `tmp/iam_actions-1.2.20230808.tar.gz` & `tmp/iam_actions-1.2.20230809.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230808.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230809.tar", max compression
```

## Comparing `iam_actions-1.2.20230808.tar` & `iam_actions-1.2.20230809.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/LICENSE
--rw-r--r--   0        0        0     2302 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/README.md
--rw-r--r--   0        0        0      228 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/__init__.py
--rw-r--r--   0        0        0  4390273 2023-08-08 02:24:50.409444 iam_actions-1.2.20230808/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-08-08 02:23:30.205008 iam_actions-1.2.20230808/iam_actions/generate/services.py
--rw-r--r--   0        0        0   566449 2023-08-08 02:24:50.409444 iam_actions-1.2.20230808/iam_actions/policies.json
--rw-r--r--   0        0        0   196077 2023-08-08 02:24:50.409444 iam_actions-1.2.20230808/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   549468 2023-08-08 02:24:50.409444 iam_actions-1.2.20230808/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-08-08 02:24:51.365449 iam_actions-1.2.20230808/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230808/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230808/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/LICENSE
+-rw-r--r--   0        0        0     2302 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/README.md
+-rw-r--r--   0        0        0      228 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4391496 2023-08-09 02:25:05.641452 iam_actions-1.2.20230809/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-08-09 02:23:26.984684 iam_actions-1.2.20230809/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   566705 2023-08-09 02:25:05.641452 iam_actions-1.2.20230809/iam_actions/policies.json
+-rw-r--r--   0        0        0   196077 2023-08-09 02:25:05.641452 iam_actions-1.2.20230809/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   549717 2023-08-09 02:25:05.641452 iam_actions-1.2.20230809/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-08-09 02:25:06.413457 iam_actions-1.2.20230809/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230809/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230809/PKG-INFO
```

### Comparing `iam_actions-1.2.20230808/LICENSE` & `iam_actions-1.2.20230809/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/README.md` & `iam_actions-1.2.20230809/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/actions.json` & `iam_actions-1.2.20230809/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999891065659527%*

 * *Differences: {"'artifact'": "{'PutAccountSettings': {'access_level': 'Write', 'description': 'Grants permission "*

 * *               "to put account settings for Artifact'}, 'GetAccountSettings': {'access_level': "*

 * *               "'Read', 'description': 'Grants permission to get the account settings for "*

 * *               "Artifact'}}",*

 * * "'backup'": "{'PutBackupVaultSharingPolicy': OrderedDict([('access_level', 'Undocumented'), "*

 * *             "('action', 'PutBackupVaultSharingPolicy'), ('condition_keys', []), ('description',  […]*

```diff
@@ -8420,18 +8420,18 @@
             "description": "Grants permission to download an AWS compliance report package",
             "orphan": false,
             "resources": [
                 "report-package"
             ]
         },
         "GetAccountSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAccountSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the account settings for Artifact",
             "orphan": false,
             "resources": []
         },
         "GetReport": {
             "access_level": "Read",
             "action": "GetReport",
             "condition_keys": [],
@@ -8466,18 +8466,18 @@
             "action": "ListReports",
             "condition_keys": [],
             "description": "Grants permission to list reports in your account",
             "orphan": false,
             "resources": []
         },
         "PutAccountSettings": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutAccountSettings",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to put account settings for Artifact",
             "orphan": false,
             "resources": []
         },
         "TerminateAgreement": {
             "access_level": "Write",
             "action": "TerminateAgreement",
             "condition_keys": [],
@@ -11334,14 +11334,22 @@
             ],
             "description": "Grants permission to create a new legal hold",
             "orphan": false,
             "resources": [
                 "legalHold"
             ]
         },
+        "CreateLogicallyAirGappedBackupVault": {
+            "access_level": "Undocumented",
+            "action": "CreateLogicallyAirGappedBackupVault",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateReportPlan": {
             "access_level": "Write",
             "action": "CreateReportPlan",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "backup:FrameworkArns"
@@ -11408,14 +11416,22 @@
             "condition_keys": [],
             "description": "Grants permission to remove the notifications from a backup vault",
             "orphan": false,
             "resources": [
                 "backupVault"
             ]
         },
+        "DeleteBackupVaultSharingPolicy": {
+            "access_level": "Undocumented",
+            "action": "DeleteBackupVaultSharingPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteFramework": {
             "access_level": "Write",
             "action": "DeleteFramework",
             "condition_keys": [],
             "description": "Grants permission to delete a framework",
             "orphan": false,
             "resources": [
@@ -11618,14 +11634,22 @@
             "condition_keys": [],
             "description": "Grants permission to get backup vault notifications",
             "orphan": false,
             "resources": [
                 "backupVault"
             ]
         },
+        "GetBackupVaultSharingPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetBackupVaultSharingPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetLegalHold": {
             "access_level": "Read",
             "action": "GetLegalHold",
             "condition_keys": [],
             "description": "Grants permission to get a legal hold",
             "orphan": false,
             "resources": [
@@ -11730,14 +11754,22 @@
             "access_level": "List",
             "action": "ListProtectedResources",
             "condition_keys": [],
             "description": "Grants permission to list protected resources by AWS Backup",
             "orphan": false,
             "resources": []
         },
+        "ListProtectedResourcesByBackupVault": {
+            "access_level": "Undocumented",
+            "action": "ListProtectedResourcesByBackupVault",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListRecoveryPointsByBackupVault": {
             "access_level": "List",
             "action": "ListRecoveryPointsByBackupVault",
             "condition_keys": [],
             "description": "Grants permission to list recovery points inside a backup vault",
             "orphan": false,
             "resources": [
@@ -11829,14 +11861,22 @@
             "condition_keys": [],
             "description": "Grants permission to add an SNS topic to the backup vault",
             "orphan": false,
             "resources": [
                 "backupVault"
             ]
         },
+        "PutBackupVaultSharingPolicy": {
+            "access_level": "Undocumented",
+            "action": "PutBackupVaultSharingPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartBackupJob": {
             "access_level": "Write",
             "action": "StartBackupJob",
             "condition_keys": [],
             "description": "Grants permission to start a new backup job",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230808/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230809/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230809/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/generate/generate.py` & `iam_actions-1.2.20230809/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230809/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230809/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/generate/services.py` & `iam_actions-1.2.20230809/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/policies.json` & `iam_actions-1.2.20230809/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999969019817548%*

 * *Differences: {"'serviceMap'": "{'AWS Backup': {'Actions': {insert: [(8, 'CreateLogicallyAirGappedBackupVault'), "*

 * *                 "(16, 'DeleteBackupVaultSharingPolicy'), (40, 'GetBackupVaultSharingPolicy'), "*

 * *                 "(54, 'ListProtectedResourcesByBackupVault'), (65, "*

 * *                 "'PutBackupVaultSharingPolicy')]}, 'conditionKeys': {insert: [(7, "*

 * *                 "'backup:MaxRetentionDays'), (8, 'backup:MinRetentionDays')]}}}"}*

```diff
@@ -961,21 +961,23 @@
                 "CopyFromBackupVault",
                 "CopyIntoBackupVault",
                 "CreateBackupPlan",
                 "CreateBackupSelection",
                 "CreateBackupVault",
                 "CreateFramework",
                 "CreateLegalHold",
+                "CreateLogicallyAirGappedBackupVault",
                 "CreateReportPlan",
                 "DeleteBackupPlan",
                 "DeleteBackupSelection",
                 "DeleteBackupVault",
                 "DeleteBackupVaultAccessPolicy",
                 "DeleteBackupVaultLockConfiguration",
                 "DeleteBackupVaultNotifications",
+                "DeleteBackupVaultSharingPolicy",
                 "DeleteFramework",
                 "DeleteRecoveryPoint",
                 "DeleteReportPlan",
                 "DescribeBackupJob",
                 "DescribeBackupVault",
                 "DescribeCopyJob",
                 "DescribeFramework",
@@ -991,37 +993,40 @@
                 "ExportBackupPlanTemplate",
                 "GetBackupPlan",
                 "GetBackupPlanFromJSON",
                 "GetBackupPlanFromTemplate",
                 "GetBackupSelection",
                 "GetBackupVaultAccessPolicy",
                 "GetBackupVaultNotifications",
+                "GetBackupVaultSharingPolicy",
                 "GetLegalHold",
                 "GetRecoveryPointRestoreMetadata",
                 "GetSupportedResourceTypes",
                 "ListBackupJobs",
                 "ListBackupPlanTemplates",
                 "ListBackupPlanVersions",
                 "ListBackupPlans",
                 "ListBackupSelections",
                 "ListBackupVaults",
                 "ListCopyJobs",
                 "ListFrameworks",
                 "ListLegalHolds",
                 "ListProtectedResources",
+                "ListProtectedResourcesByBackupVault",
                 "ListRecoveryPointsByBackupVault",
                 "ListRecoveryPointsByLegalHold",
                 "ListRecoveryPointsByResource",
                 "ListReportJobs",
                 "ListReportPlans",
                 "ListRestoreJobs",
                 "ListTags",
                 "PutBackupVaultAccessPolicy",
                 "PutBackupVaultLockConfiguration",
                 "PutBackupVaultNotifications",
+                "PutBackupVaultSharingPolicy",
                 "StartBackupJob",
                 "StartCopyJob",
                 "StartReportJob",
                 "StartRestoreJob",
                 "StopBackupJob",
                 "TagResource",
                 "UntagResource",
@@ -1037,15 +1042,17 @@
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "backup:ChangeableForDays",
                 "backup:CopyTargetOrgPaths",
                 "backup:CopyTargets",
-                "backup:FrameworkArns"
+                "backup:FrameworkArns",
+                "backup:MaxRetentionDays",
+                "backup:MinRetentionDays"
             ]
         },
         "AWS Backup Gateway": {
             "ARNFormat": "arn:aws:backup-gateway:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:*:backup-gateway:.+:.+:.+",
             "Actions": [
                 "AssociateGatewayToServer",
```

### Comparing `iam_actions-1.2.20230808/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230809/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230808/iam_actions/services.json` & `iam_actions-1.2.20230809/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999675847682263%*

 * *Differences: {"'backup'": "{'Actions': {insert: [(8, 'CreateLogicallyAirGappedBackupVault'), (16, "*

 * *             "'DeleteBackupVaultSharingPolicy'), (40, 'GetBackupVaultSharingPolicy'), (54, "*

 * *             "'ListProtectedResourcesByBackupVault'), (65, 'PutBackupVaultSharingPolicy')]}, "*

 * *             "'ConditionKeys': {insert: [(7, 'backup:MaxRetentionDays'), (8, "*

 * *             "'backup:MinRetentionDays')]}}"}*

```diff
@@ -1819,21 +1819,23 @@
             "CopyFromBackupVault",
             "CopyIntoBackupVault",
             "CreateBackupPlan",
             "CreateBackupSelection",
             "CreateBackupVault",
             "CreateFramework",
             "CreateLegalHold",
+            "CreateLogicallyAirGappedBackupVault",
             "CreateReportPlan",
             "DeleteBackupPlan",
             "DeleteBackupSelection",
             "DeleteBackupVault",
             "DeleteBackupVaultAccessPolicy",
             "DeleteBackupVaultLockConfiguration",
             "DeleteBackupVaultNotifications",
+            "DeleteBackupVaultSharingPolicy",
             "DeleteFramework",
             "DeleteRecoveryPoint",
             "DeleteReportPlan",
             "DescribeBackupJob",
             "DescribeBackupVault",
             "DescribeCopyJob",
             "DescribeFramework",
@@ -1849,37 +1851,40 @@
             "ExportBackupPlanTemplate",
             "GetBackupPlan",
             "GetBackupPlanFromJSON",
             "GetBackupPlanFromTemplate",
             "GetBackupSelection",
             "GetBackupVaultAccessPolicy",
             "GetBackupVaultNotifications",
+            "GetBackupVaultSharingPolicy",
             "GetLegalHold",
             "GetRecoveryPointRestoreMetadata",
             "GetSupportedResourceTypes",
             "ListBackupJobs",
             "ListBackupPlanTemplates",
             "ListBackupPlanVersions",
             "ListBackupPlans",
             "ListBackupSelections",
             "ListBackupVaults",
             "ListCopyJobs",
             "ListFrameworks",
             "ListLegalHolds",
             "ListProtectedResources",
+            "ListProtectedResourcesByBackupVault",
             "ListRecoveryPointsByBackupVault",
             "ListRecoveryPointsByLegalHold",
             "ListRecoveryPointsByResource",
             "ListReportJobs",
             "ListReportPlans",
             "ListRestoreJobs",
             "ListTags",
             "PutBackupVaultAccessPolicy",
             "PutBackupVaultLockConfiguration",
             "PutBackupVaultNotifications",
+            "PutBackupVaultSharingPolicy",
             "StartBackupJob",
             "StartCopyJob",
             "StartReportJob",
             "StartRestoreJob",
             "StopBackupJob",
             "TagResource",
             "UntagResource",
@@ -1893,15 +1898,17 @@
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "backup:ChangeableForDays",
             "backup:CopyTargetOrgPaths",
             "backup:CopyTargets",
-            "backup:FrameworkArns"
+            "backup:FrameworkArns",
+            "backup:MaxRetentionDays",
+            "backup:MinRetentionDays"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Backup"
         ]
     },
     "backup-gateway": {
```

### Comparing `iam_actions-1.2.20230808/pyproject.toml` & `iam_actions-1.2.20230809/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230808"
+version = "1.2.20230809"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230808/setup.py` & `iam_actions-1.2.20230809/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230808',
+    'version': '1.2.20230809',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230808/PKG-INFO` & `iam_actions-1.2.20230809/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230808
+Version: 1.2.20230809
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


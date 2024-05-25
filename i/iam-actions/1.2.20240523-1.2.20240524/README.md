# Comparing `tmp/iam_actions-1.2.20240523.tar.gz` & `tmp/iam_actions-1.2.20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240523.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240524.tar", max compression
```

## Comparing `iam_actions-1.2.20240523.tar` & `iam_actions-1.2.20240524.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/README.md
--rw-r--r--   0        0        0      228 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/__init__.py
--rw-r--r--   0        0        0  4847772 2024-05-23 02:24:06.736391 iam_actions-1.2.20240523/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-23 02:22:22.212231 iam_actions-1.2.20240523/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-23 02:22:22.216231 iam_actions-1.2.20240523/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-23 02:22:22.216231 iam_actions-1.2.20240523/iam_actions/generate/services.py
--rw-r--r--   0        0        0   631317 2024-05-23 02:24:06.736391 iam_actions-1.2.20240523/iam_actions/policies.json
--rw-r--r--   0        0        0   209717 2024-05-23 02:24:06.736391 iam_actions-1.2.20240523/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   612218 2024-05-23 02:24:06.736391 iam_actions-1.2.20240523/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-23 02:24:07.428392 iam_actions-1.2.20240523/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240523/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240523/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/README.md
+-rw-r--r--   0        0        0      228 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4849776 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   631731 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/policies.json
+-rw-r--r--   0        0        0   209748 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   612689 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-24 02:24:50.664909 iam_actions-1.2.20240524/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240524/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240524/PKG-INFO
```

### Comparing `iam_actions-1.2.20240523/LICENSE` & `iam_actions-1.2.20240524/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/README.md` & `iam_actions-1.2.20240524/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/actions.json` & `iam_actions-1.2.20240524/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972654337986097%*

 * *Differences: {"'chatbot'": "{'ListTagsForResource': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'ListTagsForResource'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *              "AWS'), ('orphan', False), ('resources', [])]), 'UntagResource': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', 'UntagResource'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), ('resources', [])]), ' […]*

```diff
@@ -16902,14 +16902,22 @@
             "access_level": "Read",
             "action": "ListMicrosoftTeamsUserIdentities",
             "condition_keys": [],
             "description": "Grants permission to describe AWS Chatbot Microsoft Teams User Identities",
             "orphan": false,
             "resources": []
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RedeemMicrosoftTeamsOauthCode": {
             "access_level": "Write",
             "action": "RedeemMicrosoftTeamsOauthCode",
             "condition_keys": [],
             "description": "Grants permission to redeem previously generated parameters with Microsoft APIs, to acquire OAuth tokens to be used by the AWS Chatbot service",
             "orphan": false,
             "resources": []
@@ -16918,14 +16926,30 @@
             "access_level": "Write",
             "action": "RedeemSlackOauthCode",
             "condition_keys": [],
             "description": "Grants permission to redeem previously generated parameters with Slack API, to acquire OAuth tokens to be used by the AWS Chatbot service",
             "orphan": false,
             "resources": []
         },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateAccountPreferences": {
             "access_level": "Write",
             "action": "UpdateAccountPreferences",
             "condition_keys": [],
             "description": "Grants permission to update AWS Chatbot account preferences",
             "orphan": false,
             "resources": []
@@ -56164,14 +56188,22 @@
             ],
             "description": "Grants permission to cancel the deprecation of the specified AMI",
             "orphan": false,
             "resources": [
                 "image"
             ]
         },
+        "DisableImageDeregistrationProtection": {
+            "access_level": "Undocumented",
+            "action": "DisableImageDeregistrationProtection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DisableIpamOrganizationAdminAccount": {
             "access_level": "Write",
             "action": "DisableIpamOrganizationAdminAccount",
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to disable an AWS Organizations member account as an Amazon VPC IP Address Manager (IPAM) admin account",
@@ -56671,14 +56703,22 @@
             ],
             "description": "Grants permission to enable deprecation of the specified AMI at the specified date and time",
             "orphan": false,
             "resources": [
                 "image"
             ]
         },
+        "EnableImageDeregistrationProtection": {
+            "access_level": "Undocumented",
+            "action": "EnableImageDeregistrationProtection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "EnableIpamOrganizationAdminAccount": {
             "access_level": "Write",
             "action": "EnableIpamOrganizationAdminAccount",
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to enable an AWS Organizations member account as an Amazon VPC IP Address Manager (IPAM) admin account",
@@ -57082,14 +57122,22 @@
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to view the default instance metadata service (IMDS) settings set for your account in the specified Region",
             "orphan": false,
             "resources": []
         },
+        "GetInstanceTpmEkPub": {
+            "access_level": "Undocumented",
+            "action": "GetInstanceTpmEkPub",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetInstanceTypesFromInstanceRequirements": {
             "access_level": "List",
             "action": "GetInstanceTypesFromInstanceRequirements",
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to view a list of instance types with specified instance attributes",
@@ -66976,14 +67024,22 @@
             "condition_keys": [],
             "description": "Grants permission to execute interactive workloads on an application",
             "orphan": false,
             "resources": [
                 "application"
             ]
         },
+        "AccessLivyEndpoints": {
+            "access_level": "Undocumented",
+            "action": "AccessLivyEndpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CancelJobRun": {
             "access_level": "Write",
             "action": "CancelJobRun",
             "condition_keys": [],
             "description": "Grants permission to cancel a job run",
             "orphan": false,
             "resources": [
@@ -161321,14 +161377,32 @@
             "action": "StartSupportPlanUpdate",
             "condition_keys": [],
             "description": "Grants permission to update the support plan for this AWS account",
             "orphan": false,
             "resources": []
         }
     },
+    "supportrecommendations": {
+        "GetSupportTroubleshootingResponse": {
+            "access_level": "Undocumented",
+            "action": "GetSupportTroubleshootingResponse",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartSupportTroubleshooting": {
+            "access_level": "Undocumented",
+            "action": "StartSupportTroubleshooting",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "sustainability": {
         "GetCarbonFootprintSummary": {
             "access_level": "Read",
             "action": "GetCarbonFootprintSummary",
             "condition_keys": [],
             "description": "Grants permission to view the carbon footprint tool",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20240523/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240524/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240524/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/generate/generate.py` & `iam_actions-1.2.20240524/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240524/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240524/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/generate/services.py` & `iam_actions-1.2.20240524/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240523/iam_actions/policies.json` & `iam_actions-1.2.20240524/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997566459124616%*

 * *Differences: {"'serviceMap'": "{'Amazon EMR Serverless': {'Actions': {insert: [(1, 'AccessLivyEndpoints')]}}, "*

 * *                 "'Amazon EC2': {'Actions': {insert: [(391, "*

 * *                 "'DisableImageDeregistrationProtection'), (423, "*

 * *                 "'EnableImageDeregistrationProtection'), (452, 'GetInstanceTpmEkPub')]}}, 'AWS "*

 * *                 "Chatbot': {'Actions': {insert: [(22, 'ListTagsForResource'), (25, "*

 * *                 "'TagResource'), (26, 'UntagResource')]}}, 'AWS Support Recommendations': "*

 * *        […]*

```diff
@@ -1495,16 +1495,19 @@
                 "GetAccountPreferences",
                 "GetMicrosoftTeamsChannelConfiguration",
                 "GetMicrosoftTeamsOauthParameters",
                 "GetSlackOauthParameters",
                 "ListMicrosoftTeamsChannelConfigurations",
                 "ListMicrosoftTeamsConfiguredTeams",
                 "ListMicrosoftTeamsUserIdentities",
+                "ListTagsForResource",
                 "RedeemMicrosoftTeamsOauthCode",
                 "RedeemSlackOauthCode",
+                "TagResource",
+                "UntagResource",
                 "UpdateAccountPreferences",
                 "UpdateChimeWebhookConfiguration",
                 "UpdateMicrosoftTeamsChannelConfiguration",
                 "UpdateSlackChannelConfiguration"
             ],
             "HasResource": true,
             "StringPrefix": "chatbot"
@@ -9917,14 +9920,22 @@
                 "GetSupportPlan",
                 "GetSupportPlanUpdateStatus",
                 "StartSupportPlanUpdate"
             ],
             "HasResource": false,
             "StringPrefix": "supportplans"
         },
+        "AWS Support Recommendations": {
+            "Actions": [
+                "GetSupportTroubleshootingResponse",
+                "StartSupportTroubleshooting"
+            ],
+            "HasResource": false,
+            "StringPrefix": "supportrecommendations"
+        },
         "AWS Sustainability": {
             "ARNFormat": "arn:${Partition}:sustainability:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:${Partition}:sustainability:.+:.+:.+",
             "Actions": [
                 "GetCarbonFootprintSummary"
             ],
             "HasResource": false,
@@ -14314,14 +14325,15 @@
                 "DisableAwsNetworkPerformanceMetricSubscription",
                 "DisableEbsEncryptionByDefault",
                 "DisableFastLaunch",
                 "DisableFastSnapshotRestores",
                 "DisableImage",
                 "DisableImageBlockPublicAccess",
                 "DisableImageDeprecation",
+                "DisableImageDeregistrationProtection",
                 "DisableIpamOrganizationAdminAccount",
                 "DisableSerialConsoleAccess",
                 "DisableSnapshotBlockPublicAccess",
                 "DisableTransitGatewayRouteTablePropagation",
                 "DisableVgwRoutePropagation",
                 "DisableVpcClassicLink",
                 "DisableVpcClassicLinkDnsSupport",
@@ -14345,14 +14357,15 @@
                 "EnableAwsNetworkPerformanceMetricSubscription",
                 "EnableEbsEncryptionByDefault",
                 "EnableFastLaunch",
                 "EnableFastSnapshotRestores",
                 "EnableImage",
                 "EnableImageBlockPublicAccess",
                 "EnableImageDeprecation",
+                "EnableImageDeregistrationProtection",
                 "EnableIpamOrganizationAdminAccount",
                 "EnableReachabilityAnalyzerOrganizationSharing",
                 "EnableSerialConsoleAccess",
                 "EnableSnapshotBlockPublicAccess",
                 "EnableTransitGatewayRouteTablePropagation",
                 "EnableVgwRoutePropagation",
                 "EnableVolumeIO",
@@ -14373,14 +14386,15 @@
                 "GetEbsDefaultKmsKeyId",
                 "GetEbsEncryptionByDefault",
                 "GetFlowLogsIntegrationTemplate",
                 "GetGroupsForCapacityReservation",
                 "GetHostReservationPurchasePreview",
                 "GetImageBlockPublicAccessState",
                 "GetInstanceMetadataDefaults",
+                "GetInstanceTpmEkPub",
                 "GetInstanceTypesFromInstanceRequirements",
                 "GetInstanceUefiData",
                 "GetIpamAddressHistory",
                 "GetIpamDiscoveredAccounts",
                 "GetIpamDiscoveredPublicAddresses",
                 "GetIpamDiscoveredResourceCidrs",
                 "GetIpamPoolAllocations",
@@ -14903,14 +14917,15 @@
             ]
         },
         "Amazon EMR Serverless": {
             "ARNFormat": "arn:aws:emr-serverless:${Region}:${Account}:/${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:emr-serverless:.+",
             "Actions": [
                 "AccessInteractiveEndpoints",
+                "AccessLivyEndpoints",
                 "CancelJobRun",
                 "CreateApplication",
                 "DeleteApplication",
                 "GetApplication",
                 "GetDashboardForJobRun",
                 "GetJobRun",
                 "ListApplications",
```

### Comparing `iam_actions-1.2.20240523/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240524/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974683544303797%*

 * *Differences: {"'supportrecommendations'": 'OrderedDict()'}*

```diff
@@ -6584,14 +6584,15 @@
             "arn_pattern": "arn:*:iam::*:user/*",
             "condition_keys": null
         }
     },
     "support": {},
     "supportapp": {},
     "supportplans": {},
+    "supportrecommendations": {},
     "sustainability": {},
     "swf": {
         "domain": {
             "arn_pattern": "arn:*:swf::*:/domain/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
```

### Comparing `iam_actions-1.2.20240523/iam_actions/services.json` & `iam_actions-1.2.20240524/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974514443777323%*

 * *Differences: {"'chatbot'": "{'Actions': {insert: [(22, 'ListTagsForResource'), (25, 'TagResource'), (26, "*

 * *              "'UntagResource')]}}",*

 * * "'ec2'": "{'Actions': {insert: [(391, 'DisableImageDeregistrationProtection'), (423, "*

 * *          "'EnableImageDeregistrationProtection'), (452, 'GetInstanceTpmEkPub')]}}",*

 * * "'emr-serverless'": "{'Actions': {insert: [(1, 'AccessLivyEndpoints')]}}",*

 * * "'supportrecommendations'": "OrderedDict([('Actions', ['GetSupportTroubleshootingResponse', "*

 * *                             "'StartS […]*

```diff
@@ -2719,16 +2719,19 @@
             "GetAccountPreferences",
             "GetMicrosoftTeamsChannelConfiguration",
             "GetMicrosoftTeamsOauthParameters",
             "GetSlackOauthParameters",
             "ListMicrosoftTeamsChannelConfigurations",
             "ListMicrosoftTeamsConfiguredTeams",
             "ListMicrosoftTeamsUserIdentities",
+            "ListTagsForResource",
             "RedeemMicrosoftTeamsOauthCode",
             "RedeemSlackOauthCode",
+            "TagResource",
+            "UntagResource",
             "UpdateAccountPreferences",
             "UpdateChimeWebhookConfiguration",
             "UpdateMicrosoftTeamsChannelConfiguration",
             "UpdateSlackChannelConfiguration"
         ],
         "ConditionKeys": [],
         "HasResource": true,
@@ -7755,14 +7758,15 @@
             "DisableAwsNetworkPerformanceMetricSubscription",
             "DisableEbsEncryptionByDefault",
             "DisableFastLaunch",
             "DisableFastSnapshotRestores",
             "DisableImage",
             "DisableImageBlockPublicAccess",
             "DisableImageDeprecation",
+            "DisableImageDeregistrationProtection",
             "DisableIpamOrganizationAdminAccount",
             "DisableSerialConsoleAccess",
             "DisableSnapshotBlockPublicAccess",
             "DisableTransitGatewayRouteTablePropagation",
             "DisableVgwRoutePropagation",
             "DisableVpcClassicLink",
             "DisableVpcClassicLinkDnsSupport",
@@ -7786,14 +7790,15 @@
             "EnableAwsNetworkPerformanceMetricSubscription",
             "EnableEbsEncryptionByDefault",
             "EnableFastLaunch",
             "EnableFastSnapshotRestores",
             "EnableImage",
             "EnableImageBlockPublicAccess",
             "EnableImageDeprecation",
+            "EnableImageDeregistrationProtection",
             "EnableIpamOrganizationAdminAccount",
             "EnableReachabilityAnalyzerOrganizationSharing",
             "EnableSerialConsoleAccess",
             "EnableSnapshotBlockPublicAccess",
             "EnableTransitGatewayRouteTablePropagation",
             "EnableVgwRoutePropagation",
             "EnableVolumeIO",
@@ -7814,14 +7819,15 @@
             "GetEbsDefaultKmsKeyId",
             "GetEbsEncryptionByDefault",
             "GetFlowLogsIntegrationTemplate",
             "GetGroupsForCapacityReservation",
             "GetHostReservationPurchasePreview",
             "GetImageBlockPublicAccessState",
             "GetInstanceMetadataDefaults",
+            "GetInstanceTpmEkPub",
             "GetInstanceTypesFromInstanceRequirements",
             "GetInstanceUefiData",
             "GetIpamAddressHistory",
             "GetIpamDiscoveredAccounts",
             "GetIpamDiscoveredPublicAddresses",
             "GetIpamDiscoveredResourceCidrs",
             "GetIpamPoolAllocations",
@@ -9131,14 +9137,15 @@
             "arn:aws:emr-serverless:${Region}:${Account}:/${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
             "^arn:aws:emr-serverless:.+"
         ],
         "Actions": [
             "AccessInteractiveEndpoints",
+            "AccessLivyEndpoints",
             "CancelJobRun",
             "CreateApplication",
             "DeleteApplication",
             "GetApplication",
             "GetDashboardForJobRun",
             "GetJobRun",
             "ListApplications",
@@ -22580,14 +22587,27 @@
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "AWS Support Plans"
         ]
     },
+    "supportrecommendations": {
+        "ARNFormats": [],
+        "ARNRegexes": [],
+        "Actions": [
+            "GetSupportTroubleshootingResponse",
+            "StartSupportTroubleshooting"
+        ],
+        "ConditionKeys": [],
+        "HasResource": false,
+        "ServiceNames": [
+            "AWS Support Recommendations"
+        ]
+    },
     "sustainability": {
         "ARNFormats": [
             "arn:${Partition}:sustainability:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:${Partition}:sustainability:.+:.+:.+"
         ],
```

### Comparing `iam_actions-1.2.20240523/pyproject.toml` & `iam_actions-1.2.20240524/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240523"
+version = "1.2.20240524"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240523/setup.py` & `iam_actions-1.2.20240524/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240523',
+    'version': '1.2.20240524',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240523/PKG-INFO` & `iam_actions-1.2.20240524/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240523
+Version: 1.2.20240524
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


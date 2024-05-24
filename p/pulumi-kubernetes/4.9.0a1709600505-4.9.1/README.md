# Comparing `tmp/pulumi_kubernetes-4.9.0a1709600505.tar.gz` & `tmp/pulumi_kubernetes-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes-4.9.0a1709600505.tar", last modified: Tue Mar  5 01:09:25 2024, max compression
+gzip compressed data, was "pulumi_kubernetes-4.9.1.tar", last modified: Wed Mar 13 21:56:02 2024, max compression
```

## Comparing `pulumi_kubernetes-4.9.0a1709600505.tar` & `pulumi_kubernetes-4.9.1.tar`

### file list

```diff
@@ -1,679 +1,679 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.925001 pulumi_kubernetes-4.9.0a1709600505/
--rw-r--r--   0 runner    (1000) runner    (1000)     9355 2024-03-05 01:09:25.925001 pulumi_kubernetes-4.9.0a1709600505/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     8829 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.833001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/
--rw-r--r--   0 runner    (1000) runner    (1000)    41042 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6932 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40823 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9217 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.833001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/
--rw-r--r--   0 runner    (1000) runner    (1000)      785 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.833001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11822 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11454 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13420 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11892 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11524 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13490 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      572 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   126826 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   121006 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.837001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12116 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13124 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11508 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14722 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11339 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13719 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   155949 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   162393 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.837001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12082 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11469 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13680 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12114 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13122 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11505 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14720 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11336 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13717 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12156 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11539 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13754 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      857 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   265511 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   267814 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.841001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/
--rw-r--r--   0 runner    (1000) runner    (1000)     9255 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/CustomResource.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7835 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/CustomResourcePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      672 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.841001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11920 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11390 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13496 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      413 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   212914 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   203375 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.841001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11420 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10673 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12986 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      413 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   183209 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   173449 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.841001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/
--rw-r--r--   0 runner    (1000) runner    (1000)      571 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.841001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11560 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/APIService.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11038 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/APIServiceList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13173 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30708 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32896 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.845001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    10830 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/APIService.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9978 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12433 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30275 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32487 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.845001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/
--rw-r--r--   0 runner    (1000) runner    (1000)      677 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.845001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13236 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ControllerRevision.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11036 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ControllerRevisionList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14778 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11854 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DaemonSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10767 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DaemonSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13462 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DaemonSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19970 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/Deployment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10412 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DeploymentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16049 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DeploymentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12580 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ReplicaSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11164 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ReplicaSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14188 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24360 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/StatefulSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10887 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/StatefulSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15062 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/StatefulSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      743 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   177605 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   218849 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.849001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13246 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11051 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14788 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14022 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/Deployment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10427 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/DeploymentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15635 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12724 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/StatefulSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9792 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14322 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      572 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    92195 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   112665 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.853001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/
--rw-r--r--   0 runner    (1000) runner    (1000)    13246 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11051 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14788 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11864 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DaemonSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10782 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13472 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14022 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/Deployment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10427 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DeploymentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15635 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12590 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11179 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14198 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12724 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/StatefulSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9792 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14322 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      743 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   147337 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   187289 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.853001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/
--rw-r--r--   0 runner    (1000) runner    (1000)      439 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.853001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)     9955 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10119 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11538 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30765 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28907 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.853001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/
--rw-r--r--   0 runner    (1000) runner    (1000)      853 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.853001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12143 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10846 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13756 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22804 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28045 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.853001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/
--rw-r--r--   0 runner    (1000) runner    (1000)    12613 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10976 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14226 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   109207 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   137695 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.857001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12623 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10983 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14236 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    99993 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   138421 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.857001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/
--rw-r--r--   0 runner    (1000) runner    (1000)    12623 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10991 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14236 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   107200 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   135212 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.857001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/
--rw-r--r--   0 runner    (1000) runner    (1000)      689 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.857001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11846 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/CronJob.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10740 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/CronJobList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13454 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/CronJobPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17964 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/Job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10598 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/JobList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15544 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/JobPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      428 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   122675 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   137364 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11888 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/CronJob.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10787 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/CronJobList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13496 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23861 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24638 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11890 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/CronJob.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10790 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/CronJobList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13498 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23742 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24519 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/
--rw-r--r--   0 runner    (1000) runner    (1000)      731 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13158 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10712 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14724 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      416 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44481 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    53207 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12314 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10841 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13880 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      395 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13356 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14968 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    10967 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10249 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12560 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      416 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23273 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26601 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.861001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/
--rw-r--r--   0 runner    (1000) runner    (1000)      559 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.865001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11052 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/Lease.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10706 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/LeaseList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12650 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/LeasePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12162 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12069 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.865001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    10990 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/Lease.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10721 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/LeaseList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12588 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12131 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12038 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.865001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.873001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    10930 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12530 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/BindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16018 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ConfigMap.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10715 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ConfigMapList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17591 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ConfigMapPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13511 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Endpoints.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10707 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EndpointsList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15104 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EndpointsPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28454 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Event.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10569 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EventList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30221 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EventPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11110 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/LimitRange.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11190 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/LimitRangeList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12703 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/LimitRangePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11558 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Namespace.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11197 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NamespaceList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13156 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NamespacePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11429 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Node.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10636 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NodeList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13027 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NodePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12176 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolume.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12008 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11583 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13642 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11312 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13774 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15709 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Pod.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10883 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14961 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11301 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodTemplate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10783 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodTemplateList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12894 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodTemplatePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12742 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ReplicationController.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11515 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ReplicationControllerList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14340 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11565 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ResourceQuota.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11219 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ResourceQuotaList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13163 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18698 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Secret.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10950 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/SecretList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20020 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/SecretPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17132 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18490 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceAccount.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11280 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceAccountList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20143 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceAccountPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10667 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16406 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServicePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1686 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/_enums.py
--rw-r--r--   0 runner    (1000) runner    (1000)  1588783 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)  1634057 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.877001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/
--rw-r--r--   0 runner    (1000) runner    (1000)      547 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.877001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    16252 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/EndpointSlice.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10569 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/EndpointSliceList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17826 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43563 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41636 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.877001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    16262 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10532 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17836 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35598 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33494 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.877001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.877001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    33307 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/Event.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10718 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/EventList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35127 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/EventPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19318 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19050 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.881001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    29243 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/Event.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10733 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/EventList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31053 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/EventPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17860 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16467 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.881001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/
--rw-r--r--   0 runner    (1000) runner    (1000)      419 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.881001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11876 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10800 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13484 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14034 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/Deployment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10445 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15647 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13728 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/Ingress.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10778 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/IngressList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15336 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11273 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11160 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12871 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11347 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11234 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12945 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12602 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11197 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14210 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      824 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   288488 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   316040 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.881001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/
--rw-r--r--   0 runner    (1000) runner    (1000)     1053 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.885001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12587 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/FlowSchema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10956 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/FlowSchemaList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14205 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12831 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11496 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14449 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   114053 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   123720 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.885001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12599 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10974 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14217 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12843 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11514 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14461 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    93706 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   102811 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.889001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12597 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10971 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14215 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11511 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14459 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    93700 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   102805 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.889001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/
--rw-r--r--   0 runner    (1000) runner    (1000)    12597 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10971 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14215 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11511 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14459 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   113331 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   122998 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.889001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/
--rw-r--r--   0 runner    (1000) runner    (1000)    12597 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10971 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14215 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11511 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14459 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   113327 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   122994 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.889001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.893001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/
--rw-r--r--   0 runner    (1000) runner    (1000)    61450 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/Release.py
--rw-r--r--   0 runner    (1000) runner    (1000)      327 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3999 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28195 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/helm.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7187 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.893001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/kustomize/
--rw-r--r--   0 runner    (1000) runner    (1000)      263 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/kustomize/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6671 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/kustomize/kustomize.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.893001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.893001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    15520 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/Status.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17179 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/StatusPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   115603 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   115305 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.893001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/
--rw-r--r--   0 runner    (1000) runner    (1000)      719 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.893001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    19184 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/Ingress.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12038 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10509 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13636 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10784 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15340 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11600 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/NetworkPolicy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10948 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/NetworkPolicyList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13203 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      551 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   126762 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   133939 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.897001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12370 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10946 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13963 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12226 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/IPAddress.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10850 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13819 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11865 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ServiceCIDR.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10932 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13463 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      548 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34259 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35250 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.897001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13742 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/Ingress.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12078 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10554 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13676 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10799 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15350 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      455 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54059 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    57257 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.897001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/
--rw-r--r--   0 runner    (1000) runner    (1000)      683 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.897001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    17524 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/RuntimeClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10929 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/RuntimeClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19157 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/RuntimeClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14552 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15712 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.901001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12189 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10947 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13765 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20390 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22634 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.901001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    17930 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/RuntimeClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10944 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19563 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14755 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15928 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1685 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.901001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.901001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11632 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11135 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13235 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      398 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27765 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36012 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.901001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    10902 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10000 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12495 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11209 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11084 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12807 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   106813 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   106119 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24695 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/provider.py
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/pulumi-plugin.json
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.901001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/
--rw-r--r--   0 runner    (1000) runner    (1000)      683 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.905001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13177 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRole.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12995 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10739 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14617 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10494 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14830 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10734 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/Role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13272 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10494 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14894 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10249 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12337 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RolePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      644 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42239 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42688 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.905001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13415 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13147 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11001 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14769 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10742 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15068 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10958 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/Role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13410 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10746 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15032 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10489 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12561 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      644 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43219 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44116 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.909001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13413 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13145 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11004 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14767 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10739 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15066 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10956 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/Role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13408 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10743 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15030 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10484 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12559 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RolePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      644 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42923 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43824 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.909001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/
--rw-r--r--   0 runner    (1000) runner    (1000)      585 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.913001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    11150 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10590 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12721 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11794 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10564 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13370 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11484 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10820 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13055 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16437 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10570 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18061 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    59521 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    77374 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.913001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/
--rw-r--r--   0 runner    (1000) runner    (1000)    11360 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10821 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12931 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11794 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10564 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13370 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11484 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10820 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13055 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16437 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10570 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18061 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      713 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    63467 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    85824 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.913001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/
--rw-r--r--   0 runner    (1000) runner    (1000)      719 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.913001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    17212 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/PriorityClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10954 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/PriorityClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18777 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7318 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6955 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.917001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    17744 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10972 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19309 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7584 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7323 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.917001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    17742 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10969 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19307 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7583 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7322 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.917001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/
--rw-r--r--   0 runner    (1000) runner    (1000)      421 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.917001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)     9676 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/PodPreset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10866 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11249 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12130 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11192 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.917001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/
--rw-r--r--   0 runner    (1000) runner    (1000)      701 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.921001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12783 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIDriver.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10807 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIDriverList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14354 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIDriverPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11643 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSINode.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10737 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSINodeList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13214 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSINodePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24161 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11158 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25753 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22861 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/StorageClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10940 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/StorageClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24485 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/StorageClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12090 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/VolumeAttachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11086 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13671 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      755 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   105133 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   111771 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.921001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/
--rw-r--r--   0 runner    (1000) runner    (1000)    12020 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11104 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13601 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15718 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11281 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17247 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26445 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32971 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.925001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/
--rw-r--r--   0 runner    (1000) runner    (1000)    13183 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIDriver.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10822 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14754 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11541 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSINode.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10752 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSINodeList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13112 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24071 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11173 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25663 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22731 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/StorageClass.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10955 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/StorageClassList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24355 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12018 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11101 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13599 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py
--rw-r--r--   0 runner    (1000) runner    (1000)      755 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    98721 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   105646 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.925001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/yaml/
--rw-r--r--   0 runner    (1000) runner    (1000)      258 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/yaml/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   105547 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/yaml/yaml.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-05 01:09:25.925001 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     9355 2024-03-05 01:09:25.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)    29922 2024-03-05 01:09:25.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-05 01:09:25.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       70 2024-03-05 01:09:25.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-03-05 01:09:25.000000 pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      751 2024-03-05 01:09:12.000000 pulumi_kubernetes-4.9.0a1709600505/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-05 01:09:25.925001 pulumi_kubernetes-4.9.0a1709600505/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.091581 pulumi_kubernetes-4.9.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     9345 2024-03-13 21:56:02.091581 pulumi_kubernetes-4.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     8829 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:01.995580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/
+-rw-r--r--   0 runner    (1000) runner    (1000)    41042 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6932 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40823 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9217 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:01.995580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/
+-rw-r--r--   0 runner    (1000) runner    (1000)      785 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:01.999580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11822 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11454 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13420 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11892 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11524 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13490 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      572 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   126826 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   121006 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:01.999580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12116 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13124 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11508 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14722 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11339 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13719 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   155949 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   162393 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.003580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12082 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11469 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13680 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12114 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13122 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11505 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14720 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11336 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13717 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12156 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11539 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13754 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      857 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   265511 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   267814 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.003580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/
+-rw-r--r--   0 runner    (1000) runner    (1000)     9255 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/CustomResource.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7835 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/CustomResourcePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      672 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.003580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11920 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11390 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13496 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      413 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   212914 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   203375 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.007580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11420 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10673 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12986 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      413 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   183209 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   173449 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.007580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/
+-rw-r--r--   0 runner    (1000) runner    (1000)      571 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.007580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11560 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/APIService.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11038 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/APIServiceList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13173 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30708 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32896 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.007580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    10830 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/APIService.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9978 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12433 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30275 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32487 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.007580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/
+-rw-r--r--   0 runner    (1000) runner    (1000)      677 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.011580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13236 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ControllerRevision.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11036 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ControllerRevisionList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14778 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11854 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DaemonSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10767 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DaemonSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13462 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DaemonSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19970 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/Deployment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10412 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DeploymentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16049 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DeploymentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12580 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ReplicaSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11164 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ReplicaSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14188 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24360 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/StatefulSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10887 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/StatefulSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15062 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/StatefulSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      743 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   177605 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   218849 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.011580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13246 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11051 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14788 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14022 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/Deployment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10427 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/DeploymentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15635 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12724 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/StatefulSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9792 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14322 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      572 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    92195 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   112665 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.015581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13246 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11051 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14788 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11864 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DaemonSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10782 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13472 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14022 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/Deployment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10427 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DeploymentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15635 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12590 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11179 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14198 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12724 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/StatefulSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9792 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14322 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      743 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   147337 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   187289 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.015581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/
+-rw-r--r--   0 runner    (1000) runner    (1000)      439 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.015581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     9955 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10119 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11538 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30765 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28907 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.015581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/
+-rw-r--r--   0 runner    (1000) runner    (1000)      853 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.019580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12143 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10846 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13756 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22804 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28045 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.019580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12613 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10976 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14226 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   109207 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   137695 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.019580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12623 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10983 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14236 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    99993 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   138421 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.019580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12623 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10991 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14236 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      410 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   107200 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   135212 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.019580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/
+-rw-r--r--   0 runner    (1000) runner    (1000)      689 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.023580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11846 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/CronJob.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10740 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/CronJobList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13454 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/CronJobPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17964 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/Job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10598 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/JobList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15544 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/JobPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      428 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   122675 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   137364 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.023580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11888 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/CronJob.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10787 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/CronJobList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13496 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23861 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24638 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.023580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11890 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/CronJob.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10790 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/CronJobList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13498 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23742 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24519 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.023580 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/
+-rw-r--r--   0 runner    (1000) runner    (1000)      731 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13158 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10712 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14724 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      416 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44481 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    53207 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12314 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10841 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13880 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      395 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13356 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14968 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    10967 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10249 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12560 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      416 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23273 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26601 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/
+-rw-r--r--   0 runner    (1000) runner    (1000)      559 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11052 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/Lease.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10706 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/LeaseList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12650 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/LeasePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12162 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12069 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    10990 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/Lease.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10721 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/LeaseList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12588 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12131 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12038 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.027581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.039581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    10930 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12530 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/BindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16018 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ConfigMap.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10715 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ConfigMapList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17591 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ConfigMapPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13511 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Endpoints.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10707 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EndpointsList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15104 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EndpointsPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28454 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Event.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10569 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EventList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30221 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EventPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11110 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/LimitRange.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11190 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/LimitRangeList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12703 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/LimitRangePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11558 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Namespace.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11197 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NamespaceList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13156 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NamespacePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11429 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Node.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10636 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NodeList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13027 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NodePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12176 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolume.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12008 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11583 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13642 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11312 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13774 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15709 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Pod.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10883 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14961 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11301 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodTemplate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10783 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodTemplateList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12894 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodTemplatePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12742 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ReplicationController.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11515 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ReplicationControllerList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14340 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11565 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ResourceQuota.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11219 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ResourceQuotaList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13163 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18698 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Secret.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10950 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/SecretList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20020 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/SecretPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17132 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18490 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceAccount.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11280 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceAccountList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20143 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceAccountPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10667 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16406 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServicePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1686 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/_enums.py
+-rw-r--r--   0 runner    (1000) runner    (1000)  1588783 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)  1634057 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.039581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/
+-rw-r--r--   0 runner    (1000) runner    (1000)      547 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.039581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16252 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/EndpointSlice.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10569 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/EndpointSliceList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17826 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43563 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41636 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.043581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    16262 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10532 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17836 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35598 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33494 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.043581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/
+-rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.043581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    33307 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/Event.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10718 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/EventList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35127 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/EventPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19318 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19050 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.043581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    29243 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/Event.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10733 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/EventList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31053 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/EventPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17860 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16467 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.043581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/
+-rw-r--r--   0 runner    (1000) runner    (1000)      419 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.047581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11876 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10800 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13484 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14034 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/Deployment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10445 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15647 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13728 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/Ingress.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10778 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/IngressList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15336 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11273 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11160 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12871 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11347 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11234 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12945 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12602 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11197 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14210 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      824 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   288488 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   316040 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.047581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1053 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.047581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12587 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/FlowSchema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10956 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/FlowSchemaList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14205 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12831 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11496 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14449 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   114053 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   123720 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.051581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12599 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10974 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14217 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12843 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11514 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14461 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    93706 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   102811 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.051581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12597 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10971 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14215 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11511 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14459 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    93700 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   102805 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12597 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10971 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14215 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11511 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14459 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   113331 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   122998 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12597 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10971 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14215 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11511 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14459 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   113327 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   122994 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/
+-rw-r--r--   0 runner    (1000) runner    (1000)    61450 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/Release.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      327 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3999 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28219 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/helm.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7187 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/kustomize/
+-rw-r--r--   0 runner    (1000) runner    (1000)      263 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/kustomize/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6828 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/kustomize/kustomize.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.055581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    15520 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/Status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17179 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/StatusPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   115603 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   115305 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.059581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/
+-rw-r--r--   0 runner    (1000) runner    (1000)      719 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.059581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    19184 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/Ingress.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12038 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10509 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13636 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10784 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15340 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11600 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/NetworkPolicy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10948 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/NetworkPolicyList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13203 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      551 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   126762 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   133939 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.059581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12370 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10946 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13963 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12226 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/IPAddress.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10850 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13819 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11865 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ServiceCIDR.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10932 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13463 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      548 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34259 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35250 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.063581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13742 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/Ingress.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12078 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10554 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13676 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10799 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15350 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      455 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54059 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    57257 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.063581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/
+-rw-r--r--   0 runner    (1000) runner    (1000)      683 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.063581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17524 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/RuntimeClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10929 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/RuntimeClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19157 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/RuntimeClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14552 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15712 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.063581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12189 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10947 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13765 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20390 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22634 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.063581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17930 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/RuntimeClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10944 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19563 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14755 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15928 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1685 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.067581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/
+-rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.067581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11632 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11135 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13235 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      398 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27765 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36012 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.067581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    10902 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10000 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12495 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11209 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11084 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12807 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   106813 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   106119 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24695 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/provider.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/pulumi-plugin.json
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.067581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/
+-rw-r--r--   0 runner    (1000) runner    (1000)      683 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.071581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13177 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRole.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12995 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10739 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14617 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10494 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14830 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10734 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/Role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13272 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10494 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14894 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10249 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12337 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RolePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      644 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42239 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42688 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.071581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13415 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13147 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11001 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14769 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10742 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15068 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10958 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/Role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13410 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10746 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15032 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10489 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12561 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      644 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43219 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44116 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.075581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13413 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13145 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11004 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14767 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10739 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15066 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10956 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/Role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13408 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10743 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15030 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10484 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12559 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RolePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      644 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42923 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43824 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.075581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/
+-rw-r--r--   0 runner    (1000) runner    (1000)      585 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.075581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11150 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10590 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12721 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11794 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10564 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13370 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11484 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10820 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13055 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16437 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10570 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18061 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    59521 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    77374 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.079581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/
+-rw-r--r--   0 runner    (1000) runner    (1000)    11360 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10821 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12931 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11794 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10564 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13370 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11484 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10820 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13055 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16437 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10570 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18061 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      713 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    63467 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    85824 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.079581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/
+-rw-r--r--   0 runner    (1000) runner    (1000)      719 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.079581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17212 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/PriorityClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10954 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/PriorityClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18777 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7318 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6955 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.079581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17744 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10972 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19309 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7584 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7323 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.083581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    17742 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10969 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19307 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7583 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7322 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.083581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/
+-rw-r--r--   0 runner    (1000) runner    (1000)      421 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.083581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     9676 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/PodPreset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10866 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11249 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12130 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11192 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.083581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/
+-rw-r--r--   0 runner    (1000) runner    (1000)      701 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.083581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12783 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIDriver.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10807 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIDriverList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14354 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIDriverPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11643 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSINode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10737 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSINodeList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13214 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSINodePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24161 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11158 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25753 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22861 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/StorageClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10940 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/StorageClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24485 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/StorageClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12090 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/VolumeAttachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11086 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13671 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      755 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   105133 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   111771 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.087581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12020 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11104 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13601 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15718 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11281 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17247 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26445 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32971 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.087581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/
+-rw-r--r--   0 runner    (1000) runner    (1000)    13183 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIDriver.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10822 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14754 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11541 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSINode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10752 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSINodeList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13112 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24071 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11173 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25663 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22731 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/StorageClass.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10955 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/StorageClassList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24355 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12018 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11101 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13599 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      755 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    98721 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   105646 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.091581 pulumi_kubernetes-4.9.1/pulumi_kubernetes/yaml/
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/yaml/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   105671 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes/yaml/yaml.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-13 21:56:02.091581 pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     9345 2024-03-13 21:56:01.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)    29922 2024-03-13 21:56:01.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-13 21:56:01.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       71 2024-03-13 21:56:01.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-03-13 21:56:01.000000 pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      741 2024-03-13 21:55:49.000000 pulumi_kubernetes-4.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-13 21:56:02.091581 pulumi_kubernetes-4.9.1/setup.cfg
```

### Comparing `pulumi_kubernetes-4.9.0a1709600505/PKG-INFO` & `pulumi_kubernetes-4.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes
-Version: 4.9.0a1709600505
+Version: 4.9.1
 Summary: A Pulumi package for creating and managing Kubernetes resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes
 Keywords: pulumi,kubernetes,category/cloud,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
-Requires-Dist: pulumi<4.0.0,>=3.25.0
+Requires-Dist: pulumi<4.0.0,>=3.109.0
 Requires-Dist: requests<3.0,>=2.21
 Requires-Dist: semver>=2.8.1
 
 [![Build Status](https://travis-ci.com/pulumi/pulumi-kubernetes.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-ci.com/pulumi/pulumi-kubernetes)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fkubernetes.svg)](https://www.npmjs.com/package/@pulumi/kubernetes)
 [![Python version](https://badge.fury.io/py/pulumi-kubernetes.svg)](https://pypi.org/project/pulumi-kubernetes/)
```

### Comparing `pulumi_kubernetes-4.9.0a1709600505/README.md` & `pulumi_kubernetes-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/_tables.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/_utilities.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicy.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingAdmissionPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/CustomResource.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/CustomResource.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/CustomResourcePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/CustomResourcePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiextensions/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiextensions/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/APIService.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/APIService.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/APIServiceList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/APIServiceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/APIService.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/APIService.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apiregistration/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apiregistration/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ControllerRevision.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ControllerRevision.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ControllerRevisionList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ControllerRevisionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DaemonSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DaemonSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DaemonSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DaemonSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DaemonSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DaemonSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/Deployment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DeploymentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/DeploymentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ReplicaSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ReplicaSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ReplicaSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ReplicaSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/StatefulSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/StatefulSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/StatefulSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/StatefulSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/StatefulSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/StatefulSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/Deployment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/DeploymentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/StatefulSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/StatefulSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DaemonSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DaemonSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/Deployment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DeploymentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/StatefulSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/StatefulSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/apps/v1beta2/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/apps/v1beta2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/autoscaling/v2beta2/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/autoscaling/v2beta2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/CronJob.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/CronJob.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/CronJobList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/CronJobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/CronJobPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/CronJobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/Job.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/Job.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/JobList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/JobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/JobPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/JobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/CronJob.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/CronJob.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/CronJobList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/CronJobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/CronJob.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/CronJob.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/CronJobList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/CronJobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/batch/v2alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/batch/v2alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/certificates/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/certificates/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/Lease.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/Lease.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/LeaseList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/LeaseList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/LeasePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/LeasePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/Lease.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/Lease.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/LeaseList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/LeaseList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/coordination/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/coordination/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Binding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/BindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/BindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ConfigMap.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ConfigMap.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ConfigMapList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ConfigMapList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ConfigMapPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ConfigMapPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Endpoints.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EndpointsList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EndpointsList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EndpointsPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EndpointsPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Event.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Event.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EventList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EventList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/EventPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/EventPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/LimitRange.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/LimitRange.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/LimitRangeList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/LimitRangeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/LimitRangePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/LimitRangePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Namespace.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NamespaceList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NamespaceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NamespacePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NamespacePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Node.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Node.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NodeList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NodeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/NodePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/NodePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolume.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolume.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumeList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PersistentVolumePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PersistentVolumePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Pod.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodTemplate.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodTemplate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodTemplateList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodTemplateList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/PodTemplatePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/PodTemplatePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ReplicationController.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ReplicationController.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ReplicationControllerList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ReplicationControllerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ResourceQuota.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ResourceQuota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ResourceQuotaList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ResourceQuotaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Secret.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/SecretList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/SecretList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/SecretPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/SecretPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/Service.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/Service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceAccount.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceAccount.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceAccountList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceAccountList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceAccountPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceAccountPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServiceList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServiceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/ServicePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/ServicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/core/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/core/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/EndpointSlice.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/EndpointSlice.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/EndpointSliceList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/EndpointSliceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/discovery/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/discovery/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/Event.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/Event.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/EventList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/EventList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/EventPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/EventPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/Event.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/Event.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/EventList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/EventList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/EventPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/EventPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/events/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/events/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/Deployment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/Ingress.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/Ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/IngressList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/IngressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/extensions/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/extensions/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/FlowSchema.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/FlowSchemaList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/FlowSchemaPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/Release.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/Release.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/helm.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/helm.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,12 +610,12 @@
 
     invoke_opts = _get_invoke_options(opts)
     
     transformations = config.transformations if config.transformations is not None else []
     if config.skip_await:
         transformations.append(_skip_await)
 
-    def invoke_helm_template(opts):
-        inv = pulumi.runtime.invoke('kubernetes:helm:template', {'jsonOpts': opts}, invoke_opts)
-        return (inv.value or {}).get('result', [])
-    objects = json_opts.apply(invoke_helm_template)
+    async def invoke_helm_template_async(opts):
+        inv = await pulumi.runtime.invoke_async('kubernetes:helm:template', {'jsonOpts': opts}, invoke_opts)
+        return (inv or {}).get('result', [])
+    objects = json_opts.apply(invoke_helm_template_async)
     return objects.apply(lambda x: _parse_yaml_document(x, opts, transformations))
```

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/helm/v3/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/helm/v3/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/kustomize/kustomize.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/kustomize/kustomize.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,26 +107,28 @@
 
         if resource_prefix:
             name = f"{resource_prefix}-{name}"
         super(Directory, self).__init__("kubernetes:kustomize:Directory", name, __props__, opts)
 
         child_opts = _get_child_options(self, opts)
         invoke_opts = _get_invoke_options(child_opts)
-        
-        __ret__ = pulumi.runtime.invoke(
-            'kubernetes:kustomize:directory', {'directory': directory}, invoke_opts)
-
-        # Handle the cases when the provider is not fully configured:
-        #   https://github.com/pulumi/pulumi/blob/v3.60.1/sdk/go/common/resource/plugin/provider_plugin.go#L1364-L1367
-        result = (__ret__.value or {}).get('result', [])
+
+        async def invoke_kustomize_directory_async():
+            inv = await pulumi.runtime.invoke_async(
+                'kubernetes:kustomize:directory', {'directory': directory}, invoke_opts)
+            # Handle the cases when the provider is not fully configured:
+            # https://github.com/pulumi/pulumi/blob/v3.60.1/sdk/go/common/resource/plugin/provider_plugin.go#L1364-L1367
+            return (inv or {}).get('result', [])
+
+        result = pulumi.Output.from_input(invoke_kustomize_directory_async())
 
         # Note: Unlike NodeJS, Python requires that we "pull" on our futures in order to get them scheduled for
         # execution. In order to do this, we leverage the engine's RegisterResourceOutputs to wait for the
         # resolution of all resources that this YAML document created.
-        self.resources = _parse_yaml_document(result, child_opts, transformations, resource_prefix)
+        self.resources = result.apply(lambda x: _parse_yaml_document(x, child_opts, transformations, resource_prefix))
         self.register_outputs({"resources": self.resources})
 
     def translate_output_property(self, prop: str) -> str:
         return _tables.CAMEL_TO_SNAKE_CASE_TABLE.get(prop) or prop
 
     def translate_input_property(self, prop: str) -> str:
         return _tables.SNAKE_TO_CAMEL_CASE_TABLE.get(prop) or prop
```

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/Status.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/Status.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/StatusPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/StatusPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/meta/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/meta/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/Ingress.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/Ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/IngressPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/IngressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/NetworkPolicy.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/NetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/NetworkPolicyList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/NetworkPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/IPAddress.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/IPAddress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ServiceCIDR.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ServiceCIDR.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/ServiceCIDRPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/Ingress.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/Ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/IngressPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/IngressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/networking/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/networking/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/RuntimeClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/RuntimeClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/RuntimeClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/RuntimeClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/RuntimeClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/RuntimeClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/RuntimeClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/RuntimeClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/node/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/node/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/policy/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/policy/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/provider.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRole.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRole.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRoleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/Role.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/Role.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RoleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/RolePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/RolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/Role.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/Role.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RoleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/Role.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/Role.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RoleList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/RolePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/RolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/rbac/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/rbac/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/resource/v1alpha2/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/resource/v1alpha2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/PriorityClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/PriorityClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/PriorityClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/PriorityClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/scheduling/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/scheduling/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/PodPreset.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/PodPreset.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/settings/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/settings/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIDriver.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIDriver.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIDriverList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIDriverList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIDriverPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIDriverPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSINode.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSINode.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSINodeList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSINodeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSINodePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSINodePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/StorageClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/StorageClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/StorageClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/StorageClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/StorageClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/StorageClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/VolumeAttachment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/VolumeAttachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/VolumeAttributesClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1alpha1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIDriver.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIDriver.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSINode.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSINode.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSINodeList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSINodeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/StorageClass.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/StorageClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/StorageClassList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/StorageClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/__init__.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/_inputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/storage/v1beta1/outputs.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/storage/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes/yaml/yaml.py` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes/yaml/yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,16 @@
             cf = ConfigFile(
                 file, file_id=file, transformations=transformations, resource_prefix=resource_prefix, opts=child_opts)
             # Add any new ConfigFile resources to the ConfigGroup's resources
             self.resources = pulumi.Output.all(cf.resources, self.resources).apply(lambda x: {**x[0], **x[1]})
 
         for text in yaml:
             invoke_opts = _get_invoke_options(child_opts)
-            __ret__ = invoke_yaml_decode(text, invoke_opts)
-            resources = _parse_yaml_document(__ret__, child_opts, transformations, resource_prefix)
+            decoded = pulumi.Output.from_input(_invoke_yaml_decode_async(text, invoke_opts))
+            resources = decoded.apply(lambda x: _parse_yaml_document(x, child_opts, transformations, resource_prefix))
             # Add any new YAML resources to the ConfigGroup's resources
             self.resources = pulumi.Output.all(resources, self.resources).apply(lambda x: {**x[0], **x[1]})
 
         # Note: Unlike NodeJS, Python requires that we "pull" on our futures in order to get them scheduled for
         # execution. In order to do this, we leverage the engine's RegisterResourceOutputs to wait for the
         # resolution of all resources that this YAML document created.
         self.register_outputs({"resources": self.resources})
@@ -333,20 +333,20 @@
         child_opts = _get_child_options(self, opts)
 
         transformations = transformations if transformations is not None else []
         if skip_await:
             transformations.append(_skip_await)
  
         invoke_opts = _get_invoke_options(child_opts)
-        __ret__ = invoke_yaml_decode(text, invoke_opts)
+        decoded = pulumi.Output.from_input(_invoke_yaml_decode_async(text, invoke_opts))
 
         # Note: Unlike NodeJS, Python requires that we "pull" on our futures in order to get them scheduled for
         # execution. In order to do this, we leverage the engine's RegisterResourceOutputs to wait for the
         # resolution of all resources that this YAML document created.
-        self.resources = _parse_yaml_document(__ret__, child_opts, transformations, resource_prefix)
+        self.resources = decoded.apply(lambda x: _parse_yaml_document(x, child_opts, transformations, resource_prefix))
         self.register_outputs({"resources": self.resources})
 
     def translate_output_property(self, prop: str) -> str:
         return _tables.CAMEL_TO_SNAKE_CASE_TABLE.get(prop) or prop
 
     def translate_input_property(self, prop: str) -> str:
         return _tables.SNAKE_TO_CAMEL_CASE_TABLE.get(prop) or prop
@@ -2002,10 +2002,10 @@
         return [identifier.apply(
             lambda x: (f"apiextensions.k8s.io/v1beta1/CustomResourceDefinition:{x}",
                        CustomResourceDefinition(f"{x}", opts, **obj)))]
     return [identifier.apply(
         lambda x: (f"{gvk}:{x}",
                    CustomResource(f"{x}", api_version, kind, spec, metadata, opts)))]
 
-def invoke_yaml_decode(text, invoke_opts):
-    inv = pulumi.runtime.invoke('kubernetes:yaml:decode', {'text': text}, invoke_opts)
-    return (inv.value or {}).get('result', [])
+async def _invoke_yaml_decode_async(text, invoke_opts):
+    inv = await pulumi.runtime.invoke_async('kubernetes:yaml:decode', {'text': text}, invoke_opts)
+    return (inv or {}).get('result', [])
```

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/PKG-INFO` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes
-Version: 4.9.0a1709600505
+Version: 4.9.1
 Summary: A Pulumi package for creating and managing Kubernetes resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes
 Keywords: pulumi,kubernetes,category/cloud,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
-Requires-Dist: pulumi<4.0.0,>=3.25.0
+Requires-Dist: pulumi<4.0.0,>=3.109.0
 Requires-Dist: requests<3.0,>=2.21
 Requires-Dist: semver>=2.8.1
 
 [![Build Status](https://travis-ci.com/pulumi/pulumi-kubernetes.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-ci.com/pulumi/pulumi-kubernetes)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fkubernetes.svg)](https://www.npmjs.com/package/@pulumi/kubernetes)
 [![Python version](https://badge.fury.io/py/pulumi-kubernetes.svg)](https://pypi.org/project/pulumi-kubernetes/)
```

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pulumi_kubernetes.egg-info/SOURCES.txt` & `pulumi_kubernetes-4.9.1/pulumi_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.9.0a1709600505/pyproject.toml` & `pulumi_kubernetes-4.9.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes"
   description = "A Pulumi package for creating and managing Kubernetes resources."
-  dependencies = ["parver>=0.2.1", "pulumi>=3.25.0,<4.0.0", "requests>=2.21,<3.0", "semver>=2.8.1"]
+  dependencies = ["parver>=0.2.1", "pulumi>=3.109.0,<4.0.0", "requests>=2.21,<3.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kubernetes", "category/cloud", "kind/native"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.9.0a1709600505"
+  version = "4.9.1"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-kubernetes"
 
 [build-system]
```


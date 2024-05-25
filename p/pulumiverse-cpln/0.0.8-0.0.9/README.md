# Comparing `tmp/pulumiverse_cpln-0.0.8.tar.gz` & `tmp/pulumiverse_cpln-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_cpln-0.0.8.tar", last modified: Wed Mar 20 13:34:10 2024, max compression
+gzip compressed data, was "pulumiverse_cpln-0.0.9.tar", last modified: Wed Mar 20 13:49:07 2024, max compression
```

## Comparing `pulumiverse_cpln-0.0.8.tar` & `pulumiverse_cpln-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:34:10.047455 pulumiverse_cpln-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-20 13:34:10.047455 pulumiverse_cpln-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:34:10.043455 pulumiverse_cpln-0.0.8/pulumiverse_cpln/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   234148 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/audit_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    20061 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/cloud_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:34:10.047455 pulumiverse_cpln-0.0.8/pulumiverse_cpln/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/domain_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_cloud_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_gvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_org.py
--rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    31390 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/gvc.py
--rw-r--r--   0 runner    (1001) docker     (127)    29122 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    20870 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/org.py
--rw-r--r--   0 runner    (1001) docker     (127)    20457 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/org_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/org_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)   223249 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22444 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/service_account_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/volume_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:34:10.047455 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-20 13:34:10.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-20 13:34:10.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:34:10.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:34:10.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 13:34:10.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 13:34:10.000000 pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:34:10.047455 pulumiverse_cpln-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-20 13:34:09.000000 pulumiverse_cpln-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:49:07.876498 pulumiverse_cpln-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-20 13:49:07.876498 pulumiverse_cpln-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:49:07.876498 pulumiverse_cpln-0.0.9/pulumiverse_cpln/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234148 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/audit_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20061 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/cloud_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:49:07.876498 pulumiverse_cpln-0.0.9/pulumiverse_cpln/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/domain_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_cloud_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_gvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31390 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/gvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29122 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20870 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/org.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20457 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/org_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/org_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)   223249 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22444 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/service_account_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/volume_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:49:07.876498 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:49:07.876498 pulumiverse_cpln-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-20 13:49:07.000000 pulumiverse_cpln-0.0.9/setup.py
```

### Comparing `pulumiverse_cpln-0.0.8/PKG-INFO` & `pulumiverse_cpln-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_cpln
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Control Plane (cpln) resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-cpln
 Keywords: pulumi cpln category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_cpln-0.0.8/README.md` & `pulumiverse_cpln-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/__init__.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/_inputs.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/_utilities.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/agent.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/agent.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/audit_context.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/audit_context.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/cloud_account.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/config/vars.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/domain.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/domain_route.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/domain_route.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_cloud_account.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_gvc.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_gvc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_location.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_location.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_locations.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_locations.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/get_org.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/get_org.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/group.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/gvc.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/gvc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/identity.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/identity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/org.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/org.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/org_logging.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/org_logging.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/org_tracing.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/org_tracing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/outputs.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/policy.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/provider.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/secret.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/service_account.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/service_account_key.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/service_account_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/volume_set.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/volume_set.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln/workload.py` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln/workload.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/PKG-INFO` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-cpln
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Control Plane (cpln) resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-cpln
 Keywords: pulumi cpln category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_cpln-0.0.8/pulumiverse_cpln.egg-info/SOURCES.txt` & `pulumiverse_cpln-0.0.9/pulumiverse_cpln.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_cpln-0.0.8/setup.py` & `pulumiverse_cpln-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "cpln Pulumi Package - Development Version"
```


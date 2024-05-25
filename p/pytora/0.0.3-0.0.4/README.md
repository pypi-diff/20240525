# Comparing `tmp/pytora-0.0.3.tar.gz` & `tmp/pytora-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytora-0.0.3.tar", last modified: Tue May 14 14:24:37 2024, max compression
+gzip compressed data, was "pytora-0.0.4.tar", last modified: Sat May 25 15:51:54 2024, max compression
```

## Comparing `pytora-0.0.3.tar` & `pytora-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hauzenbe  (5109) bioinf    (1001)        0 2024-05-14 14:24:37.783186 pytora-0.0.3/
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      819 2024-05-14 14:24:37.779982 pytora-0.0.3/PKG-INFO
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      416 2024-05-14 14:15:17.000000 pytora-0.0.3/README.md
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      495 2024-05-14 14:24:32.000000 pytora-0.0.3/pyproject.toml
-drwxr-xr-x   0 hauzenbe  (5109) bioinf    (1001)        0 2024-05-14 14:24:37.749935 pytora-0.0.3/pytora/
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)       46 2024-05-14 13:58:58.000000 pytora-0.0.3/pytora/__init__.py
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)     1994 2024-05-14 13:34:12.000000 pytora-0.0.3/pytora/lora_layer.py
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)     2684 2024-05-14 14:24:04.000000 pytora-0.0.3/pytora/utils.py
-drwxr-xr-x   0 hauzenbe  (5109) bioinf    (1001)        0 2024-05-14 14:24:37.775234 pytora-0.0.3/pytora.egg-info/
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      819 2024-05-14 14:24:37.000000 pytora-0.0.3/pytora.egg-info/PKG-INFO
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      229 2024-05-14 14:24:37.000000 pytora-0.0.3/pytora.egg-info/SOURCES.txt
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)        1 2024-05-14 14:24:37.000000 pytora-0.0.3/pytora.egg-info/dependency_links.txt
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)       13 2024-05-14 14:24:37.000000 pytora-0.0.3/pytora.egg-info/requires.txt
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)        7 2024-05-14 14:24:37.000000 pytora-0.0.3/pytora.egg-info/top_level.txt
--rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)       38 2024-05-14 14:24:37.784006 pytora-0.0.3/setup.cfg
+drwxr-xr-x   0 hauzenbe  (5109) bioinf    (1001)        0 2024-05-25 15:51:53.991886 pytora-0.0.4/
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      819 2024-05-25 15:51:53.987722 pytora-0.0.4/PKG-INFO
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      416 2024-05-14 14:15:17.000000 pytora-0.0.4/README.md
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      495 2024-05-25 15:48:36.000000 pytora-0.0.4/pyproject.toml
+drwxr-xr-x   0 hauzenbe  (5109) bioinf    (1001)        0 2024-05-25 15:51:53.948394 pytora-0.0.4/pytora/
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)       46 2024-05-14 13:58:58.000000 pytora-0.0.4/pytora/__init__.py
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)     1994 2024-05-14 13:34:12.000000 pytora-0.0.4/pytora/lora_layer.py
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)     2918 2024-05-25 13:01:32.000000 pytora-0.0.4/pytora/utils.py
+drwxr-xr-x   0 hauzenbe  (5109) bioinf    (1001)        0 2024-05-25 15:51:53.981806 pytora-0.0.4/pytora.egg-info/
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      819 2024-05-25 15:51:53.000000 pytora-0.0.4/pytora.egg-info/PKG-INFO
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)      229 2024-05-25 15:51:53.000000 pytora-0.0.4/pytora.egg-info/SOURCES.txt
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)        1 2024-05-25 15:51:53.000000 pytora-0.0.4/pytora.egg-info/dependency_links.txt
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)       13 2024-05-25 15:51:53.000000 pytora-0.0.4/pytora.egg-info/requires.txt
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)        7 2024-05-25 15:51:53.000000 pytora-0.0.4/pytora.egg-info/top_level.txt
+-rw-r--r--   0 hauzenbe  (5109) bioinf    (1001)       38 2024-05-25 15:51:53.992899 pytora-0.0.4/setup.cfg
```

### Comparing `pytora-0.0.3/PKG-INFO` & `pytora-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytora
-Version: 0.0.3
+Version: 0.0.4
 Summary: A minimal PyTorch implementation of LoRA
 Author-email: Lukas Hauzenberger <lukas.hauzenberger@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pytora-0.0.3/pytora/lora_layer.py` & `pytora-0.0.4/pytora/lora_layer.py`

 * *Files identical despite different names*

### Comparing `pytora-0.0.3/pytora/utils.py` & `pytora-0.0.4/pytora/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import torch
 from torch import nn
 from torch.nn.utils.parametrize import register_parametrization, remove_parametrizations
-from transformers import Conv1D
+import importlib
 from functools import partial
 from collections import OrderedDict
 
 from .lora_layer import LoraLayer
 
 from typing import Optional
 
 
+_TRANSFORMERS_AVAILABLE = importlib.util.find_spec("transformers") is not None
+if _TRANSFORMERS_AVAILABLE:
+    from transformers import Conv1D
+
+
 def module_name_check(
     name: str,
     include_names: Optional[list[str]] = None,
     exclude_names: Optional[list[str]] = None,
 ):
     if include_names is not None:
         inclusion = [n == name[-len(n):] for n in include_names]
@@ -39,34 +44,35 @@
         module_name_check,
         include_names = include_names,
         exclude_names = exclude_names
     )
 
     for name, module in model.named_modules():
         
-        if type(module) == torch.nn.Linear and check(name):
-            l = LoraLayer(
-                weight = module.weight,
-                r = lora_r,
-                alpha = lora_alpha,
-                dropout_prob = lora_dropout
-            )
-            register_parametrization(module, "weight", l)
-            module.weight.requires_grad = False
-        # same as linear layer, was implemented to keep gpt2 style
-        elif type(module) == Conv1D and check(name):
-            l = LoraLayer(
-                weight = module.weight,
-                r = lora_r,
-                alpha = lora_alpha,
-                dropout_prob = lora_dropout,
-                fan_in_fan_out = True
-            )
-            register_parametrization(module, "weight", l)
-            module.weight.requires_grad = False
+        if check(name):
+            if type(module) == torch.nn.Linear:
+                l = LoraLayer(
+                    weight = module.weight,
+                    r = lora_r,
+                    alpha = lora_alpha,
+                    dropout_prob = lora_dropout
+                )
+                register_parametrization(module, "weight", l)
+                module.weight.requires_grad = False
+            elif _TRANSFORMERS_AVAILABLE and type(module) == Conv1D:
+                # same as linear layer, was implemented to keep gpt2 style
+                l = LoraLayer(
+                    weight = module.weight,
+                    r = lora_r,
+                    alpha = lora_alpha,
+                    dropout_prob = lora_dropout,
+                    fan_in_fan_out = True
+                )
+                register_parametrization(module, "weight", l)
+                module.weight.requires_grad = False
 
 
 @torch.no_grad()
 def remove_lora(
     model: nn.Module,
     merge: bool = True,
     return_lora_state_dict: bool = True,
```

### Comparing `pytora-0.0.3/pytora.egg-info/PKG-INFO` & `pytora-0.0.4/pytora.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytora
-Version: 0.0.3
+Version: 0.0.4
 Summary: A minimal PyTorch implementation of LoRA
 Author-email: Lukas Hauzenberger <lukas.hauzenberger@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


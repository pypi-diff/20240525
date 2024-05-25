# Comparing `tmp/lycoris_lora-3.0.0.dev2.tar.gz` & `tmp/lycoris_lora-3.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-3.0.0.dev2.tar", last modified: Sat May 18 10:28:22 2024, max compression
+gzip compressed data, was "lycoris_lora-3.0.0.dev3.tar", last modified: Fri May 24 09:00:20 2024, max compression
```

## Comparing `lycoris_lora-3.0.0.dev2.tar` & `lycoris_lora-3.0.0.dev3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 10:28:22.026153 lycoris_lora-3.0.0.dev2/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev2/LICENSE.md
--rw-rw-rw-   0        0        0      527 2024-05-18 10:28:22.026153 lycoris_lora-3.0.0.dev2/PKG-INFO
--rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 10:28:22.004624 lycoris_lora-3.0.0.dev2/lycoris/
--rw-rw-rw-   0        0        0      588 2024-05-18 10:27:24.000000 lycoris_lora-3.0.0.dev2/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev2/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:28:22.006129 lycoris_lora-3.0.0.dev2/lycoris/functional/
--rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev2/lycoris/functional/__init__.py
--rw-rw-rw-   0        0        0     2379 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev2/lycoris/functional/general.py
--rw-rw-rw-   0        0        0     3354 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev2/lycoris/functional/locon.py
--rw-rw-rw-   0        0        0     5259 2024-05-17 12:55:00.000000 lycoris_lora-3.0.0.dev2/lycoris/functional/loha.py
--rw-rw-rw-   0        0        0    31780 2024-05-18 10:06:20.000000 lycoris_lora-3.0.0.dev2/lycoris/kohya.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev2/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:28:22.012637 lycoris_lora-3.0.0.dev2/lycoris/modules/
--rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     8136 2024-05-18 09:26:28.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     7635 2024-05-18 08:00:24.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     6971 2024-05-18 10:13:54.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     5775 2024-05-18 08:01:04.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/full.py
--rw-rw-rw-   0        0        0     7140 2024-05-18 10:13:31.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    11185 2024-05-18 10:28:02.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    10688 2024-05-18 09:10:27.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    15618 2024-05-18 09:11:19.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev2/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:28:22.014642 lycoris_lora-3.0.0.dev2/lycoris/utils/
--rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-3.0.0.dev2/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev2/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev2/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev2/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev2/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18779 2024-05-15 08:22:10.000000 lycoris_lora-3.0.0.dev2/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-18 10:28:22.025154 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-18 10:28:21.000000 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      879 2024-05-18 10:28:21.000000 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 10:28:21.000000 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2024-05-18 10:28:21.000000 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 10:28:21.000000 lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 10:28:22.026153 lycoris_lora-3.0.0.dev2/setup.cfg
--rw-rw-rw-   0        0        0      638 2024-05-18 10:28:12.000000 lycoris_lora-3.0.0.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:00:20.119180 lycoris_lora-3.0.0.dev3/
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev3/LICENSE.md
+-rw-rw-rw-   0        0        0      444 2024-05-24 09:00:20.119180 lycoris_lora-3.0.0.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:00:20.097626 lycoris_lora-3.0.0.dev3/lycoris/
+-rw-rw-rw-   0        0        0      588 2024-05-18 10:27:24.000000 lycoris_lora-3.0.0.dev3/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev3/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:00:20.099629 lycoris_lora-3.0.0.dev3/lycoris/functional/
+-rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev3/lycoris/functional/__init__.py
+-rw-rw-rw-   0        0        0     2429 2024-05-18 15:09:35.000000 lycoris_lora-3.0.0.dev3/lycoris/functional/general.py
+-rw-rw-rw-   0        0        0     3354 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev3/lycoris/functional/locon.py
+-rw-rw-rw-   0        0        0     5259 2024-05-17 12:55:00.000000 lycoris_lora-3.0.0.dev3/lycoris/functional/loha.py
+-rw-rw-rw-   0        0        0    31780 2024-05-18 10:06:20.000000 lycoris_lora-3.0.0.dev3/lycoris/kohya.py
+-rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev3/lycoris/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:00:20.105146 lycoris_lora-3.0.0.dev3/lycoris/modules/
+-rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     9576 2024-05-24 08:45:31.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/base.py
+-rw-rw-rw-   0        0        0     8349 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/boft.py
+-rw-rw-rw-   0        0        0     7743 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/diag_oft.py
+-rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     6439 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/full.py
+-rw-rw-rw-   0        0        0     7870 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     2078 2024-03-11 06:14:46.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    11601 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    11389 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    16594 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev3/lycoris/modules/norms.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:00:20.106654 lycoris_lora-3.0.0.dev3/lycoris/utils/
+-rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-3.0.0.dev3/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev3/lycoris/utils/bnb.py
+-rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev3/lycoris/utils/logger.py
+-rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev3/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev3/lycoris/utils/xformers_utils.py
+-rw-rw-rw-   0        0        0    18779 2024-05-15 08:22:10.000000 lycoris_lora-3.0.0.dev3/lycoris/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:00:20.118177 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      444 2024-05-24 09:00:20.000000 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2024-05-24 09:00:20.000000 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:00:20.000000 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-05-24 09:00:20.000000 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 09:00:20.000000 lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:00:20.119180 lycoris_lora-3.0.0.dev3/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-24 09:00:16.000000 lycoris_lora-3.0.0.dev3/setup.py
```

### Comparing `lycoris_lora-3.0.0.dev2/LICENSE.md` & `lycoris_lora-3.0.0.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/README.md` & `lycoris_lora-3.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/__init__.py` & `lycoris_lora-3.0.0.dev3/lycoris/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/config.py` & `lycoris_lora-3.0.0.dev3/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/functional/general.py` & `lycoris_lora-3.0.0.dev3/lycoris/functional/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 def power2factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
     """
     m = 2k
     n = 2**p
     m*n = dim
     """
+    if factor == -1:
+        factor = dimension
 
     # Find the first solution and check if it is even doable
     m = n = 0
     while m <= factor:
         m += 2
         while dimension % m != 0 and m < dimension:
             m += 2
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/functional/locon.py` & `lycoris_lora-3.0.0.dev3/lycoris/functional/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/functional/loha.py` & `lycoris_lora-3.0.0.dev3/lycoris/functional/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/kohya.py` & `lycoris_lora-3.0.0.dev3/lycoris/kohya.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/logging.py` & `lycoris_lora-3.0.0.dev3/lycoris/logging.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/__init__.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/base.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import OrderedDict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+import torch.nn.utils.parametrize as parametrize
 
 from ..utils.bnb import QuantLinears, log_bypass
 
 
 class ModuleCustomSD(nn.Module):
     def __init__(self):
         super().__init__()
@@ -177,14 +178,46 @@
             nn.Identity() if rank_dropout == 0.0 else nn.Dropout(rank_dropout)
         )
 
         self.multiplier = multiplier
         self.org_forward = org_module.forward
         self.org_module = [org_module]
 
+    @classmethod
+    def parametrize(cls, org_module, attr, *args, **kwargs):
+        target_param = getattr(org_module, attr)
+        kwargs["bypass_mode"] = False
+        if target_param.dim() == 2:
+            proxy_module = nn.Linear(
+                target_param.shape[0], target_param.shape[1], bias=False
+            )
+            proxy_module.weight = target_param
+        elif target_param.dim() > 2:
+            module_type = [
+                None,
+                None,
+                None,
+                nn.Conv1d,
+                nn.Conv2d,
+                nn.Conv3d,
+                None,
+                None,
+            ][target_param.dim()]
+            proxy_module = module_type(
+                target_param.shape[0],
+                target_param.shape[1],
+                *target_param.shape[2:],
+            )
+            proxy_module.weight = target_param
+        module_obj = cls("", proxy_module, *args, **kwargs)
+        module_obj.forward = module_obj.parametrize_forward
+        module_obj.to(target_param.device)
+        parametrize.register_parametrization(org_module, attr, module_obj)
+        return module_obj
+
     @property
     def dtype(self):
         return self.dtype_tensor.dtype
 
     @property
     def device(self):
         return self.dtype_tensor.device
@@ -227,9 +260,14 @@
 
     def bypass_forward_diff(self, x, scale=1):
         raise NotImplementedError
 
     def bypass_forward(self, x, scale=1):
         raise NotImplementedError
 
+    def parametrize_forward(self, x: torch.Tensor, *args, **kwargs):
+        return self.get_merged_weight(
+            multiplier=self.multiplier, shape=x.shape, device=x.device
+        )[0].to(x.dtype)
+
     def forward(self, *args, **kwargs):
         raise NotImplementedError
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/boft.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/boft.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
         return inp
 
     def get_diff_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device, diff=True)
         if shape is not None:
             diff = diff.view(shape)
-        return diff
+        return diff, None
 
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device)
         if shape is not None:
             diff = diff.view(shape)
         return diff, None
 
@@ -196,37 +196,47 @@
         else:
             w = self.make_weight(scale, x.device)
             kw_dict = self.kw_dict | {"weight": w, "bias": self.org_module[0].bias}
             return self.op(x, **kw_dict)
 
 
 if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    boft = ButterflyOFTModule(
-        "test", base, 1, 4, 1, weight_decompose=True, factor=8
-    ).cuda()
-    print(boft)
-    test_input = torch.randn(1, 77, 128).cuda()
-    test_output = boft(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qboft = ButterflyOFTModule(
-        "test", base_4bit, 1, 4, 1, weight_decompose=False
-    ).cuda()
-    print(qboft)
-    test_output = qboft(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    boft = ButterflyOFTModule(
-        "test", base, 1, 4, 1, weight_decompose=True, use_tucker=True
-    )
-    print(boft)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = boft(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+    device = torch.device("cuda")
+    module = ButterflyOFTModule
+    with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
+        base = nn.Linear(128, 128).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        print(net)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base_4bit = LinearNF4(128, 128, device="cuda")
+        base_4bit.load_state_dict(base.state_dict())
+        base_4bit.to(device)
+        qnet = module("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
+        print(qnet)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = qnet(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
+        )
+        print(net)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        ).to(device)
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/diag_oft.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/diag_oft.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                 weight = weight + (self.rescale - 1) * org_weight
         return weight
 
     def get_diff_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device, diff=True)
         if shape is not None:
             diff = diff.view(shape)
-        return diff
+        return diff, None
 
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
         diff = self.make_weight(scale=multiplier, device=device)
         if shape is not None:
             diff = diff.view(shape)
         return diff, None
 
@@ -181,31 +181,47 @@
         else:
             w = self.make_weight(scale, x.device)
             kw_dict = self.kw_dict | {"weight": w, "bias": self.org_module[0].bias}
             return self.op(x, **kw_dict)
 
 
 if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    doft = DiagOFTModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
-    print(doft)
-    test_input = torch.randn(1, 77, 128).cuda()
-    test_output = doft(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qdoft = DiagOFTModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
-    print(qdoft)
-    test_output = qdoft(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    doft = DiagOFTModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(doft)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = doft(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+    device = torch.device("cuda")
+    module = DiagOFTModule
+    with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
+        base = nn.Linear(128, 128).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        print(net)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base_4bit = LinearNF4(128, 128, device="cuda")
+        base_4bit.load_state_dict(base.state_dict())
+        base_4bit.to(device)
+        qnet = module("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
+        print(qnet)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = qnet(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
+        )
+        print(net)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        ).to(device)
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/dylora.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/full.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/full.py`

 * *Files 7% similar despite different names*

```diff
@@ -154,22 +154,37 @@
         scale = self.multiplier
         weight, bias = self.make_weight(scale, x.device)
         kw_dict = self.kw_dict | {"weight": weight, "bias": bias}
         return self.op(x, **kw_dict)
 
 
 if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    full = FullModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
-    print(full)
-    test_input = torch.randn(1, 77, 128).cuda()
-    test_output = full(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+    device = torch.device("cuda")
+    module = FullModule
+    with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
+        base = nn.Linear(128, 128).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        print(net)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
 
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    full = FullModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(full)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = full(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
+        )
+        print(net)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        ).to(device)
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/glora.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/glora.py`

 * *Files 9% similar despite different names*

```diff
@@ -165,32 +165,47 @@
         return (
             self.org_forward(x + self.dropout(self.a2(ax_mid)) * self.scale)
             + self.dropout(self.b2(bx_mid)) * self.scale
         )
 
 
 if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    glora = GLoRAModule("test", base, 1, 4, 1, weight_decompose=True).cuda()
-    print(glora)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = glora(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+    device = torch.device("cuda")
+    module = GLoRAModule
+    with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
+        base = nn.Linear(128, 128).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        print(net)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
 
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qglora = GLoRAModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
-    print(qglora)
-    test_input = torch.randn(1, 128).cuda()
-    test_output = qglora(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+        base_4bit = LinearNF4(128, 128, device="cuda")
+        base_4bit.load_state_dict(base.state_dict())
+        base_4bit.to(device)
+        qnet = module("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
+        print(qnet)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = qnet(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
 
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    glora = GLoRAModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(glora)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = glora(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
+        )
+        print(net)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        ).to(device)
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/ia3.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/locon.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/locon.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,19 +179,20 @@
     def get_diff_weight(self, multiplier=1, shape=None, device=None):
         scale = self.scale * multiplier
         diff = self.make_weight(device=device) * scale
         if shape is not None:
             diff = diff.view(shape)
         if device is not None:
             diff = diff.to(device)
-        return diff
+        return diff, None
 
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
-        merged = self.org_module[0].weight.data + self.get_diff_weight(
-            multiplier=multiplier, shape=shape, device=device
+        merged = (
+            self.org_module[0].weight.data
+            + self.get_diff_weight(multiplier=multiplier, shape=shape, device=device)[0]
         )
         if self.wd:
             merged = self.apply_weight_decompose(merged)
         return merged, None
 
     def apply_weight_decompose(self, weight):
         weight = weight.to(self.dora_scale.dtype)
@@ -274,37 +275,46 @@
             return self.op(x, weight, bias, **self.kw_dict)
         else:
             return self.bypass_forward(x, scale=self.multiplier)
 
 
 if __name__ == "__main__":
     device = torch.device("cuda")
+    module = LoConModule
     with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
         base = nn.Linear(128, 128).to(device).half()
-        net = LoConModule("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
         print(net)
         test_input = torch.randn(1, 128).to(device).half()
         test_output = net(test_input)
         torch.sum(test_output).backward()
         print(test_output.shape)
 
         base_4bit = LinearNF4(128, 128, device="cuda")
         base_4bit.load_state_dict(base.state_dict())
         base_4bit.to(device)
-        qnet = LoConModule("test", base_4bit, 1, 4, 1, weight_decompose=False).to(
-            device
-        )
+        qnet = module("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
         print(qnet)
         test_input = torch.randn(1, 128).to(device).half()
         test_output = qnet(test_input)
         torch.sum(test_output).backward()
         print(test_output.shape)
 
         base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
-        net = LoConModule(
-            "test", base, 1, 4, 1, weight_decompose=True, use_tucker=True
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
         )
         print(net)
         test_input = torch.randn(1, 128, 16, 16).to(device).half()
         test_output = net(test_input)
         torch.sum(test_output).backward()
         print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        )
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/loha.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/loha.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,23 +177,24 @@
         return weight
 
     def get_diff_weight(self, multiplier=1, shape=None, device=None):
         scale = self.scale * multiplier
         diff = self.get_weight(shape) * scale
         if device is not None:
             diff = diff.to(device)
-        return diff
+        return diff, None
 
     def get_merged_weight(self, multiplier=1, shape=None, device=None):
-        merged = self.org_module[0].weight.data + self.get_diff_weight(
-            multiplier=multiplier, shape=shape, device=device
+        merged = (
+            self.org_module[0].weight.data
+            + self.get_diff_weight(multiplier=multiplier, shape=shape, device=device)[0]
         )
         if self.wd:
             merged = self.apply_weight_decompose(merged)
-        return merged
+        return merged, None
 
     def apply_weight_decompose(self, weight):
         weight = weight.to(self.dora_scale.dtype)
         weight_norm = (
             weight.transpose(0, 1)
             .reshape(weight.shape[1], -1)
             .norm(dim=1, keepdim=True)
@@ -265,32 +266,46 @@
             if self.wd:
                 weight = self.apply_weight_decompose(weight)
             return self.op(x, weight.view(self.shape), bias, **self.kw_dict)
 
 
 if __name__ == "__main__":
     device = torch.device("cuda")
-    base = nn.Linear(128, 128).to(device)
-    loha = LohaModule("test", base, 1, 4, 1, weight_decompose=True).to(device)
-    print(loha)
-    test_input = torch.randn(1, 128).to(device)
-    test_output = loha(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.to(device)
-    qloha = LohaModule("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
-    print(qloha)
-    test_input = torch.randn(1, 128).to(device)
-    test_output = qloha(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    loha = LohaModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(loha)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = loha(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+    module = LohaModule
+    with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
+        base = nn.Linear(128, 128).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        print(net)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base_4bit = LinearNF4(128, 128, device="cuda")
+        base_4bit.load_state_dict(base.state_dict())
+        base_4bit.to(device)
+        qnet = module("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
+        print(qnet)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = qnet(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
+        )
+        print(net)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        )
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/lokr.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/lokr.py`

 * *Files 14% similar despite different names*

```diff
@@ -258,23 +258,29 @@
             drop = (torch.rand(weight.size(0)) > self.rank_dropout).to(dtype)
             drop = drop.view(-1, *[1] * len(weight.shape[1:]))
             if self.rank_dropout_scale:
                 drop /= drop.mean()
             weight *= drop
         return weight
 
-    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+    def get_diff_weight(self, multiplier=1, shape=None, device=None):
         scale = self.scale * multiplier
         diff = self.get_weight(shape) * scale
         if device is not None:
             diff = diff.to(device)
-        merged = self.org_module[0].weight.data + diff
+        return diff, None
+
+    def get_merged_weight(self, multiplier=1, shape=None, device=None):
+        merged = (
+            self.org_module[0].weight.data
+            + self.get_diff_weight(multiplier=multiplier, shape=shape, device=device)[0]
+        )
         if self.wd:
             merged = self.apply_weight_decompose(merged)
-        return merged
+        return merged, None
 
     def apply_weight_decompose(self, weight):
         weight = weight.to(self.dora_scale.dtype)
         weight_norm = (
             weight.transpose(0, 1)
             .reshape(weight.shape[1], -1)
             .norm(dim=1, keepdim=True)
@@ -390,31 +396,47 @@
 
             if self.wd:
                 weight = self.apply_weight_decompose(weight)
             return self.op(x, weight.view(self.shape), bias, **self.kw_dict)
 
 
 if __name__ == "__main__":
-    base = nn.Linear(128, 128).cuda()
-    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, factor=8).cuda()
-    print(lokr)
-    test_input = torch.randn(1, 77, 128).cuda()
-    test_output = lokr(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base_4bit = LinearNF4(128, 128)
-    base_4bit.load_state_dict(base.state_dict())
-    base_4bit.cuda()
-    qlokr = LokrModule("test", base_4bit, 1, 4, 1, weight_decompose=False).cuda()
-    print(qlokr)
-    test_output = qlokr(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
-
-    base = nn.Conv2d(128, 128, 3, 1, 1)
-    lokr = LokrModule("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True)
-    print(lokr)
-    test_input = torch.randn(1, 128, 16, 16)
-    test_output = lokr(test_input)
-    torch.sum(test_output).backward()
-    print(test_output.shape)
+    device = torch.device("cuda")
+    module = LokrModule
+    with torch.autocast("cuda" if torch.cuda.is_available() else "cpu"):
+        base = nn.Linear(128, 128).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True).to(device)
+        print(net)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base_4bit = LinearNF4(128, 128, device="cuda")
+        base_4bit.load_state_dict(base.state_dict())
+        base_4bit.to(device)
+        qnet = module("test", base_4bit, 1, 4, 1, weight_decompose=False).to(device)
+        print(qnet)
+        test_input = torch.randn(1, 128).to(device).half()
+        test_output = qnet(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module("test", base, 1, 4, 1, weight_decompose=True, use_tucker=True).to(
+            device
+        )
+        print(net)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = net(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
+
+        base = nn.Conv2d(128, 128, 3, 1, 1).to(device).half()
+        net = module.parametrize(
+            base, "weight", 1, 4, 1, weight_decompose=True, use_tucker=True
+        )
+        print(base)
+        test_input = torch.randn(1, 128, 16, 16).to(device).half()
+        test_output = base(test_input)
+        torch.sum(test_output).backward()
+        print(test_output.shape)
```

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/modules/norms.py` & `lycoris_lora-3.0.0.dev3/lycoris/modules/norms.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/utils/__init__.py` & `lycoris_lora-3.0.0.dev3/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/utils/logger.py` & `lycoris_lora-3.0.0.dev3/lycoris/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris/wrapper.py` & `lycoris_lora-3.0.0.dev3/lycoris/wrapper.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-3.0.0.dev3/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev2/setup.py` & `lycoris_lora-3.0.0.dev3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lycoris_lora",
     packages=find_packages(),
-    version="3.0.0.dev2",
+    version="3.0.0.dev3",
     url="https://github.com/KohakuBlueleaf/LyCORIS",
     description="Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
     author="Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=[
         "torch",
-        "safetensors",
-        "diffusers",
-        "transformers",
         "einops",
         "toml",
     ],
     python_requires=">=3.10",
 )
```


# Comparing `tmp/alphafold3_pytorch-0.0.8.tar.gz` & `tmp/alphafold3_pytorch-0.0.9.tar.gz`

## Comparing `alphafold3_pytorch-0.0.8.tar` & `alphafold3_pytorch-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/.env.sample
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0    80699 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/tests/test_af3.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/LICENSE
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.env.sample
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0    80825 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/tests/test_af3.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/README.md
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.9/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.0.8/alphafold3.png` & `alphafold3_pytorch-0.0.9/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/.github/workflows/publish.yml` & `alphafold3_pytorch-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.0.9/alphafold3_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.0.9/alphafold3_pytorch/alphafold3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1736,28 +1736,34 @@
             network_condition_kwargs = network_condition_kwargs
         )
 
         # main diffusion mse loss
 
         losses = F.mse_loss(denoised_atom_pos, normalized_atom_pos, reduction = 'none')
 
-        losses = losses * self.loss_weight(padded_sigmas)
+        loss_weights = self.loss_weight(padded_sigmas)
+
+        losses = losses * loss_weights
 
         loss = losses[atom_mask].mean()
 
         # proposed extra bond loss during finetuning
 
         if add_bond_loss:
+            atompair_mask = einx.logical_and('b i, b j -> b i j', atom_mask, atom_mask)
+
             denoised_cdist = torch.cdist(denoised_atom_pos, denoised_atom_pos, p = 2)
             normalized_cdist = torch.cdist(normalized_atom_pos, normalized_atom_pos, p = 2)
 
             bond_losses = F.mse_loss(denoised_cdist, normalized_cdist, reduction = 'none')
-            atompair_mask = einx.logical_and('b i, b j -> b i j', atom_mask, atom_mask)
+            bond_losses = bond_losses * loss_weights
+
+            bond_loss = bond_losses[atompair_mask].mean()
 
-            loss = loss + bond_losses[atompair_mask].mean()
+            loss = loss + bond_loss
 
         # proposed auxiliary smooth lddt loss
 
         if add_smooth_lddt_loss:
             assert exists(additional_residue_feats)
             w = self.net.atoms_per_window
```

### Comparing `alphafold3_pytorch-0.0.8/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.0.9/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.0.9/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.0.9/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/tests/test_af3.py` & `alphafold3_pytorch-0.0.9/tests/test_af3.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/.gitignore` & `alphafold3_pytorch-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/LICENSE` & `alphafold3_pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/README.md` & `alphafold3_pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.8/pyproject.toml` & `alphafold3_pytorch-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.0.8"
+version = "0.0.9"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
@@ -23,17 +23,17 @@
 ]
 
 dependencies = [
     "beartype",
     "einops>=0.8.0",
     "einx>=0.2.2",
     "environs",
+    "jaxtyping>=0.2.28",
     "torch>=2.1",
     "tqdm",
-    "jaxtyping>=0.2.28"
 ]
 
 [project.urls]
 Homepage = "https://pypi.org/project/alphafold3-pytorch/"
 Repository = "https://github.com/lucidrains/alphafold3-pytorch"
 
 [project.optional-dependencies]
```

### Comparing `alphafold3_pytorch-0.0.8/PKG-INFO` & `alphafold3_pytorch-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.8 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.9 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```


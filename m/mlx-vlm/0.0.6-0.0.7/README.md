# Comparing `tmp/mlx_vlm-0.0.6.tar.gz` & `tmp/mlx_vlm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_vlm-0.0.6.tar", last modified: Fri May 24 15:59:32 2024, max compression
+gzip compressed data, was "mlx_vlm-0.0.7.tar", last modified: Sat May 25 19:18:35 2024, max compression
```

## Comparing `mlx_vlm-0.0.6.tar` & `mlx_vlm-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/chat_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/idefics2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/idefics2/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/llava/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/llava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.282876 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/nanoLlava.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/paligemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/models/paligemma/vision.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/prompt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/sample_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/mlx_vlm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/tokenizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/mlx_vlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/mlx_vlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 15:59:32.000000 mlx_vlm-0.0.6/mlx_vlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:59:32.286876 mlx_vlm-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-24 15:59:24.000000 mlx_vlm-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.716357 mlx_vlm-0.0.7/mlx_vlm/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/chat_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.716357 mlx_vlm-0.0.7/mlx_vlm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.716357 mlx_vlm-0.0.7/mlx_vlm/models/idefics2/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/idefics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/idefics2/idefics2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/idefics2/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/idefics2/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.716357 mlx_vlm-0.0.7/mlx_vlm/models/llava/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/llava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/llava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/llava/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/llava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/nanoLlava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/mlx_vlm/models/paligemma/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/paligemma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/paligemma/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/paligemma/paligemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/models/paligemma/vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/prompt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/sample_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/mlx_vlm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/tokenizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28071 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/mlx_vlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/mlx_vlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 19:18:35.000000 mlx_vlm-0.0.7/mlx_vlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-25 19:18:35.000000 mlx_vlm-0.0.7/mlx_vlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:18:35.000000 mlx_vlm-0.0.7/mlx_vlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-25 19:18:35.000000 mlx_vlm-0.0.7/mlx_vlm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 19:18:35.000000 mlx_vlm-0.0.7/mlx_vlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 19:18:35.000000 mlx_vlm-0.0.7/mlx_vlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:18:35.720358 mlx_vlm-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-25 19:18:28.000000 mlx_vlm-0.0.7/setup.py
```

### Comparing `mlx_vlm-0.0.6/LICENSE` & `mlx_vlm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/PKG-INFO` & `mlx_vlm-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_vlm-0.0.6/README.md` & `mlx_vlm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/chat_ui.py` & `mlx_vlm-0.0.7/mlx_vlm/chat_ui.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/convert.py` & `mlx_vlm-0.0.7/mlx_vlm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/generate.py` & `mlx_vlm-0.0.7/mlx_vlm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/base.py` & `mlx_vlm-0.0.7/mlx_vlm/models/base.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/idefics2/idefics2.py` & `mlx_vlm-0.0.7/mlx_vlm/models/idefics2/idefics2.py`

 * *Files 13% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             keys = mx.concatenate([key_cache, keys], axis=2)
             values = mx.concatenate([value_cache, values], axis=2)
 
         output = mx.fast.scaled_dot_product_attention(
             queries, keys, values, scale=self.scale
         )
         output = output.transpose(0, 2, 1, 3).reshape(B, L, -1)
-        return self.o_proj(output), (keys, values)
+        return self.o_proj(output)
 
 
 class Idefics2PerceiverLayer(nn.Module):
     def __init__(self, config: ModelConfig):
         super().__init__()
         self.hidden_size = config.text_config.hidden_size
         self.n_latents = config.perceiver_config.resampler_n_latents
@@ -128,15 +128,15 @@
         x: mx.array,
         hidden_states: mx.array,
         mask: Optional[mx.array] = None,
     ) -> mx.array:
         latents = self.input_latents_norm(x)
         context = self.input_context_norm(hidden_states)
 
-        latents, _ = self.self_attn(latents, context, mask=mask)
+        latents = self.self_attn(latents, context, mask=mask)
 
         latents = x + latents
         r = latents
 
         latents = self.post_attention_layernorm(latents)
         latents = self.mlp(latents)
         latents = r + latents
@@ -215,38 +215,44 @@
 
         inputs_embeds = self.language_model.embed_tokens(input_ids)
 
         pooler_output, embeddings, hidden_state = self.vision_model(
             pixel_values[0].transpose(0, 2, 3, 1), output_hidden_states=True
         )
 
-        image_features = hidden_state[-1].astype(pixel_values.dtype)
+        image_features = pooler_output[None, :].astype(pixel_values.dtype)
 
         image_features = self.connector(image_features, mask=None)
 
         final_inputs_embeds = self._prepare_inputs_for_multimodal(
             image_features, inputs_embeds, input_ids
         )
         return final_inputs_embeds
 
     def _prepare_inputs_for_multimodal(self, image_features, inputs_embeds, input_ids):
-
         image_token_index = self.config.image_token_index
         num_images, num_image_patches, embed_dim = image_features.shape
-        special_image_token_mask = input_ids == image_token_index
-
-        reshaped_image_hidden_states = image_features.reshape(-1, embed_dim)
 
-        # Find the positions of the <image> tokens in the input_ids
-        image_token_positions = mx.array(np.where(special_image_token_mask)[1])
+        # Positions of <image> tokens in input_ids, assuming batch size is 1
+        image_positions = np.where(input_ids[0] == image_token_index)[0].tolist()
 
-        # Advanced indexing to place reshaped image features at the corresponding positions
-        inputs_embeds[0, image_token_positions, :] = reshaped_image_hidden_states
+        text_segments = []
+        start_idx = 0
 
-        return inputs_embeds
+        for position in image_positions:
+            text_segments.append(inputs_embeds[:, start_idx:position])
+            start_idx = position + 1
+
+        image_embeddings = mx.split(image_features, image_features.shape[0])
+        final_embeddings = [v for p in zip(text_segments, image_embeddings) for v in p]
+        final_embeddings += [inputs_embeds[:, start_idx:]]
+
+        # Create a final embedding of shape
+        # (1, num_image_patches*num_images + sequence_len, embed_dim)
+        return mx.concatenate(final_embeddings, axis=1)
 
     def __call__(
         self, input_ids: mx.array, pixel_values: mx.array, mask: mx.array, cache=None
     ):
         input_embeddings = self.get_input_embeddings(input_ids, pixel_values)
         logits, cache = self.language_model(
             inputs=input_ids, cache=cache, inputs_embeds=input_embeddings
```

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/idefics2/language.py` & `mlx_vlm-0.0.7/mlx_vlm/models/idefics2/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     hidden_size: int
     num_hidden_layers: int
     intermediate_size: int
     num_attention_heads: int
     rms_norm_eps: float
     vocab_size: int
     num_key_value_heads: int
-    rope_theta: float = 10000.0
+    rope_theta: float = 1000000.0
     rope_traditional: bool = False
     tie_word_embeddings: bool = False
 
     @classmethod
     def from_dict(cls, params):
         return cls(
             **{
```

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/idefics2/vision.py` & `mlx_vlm-0.0.7/mlx_vlm/models/idefics2/vision.py`

 * *Files 11% similar despite different names*

```diff
@@ -131,14 +131,31 @@
 
 
 class Encoder(nn.Module):
     def __init__(self, config: VisionConfig):
         super().__init__()
         self.layers = [EncoderLayer(config) for _ in range(config.num_hidden_layers)]
 
+    def __call__(
+        self,
+        x: mx.array,
+        output_hidden_states: Optional[bool] = None,
+        mask: Optional[mx.array] = None,
+    ) -> mx.array:
+        encoder_states = (x,) if output_hidden_states else None
+        h = x
+        for l in self.layers:
+            x = l(x, mask=mask)
+            if output_hidden_states:
+                encoder_states = encoder_states + (x,)
+
+            h = x[0]
+
+        return (h, encoder_states)
+
 
 class VisionEmbeddings(nn.Module):
     def __init__(self, config: VisionConfig):
         super().__init__()
         self.config = config
         self.embed_dim = config.hidden_size
         self.image_size = config.image_size
@@ -159,59 +176,38 @@
         B, H, W, C = x.shape
         patch_embeddings = self.patch_embedding(x)
         patch_embeddings = mx.flatten(patch_embeddings, start_axis=1, end_axis=2)
         max_nb_patches_h, max_nb_patches_w = (
             H // self.patch_size,
             W // self.patch_size,
         )
-        N = max_nb_patches_h * max_nb_patches_w
-        boundaries = np.arange(1 / self.num_patches, 1.0, 1 / self.num_patches)
-        sequence = np.zeros((max_nb_patches_h * max_nb_patches_w))
-
-        position_ids = np.zeros_like(mask, dtype=int)
-
-        def bucketize(values, boundaries):
-            idx = (
-                np.digitize(values, boundaries, right=True) - 1
-            )  # adjust indices to match 'right=True'
-            idx[idx == -1] = 0  # Handle any -1 indices that may appear
-            return idx
+        boundaries = np.linspace(
+            1 / self.num_patches, 1.0, self.num_patches, endpoint=False
+        )
+        position_ids = np.zeros((B, max_nb_patches_h * max_nb_patches_w), dtype=int)
 
-        for batch_idx, p_attn_mask in enumerate(np.array(mask)):
+        for batch_idx, p_attn_mask in enumerate(mask):
+            p_attn_mask = np.array(p_attn_mask)
             nb_patches_h = p_attn_mask[:, 0].sum()
-            nb_patches_w = p_attn_mask[0].sum()
+            nb_patches_w = p_attn_mask[0, :].sum()
 
-            fractional_coords_h = np.linspace(0, 1 - 1e-6, nb_patches_h)
-            fractional_coords_w = np.linspace(0, 1 - 1e-6, nb_patches_w)
+            fractional_coords_h = np.linspace(0, 1, nb_patches_h, endpoint=False)
+            fractional_coords_w = np.linspace(0, 1, nb_patches_w, endpoint=False)
 
-            bucket_coords_h = bucketize(fractional_coords_h, boundaries)
-            bucket_coords_w = bucketize(fractional_coords_w, boundaries)
+            bucket_coords_h = (
+                np.digitize(fractional_coords_h, boundaries, right=True) - 1
+            )
+            bucket_coords_w = (
+                np.digitize(fractional_coords_w, boundaries, right=True) - 1
+            )
 
             pos_ids = (
                 bucket_coords_h[:, None] * self.num_patches + bucket_coords_w
             ).flatten()
-
-            flat_indices = np.flatnonzero(
-                p_attn_mask
-            )  # Get flat indices where p_attn_mask is non-zero
-
-            # Ensure pos_ids has sufficient length
-            if len(pos_ids) < len(flat_indices):
-                raise ValueError(
-                    "Not enough pos_ids generated: {} needed, but only {} generated.".format(
-                        len(flat_indices), len(pos_ids)
-                    )
-                )
-
-            # Apply position ids to the positions indicated by p_attn_mask
-            position_ids[batch_idx].flat[flat_indices] = pos_ids[
-                : len(flat_indices) + 1
-            ]
-
-        position_ids = position_ids.reshape(B, N)
+            position_ids[batch_idx][p_attn_mask.reshape(-1)] = pos_ids
 
         embeddings = patch_embeddings
         embeddings += self.position_embedding(mx.array(position_ids))
         return embeddings
 
 
 class VisionModel(nn.Module):
@@ -242,24 +238,19 @@
                     D // patch_size,
                 ),
                 dtype=mx.bool_,
             )
 
         x = self.embeddings(x, mask=patch_attention_mask)
 
-        encoder_states = (x,) if output_hidden_states else None
-
-        for layers in self.encoder.layers:
-            x = layers(x, mask=None)
-            if output_hidden_states:
-                encoder_states = encoder_states + (x,)
+        encoder_outputs = self.encoder(x=x, output_hidden_states=output_hidden_states)
 
-        pooler_output = self.post_layernorm(x[:, -1, :])
+        pooler_output = self.post_layernorm(encoder_outputs[0])
 
-        return pooler_output, x, encoder_states
+        return pooler_output, x, encoder_outputs[-1]
 
     def sanitize(self, weights):
         sanitized_weights = {}
         for k, v in weights.items():
             if "patch_embedding.weight" in k:
                 # PyTorch conv2d weight tensors have shape:
                 #   [out_channels, in_channels, kH, KW]
```

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/llava/language.py` & `mlx_vlm-0.0.7/mlx_vlm/models/llava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/llava/llava.py` & `mlx_vlm-0.0.7/mlx_vlm/models/llava/llava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/llava/vision.py` & `mlx_vlm-0.0.7/mlx_vlm/models/llava/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/language.py` & `mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/nanoLlava.py` & `mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/nanoLlava.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/nanoLlava/vision.py` & `mlx_vlm-0.0.7/mlx_vlm/models/nanoLlava/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/paligemma/language.py` & `mlx_vlm-0.0.7/mlx_vlm/models/paligemma/language.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/paligemma/paligemma.py` & `mlx_vlm-0.0.7/mlx_vlm/models/paligemma/paligemma.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/models/paligemma/vision.py` & `mlx_vlm-0.0.7/mlx_vlm/models/paligemma/vision.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/prompt_utils.py` & `mlx_vlm-0.0.7/mlx_vlm/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/sample_utils.py` & `mlx_vlm-0.0.7/mlx_vlm/sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/tests/test_models.py` & `mlx_vlm-0.0.7/mlx_vlm/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/tokenizer_utils.py` & `mlx_vlm-0.0.7/mlx_vlm/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm/utils.py` & `mlx_vlm-0.0.7/mlx_vlm/utils.py`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/mlx_vlm.egg-info/PKG-INFO` & `mlx_vlm-0.0.7/mlx_vlm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-vlm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Vision LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/Blaizzy/mlx-vlm
 Author: Prince Canuma
 Author-email: prince.gdt@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx_vlm-0.0.6/mlx_vlm.egg-info/SOURCES.txt` & `mlx_vlm-0.0.7/mlx_vlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx_vlm-0.0.6/setup.py` & `mlx_vlm-0.0.7/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/vbinsta-0.1.5.tar.gz` & `tmp/vbinsta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbinsta-0.1.5.tar", max compression
+gzip compressed data, was "vbinsta-0.1.6.tar", max compression
```

## Comparing `vbinsta-0.1.5.tar` & `vbinsta-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.5/README.md
--rw-r--r--   0        0        0      368 2024-05-25 17:25:19.654738 vbinsta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.5/vbinsta/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.5/vbinsta/__main__.py
--rw-r--r--   0        0        0     1236 2024-05-25 15:57:02.621318 vbinsta-0.1.5/vbinsta/choice_option.py
--rw-r--r--   0        0        0     3605 2024-05-25 17:25:23.183185 vbinsta-0.1.5/vbinsta/function_gpt.py
--rw-r--r--   0        0        0     2725 2024-05-25 17:25:26.416875 vbinsta-0.1.5/vbinsta/functions.py
--rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.5/vbinsta/main.py
--rw-r--r--   0        0        0     4178 2024-05-25 17:25:25.115487 vbinsta-0.1.5/vbinsta/token_cost_calculations.py
--rw-r--r--   0        0        0     2302 2024-05-25 16:07:03.530032 vbinsta-0.1.5/vbinsta/upload.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.6/README.md
+-rw-r--r--   0        0        0      368 2024-05-25 17:45:18.890072 vbinsta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.6/vbinsta/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.6/vbinsta/__main__.py
+-rw-r--r--   0        0        0     1236 2024-05-25 15:57:02.621318 vbinsta-0.1.6/vbinsta/choice_option.py
+-rw-r--r--   0        0        0     3605 2024-05-25 17:25:23.183185 vbinsta-0.1.6/vbinsta/function_gpt.py
+-rw-r--r--   0        0        0     2725 2024-05-25 17:25:26.416875 vbinsta-0.1.6/vbinsta/functions.py
+-rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.6/vbinsta/main.py
+-rw-r--r--   0        0        0     4178 2024-05-25 17:25:25.115487 vbinsta-0.1.6/vbinsta/token_cost_calculations.py
+-rw-r--r--   0        0        0     2304 2024-05-25 17:45:13.207620 vbinsta-0.1.6/vbinsta/upload.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.6/PKG-INFO
```

### Comparing `vbinsta-0.1.5/vbinsta/choice_option.py` & `vbinsta-0.1.6/vbinsta/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.5/vbinsta/function_gpt.py` & `vbinsta-0.1.6/vbinsta/function_gpt.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.5/vbinsta/functions.py` & `vbinsta-0.1.6/vbinsta/functions.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.5/vbinsta/token_cost_calculations.py` & `vbinsta-0.1.6/vbinsta/token_cost_calculations.py`

 * *Files identical despite different names*

### Comparing `vbinsta-0.1.5/vbinsta/upload.py` & `vbinsta-0.1.6/vbinsta/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         image[0], prompt, model, os.getenv('OPENAI_API_KEY'), 1500)
     # Verify if the login was successful
     if client.user_id:
         print("Login successful!: @10xphysics")
         if len(image) == 1:
             with Console().status("Uploading image...", spinner="dots"):
                 upload_single_image(
-                    client, image[0], caption + "\n\n Captions generated using gpt-4o!")
+                    client, image[0:1], caption + "\n\n Captions generated using gpt-4o!")
         if len(image) > 1:
             with Console().status("Uploading carousel...", spinner="dots"):
                 upload_carousel(client, image, caption +
                                 "\n\n Captions generated using gpt-4o!")
 
     else:
         print("Login failed.")
```


# Comparing `tmp/jetson_examples-0.0.8.tar.gz` & `tmp/jetson_examples-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson_examples-0.0.8.tar", last modified: Sat May 11 08:42:04 2024, max compression
+gzip compressed data, was "jetson_examples-0.1.0.tar", last modified: Sat May 25 08:53:18 2024, max compression
```

## Comparing `jetson_examples-0.0.8.tar` & `jetson_examples-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,68 @@
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1066 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/LICENSE
--rw-r--r--   0 nvidia    (1001) nvidia    (1001)     4731 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/PKG-INFO
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     4081 2024-05-11 03:18:46.000000 jetson_examples-0.0.8/README.md
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/jetson_examples.egg-info/
--rw-r--r--   0 nvidia    (1001) nvidia    (1001)     4731 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/PKG-INFO
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      950 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/SOURCES.txt
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)        1 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/dependency_links.txt
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       58 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/entry_points.txt
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       27 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/top_level.txt
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1081 2024-05-11 08:38:00.000000 jetson_examples-0.0.8/pyproject.toml
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       22 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/__init__.py
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1821 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/main.py
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      134 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      127 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/check.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/live-llava/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)    10137 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/live-llava/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llama3/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      226 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llama3/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llava/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      148 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llava/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llava-v1.5-7b/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      147 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llava-v1.5-7b/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llava-v1.6-vicuna-7b/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      165 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/nanodb/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      247 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/nanodb/readme.md
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     2571 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/nanodb/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/nanoowl/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      161 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/nanoowl/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/ollama/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      143 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/ollama/run.sh
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1370 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/stable-diffusion-webui/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       57 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/stable-diffusion-webui/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/text-generation-webui/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      304 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/text-generation-webui/run.sh
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      900 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/update.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/whisper/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       43 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/whisper/run.sh
-drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/yolov8-counter/
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1500 2024-05-11 03:18:28.000000 jetson_examples-0.0.8/reComputer/scripts/yolov8-counter/readme.md
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      817 2024-05-11 02:05:15.000000 jetson_examples-0.0.8/reComputer/scripts/yolov8-counter/run.sh
--rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       38 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/setup.cfg
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-05-25 08:46:19.000000 jetson_examples-0.1.0/LICENSE
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     4846 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     4196 2024-05-25 08:46:19.000000 jetson_examples-0.1.0/README.md
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/jetson_examples.egg-info/
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     4846 2024-05-25 08:53:18.000000 jetson_examples-0.1.0/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1736 2024-05-25 08:53:18.000000 jetson_examples-0.1.0/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-05-25 08:53:18.000000 jetson_examples-0.1.0/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-05-25 08:53:18.000000 jetson_examples-0.1.0/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       27 2024-05-25 08:53:18.000000 jetson_examples-0.1.0/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1081 2024-05-25 08:48:57.000000 jetson_examples-0.1.0/pyproject.toml
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       22 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/__init__.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2088 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/main.py
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      237 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      127 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/check.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      898 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/clean.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/live-llava/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/live-llava/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    10137 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/live-llava/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/llama3/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llama3/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      328 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llama3/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/llava/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       70 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/llava-v1.5-7b/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava-v1.5-7b/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava-v1.5-7b/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/llava-v1.6-vicuna-7b/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava-v1.6-vicuna-7b/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      269 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/nanodb/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/nanodb/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      247 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/nanodb/readme.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2571 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/nanodb/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.094819 jetson_examples-0.1.0/reComputer/scripts/nanoowl/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/nanoowl/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      264 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/nanoowl/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/ollama/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/ollama/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      246 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/ollama/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1032 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/stable-diffusion-webui/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/stable-diffusion-webui/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/stable-diffusion-webui/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/text-generation-webui/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/text-generation-webui/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      407 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/text-generation-webui/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      900 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/update.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/whisper/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/whisper/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      146 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/whisper/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/yolov8-rail-inspection/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2008 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8-rail-inspection/readme.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      809 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8-rail-inspection/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      167 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/Dockerfile
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1122 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/README.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1307 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/app.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      130 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/templates/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      524 2024-05-25 08:44:32.000000 jetson_examples-0.1.0/reComputer/scripts/yolov8:detect/templates/index.html
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-05-25 08:53:18.098819 jetson_examples-0.1.0/setup.cfg
```

### Comparing `jetson_examples-0.0.8/LICENSE` & `jetson_examples-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.8/PKG-INFO` & `jetson_examples-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,100 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.8
+Version: 0.1.0
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# jetson-examples
+
 <div align="center">
   <img alt="jetson" width="1200px" src="https://files.seeedstudio.com/wiki/reComputer-Jetson/jetson-examples/Jetson1200x300.png">
 </div>
 
-# jetson-examples
-
 [![Discord](https://dcbadge.vercel.app/api/server/5BQCkty7vN?style=flat&compact=true)](https://discord.gg/5BQCkty7vN)
 
-This repository provides examples for running AI models and applications on NVIDIA Jetson devices.  For generative AI, it supports a variety of examples including text generation, image generation, vision transformers, vector databases, and audio models.
-To run the examples, you need to install the jetson-examples package and use the Seeed Studio [reComputer](https://www.seeedstudio.com/reComputer-J4012-p-5586.html), the edge AI device powered by Jetson Orin.  The repo aims to make it easy to deploy state-of-the-art AI models, with just one line of command, on Jetson devices for tasks like language understanding, computer vision, and multimodal processing.
+This repository provides examples for running AI models and applications on [NVIDIA Jetson devices](https://www.seeedstudio.com/reComputer-J4012-p-5586.html) with a single command.
+
+This repo builds upon the work of the [jetson-containers](https://github.com/dusty-nv/jetson-containers), which provides a modular container build system for various AI/ML packages on NVIDIA Jetson devices. 
+
+## Features
+- 🚀 **Easy Deployment:** Deploy state-of-the-art AI models on Jetson devices in one line.
+- 🔄 **Versatile Examples:** Supports text generation, image generation, vision transformers, computer vision and so on.
+- ⚡ **Optimized for Jetson:** Leverages Nvidia Jetson hardware for efficient performance.
 
-This repo builds upon the work of the [Jetson Containers](https://github.com/dusty-nv/jetson-containers), which provides a modular container build system for various AI/ML packages on NVIDIA Jetson devices. It also leverages resources and tutorials from the [Jetson Generative AI Lab](https://www.jetson-ai-lab.com/index.html), which showcases bringing generative AI to the edge, powered by Jetson hardware.
 
 ## Install
+To install the package, run:
 
 ```sh
-pip install jetson-examples
+pip3 install jetson-examples
 ```
 
-- [more installation methods](./docs/install.md)
-- If you have already installed, you can use `pip install jetson-examples --upgrade` to update.
+> Notes: 
+> - Check [here](./docs/install.md) for more installation methods 
+> - To upgrade to the latest version, use:  `pip3 install jetson-examples --upgrade`.
 
-## Quickstart
 
-To run and chat with [LLaVA](https://www.jetson-ai-lab.com/tutorial_llava.html):
+
+## Quickstart
+To run and chat with [LLaVA](https://www.jetson-ai-lab.com/tutorial_llava.html), execute:
 
 ```sh
 reComputer run llava
 ```
+<div align="center">
+  <img alt="jetson" width="1200px" src="./docs/assets/llava.png">
+</div>
 
 ## Example list
 
-reComputer supports a list of examples from [jetson-ai-lab](https://www.jetson-ai-lab.com/)
-
 Here are some examples that can be run:
 
-| Example                                          | Type                     | Model/Data Size | Image Size | Command                                 |
+| Example                                          | Type                     | Model/Data Size | Docker Image Size | Command                                 |
 | ------------------------------------------------ | ------------------------ | --------------- | ---------- | --------------------------------------- |
 | 🆕 llama3                                         | Text (LLM)               | 4.9GB           | 10.5GB     | `reComputer run llama3`                 |
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-| [yolov8-counter](/reComputer/scripts/yolov8-counter/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8_counter`  |
+| [🆕 yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
-Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
+## Development
+Want to add your own example? Check out the [development guide](./docs/develop.md).
+
+We welcome contributions to improve jetson-examples! If you have an example you'd like to share, please submit a pull request. Thank you to all of our contributors! 🙏
 
 ## TODO List
 
 - [ ] check disk space enough or not before run
 - [ ] allow to setting some configs, such as `BASE_PATH`
 - [ ] detect host environment and install what we need
 - [ ] support jetson-containers update
 - [ ] all type jetson support checking list
 - [ ] better table to show example's difference
 - [ ] try jetpack 6.0
+
+
+## License
+This project is licensed under the MIT License. 
+
+## Resources
+- https://github.com/dusty-nv/jetson-containers
+- https://www.jetson-ai-lab.com/
+- https://www.ultralytics.com/
+
```

### Comparing `jetson_examples-0.0.8/README.md` & `jetson_examples-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,85 @@
+# jetson-examples
+
 <div align="center">
   <img alt="jetson" width="1200px" src="https://files.seeedstudio.com/wiki/reComputer-Jetson/jetson-examples/Jetson1200x300.png">
 </div>
 
-# jetson-examples
-
 [![Discord](https://dcbadge.vercel.app/api/server/5BQCkty7vN?style=flat&compact=true)](https://discord.gg/5BQCkty7vN)
 
-This repository provides examples for running AI models and applications on NVIDIA Jetson devices.  For generative AI, it supports a variety of examples including text generation, image generation, vision transformers, vector databases, and audio models.
-To run the examples, you need to install the jetson-examples package and use the Seeed Studio [reComputer](https://www.seeedstudio.com/reComputer-J4012-p-5586.html), the edge AI device powered by Jetson Orin.  The repo aims to make it easy to deploy state-of-the-art AI models, with just one line of command, on Jetson devices for tasks like language understanding, computer vision, and multimodal processing.
+This repository provides examples for running AI models and applications on [NVIDIA Jetson devices](https://www.seeedstudio.com/reComputer-J4012-p-5586.html) with a single command.
+
+This repo builds upon the work of the [jetson-containers](https://github.com/dusty-nv/jetson-containers), which provides a modular container build system for various AI/ML packages on NVIDIA Jetson devices. 
+
+## Features
+- 🚀 **Easy Deployment:** Deploy state-of-the-art AI models on Jetson devices in one line.
+- 🔄 **Versatile Examples:** Supports text generation, image generation, vision transformers, computer vision and so on.
+- ⚡ **Optimized for Jetson:** Leverages Nvidia Jetson hardware for efficient performance.
 
-This repo builds upon the work of the [Jetson Containers](https://github.com/dusty-nv/jetson-containers), which provides a modular container build system for various AI/ML packages on NVIDIA Jetson devices. It also leverages resources and tutorials from the [Jetson Generative AI Lab](https://www.jetson-ai-lab.com/index.html), which showcases bringing generative AI to the edge, powered by Jetson hardware.
 
 ## Install
+To install the package, run:
 
 ```sh
-pip install jetson-examples
+pip3 install jetson-examples
 ```
 
-- [more installation methods](./docs/install.md)
-- If you have already installed, you can use `pip install jetson-examples --upgrade` to update.
+> Notes: 
+> - Check [here](./docs/install.md) for more installation methods 
+> - To upgrade to the latest version, use:  `pip3 install jetson-examples --upgrade`.
 
-## Quickstart
 
-To run and chat with [LLaVA](https://www.jetson-ai-lab.com/tutorial_llava.html):
+
+## Quickstart
+To run and chat with [LLaVA](https://www.jetson-ai-lab.com/tutorial_llava.html), execute:
 
 ```sh
 reComputer run llava
 ```
+<div align="center">
+  <img alt="jetson" width="1200px" src="./docs/assets/llava.png">
+</div>
 
 ## Example list
 
-reComputer supports a list of examples from [jetson-ai-lab](https://www.jetson-ai-lab.com/)
-
 Here are some examples that can be run:
 
-| Example                                          | Type                     | Model/Data Size | Image Size | Command                                 |
+| Example                                          | Type                     | Model/Data Size | Docker Image Size | Command                                 |
 | ------------------------------------------------ | ------------------------ | --------------- | ---------- | --------------------------------------- |
 | 🆕 llama3                                         | Text (LLM)               | 4.9GB           | 10.5GB     | `reComputer run llama3`                 |
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-| [yolov8-counter](/reComputer/scripts/yolov8-counter/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8_counter`  |
+| [🆕 yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
-Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
+## Development
+Want to add your own example? Check out the [development guide](./docs/develop.md).
+
+We welcome contributions to improve jetson-examples! If you have an example you'd like to share, please submit a pull request. Thank you to all of our contributors! 🙏
 
 ## TODO List
 
 - [ ] check disk space enough or not before run
 - [ ] allow to setting some configs, such as `BASE_PATH`
 - [ ] detect host environment and install what we need
 - [ ] support jetson-containers update
 - [ ] all type jetson support checking list
 - [ ] better table to show example's difference
 - [ ] try jetpack 6.0
+
+
+## License
+This project is licensed under the MIT License. 
+
+## Resources
+- https://github.com/dusty-nv/jetson-containers
+- https://www.jetson-ai-lab.com/
+- https://www.ultralytics.com/
+
```

### Comparing `jetson_examples-0.0.8/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.1.0/jetson_examples.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,100 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.8
+Version: 0.1.0
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# jetson-examples
+
 <div align="center">
   <img alt="jetson" width="1200px" src="https://files.seeedstudio.com/wiki/reComputer-Jetson/jetson-examples/Jetson1200x300.png">
 </div>
 
-# jetson-examples
-
 [![Discord](https://dcbadge.vercel.app/api/server/5BQCkty7vN?style=flat&compact=true)](https://discord.gg/5BQCkty7vN)
 
-This repository provides examples for running AI models and applications on NVIDIA Jetson devices.  For generative AI, it supports a variety of examples including text generation, image generation, vision transformers, vector databases, and audio models.
-To run the examples, you need to install the jetson-examples package and use the Seeed Studio [reComputer](https://www.seeedstudio.com/reComputer-J4012-p-5586.html), the edge AI device powered by Jetson Orin.  The repo aims to make it easy to deploy state-of-the-art AI models, with just one line of command, on Jetson devices for tasks like language understanding, computer vision, and multimodal processing.
+This repository provides examples for running AI models and applications on [NVIDIA Jetson devices](https://www.seeedstudio.com/reComputer-J4012-p-5586.html) with a single command.
+
+This repo builds upon the work of the [jetson-containers](https://github.com/dusty-nv/jetson-containers), which provides a modular container build system for various AI/ML packages on NVIDIA Jetson devices. 
+
+## Features
+- 🚀 **Easy Deployment:** Deploy state-of-the-art AI models on Jetson devices in one line.
+- 🔄 **Versatile Examples:** Supports text generation, image generation, vision transformers, computer vision and so on.
+- ⚡ **Optimized for Jetson:** Leverages Nvidia Jetson hardware for efficient performance.
 
-This repo builds upon the work of the [Jetson Containers](https://github.com/dusty-nv/jetson-containers), which provides a modular container build system for various AI/ML packages on NVIDIA Jetson devices. It also leverages resources and tutorials from the [Jetson Generative AI Lab](https://www.jetson-ai-lab.com/index.html), which showcases bringing generative AI to the edge, powered by Jetson hardware.
 
 ## Install
+To install the package, run:
 
 ```sh
-pip install jetson-examples
+pip3 install jetson-examples
 ```
 
-- [more installation methods](./docs/install.md)
-- If you have already installed, you can use `pip install jetson-examples --upgrade` to update.
+> Notes: 
+> - Check [here](./docs/install.md) for more installation methods 
+> - To upgrade to the latest version, use:  `pip3 install jetson-examples --upgrade`.
 
-## Quickstart
 
-To run and chat with [LLaVA](https://www.jetson-ai-lab.com/tutorial_llava.html):
+
+## Quickstart
+To run and chat with [LLaVA](https://www.jetson-ai-lab.com/tutorial_llava.html), execute:
 
 ```sh
 reComputer run llava
 ```
+<div align="center">
+  <img alt="jetson" width="1200px" src="./docs/assets/llava.png">
+</div>
 
 ## Example list
 
-reComputer supports a list of examples from [jetson-ai-lab](https://www.jetson-ai-lab.com/)
-
 Here are some examples that can be run:
 
-| Example                                          | Type                     | Model/Data Size | Image Size | Command                                 |
+| Example                                          | Type                     | Model/Data Size | Docker Image Size | Command                                 |
 | ------------------------------------------------ | ------------------------ | --------------- | ---------- | --------------------------------------- |
 | 🆕 llama3                                         | Text (LLM)               | 4.9GB           | 10.5GB     | `reComputer run llama3`                 |
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-| [yolov8-counter](/reComputer/scripts/yolov8-counter/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8_counter`  |
+| [🆕 yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
-Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
+## Development
+Want to add your own example? Check out the [development guide](./docs/develop.md).
+
+We welcome contributions to improve jetson-examples! If you have an example you'd like to share, please submit a pull request. Thank you to all of our contributors! 🙏
 
 ## TODO List
 
 - [ ] check disk space enough or not before run
 - [ ] allow to setting some configs, such as `BASE_PATH`
 - [ ] detect host environment and install what we need
 - [ ] support jetson-containers update
 - [ ] all type jetson support checking list
 - [ ] better table to show example's difference
 - [ ] try jetpack 6.0
+
+
+## License
+This project is licensed under the MIT License. 
+
+## Resources
+- https://github.com/dusty-nv/jetson-containers
+- https://www.jetson-ai-lab.com/
+- https://www.ultralytics.com/
+
```

### Comparing `jetson_examples-0.0.8/pyproject.toml` & `jetson_examples-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jetson-examples"
-version = "0.0.8"
+version = "0.1.0"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "Running Gen AI models and applications on NVIDIA Jetson devices with one-line command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `jetson_examples-0.0.8/reComputer/main.py` & `jetson_examples-0.1.0/reComputer/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import sys
 
 
-def script(name):
+def path_of_script(name):
     script_path = os.path.join(os.path.dirname(__file__), "scripts", name)
     return script_path
 
 
 def list_all_examples(folder_path):
     directory_names = []
     for item in os.listdir(folder_path):
@@ -19,22 +19,25 @@
 
 def run_script():
 
     if len(sys.argv) == 3:
         if sys.argv[1] == "run":
             example_name = sys.argv[2]
             # TODO: maybe use python instead of shell is better
-            subprocess.run(["bash", script("run.sh"), example_name])
+            subprocess.run(["bash", path_of_script("run.sh"), example_name])
+        if sys.argv[1] == "clean":
+            example_name = sys.argv[2]
+            subprocess.run(["bash", path_of_script("clean.sh"), example_name])
         else:
-            print("Only Support `run` for now. try `reComputer run llava` .")
+            print("Only Support `run` or `clean` for now. try `reComputer run llava` .")
     elif len(sys.argv) == 2:
         if sys.argv[1] == "check":
-            subprocess.run(["bash", script("check.sh")])
+            subprocess.run(["bash", path_of_script("check.sh")])
         elif sys.argv[1] == "update":
-            subprocess.run(["bash", script("update.sh")])
+            subprocess.run(["bash", path_of_script("update.sh")])
         elif sys.argv[1] == "list":
             example_folder = os.path.join(os.path.dirname(__file__), "scripts")
             directories = list_all_examples(example_folder)
             print("example list:")
             index = 1
             for directory in directories:
                 print("{:03d}".format(index), "|", directory)
@@ -43,14 +46,15 @@
         else:
             print("reComputer help:")
             print("---")
             print("`reComputer check`   | check system.")
             print("`reComputer update`  | update jetson-ai-lab.")
             print("`reComputer list`    | list all examples.")
             print("`reComputer run xxx` | run an example.")
+            print("`reComputer clean xxx` | clean an example's data.")
             print("---")
     else:
         print("Error Usage! try `reComputer help`.")
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `jetson_examples-0.0.8/reComputer/scripts/live-llava/run.sh` & `jetson_examples-0.1.0/reComputer/scripts/live-llava/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.8/reComputer/scripts/nanodb/run.sh` & `jetson_examples-0.1.0/reComputer/scripts/nanodb/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.8/reComputer/scripts/run.sh` & `jetson_examples-0.1.0/reComputer/scripts/update.sh`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,27 @@
 #!/bin/bash
-
-check_is_jetson_or_not() {
-    model_file="/proc/device-tree/model"
-    
-    if [ -f "/proc/device-tree/model" ]; then
-        model=$(tr -d '\0' < /proc/device-tree/model | tr '[:upper:]' '[:lower:]')
-        if [[ $model =~ jetson|orin|nv|agx ]]; then
-            echo "INFO: machine[$model] confirmed..."
-        else
-            echo "WARNING: machine[$model] maybe not support..."
-            exit 1
-        fi
-    else
-        echo "ERROR: machine[$model] not support this..."
-        exit 1
-    fi
-}
-check_is_jetson_or_not
-
-echo "run example：$1"
+echo "--update jetson-containers repo--"
 BASE_PATH=/home/$USER/reComputer
-
-echo "----example init----"
 mkdir -p $BASE_PATH/
+
 JETSON_REPO_PATH="$BASE_PATH/jetson-containers"
 BASE_JETSON_LAB_GIT="https://github.com/dusty-nv/jetson-containers/tree/d1573a3e8d7ba3fef36ebb23a7391e60eaf64db7"
+
 if [ -d $JETSON_REPO_PATH ]; then
     echo "jetson-ai-lab existed."
+    # 5 publish to Test PyPI
+    read -p "follow the newest version maybe bring bugs, are you sure about the update? (y/n): " choice
+    if [[ $choice == "y" || $choice == "Y" ]]; then
+        cd $JETSON_REPO_PATH
+        git pull
+        pip3 install -r requirements.txt
+    else
+        echo "skip update."
+    fi
 else
     echo "jetson-ai-lab does not installed. start init..."
     cd $BASE_PATH/
     git clone --depth=1 $BASE_JETSON_LAB_GIT
     cd $JETSON_REPO_PATH
     sudo apt update; sudo apt install -y python3-pip
     pip3 install -r requirements.txt
-fi
-
-echo "----example start----"
-cd $JETSON_REPO_PATH
-script_dir=$(dirname "$0")
-start_script=$script_dir/$1/run.sh
-if [ -f $start_script ]; then
-    bash $start_script
-else
-    echo "ERROR: Example[$1] Not Found."
-fi
-echo "----example done----"
+fi
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


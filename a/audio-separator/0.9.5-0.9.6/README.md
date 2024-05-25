# Comparing `tmp/audio_separator-0.9.5.tar.gz` & `tmp/audio_separator-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.9.5.tar", max compression
+gzip compressed data, was "audio_separator-0.9.6.tar", max compression
```

## Comparing `audio_separator-0.9.5.tar` & `audio_separator-0.9.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-12-21 23:51:20.975472 audio_separator-0.9.5/LICENSE
--rw-r--r--   0        0        0     9992 2023-12-21 23:51:20.975472 audio_separator-0.9.5/README.md
--rw-r--r--   0        0        0       33 2023-12-21 23:51:20.975472 audio_separator-0.9.5/audio_separator/__init__.py
--rw-r--r--   0        0        0    20028 2023-12-21 23:51:20.975472 audio_separator-0.9.5/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-12-21 23:51:20.975472 audio_separator-0.9.5/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     3662 2023-12-21 23:51:20.975472 audio_separator-0.9.5/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-12-21 23:51:20.975472 audio_separator-0.9.5/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0     1240 2023-12-21 23:51:20.975472 audio_separator-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    11310 1970-01-01 00:00:00.000000 audio_separator-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-22 00:35:14.526217 audio_separator-0.9.6/LICENSE
+-rw-r--r--   0        0        0    11135 2023-12-22 00:35:14.526217 audio_separator-0.9.6/README.md
+-rw-r--r--   0        0        0       33 2023-12-22 00:35:14.526217 audio_separator-0.9.6/audio_separator/__init__.py
+-rw-r--r--   0        0        0    20028 2023-12-22 00:35:14.526217 audio_separator-0.9.6/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-12-22 00:35:14.526217 audio_separator-0.9.6/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3662 2023-12-22 00:35:14.526217 audio_separator-0.9.6/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-12-22 00:35:14.530217 audio_separator-0.9.6/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0     1240 2023-12-22 00:35:14.530217 audio_separator-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    12453 1970-01-01 00:00:00.000000 audio_separator-0.9.6/PKG-INFO
```

### Comparing `audio_separator-0.9.5/LICENSE` & `audio_separator-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.9.5/README.md` & `audio_separator-0.9.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Audio Separator 🎶
 
 [![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
+[![Docker pulls](https://img.shields.io/docker/pulls/beveradb/audio-separator.svg)](https://hub.docker.com/r/beveradb/audio-separator/tags)
 
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
 The primary stem typically contains the instrumental part of the audio, while the secondary stem contains the vocals, but in some models this is reversed.
 
@@ -64,14 +65,35 @@
 - `pip install --force-reinstall "optimum[onnxruntime-gpu]"`
 
 Depending on your CUDA version and hardware, you may need to install torch from the `cu118` index instead:
 - `pip install --force-reinstall torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118`
 
 > Note: if anyone knows how to make this cleaner so we can support both different platform-specific dependencies for hardware acceleration without a separate installation process for each, please let me know or raise a PR!
 
+## Usage in Docker 🐳
+
+There are [images published on Docker Hub](https://hub.docker.com/r/beveradb/audio-separator/tags) for GPU (CUDA) and CPU inferencing, for both `amd64` and `arm64` platforms.
+
+You probably want to volume-mount a folder containing whatever file you want to separate, which can then also be used as the output folder.
+
+For example, if the current directory contains your input file `input.wav`, you could run `audio-separator` like so:
+
+```
+docker run -it -v `pwd`:/usr/src/app beveradb/audio-separator input.wav
+```
+
+If you're using a machine with a GPU, you'll want to use the GPU specific image and pass in the GPU device to the container, like this:
+
+```
+docker run -it --gpus all -v `pwd`:/usr/src/app beveradb/audio-separator:gpu input.wav
+```
+
+If the GPU isn't being detected, make sure your docker runtime environment is passing through the GPU correctly - there are [various guides](https://www.celantur.com/blog/run-cuda-in-docker-on-linux/) online to help with that.
+
+
 ## Usage 🚀
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
```

### Comparing `audio_separator-0.9.5/audio_separator/separator.py` & `audio_separator-0.9.6/audio_separator/separator.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.9.5/audio_separator/utils/cli.py` & `audio_separator-0.9.6/audio_separator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.9.5/audio_separator/utils/spec_utils.py` & `audio_separator-0.9.6/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.9.5/pyproject.toml` & `audio_separator-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.9.5"
+version = "0.9.6"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 homepage = "https://github.com/karaokenerds/python-audio-separator"
 repository = "https://github.com/karaokenerds/python-audio-separator"
```

### Comparing `audio_separator-0.9.5/PKG-INFO` & `audio_separator-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.9.5
+Version: 0.9.6
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -29,14 +29,15 @@
 Project-URL: Documentation, https://github.com/karaokenerds/python-audio-separator/blob/main/README.md
 Project-URL: Repository, https://github.com/karaokenerds/python-audio-separator
 Description-Content-Type: text/markdown
 
 # Audio Separator 🎶
 
 [![PyPI version](https://badge.fury.io/py/audio-separator.svg)](https://badge.fury.io/py/audio-separator)
+[![Docker pulls](https://img.shields.io/docker/pulls/beveradb/audio-separator.svg)](https://hub.docker.com/r/beveradb/audio-separator/tags)
 
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 
 Audio Separator is a Python package that allows you to separate an audio file into two stems, primary and secondary, using a model in the ONNX format trained by @Anjok07 for use with UVR (https://github.com/Anjok07/ultimatevocalremovergui).
 
 The primary stem typically contains the instrumental part of the audio, while the secondary stem contains the vocals, but in some models this is reversed.
 
@@ -96,14 +97,35 @@
 - `pip install --force-reinstall "optimum[onnxruntime-gpu]"`
 
 Depending on your CUDA version and hardware, you may need to install torch from the `cu118` index instead:
 - `pip install --force-reinstall torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118`
 
 > Note: if anyone knows how to make this cleaner so we can support both different platform-specific dependencies for hardware acceleration without a separate installation process for each, please let me know or raise a PR!
 
+## Usage in Docker 🐳
+
+There are [images published on Docker Hub](https://hub.docker.com/r/beveradb/audio-separator/tags) for GPU (CUDA) and CPU inferencing, for both `amd64` and `arm64` platforms.
+
+You probably want to volume-mount a folder containing whatever file you want to separate, which can then also be used as the output folder.
+
+For example, if the current directory contains your input file `input.wav`, you could run `audio-separator` like so:
+
+```
+docker run -it -v `pwd`:/usr/src/app beveradb/audio-separator input.wav
+```
+
+If you're using a machine with a GPU, you'll want to use the GPU specific image and pass in the GPU device to the container, like this:
+
+```
+docker run -it --gpus all -v `pwd`:/usr/src/app beveradb/audio-separator:gpu input.wav
+```
+
+If the GPU isn't being detected, make sure your docker runtime environment is passing through the GPU correctly - there are [various guides](https://www.celantur.com/blog/run-cuda-in-docker-on-linux/) online to help with that.
+
+
 ## Usage 🚀
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
```


# Comparing `tmp/pyresidfp-0.8.2.tar.gz` & `tmp/pyresidfp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.8.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyresidfp-0.9.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.8.2.tar` & `pyresidfp-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     4158 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/COPYING
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/README.md
--rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/PythonSid.cpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/PythonSid.h
--rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/config.h.in
--rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/__init__.py
--rw-r--r--   0        0        0     8351 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/_pyresidfp.pyi
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/_version.py
--rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/musical_scale.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/py.typed
--rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/registers.py
--rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0        0        0     9187 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/pyresidfp.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/AUTHORS
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/COPYING
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Dac.cpp
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Dac.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/ExternalFilter.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/ExternalFilter.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Filter.cpp
--rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Filter.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Filter6581.cpp
--rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Filter6581.h
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Filter8580.cpp
--rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Filter8580.h
--rw-r--r--   0        0        0     2474 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/FilterModelConfig.h
--rw-r--r--   0        0        0    10442 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0        0        0     8941 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Integrator6581.cpp
--rw-r--r--   0        0        0     9237 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Integrator6581.h
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Integrator8580.cpp
--rw-r--r--   0        0        0     3530 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Integrator8580.h
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/OpAmp.cpp
--rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/OpAmp.h
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Potentiometer.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/README
--rw-r--r--   0        0        0    13918 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/SID.cpp
--rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/SID.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Spline.cpp
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Spline.h
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/Voice.h
--rw-r--r--   0        0        0     5951 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0        0        0     4297 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/WaveformCalculator.h
--rw-r--r--   0        0        0    14415 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0        0        0    12098 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/WaveformGenerator.h
--rw-r--r--   0        0        0     2001 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/array.h
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/resample/Resampler.h
--rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/resample/SincResampler.h
--rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/siddefs-fp.h.in
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/residfp/version.cc
--rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/src/sidcxx11.h
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/tests/test_basic.py
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/tests/test_versions.py
--rw-r--r--   0        0        0     3172 2022-11-09 12:37:21.000000 pyresidfp-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     4158 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/README.md
+-rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/PythonSid.h
+-rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/config.h.in
+-rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0     8351 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/_pyresidfp.pyi
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/py.typed
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     9187 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/COPYING
+-rw-r--r--   0        0        0     3251 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2474 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0    10652 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     9152 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9237 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3530 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/README
+-rw-r--r--   0        0        0    13952 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9862 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/Voice.h
+-rw-r--r--   0        0        0     8280 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     3935 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    16251 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    12878 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     2001 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11698 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/residfp/version.cc
+-rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/src/sidcxx11.h
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/tests/test_basic.py
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/tests/test_versions.py
+-rw-r--r--   0        0        0     3122 2022-11-09 12:37:21.000000 pyresidfp-0.9.0/PKG-INFO
```

### Comparing `pyresidfp-0.8.2/CMakeLists.txt` & `pyresidfp-0.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/COPYING` & `pyresidfp-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/README.md` & `pyresidfp-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/pyproject.toml` & `pyresidfp-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -36,28 +36,27 @@
 authors = [
   { name="Sebastian Klemke", email="pypi@nerdheim.de" },
 ]
 description = "Emulates the SID sound-chip"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: C++",
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Operating System :: OS Independent",
     "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis",
     "Topic :: System :: Emulators",
     "Intended Audience :: Developers",
     "Development Status :: 2 - Pre-Alpha",
 ]
-requires-python = ">=3.7.0,<4.0.0"
+requires-python = ">=3.8.0,<4.0.0"
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/pyresidfp/pyresidfp"
 "Bug Tracker" = "https://github.com/pyresidfp/pyresidfp/issues"
```

### Comparing `pyresidfp-0.8.2/src/PythonSid.cpp` & `pyresidfp-0.9.0/src/PythonSid.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/PythonSid.h` & `pyresidfp-0.9.0/src/PythonSid.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/config.h.in` & `pyresidfp-0.9.0/src/config.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/pyresidfp/__init__.py` & `pyresidfp-0.9.0/src/pyresidfp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/pyresidfp/_pyresidfp.pyi` & `pyresidfp-0.9.0/src/pyresidfp/_pyresidfp.pyi`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/pyresidfp/musical_scale.py` & `pyresidfp-0.9.0/src/pyresidfp/musical_scale.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/pyresidfp/registers.py` & `pyresidfp-0.9.0/src/pyresidfp/registers.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.9.0/src/pyresidfp/sound_interface_device.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/pyresidfp.cpp` & `pyresidfp-0.9.0/src/pyresidfp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/COPYING` & `pyresidfp-0.9.0/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Dac.cpp` & `pyresidfp-0.9.0/src/residfp/Dac.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
     // Non-linearity parameter, 8580 DACs are perfectly linear
     const double _2R_div_R = chipModel == MOS6581 ? 2.20 : 2.00;
 
     // 6581 DACs are not terminated by a 2R resistor
     const bool term = chipModel == MOS8580;
 
+    double Vsum = 0.;
+
     // Calculate voltage contribution by each individual bit in the R-2R ladder.
     for (unsigned int set_bit = 0; set_bit < dacLength; set_bit++)
     {
         double Vn = 1.;                   // Normalized bit voltage.
         double R = 1.;                    // Normalized R
         const double _2R = _2R_div_R * R; // 2R
         double Rn = term ?                // Rn = 2R for correct termination,
@@ -98,24 +100,18 @@
             Rn += R;
             const double I = Vn / Rn;
             Rn = (_2R * Rn) / (_2R + Rn); // 2R || Rn
             Vn = Rn * I;
         }
 
         dac[set_bit] = Vn;
+        Vsum += Vn;
     }
 
     // Normalize to integerish behavior
-    double Vsum = 0.;
-
-    for (unsigned int i = 0; i < dacLength; i++)
-    {
-        Vsum += dac[i];
-    }
-
     Vsum /= 1 << dacLength;
 
     for (unsigned int i = 0; i < dacLength; i++)
     {
         dac[i] /= Vsum;
     }
 }
```

### Comparing `pyresidfp-0.8.2/src/residfp/Dac.h` & `pyresidfp-0.9.0/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.9.0/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.9.0/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.9.0/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/ExternalFilter.h` & `pyresidfp-0.9.0/src/residfp/ExternalFilter.h`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 /**
  * The audio output stage in a Commodore 64 consists of two STC networks, a
  * low-pass RC filter with 3 dB frequency 16kHz followed by a DC-blocker which
  * acts as a high-pass filter with a cutoff dependent on the attached audio
  * equipment impedance. Here we suppose an impedance of 10kOhm resulting
  * in a 3 dB attenuation at 1.6Hz.
  * To operate properly the 6581 audio output needs a pull-down resistor
- *(1KOhm recommended, not needed on 8580)
+ * (1KOhm recommended, not needed on 8580)
  *
  * ~~~
  *                                 9/12V
  * -----+
  * audio|       10k                  |
  *      +---o----R---o--------o-----(K)          +-----
  *  out |   |        |        |      |           |audio
@@ -76,15 +76,15 @@
 
 public:
     /**
      * SID clocking.
      *
      * @param input
      */
-    int clock(unsigned short input);
+    int clock(int input);
 
     /**
      * Constructor.
      */
     ExternalFilter();
 
     /**
@@ -104,17 +104,17 @@
 
 #if RESID_INLINING || defined(EXTERNALFILTER_CPP)
 
 namespace reSIDfp
 {
 
 RESID_INLINE
-int ExternalFilter::clock(unsigned short input)
+int ExternalFilter::clock(int input)
 {
-    const int Vi = (static_cast<unsigned int>(input)<<11) - (1 << (11+15));
+    const int Vi = (input<<11) - (1 << (11+15));
     const int dVlp = (w0lp_1_s7 * (Vi - Vlp) >> 7);
     const int dVhp = (w0hp_1_s17 * (Vlp - Vhp) >> 17);
     Vlp += dVlp;
     Vhp += dVhp;
     return (Vlp - Vhp) >> 11;
 }
```

### Comparing `pyresidfp-0.8.2/src/residfp/Filter.cpp` & `pyresidfp-0.9.0/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Filter.h` & `pyresidfp-0.9.0/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Filter6581.cpp` & `pyresidfp-0.9.0/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Filter6581.h` & `pyresidfp-0.9.0/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Filter8580.cpp` & `pyresidfp-0.9.0/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Filter8580.h` & `pyresidfp-0.9.0/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.9.0/src/residfp/FilterModelConfig.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/FilterModelConfig.h` & `pyresidfp-0.9.0/src/residfp/FilterModelConfig.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/FilterModelConfig6581.cpp` & `pyresidfp-0.9.0/src/residfp/FilterModelConfig6581.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,24 @@
  * You should have received a copy of the GNU General Public License
  * along with this program; if not, write to the Free Software
  * Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
  */
 
 #include "FilterModelConfig6581.h"
 
-#include <cmath>
-
 #include "Integrator6581.h"
 #include "OpAmp.h"
 
+#include "src/sidcxx11.h"
+
+#ifdef HAVE_CXX11
+#  include <mutex>
+#endif
+#include <cmath>
+
 namespace reSIDfp
 {
 
 #ifndef HAVE_CXX11
 /**
  * Compute log(1+x) without losing precision for small values of x
  *
@@ -86,16 +91,24 @@
   {  8.50,  0.89 },
   { 10.00,  0.81 },
   { 10.31,  0.81 },  // Approximate end of actual range
 };
 
 std::unique_ptr<FilterModelConfig6581> FilterModelConfig6581::instance(nullptr);
 
+#ifdef HAVE_CXX11
+std::mutex Instance6581_Lock;
+#endif
+
 FilterModelConfig6581* FilterModelConfig6581::getInstance()
 {
+#ifdef HAVE_CXX11
+    std::lock_guard<std::mutex> lock(Instance6581_Lock);
+#endif
+
     if (!instance.get())
     {
         instance.reset(new FilterModelConfig6581());
     }
 
     return instance.get();
 }
```

### Comparing `pyresidfp-0.8.2/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.9.0/src/residfp/FilterModelConfig6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/FilterModelConfig8580.cpp` & `pyresidfp-0.9.0/src/residfp/FilterModelConfig8580.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,20 @@
  */
 
 #include "FilterModelConfig8580.h"
 
 #include "Integrator8580.h"
 #include "OpAmp.h"
 
+#include "src/sidcxx11.h"
 
+#ifdef HAVE_CXX11
+#  include <mutex>
+#endif
+ 
 namespace reSIDfp
 {
 
 /*
  * R1 = 15.3*Ri
  * R2 =  7.3*Ri
  * R3 =  4.7*Ri
@@ -106,27 +111,35 @@
     {  5.00,  1.30 },
     {  5.10,  1.30 },
     {  8.91,  1.30 },  // Approximate end of actual range
 };
 
 std::unique_ptr<FilterModelConfig8580> FilterModelConfig8580::instance(nullptr);
 
+#ifdef HAVE_CXX11
+std::mutex Instance8580_Lock;
+#endif
+
 FilterModelConfig8580* FilterModelConfig8580::getInstance()
 {
+#ifdef HAVE_CXX11
+    std::lock_guard<std::mutex> lock(Instance8580_Lock);
+#endif
+
     if (!instance.get())
     {
         instance.reset(new FilterModelConfig8580());
     }
 
     return instance.get();
 }
 
 FilterModelConfig8580::FilterModelConfig8580() :
     FilterModelConfig(
-        0.30,   // voice voltage range FIXME measure
+        0.24,   // voice voltage range FIXME measure
         4.84,   // voice DC voltage FIXME measure
         22e-9,  // capacitor value
         9.09,   // Vdd
         0.80,   // Vth
         100e-6, // uCox
         opamp_voltage,
         OPAMP_SIZE
```

### Comparing `pyresidfp-0.8.2/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.9.0/src/residfp/FilterModelConfig8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Integrator6581.cpp` & `pyresidfp-0.9.0/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Integrator6581.h` & `pyresidfp-0.9.0/src/residfp/Integrator6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Integrator8580.cpp` & `pyresidfp-0.9.0/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Integrator8580.h` & `pyresidfp-0.9.0/src/residfp/Integrator8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/OpAmp.cpp` & `pyresidfp-0.9.0/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/OpAmp.h` & `pyresidfp-0.9.0/src/residfp/OpAmp.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Potentiometer.h` & `pyresidfp-0.9.0/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/README` & `pyresidfp-0.9.0/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/SID.cpp` & `pyresidfp-0.9.0/src/residfp/SID.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
  * Fourth chip 0x90-0xA4
  * On the 8580 that plays digis the output is 4.66 and 0x93 is the only value to reach that.
  * To me that seems as regular 8580s have somewhat wide 0-level range,
  * whereas that digi-compatible 8580 has it very narrow.
  * On my 6581R4AR has 0x3A as the only value giving the same output level as 1.prg
  */
 //@{
-unsigned int constexpr OFFSET_6581 = 0x380;
-unsigned int constexpr OFFSET_8580 = 0x9c0;
+const unsigned int OFFSET_6581 = 0x380;
+const unsigned int OFFSET_8580 = 0x9c0;
 //@}
 
 /**
  * Bus value stays alive for some time after each operation.
  * Values differs between chip models, the timings used here
  * are taken from VICE [1].
  * See also the discussion "How do I reliably detect 6581/8580 sid?" on CSDb [2].
@@ -124,16 +124,16 @@
  *   (old SID) (250407/6581)
  *   delayfrq0    ~01d00
  *
  * [1]: http://sourceforge.net/p/vice-emu/patches/99/
  * [2]: http://noname.c64.org/csdb/forums/?roomid=11&topicid=29025&showallposts=1
  */
 //@{
-int constexpr BUS_TTL_6581 = 0x01d00;
-int constexpr BUS_TTL_8580 = 0xa2000;
+const int BUS_TTL_6581 = 0x01d00;
+const int BUS_TTL_8580 = 0xa2000;
 //@}
 
 SID::SID() :
     filter6581(new Filter6581()),
     filter8580(new Filter8580()),
     externalFilter(new ExternalFilter()),
     resampler(nullptr),
@@ -207,19 +207,21 @@
 
 void SID::setChipModel(ChipModel model)
 {
     switch (model)
     {
     case MOS6581:
         filter = filter6581.get();
+        scaleFactor = 3;
         modelTTL = BUS_TTL_6581;
         break;
 
     case MOS8580:
         filter = filter8580.get();
+        scaleFactor = 5;
         modelTTL = BUS_TTL_8580;
         break;
 
     default:
         throw SIDError("Unknown chip type");
     }
```

### Comparing `pyresidfp-0.8.2/src/residfp/SID.h` & `pyresidfp-0.9.0/src/residfp/SID.h`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
 
     /// Paddle Y register support
     std::unique_ptr<Potentiometer> const potY;
 
     /// SID voices
     std::unique_ptr<Voice> voice[3];
 
+    /// Used to amplify the output by x/2 to get an adequate playback volume
+    int scaleFactor;
+
     /// Time to live for the last written value
     int busValueTtl;
 
     /// Current chip model's bus value TTL
     int modelTTL;
 
     /// Time until #voiceSync must be run.
@@ -314,15 +317,17 @@
 RESID_INLINE
 int SID::output() const
 {
     const int v1 = voice[0]->output(voice[2]->wave());
     const int v2 = voice[1]->output(voice[0]->wave());
     const int v3 = voice[2]->output(voice[1]->wave());
 
-    return externalFilter->clock(filter->clock(v1, v2, v3));
+    const int input = (scaleFactor * static_cast<unsigned int>(filter->clock(v1, v2, v3))) / 2;
+
+    return externalFilter->clock(input);
 }
 
 
 RESID_INLINE
 int SID::clock(unsigned int cycles, short* buf)
 {
     ageBusValue(cycles);
```

### Comparing `pyresidfp-0.8.2/src/residfp/Spline.cpp` & `pyresidfp-0.9.0/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Spline.h` & `pyresidfp-0.9.0/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/Voice.h` & `pyresidfp-0.9.0/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/WaveformCalculator.h` & `pyresidfp-0.9.0/src/residfp/WaveformCalculator.h`

 * *Files 5% similar despite different names*

```diff
@@ -18,54 +18,41 @@
  * along with this program; if not, write to the Free Software
  * Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
  */
 
 #ifndef WAVEFORMCALCULATOR_h
 #define WAVEFORMCALCULATOR_h
 
-#include <map>
-
 #include "array.h"
-#include "src/sidcxx11.h"
+
 #include "siddefs-fp.h"
 
 
 namespace reSIDfp
 {
 
 /**
- * Combined waveform model parameters.
- */
-typedef struct
-{
-    float threshold;
-    float pulsestrength;
-    float distance1;
-    float distance2;
-} CombinedWaveformConfig;
-
-/**
  * Combined waveform calculator for WaveformGenerator.
  * By combining waveforms, the bits of each waveform are effectively short
- * circuited. A zero bit in one waveform will result in a zero output bit
- * (thus the infamous claim that the waveforms are AND'ed).
+ * circuited, a zero bit in one waveform will result in a zero output bit,
+ * thus the claim that the waveforms are AND'ed.
  * However, a zero bit in one waveform may also affect the neighboring bits
  * in the output.
  *
  * Example:
- * 
+ *
  *                 1 1
  *     Bit #       1 0 9 8 7 6 5 4 3 2 1 0
  *                 -----------------------
  *     Sawtooth    0 0 0 1 1 1 1 1 1 0 0 0
- *     
+ *
  *     Triangle    0 0 1 1 1 1 1 1 0 0 0 0
- *     
+ *
  *     AND         0 0 0 1 1 1 1 1 0 0 0 0
- *     
+ *
  *     Output      0 0 0 0 1 1 1 0 0 0 0 0
  *
  *
  * Re-vectorized die photographs reveal the mechanism behind this behavior.
  * Each waveform selector bit acts as a switch, which directly connects
  * internal outputs into the waveform DAC inputs as follows:
  *
@@ -95,21 +82,16 @@
  * is pulled down it might affect the oscillator's adder
  * driving the top bit low.
  *
  */
 class WaveformCalculator
 {
 private:
-    typedef std::map<const CombinedWaveformConfig*, matrix_t> cw_cache_t;
-
-private:
     matrix_t wftable;
 
-    cw_cache_t PULLDOWN_CACHE;
-
 private:
     WaveformCalculator();
 
 public:
     /**
      * Get the singleton instance.
      */
```

### Comparing `pyresidfp-0.8.2/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.9.0/src/residfp/WaveformGenerator.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- * Copyright 2011-2022 Leandro Nini <drfiemost@users.sourceforge.net>
+ * Copyright 2011-2023 Leandro Nini <drfiemost@users.sourceforge.net>
  * Copyright 2007-2010 Antti Lankila
  * Copyright 2004 Dag Lem <resid@nimrod.no>
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
@@ -20,27 +20,14 @@
  * Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
  */
 
 #define WAVEFORMGENERATOR_CPP
 
 #include "WaveformGenerator.h"
 
-/*
- * This fixes tests
- *  SID/wb_testsuite/noise_writeback_check_8_to_C_old
- *  SID/wb_testsuite/noise_writeback_check_9_to_C_old
- *  SID/wb_testsuite/noise_writeback_check_A_to_C_old
- *  SID/wb_testsuite/noise_writeback_check_C_to_C_old
- *
- * but breaks SID/wf12nsr/wf12nsr
- *
- * needs more digging...
- */
-//#define NO_WB_NOI_PUL
-
 namespace reSIDfp
 {
 
 /**
  * Number of cycles after which the waveform output fades to 0 when setting
  * the waveform register to 0.
  * Values measured on warm chips (6581R3/R4 and 8580R5)
@@ -179,53 +166,150 @@
  *
  *
  * Shift phase 2 (phi2)
  * --------------------
  * On the second half of shift phase 2 c2 closes and
  * we're back to normal cycles.
  */
-void WaveformGenerator::clock_shift_register(unsigned int bit0)
+
+inline bool do_writeback(unsigned int waveform_old, unsigned int waveform_new, bool is6581)
 {
-    shift_register = (shift_register >> 1) | bit0;
+    // no writeback without combined waveforms
 
-    // New noise waveform output.
-    set_noise_output();
+    if (waveform_old <= 8)
+        // fixes SID/noisewriteback/noise_writeback_test2-{old,new}
+        return false;
+
+    if (waveform_new < 8)
+        return false;
+
+    if ((waveform_new == 8)
+        // breaks noise_writeback_check_F_to_8_old
+        // but fixes simple and scan
+        && (waveform_old != 0xf))
+    {
+        // fixes
+        // noise_writeback_check_9_to_8_old
+        // noise_writeback_check_A_to_8_old
+        // noise_writeback_check_B_to_8_old
+        // noise_writeback_check_D_to_8_old
+        // noise_writeback_check_E_to_8_old
+        // noise_writeback_check_F_to_8_old
+        // noise_writeback_check_9_to_8_new
+        // noise_writeback_check_A_to_8_new
+        // noise_writeback_check_D_to_8_new
+        // noise_writeback_check_E_to_8_new
+        // noise_writeback_test1-{old,new}
+        return false;
+    }
+
+    // What's happening here?
+    if (is6581 &&
+            ((((waveform_old & 0x3) == 0x1) && ((waveform_new & 0x3) == 0x2))
+            || (((waveform_old & 0x3) == 0x2) && ((waveform_new & 0x3) == 0x1))))
+    {
+        // fixes
+        // noise_writeback_check_9_to_A_old
+        // noise_writeback_check_9_to_E_old
+        // noise_writeback_check_A_to_9_old
+        // noise_writeback_check_A_to_D_old
+        // noise_writeback_check_D_to_A_old
+        // noise_writeback_check_E_to_9_old
+        return false;
+    }
+    if (waveform_old == 0xc)
+    {
+        // fixes
+        // noise_writeback_check_C_to_A_new
+        return false;
+    }
+    if (waveform_new == 0xc)
+    {
+        // fixes
+        // noise_writeback_check_9_to_C_old
+        // noise_writeback_check_A_to_C_old
+        return false;
+    }
+
+    // ok do the writeback
+    return true;
 }
 
-unsigned int WaveformGenerator::get_noise_writeback()
+inline unsigned int get_noise_writeback(unsigned int waveform_output)
 {
   return
     ((waveform_output & (1u << 11)) >>  9) |  // Bit 11 -> bit 20
     ((waveform_output & (1u << 10)) >>  6) |  // Bit 10 -> bit 18
     ((waveform_output & (1u <<  9)) >>  1) |  // Bit  9 -> bit 14
     ((waveform_output & (1u <<  8)) <<  3) |  // Bit  8 -> bit 11
     ((waveform_output & (1u <<  7)) <<  6) |  // Bit  7 -> bit  9
     ((waveform_output & (1u <<  6)) << 11) |  // Bit  6 -> bit  5
     ((waveform_output & (1u <<  5)) << 15) |  // Bit  5 -> bit  2
     ((waveform_output & (1u <<  4)) << 18);   // Bit  4 -> bit  0
 }
 
-void WaveformGenerator::write_shift_register()
+/*
+ * Perform the actual shifting, moving the latched value into following bits.
+ * The XORing for bit0 is done in this cycle using the test bit latched during
+ * the previous phi2 cycle.
+ */
+void WaveformGenerator::shift_phase2(unsigned int waveform_old, unsigned int waveform_new)
 {
-    if (unlikely(waveform > 0x8) && likely(!test) && likely(shift_pipeline != 1))
+    if (do_writeback(waveform_old, waveform_new, is6581))
     {
-        // Write changes to the shift register output caused by combined waveforms
-        // back into the shift register. This happens only when the register is clocked
-        // (see $D1+$81_wave_test [1]) or when the test bit is falling.
-        // A bit once set to zero cannot be changed, hence the and'ing.
-        //
-        // [1] ftp://ftp.untergrund.net/users/nata/sid_test/$D1+$81_wave_test.7z
+        // if noise is combined with another waveform the output drives the SR bits
+        shift_latch = (shift_register & shift_mask) | get_noise_writeback(waveform_output);
+    }
+
+    // bit0 = (bit22 | test | reset) ^ bit17 = 1 ^ bit17 = ~bit17
+    const unsigned int bit22 = ((test_or_reset ? 1 : 0) | shift_latch) << 22;
+    const unsigned int bit0 = (bit22 ^ (shift_latch << 17)) & (1 << 22);
+
+    shift_register = (shift_latch >> 1) | bit0;
+#ifdef TRACE
+    std::cout << std::hex << shift_latch << " -> " << shift_register << std::endl;
+#endif
+    set_noise_output();
+}
 
-#ifdef NO_WB_NOI_PUL
+void WaveformGenerator::write_shift_register()
+{
+    if (unlikely(waveform > 0x8))
+    {
+#if 0
+        // FIXME this breaks SID/wf12nsr/wf12nsr
         if (waveform == 0xc)
+            // fixes
+            // noise_writeback_check_8_to_C_old
+            // noise_writeback_check_9_to_C_old
+            // noise_writeback_check_A_to_C_old
+            // noise_writeback_check_C_to_C_old
             return;
 #endif
-        shift_register &= shift_mask | get_noise_writeback();
 
-        noise_output &= waveform_output;
+        // Write changes to the shift register output caused by combined waveforms
+        // back into the shift register.
+        if (likely(shift_pipeline != 1) && !test)
+        {
+#ifdef TRACE
+            std::cout << "write shift_register" << std::endl;
+#endif
+            // the output pulls down the SR bits
+            shift_register = shift_register & (shift_mask | get_noise_writeback(waveform_output));
+            noise_output &= waveform_output;
+        }
+        else
+        {
+#ifdef TRACE
+            std::cout << "write shift_latch" << std::endl;
+#endif
+            // shift phase 1: the output drives the SR bits
+            noise_output = waveform_output;
+        }
+
         set_no_noise_or_noise_output();
     }
 }
 
 void WaveformGenerator::set_noise_output()
 {
     noise_output =
@@ -258,34 +342,14 @@
     // not be synced. This has been verified by sampling OSC3.
     if (unlikely(msb_rising) && syncDest->sync && !(sync && syncSource->msb_rising))
     {
         syncDest->accumulator = 0;
     }
 }
 
-bool do_pre_writeback(unsigned int waveform_prev, unsigned int waveform, bool is6581)
-{
-    // no writeback without combined waveforms
-    if (waveform <= 8)
-        return false;
-    // What's happening here?
-    if (is6581 &&
-            ((((waveform_prev & 0x3) == 0x1) && ((waveform & 0x3) == 0x2))
-            || (((waveform_prev & 0x3) == 0x2) && ((waveform & 0x3) == 0x1))))
-        return false;
-    if (waveform_prev == 0xc)
-        return false;
-#ifdef NO_WB_NOI_PUL
-    if (waveform == 0xc)
-        return false;
-#endif
-    // ok do the writeback
-    return true;
-}
-
 void WaveformGenerator::set_no_noise_or_noise_output()
 {
     no_noise_or_noise_output = no_noise | noise_output;
 }
 
 void WaveformGenerator::writeCONTROL_REG(unsigned char control)
 {
@@ -348,32 +412,28 @@
         {
             // Reset accumulator.
             accumulator = 0;
 
             // Flush shift pipeline.
             shift_pipeline = 0;
 
+            // Latch the shift register value.
+            shift_latch = shift_register;
+#ifdef TRACE
+            std::cout << "shift phase 1 (test)" << std::endl;
+#endif
+
             // Set reset time for shift register.
             shift_register_reset = is6581 ? SHIFT_REGISTER_RESET_6581R3 : SHIFT_REGISTER_RESET_8580R5;
         }
         else
         {
             // When the test bit is falling, the second phase of the shift is
             // completed by enabling SRAM write.
-
-            // During first phase of the shift the bits are interconnected
-            // and the output of each bit is loaded into the following.
-            // The output may overwrite the latched value.
-            if (do_pre_writeback(waveform_prev, waveform, is6581))
-            {
-                shift_register = (shift_register & shift_mask) | get_noise_writeback();
-            }
-
-            // bit0 = (bit22 | test) ^ bit17 = 1 ^ bit17 = ~bit17
-            clock_shift_register((~shift_register << 17) & (1 << 22));
+            shift_phase2(waveform_prev, waveform);
         }
     }
 }
 
 void WaveformGenerator::waveBitfade()
 {
     waveform_output &= waveform_output >> 1;
@@ -413,15 +473,17 @@
     pulse_output = 0xfff;
 
     shift_register_reset = 0;
     shift_register = 0x7fffff;
     // when reset is released the shift register is clocked once
     // so the lower bit is zeroed out
     // bit0 = (bit22 | test) ^ bit17 = 1 ^ 1 = 0
-    clock_shift_register(0);
+    test_or_reset = true;
+    shift_latch = shift_register;
+    shift_phase2(0, 0);
 
     shift_pipeline = 0;
 
     waveform_output = 0;
     floating_output_ttl = 0;
 }
```

### Comparing `pyresidfp-0.8.2/src/residfp/WaveformGenerator.h` & `pyresidfp-0.9.0/src/residfp/WaveformGenerator.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- * Copyright 2011-2022 Leandro Nini <drfiemost@users.sourceforge.net>
+ * Copyright 2011-2023 Leandro Nini <drfiemost@users.sourceforge.net>
  * Copyright 2007-2010 Antti Lankila
  * Copyright 2004,2010 Dag Lem <resid@nimrod.no>
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
@@ -24,14 +24,21 @@
 #define WAVEFORMGENERATOR_H
 
 #include "siddefs-fp.h"
 #include "array.h"
 
 #include "src/sidcxx11.h"
 
+// print SR debugging info
+//#define TRACE 1
+
+#ifdef TRACE
+#  include <iostream>
+#endif
+
 namespace reSIDfp
 {
 
 /**
  * A 24 bit accumulator is the basis for waveform generation.
  * FREQ is added to the lower 16 bits of the accumulator each cycle.
  * The accumulator is set to zero when TEST is set, and starts counting
@@ -93,14 +100,17 @@
     short* pulldown;
 
     // PWout = (PWn/40.95)%
     unsigned int pw;
 
     unsigned int shift_register;
 
+    /// Shift register is latched when transitioning to shift phase 1.
+    unsigned int shift_latch;
+
     /// Emulation of pipeline causing bit 19 to clock the shift register.
     int shift_pipeline;
 
     unsigned int ring_msb_mask;
     unsigned int no_noise;
     unsigned int noise_output;
     unsigned int no_noise_or_noise_output;
@@ -123,32 +133,33 @@
 
     /// The OSC3 value
     unsigned int osc3;
 
     /// Remaining time to fully reset shift register.
     unsigned int shift_register_reset;
 
-    // The wave signal TTL when no waveform is selected
+    // The wave signal TTL when no waveform is selected.
     unsigned int floating_output_ttl;
 
     /// The control register bits. Gate is handled by EnvelopeGenerator.
     //@{
     bool test;
     bool sync;
     //@}
 
+    /// Test bit is latched at phi2 for the noise XOR.
+    bool test_or_reset;
+
     /// Tell whether the accumulator MSB was set high on this cycle.
     bool msb_rising;
 
     bool is6581; //-V730_NOINIT this is initialized in the SID constructor
 
 private:
-    void clock_shift_register(unsigned int bit0);
-
-    unsigned int get_noise_writeback();
+    void shift_phase2(unsigned int waveform_old, unsigned int waveform_new);
 
     void write_shift_register();
 
     void set_noise_output();
     
     void set_no_noise_or_noise_output();
 
@@ -296,20 +307,27 @@
 RESID_INLINE
 void WaveformGenerator::clock()
 {
     if (unlikely(test))
     {
         if (unlikely(shift_register_reset != 0) && unlikely(--shift_register_reset == 0))
         {
+#ifdef TRACE
+            std::cout << "shiftregBitfade" << std::endl;
+#endif
             shiftregBitfade();
+            shift_latch = shift_register;
 
             // New noise waveform output.
             set_noise_output();
         }
 
+        // Latch the test bit value for shift phase 2.
+        test_or_reset = true;
+
         // The test bit sets pulse high.
         pulse_output = 0xfff;
     }
     else
     {
         // Calculate new accumulator value;
         const unsigned int accumulator_old = accumulator;
@@ -324,18 +342,33 @@
         // Shift noise register once for each time accumulator bit 19 is set high.
         // The shift is delayed 2 cycles.
         if (unlikely((accumulator_bits_set & 0x080000) != 0))
         {
             // Pipeline: Detect rising bit, shift phase 1, shift phase 2.
             shift_pipeline = 2;
         }
-        else if (unlikely(shift_pipeline != 0) && --shift_pipeline == 0)
+        else if (unlikely(shift_pipeline != 0))
         {
-            // bit0 = (bit22 | test) ^ bit17
-            clock_shift_register(((shift_register << 22) ^ (shift_register << 17)) & (1u << 22));
+            switch (--shift_pipeline)
+            {
+            case 0:
+#ifdef TRACE
+                std::cout << "shift phase 2" << std::endl;
+#endif
+                shift_phase2(waveform, waveform);
+                break;
+            case 1:
+#ifdef TRACE
+                std::cout << "shift phase 1" << std::endl;
+#endif
+                // Start shift phase 1.
+                test_or_reset = false;
+                shift_latch = shift_register;
+                break;
+            }
         }
     }
 }
 
 RESID_INLINE
 unsigned int WaveformGenerator::output(const WaveformGenerator* ringModulator)
 {
```

### Comparing `pyresidfp-0.8.2/src/residfp/array.h` & `pyresidfp-0.9.0/src/residfp/array.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/resample/Resampler.h` & `pyresidfp-0.9.0/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.9.0/src/residfp/resample/SincResampler.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,41 @@
 #include <cstring>
 #include <cmath>
 #include <iostream>
 #include <sstream>
 
 #include "siddefs-fp.h"
 
+#include "src/sidcxx11.h"
+
 #ifdef HAVE_CONFIG_H
 #  include "config.h"
 #endif
 
 #ifdef HAVE_EMMINTRIN_H
 #  include <emmintrin.h>
 #elif defined HAVE_MMINTRIN_H
 #  include <mmintrin.h>
 #elif defined(HAVE_ARM_NEON_H)
 #  include <arm_neon.h>
 #endif
+#ifdef HAVE_CXX11
+#  include <mutex>
+#endif
 
 namespace reSIDfp
 {
 
 typedef std::map<std::string, matrix_t> fir_cache_t;
 
 /// Cache for the expensive FIR table computation results.
 fir_cache_t FIR_CACHE;
+#ifdef HAVE_CXX11
+std::mutex FIR_CACHE_Lock;
+#endif
 
 /// Maximum error acceptable in I0 is 1e-6, or ~96 dB.
 const double I0E = 1e-6;
 
 const int BITS = 16;
 
 /**
@@ -115,15 +123,15 @@
         __m128i acc = _mm_setzero_si128();
 
         const int n = bLength / 8;
 
         for (int i = 0; i < n; i++)
         {
             const __m128i tmp = _mm_madd_epi16(*(__m128i*)a, *(__m128i*)b);
-            acc = _mm_add_epi16(acc, tmp);
+            acc = _mm_add_epi32(acc, tmp);
             a += 8;
             b += 8;
         }
 
         __m128i vsum = _mm_add_epi32(acc, _mm_srli_si128(acc, 8));
         vsum = _mm_add_epi32(vsum, _mm_srli_si128(vsum, 4));
         out += _mm_cvtsi128_si32(vsum);
@@ -309,14 +317,19 @@
         // The filter test program indicates that the filter performs well, though.
     }
 
     // Create the map key
     std::ostringstream o;
     o << firN << "," << firRES << "," << cyclesPerSampleD;
     const std::string firKey = o.str();
+
+#ifdef HAVE_CXX11
+    std::lock_guard<std::mutex> lock(FIR_CACHE_Lock);
+#endif
+
     fir_cache_t::iterator lb = FIR_CACHE.lower_bound(firKey);
 
     // The FIR computation is expensive and we set sampling parameters often, but
     // from a very small set of choices. Thus, caching is used to speed initialization.
     if (lb != FIR_CACHE.end() && !(FIR_CACHE.key_comp()(firKey, lb->first)))
     {
         firTable = &(lb->second);
```

### Comparing `pyresidfp-0.8.2/src/residfp/resample/SincResampler.h` & `pyresidfp-0.9.0/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.9.0/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.9.0/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.9.0/src/residfp/siddefs-fp.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/residfp/version.cc` & `pyresidfp-0.9.0/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/src/sidcxx11.h` & `pyresidfp-0.9.0/src/sidcxx11.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/tests/test_basic.py` & `pyresidfp-0.9.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.8.2/PKG-INFO` & `pyresidfp-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.8.2
+Version: 0.9.0
 Summary: Emulates the SID sound-chip
 Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: C++
@@ -16,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: System :: Emulators
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 2 - Pre-Alpha
 Project-URL: Homepage, https://github.com/pyresidfp/pyresidfp
 Project-URL: Bug tracker, https://github.com/pyresidfp/pyresidfp/issues
-Requires-Python: <4.0.0,>=3.7.0
+Requires-Python: <4.0.0,>=3.8.0
 Description-Content-Type: text/markdown
 
 # pyresidfp
 
 Emulates the SID sound-chip in software. The C++ emulation code was copied over from
 [libsidplayfp](https://github.com/libsidplayfp/libsidplayfp).
```


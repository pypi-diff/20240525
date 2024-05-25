# Comparing `tmp/depthai-2.8.0.0.tar.gz` & `tmp/depthai-2.9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthai-2.8.0.0.tar", last modified: Fri Jul 23 13:45:02 2021, max compression
+gzip compressed data, was "depthai-2.9.0.0.tar", last modified: Sat Aug  7 07:41:06 2021, max compression
```

## Comparing `depthai-2.8.0.0.tar` & `depthai-2.9.0.0.tar`

### file list

```diff
@@ -1,374 +1,380 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.020355 depthai-2.8.0.0/
--rw-r--r--   0 root         (0) root         (0)     9871 2021-07-23 13:42:48.000000 depthai-2.8.0.0/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1068 2021-07-23 13:42:48.000000 depthai-2.8.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      309 2021-07-23 13:42:48.000000 depthai-2.8.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8637 2021-07-23 13:45:02.020355 depthai-2.8.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7369 2021-07-23 13:42:48.000000 depthai-2.8.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/ci/
--rw-r--r--   0 root         (0) root         (0)      690 2021-07-23 13:42:48.000000 depthai-2.8.0.0/ci/Dockerfile
--rwxr-xr-x   0 root         (0) root         (0)      722 2021-07-23 13:42:48.000000 depthai-2.8.0.0/ci/build-wheels.sh
--rwxr-xr-x   0 root         (0) root         (0)      215 2021-07-23 13:42:48.000000 depthai-2.8.0.0/ci/repair-whl-macos.sh
--rwxr-xr-x   0 root         (0) root         (0)      292 2021-07-23 13:42:48.000000 depthai-2.8.0.0/ci/upload-artifactory.sh
--rwxr-xr-x   0 root         (0) root         (0)      806 2021-07-23 13:42:48.000000 depthai-2.8.0.0/ci/upload-pypi.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/cmake/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/cmake/Hunter/
--rw-r--r--   0 root         (0) root         (0)      260 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/Hunter/config.cmake
--rw-r--r--   0 root         (0) root         (0)    17070 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/HunterGate.cmake
--rw-r--r--   0 root         (0) root         (0)      156 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/default_docstring.hpp.in
--rw-r--r--   0 root         (0) root         (0)       34 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/docstring.hpp.in
--rw-r--r--   0 root         (0) root         (0)     3006 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/pybind11-mkdoc.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)      115 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/toolchain/msvc.cmake
--rw-r--r--   0 root         (0) root         (0)       97 2021-07-23 13:42:48.000000 depthai-2.8.0.0/cmake/toolchain/pic.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/depthai-core/
--rw-r--r--   0 root         (0) root         (0)      388 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/.clang-format
--rw-r--r--   0 root         (0) root         (0)    14785 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/.clang-tidy
--rw-r--r--   0 root         (0) root         (0)       37 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/.git
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/depthai-core/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     8103 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/.github/workflows/main.workflow.yml
--rw-r--r--   0 root         (0) root         (0)      303 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/.gitignore
--rw-r--r--   0 root         (0) root         (0)      245 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/.gitmodules
--rw-r--r--   0 root         (0) root         (0)    21854 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1068 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5996 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/depthai-core/ci/
--rwxr-xr-x   0 root         (0) root         (0)      227 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/ci/check_format.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/cmake/
--rw-r--r--   0 root         (0) root         (0)    35978 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/CMakeRC.cmake
--rw-r--r--   0 root         (0) root         (0)     1998 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/ClangFormat.cmake
--rw-r--r--   0 root         (0) root         (0)      568 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/ClangTidy.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/cmake/Depthai/
--rw-r--r--   0 root         (0) root         (0)      151 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/Depthai/DepthaiBootloaderConfig.cmake
--rw-r--r--   0 root         (0) root         (0)      267 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/Depthai/DepthaiDeviceSideConfig.cmake
--rw-r--r--   0 root         (0) root         (0)     8402 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/DepthaiBootloaderDownloader.cmake
--rw-r--r--   0 root         (0) root         (0)    12479 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/DepthaiDownloader.cmake
--rw-r--r--   0 root         (0) root         (0)     3224 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/Flags.cmake
--rw-r--r--   0 root         (0) root         (0)      464 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/GitCommitHash.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/cmake/Hunter/
--rw-r--r--   0 root         (0) root         (0)     1690 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/Hunter/config.cmake
--rw-r--r--   0 root         (0) root         (0)    17070 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/HunterGate.cmake
--rw-r--r--   0 root         (0) root         (0)      283 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/config.hpp.in
--rw-r--r--   0 root         (0) root         (0)      518 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/depthaiConfig.cmake.in
--rw-r--r--   0 root         (0) root         (0)     1637 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/depthaiDependencies.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/cmake/sanitizers/
--rw-r--r--   0 root         (0) root         (0)     2144 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindASan.cmake
--rw-r--r--   0 root         (0) root         (0)     2292 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindMSan.cmake
--rwxr-xr-x   0 root         (0) root         (0)     3737 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindSanitizers.cmake
--rw-r--r--   0 root         (0) root         (0)     2555 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindTSan.cmake
--rw-r--r--   0 root         (0) root         (0)     1696 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindUBSan.cmake
--rwxr-xr-x   0 root         (0) root         (0)     2011 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/asan-wrapper
--rwxr-xr-x   0 root         (0) root         (0)     7684 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/sanitizers/sanitize-helpers.cmake
--rw-r--r--   0 root         (0) root         (0)     2436 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/target-public-headers.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)      162 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/toolchain/pic.cmake
--rw-r--r--   0 root         (0) root         (0)      710 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/cmake/version.hpp.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/docs/
--rw-r--r--   0 root         (0) root         (0)     1670 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/docs/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)   112781 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/docs/Doxyfile.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/include/depthai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/include/depthai/build/
--rw-r--r--   0 root         (0) root         (0)      283 2021-07-23 13:43:47.000000 depthai-2.8.0.0/depthai-core/include/depthai/build/config.hpp
--rw-r--r--   0 root         (0) root         (0)      662 2021-07-23 13:43:47.000000 depthai-2.8.0.0/depthai-core/include/depthai/build/version.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/include/depthai/common/
--rw-r--r--   0 root         (0) root         (0)      594 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/common/CameraBoardSocket.hpp
--rw-r--r--   0 root         (0) root         (0)      707 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/common/UsbSpeed.hpp
--rw-r--r--   0 root         (0) root         (0)      570 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/depthai.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/include/depthai/device/
--rw-r--r--   0 root         (0) root         (0)    20551 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/device/CalibrationHandler.hpp
--rw-r--r--   0 root         (0) root         (0)      846 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/device/CallbackHandler.hpp
--rw-r--r--   0 root         (0) root         (0)    14197 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/device/DataQueue.hpp
--rw-r--r--   0 root         (0) root         (0)    20509 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/device/Device.hpp
--rw-r--r--   0 root         (0) root         (0)     7838 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/device/DeviceBootloader.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.992354 depthai-2.8.0.0/depthai-core/include/depthai/openvino/
--rw-r--r--   0 root         (0) root         (0)     2214 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/openvino/OpenVINO.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.996354 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/
--rw-r--r--   0 root         (0) root         (0)     2622 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/AssetManager.hpp
--rw-r--r--   0 root         (0) root         (0)     7104 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/Node.hpp
--rw-r--r--   0 root         (0) root         (0)     7927 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/Pipeline.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.996354 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/
--rw-r--r--   0 root         (0) root         (0)      530 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ADatatype.hpp
--rw-r--r--   0 root         (0) root         (0)      722 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/Buffer.hpp
--rw-r--r--   0 root         (0) root         (0)     5118 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/CameraControl.hpp
--rw-r--r--   0 root         (0) root         (0)     1242 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/EdgeDetectorConfig.hpp
--rw-r--r--   0 root         (0) root         (0)      602 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/IMUData.hpp
--rw-r--r--   0 root         (0) root         (0)     5163 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ImageManipConfig.hpp
--rw-r--r--   0 root         (0) root         (0)      660 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ImgDetections.hpp
--rw-r--r--   0 root         (0) root         (0)     4530 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ImgFrame.hpp
--rw-r--r--   0 root         (0) root         (0)     3971 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/NNData.hpp
--rw-r--r--   0 root         (0) root         (0)      795 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialImgDetections.hpp
--rw-r--r--   0 root         (0) root         (0)     1446 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorConfig.hpp
--rw-r--r--   0 root         (0) root         (0)     1029 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorData.hpp
--rw-r--r--   0 root         (0) root         (0)     1827 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/StereoDepthConfig.hpp
--rw-r--r--   0 root         (0) root         (0)      917 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SystemInformation.hpp
--rw-r--r--   0 root         (0) root         (0)     1264 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/Tracklets.hpp
--rw-r--r--   0 root         (0) root         (0)      545 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatypes.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/
--rw-r--r--   0 root         (0) root         (0)     8920 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/ColorCamera.hpp
--rw-r--r--   0 root         (0) root         (0)     2714 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/DetectionNetwork.hpp
--rw-r--r--   0 root         (0) root         (0)     2179 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/EdgeDetector.hpp
--rw-r--r--   0 root         (0) root         (0)     1942 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/IMU.hpp
--rw-r--r--   0 root         (0) root         (0)     2918 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/ImageManip.hpp
--rw-r--r--   0 root         (0) root         (0)     3093 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/MonoCamera.hpp
--rw-r--r--   0 root         (0) root         (0)      670 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/MyProducer.hpp
--rw-r--r--   0 root         (0) root         (0)     2844 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/NeuralNetwork.hpp
--rw-r--r--   0 root         (0) root         (0)     3626 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/ObjectTracker.hpp
--rw-r--r--   0 root         (0) root         (0)     1367 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SPIOut.hpp
--rw-r--r--   0 root         (0) root         (0)     4335 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SpatialDetectionNetwork.hpp
--rw-r--r--   0 root         (0) root         (0)     2369 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SpatialLocationCalculator.hpp
--rw-r--r--   0 root         (0) root         (0)     8703 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/StereoDepth.hpp
--rw-r--r--   0 root         (0) root         (0)     1008 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SystemLogger.hpp
--rw-r--r--   0 root         (0) root         (0)     4446 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/VideoEncoder.hpp
--rw-r--r--   0 root         (0) root         (0)     1539 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/XLinkIn.hpp
--rw-r--r--   0 root         (0) root         (0)     1640 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/XLinkOut.hpp
--rw-r--r--   0 root         (0) root         (0)      590 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/pipeline/nodes.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/include/depthai/utility/
--rw-r--r--   0 root         (0) root         (0)      121 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/utility/Initialization.hpp
--rw-r--r--   0 root         (0) root         (0)     6249 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/utility/LockingQueue.hpp
--rw-r--r--   0 root         (0) root         (0)      320 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/utility/Pimpl.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/include/depthai/xlink/
--rw-r--r--   0 root         (0) root         (0)     2920 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/xlink/XLinkConnection.hpp
--rw-r--r--   0 root         (0) root         (0)     1950 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/include/depthai/xlink/XLinkStream.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/
--rw-r--r--   0 root         (0) root         (0)       84 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/.git
--rw-r--r--   0 root         (0) root         (0)     1084 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/
--rw-r--r--   0 root         (0) root         (0)     3688 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Bootloader.hpp
--rw-r--r--   0 root         (0) root         (0)      181 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Memory.hpp
--rw-r--r--   0 root         (0) root         (0)     1336 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/NetworkBootloaderConfig.hpp
--rw-r--r--   0 root         (0) root         (0)     2284 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/SBR.h
--rw-r--r--   0 root         (0) root         (0)      222 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Section.hpp
--rw-r--r--   0 root         (0) root         (0)      365 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Structure.hpp
--rw-r--r--   0 root         (0) root         (0)      180 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Type.hpp
--rw-r--r--   0 root         (0) root         (0)     1360 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/UsbBootloaderConfig.hpp
--rw-r--r--   0 root         (0) root         (0)      496 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/XLinkConstants.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/src/
--rw-r--r--   0 root         (0) root         (0)     5807 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/src/SBR.c
--rw-r--r--   0 root         (0) root         (0)     1621 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/
--rw-r--r--   0 root         (0) root         (0)       73 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/.git
--rw-r--r--   0 root         (0) root         (0)       85 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/invoke_hpp/
--rw-r--r--   0 root         (0) root         (0)     8630 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/invoke_hpp/invoke.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/linb/
--rw-r--r--   0 root         (0) root         (0)    15977 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/linb/any.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/
--rw-r--r--   0 root         (0) root         (0)     4230 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/client.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/
--rw-r--r--   0 root         (0) root         (0)      399 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/config.h
--rw-r--r--   0 root         (0) root         (0)     1164 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/function_meta.h
--rw-r--r--   0 root         (0) root         (0)      763 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/pack_meta.h
--rw-r--r--   0 root         (0) root         (0)     1774 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/exception.h
--rw-r--r--   0 root         (0) root         (0)      457 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/hash.h
--rw-r--r--   0 root         (0) root         (0)     5263 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/server.h
--rw-r--r--   0 root         (0) root         (0)      834 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/type.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/
--rw-r--r--   0 root         (0) root         (0)     4785 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/cereal_binary.h
--rw-r--r--   0 root         (0) root         (0)     3365 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_json.h
--rw-r--r--   0 root         (0) root         (0)     3252 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_msgpack.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.000354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/version/
--rw-r--r--   0 root         (0) root         (0)      594 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/version/core.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.004354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/tl/
--rw-r--r--   0 root         (0) root         (0)    73553 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/tl/optional.hpp
--rw-r--r--   0 root         (0) root         (0)     1068 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/LICENSE
--rw-r--r--   0 root         (0) root         (0)       80 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.004354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/
--rw-r--r--   0 root         (0) root         (0)      252 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraBoardSocket.hpp
--rw-r--r--   0 root         (0) root         (0)      443 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraImageOrientation.hpp
--rw-r--r--   0 root         (0) root         (0)      631 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraInfo.hpp
--rw-r--r--   0 root         (0) root         (0)      252 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraModel.hpp
--rw-r--r--   0 root         (0) root         (0)      577 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/ChipTemperature.hpp
--rw-r--r--   0 root         (0) root         (0)      483 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CpuUsage.hpp
--rw-r--r--   0 root         (0) root         (0)      102 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/DetectionNetworkType.hpp
--rw-r--r--   0 root         (0) root         (0)      928 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/EepromData.hpp
--rw-r--r--   0 root         (0) root         (0)      726 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Extrinsics.hpp
--rw-r--r--   0 root         (0) root         (0)      314 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/MemoryInfo.hpp
--rw-r--r--   0 root         (0) root         (0)      394 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Point2f.hpp
--rw-r--r--   0 root         (0) root         (0)      432 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Point3f.hpp
--rw-r--r--   0 root         (0) root         (0)      215 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/ProcessorType.hpp
--rw-r--r--   0 root         (0) root         (0)     3606 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Rect.hpp
--rw-r--r--   0 root         (0) root         (0)      435 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/RotatedRect.hpp
--rw-r--r--   0 root         (0) root         (0)      446 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Size2f.hpp
--rw-r--r--   0 root         (0) root         (0)      528 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/StereoRectification.hpp
--rw-r--r--   0 root         (0) root         (0)      525 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Timestamp.hpp
--rw-r--r--   0 root         (0) root         (0)      184 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/UsbSpeed.hpp
--rw-r--r--   0 root         (0) root         (0)      962 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/optional.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.004354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/
--rw-r--r--   0 root         (0) root         (0)      481 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/DatatypeEnum.hpp
--rw-r--r--   0 root         (0) root         (0)      485 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawBuffer.hpp
--rw-r--r--   0 root         (0) root         (0)     8834 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawCameraControl.hpp
--rw-r--r--   0 root         (0) root         (0)     1364 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawEdgeDetectorConfig.hpp
--rw-r--r--   0 root         (0) root         (0)     5995 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawIMUData.hpp
--rw-r--r--   0 root         (0) root         (0)     3978 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImageManipConfig.hpp
--rw-r--r--   0 root         (0) root         (0)      801 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgDetections.hpp
--rw-r--r--   0 root         (0) root         (0)     2988 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgFrame.hpp
--rw-r--r--   0 root         (0) root         (0)     1479 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawNNData.hpp
--rw-r--r--   0 root         (0) root         (0)      933 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialImgDetections.hpp
--rw-r--r--   0 root         (0) root         (0)     1513 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocationCalculatorConfig.hpp
--rw-r--r--   0 root         (0) root         (0)     1979 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocations.hpp
--rw-r--r--   0 root         (0) root         (0)     1866 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawStereoDepthConfig.hpp
--rw-r--r--   0 root         (0) root         (0)     1304 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSystemInformation.hpp
--rw-r--r--   0 root         (0) root         (0)     1809 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawTracklets.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.004354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/
--rw-r--r--   0 root         (0) root         (0)      131 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/LogConstants.hpp
--rw-r--r--   0 root         (0) root         (0)      236 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/LogLevel.hpp
--rw-r--r--   0 root         (0) root         (0)      496 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/LogMessage.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1485 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/Assets.hpp
--rw-r--r--   0 root         (0) root         (0)      378 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/NodeConnectionSchema.hpp
--rw-r--r--   0 root         (0) root         (0)      404 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/NodeIoInfo.hpp
--rw-r--r--   0 root         (0) root         (0)      401 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/NodeObjInfo.hpp
--rw-r--r--   0 root         (0) root         (0)      804 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/PipelineSchema.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/
--rw-r--r--   0 root         (0) root         (0)     3754 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ColorCameraProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     1326 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/DetectionNetworkProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      789 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/EdgeDetectorProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     1215 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/GlobalProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     6765 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/IMUProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      759 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ImageManipProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     1205 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MonoCameraProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      420 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyConsumerProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      586 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyProducerProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      867 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/NeuralNetworkProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     1085 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ObjectTrackerProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      577 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SPIOutProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     1337 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialDetectionNetworkProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      570 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialLocationCalculatorProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     4745 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/StereoDepthProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      451 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SystemLoggerProperties.hpp
--rw-r--r--   0 root         (0) root         (0)     2519 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/VideoEncoderProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      583 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkInProperties.hpp
--rw-r--r--   0 root         (0) root         (0)      562 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkOutProperties.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/xlink/
--rw-r--r--   0 root         (0) root         (0)      586 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/xlink/XLinkConstants.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.984354 depthai-2.8.0.0/depthai-core/shared/depthai-shared/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/shared/depthai-shared/src/datatype/
--rw-r--r--   0 root         (0) root         (0)     3794 2021-07-23 13:42:50.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared/src/datatype/DatatypeEnum.cpp
--rw-r--r--   0 root         (0) root         (0)     1622 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/shared/depthai-shared.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/depthai-core/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/src/bspatch/
--rw-r--r--   0 root         (0) root         (0)     7604 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/bspatch/bspatch.c
--rw-r--r--   0 root         (0) root         (0)     1722 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/bspatch/bspatch.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/src/device/
--rw-r--r--   0 root         (0) root         (0)    33290 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/device/CalibrationHandler.cpp
--rw-r--r--   0 root         (0) root         (0)     1726 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/device/CallbackHandler.cpp
--rw-r--r--   0 root         (0) root         (0)    10215 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/device/DataQueue.cpp
--rw-r--r--   0 root         (0) root         (0)    40541 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/device/Device.cpp
--rw-r--r--   0 root         (0) root         (0)    25534 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/device/DeviceBootloader.cpp
--rw-r--r--   0 root         (0) root         (0)     1970 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/device/DeviceLogger.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.008355 depthai-2.8.0.0/depthai-core/src/opencv/
--rw-r--r--   0 root         (0) root         (0)     4872 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/opencv/ImgFrame.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.012354 depthai-2.8.0.0/depthai-core/src/openvino/
--rw-r--r--   0 root         (0) root         (0)     1690 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/openvino/BlobFormat.hpp
--rw-r--r--   0 root         (0) root         (0)     5802 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/openvino/BlobReader.cpp
--rw-r--r--   0 root         (0) root         (0)     1641 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/openvino/BlobReader.hpp
--rw-r--r--   0 root         (0) root         (0)     4364 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/openvino/OpenVINO.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.012354 depthai-2.8.0.0/depthai-core/src/pipeline/
--rw-r--r--   0 root         (0) root         (0)     3274 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/AssetManager.cpp
--rw-r--r--   0 root         (0) root         (0)     2539 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/Node.cpp
--rw-r--r--   0 root         (0) root         (0)    14405 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/Pipeline.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.012354 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/
--rw-r--r--   0 root         (0) root         (0)      491 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/Buffer.cpp
--rw-r--r--   0 root         (0) root         (0)     4475 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/CameraControl.cpp
--rw-r--r--   0 root         (0) root         (0)      881 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/EdgeDetectorConfig.cpp
--rw-r--r--   0 root         (0) root         (0)      448 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/IMUData.cpp
--rw-r--r--   0 root         (0) root         (0)     5199 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/ImageManipConfig.cpp
--rw-r--r--   0 root         (0) root         (0)      516 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/ImgDetections.cpp
--rw-r--r--   0 root         (0) root         (0)     2417 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/ImgFrame.cpp
--rw-r--r--   0 root         (0) root         (0)     8390 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/NNData.cpp
--rw-r--r--   0 root         (0) root         (0)      590 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SpatialImgDetections.cpp
--rw-r--r--   0 root         (0) root         (0)     1024 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorConfig.cpp
--rw-r--r--   0 root         (0) root         (0)      796 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorData.cpp
--rw-r--r--   0 root         (0) root         (0)     1362 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/StereoDepthConfig.cpp
--rw-r--r--   0 root         (0) root         (0)     9712 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.cpp
--rw-r--r--   0 root         (0) root         (0)      659 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.hpp
--rw-r--r--   0 root         (0) root         (0)     1369 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SystemInformation.cpp
--rw-r--r--   0 root         (0) root         (0)      484 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/datatype/Tracklets.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/depthai-core/src/pipeline/node/
--rw-r--r--   0 root         (0) root         (0)    11658 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/ColorCamera.cpp
--rw-r--r--   0 root         (0) root         (0)     2739 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/DetectionNetwork.cpp
--rw-r--r--   0 root         (0) root         (0)     1128 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/EdgeDetector.cpp
--rw-r--r--   0 root         (0) root         (0)     1775 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/IMU.cpp
--rw-r--r--   0 root         (0) root         (0)     2179 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/ImageManip.cpp
--rw-r--r--   0 root         (0) root         (0)     3392 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/MonoCamera.cpp
--rw-r--r--   0 root         (0) root         (0)      742 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/MyProducer.cpp
--rw-r--r--   0 root         (0) root         (0)     3104 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/NeuralNetwork.cpp
--rw-r--r--   0 root         (0) root         (0)     1363 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/ObjectTracker.cpp
--rw-r--r--   0 root         (0) root         (0)     3285 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/SpatialDetectionNetwork.cpp
--rw-r--r--   0 root         (0) root         (0)     1035 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/SpatialLocationCalculator.cpp
--rw-r--r--   0 root         (0) root         (0)     5264 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/StereoDepth.cpp
--rw-r--r--   0 root         (0) root         (0)      677 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/SystemLogger.cpp
--rw-r--r--   0 root         (0) root         (0)     5985 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/VideoEncoder.cpp
--rw-r--r--   0 root         (0) root         (0)     1081 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/XLinkIn.cpp
--rw-r--r--   0 root         (0) root         (0)     1091 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/pipeline/node/XLinkOut.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/depthai-core/src/utility/
--rw-r--r--   0 root         (0) root         (0)     1870 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/utility/BootloaderHelper.hpp
--rw-r--r--   0 root         (0) root         (0)     2274 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/utility/Initialization.cpp
--rw-r--r--   0 root         (0) root         (0)      487 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/utility/PimplImpl.hpp
--rw-r--r--   0 root         (0) root         (0)    14404 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/utility/Resources.cpp
--rw-r--r--   0 root         (0) root         (0)     1132 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/utility/Resources.hpp
--rw-r--r--   0 root         (0) root         (0)     4960 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/utility/matrixOps.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/depthai-core/src/xlink/
--rw-r--r--   0 root         (0) root         (0)    11783 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/xlink/XLinkConnection.cpp
--rw-r--r--   0 root         (0) root         (0)     6617 2021-07-23 13:42:49.000000 depthai-2.8.0.0/depthai-core/src/xlink/XLinkStream.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/depthai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8637 2021-07-23 13:45:01.000000 depthai-2.8.0.0/depthai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16499 2021-07-23 13:45:01.000000 depthai-2.8.0.0/depthai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-23 13:45:01.000000 depthai-2.8.0.0/depthai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-23 13:45:01.000000 depthai-2.8.0.0/depthai.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2021-07-23 13:45:01.000000 depthai-2.8.0.0/depthai.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/external/
--rw-r--r--   0 root         (0) root         (0)       47 2021-07-23 13:42:48.000000 depthai-2.8.0.0/external/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/external/hedley/
--rw-r--r--   0 root         (0) root         (0)      128 2021-07-23 13:42:48.000000 depthai-2.8.0.0/external/hedley/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:01.988354 depthai-2.8.0.0/external/hedley/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/external/hedley/include/hedley/
--rw-r--r--   0 root         (0) root         (0)    74181 2021-07-23 13:42:48.000000 depthai-2.8.0.0/external/hedley/include/hedley/hedley.h
--rw-r--r--   0 root         (0) root         (0)     1124 2021-07-23 13:42:48.000000 depthai-2.8.0.0/find_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.016355 depthai-2.8.0.0/generated/
--rw-r--r--   0 root         (0) root         (0)       23 2021-07-23 13:45:01.000000 depthai-2.8.0.0/generated/version.py
--rw-r--r--   0 root         (0) root         (0)       88 2021-07-23 13:42:48.000000 depthai-2.8.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-23 13:45:02.020355 depthai-2.8.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8263 2021-07-23 13:42:48.000000 depthai-2.8.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.020355 depthai-2.8.0.0/src/
--rw-r--r--   0 root         (0) root         (0)     6332 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/CalibrationHandlerBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      138 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/CalibrationHandlerBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     6566 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DataQueueBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      129 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DataQueueBindings.hpp
--rw-r--r--   0 root         (0) root         (0)    55828 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DatatypeBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      128 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DatatypeBindings.hpp
--rw-r--r--   0 root         (0) root         (0)    15607 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DeviceBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      126 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DeviceBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     4716 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DeviceBootloaderBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      136 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/DeviceBootloaderBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     2512 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/XLinkConnectionBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      135 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/XLinkConnectionBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     4245 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/device_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)      149 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/device_bindings.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.020355 depthai-2.8.0.0/src/log/
--rw-r--r--   0 root         (0) root         (0)      509 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/log/LogBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      123 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/log/LogBindings.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.020355 depthai-2.8.0.0/src/openvino/
--rw-r--r--   0 root         (0) root         (0)     2072 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/openvino/OpenVINOBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      127 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/openvino/OpenVINOBindings.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.020355 depthai-2.8.0.0/src/pipeline/
--rw-r--r--   0 root         (0) root         (0)     2358 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/AssetManagerBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      132 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/AssetManagerBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     5983 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/CommonBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      126 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/CommonBindings.hpp
--rw-r--r--   0 root         (0) root         (0)    59589 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/NodeBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      192 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/NodeBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     6244 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/PipelineBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      128 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pipeline/PipelineBindings.hpp
--rw-r--r--   0 root         (0) root         (0)     1795 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/py_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)      538 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/pybind11_common.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-23 13:45:02.020355 depthai-2.8.0.0/src/utility/
--rw-r--r--   0 root         (0) root         (0)      407 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/utility/ResourcesBindings.cpp
--rw-r--r--   0 root         (0) root         (0)      128 2021-07-23 13:42:48.000000 depthai-2.8.0.0/src/utility/ResourcesBindings.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.314061 depthai-2.9.0.0/
+-rw-r--r--   0 root         (0) root         (0)     9871 2021-08-07 07:37:16.000000 depthai-2.9.0.0/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1068 2021-08-07 07:37:16.000000 depthai-2.9.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      309 2021-08-07 07:37:16.000000 depthai-2.9.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8637 2021-08-07 07:41:06.310061 depthai-2.9.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7369 2021-08-07 07:37:16.000000 depthai-2.9.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.262061 depthai-2.9.0.0/ci/
+-rw-r--r--   0 root         (0) root         (0)      690 2021-08-07 07:37:16.000000 depthai-2.9.0.0/ci/Dockerfile
+-rwxr-xr-x   0 root         (0) root         (0)      722 2021-08-07 07:37:16.000000 depthai-2.9.0.0/ci/build-wheels.sh
+-rwxr-xr-x   0 root         (0) root         (0)      215 2021-08-07 07:37:16.000000 depthai-2.9.0.0/ci/repair-whl-macos.sh
+-rwxr-xr-x   0 root         (0) root         (0)      292 2021-08-07 07:37:16.000000 depthai-2.9.0.0/ci/upload-artifactory.sh
+-rwxr-xr-x   0 root         (0) root         (0)      806 2021-08-07 07:37:16.000000 depthai-2.9.0.0/ci/upload-pypi.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.262061 depthai-2.9.0.0/cmake/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.262061 depthai-2.9.0.0/cmake/Hunter/
+-rw-r--r--   0 root         (0) root         (0)      196 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/Hunter/config.cmake
+-rw-r--r--   0 root         (0) root         (0)    17070 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/HunterGate.cmake
+-rw-r--r--   0 root         (0) root         (0)      156 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/default_docstring.hpp.in
+-rw-r--r--   0 root         (0) root         (0)       34 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/docstring.hpp.in
+-rw-r--r--   0 root         (0) root         (0)     3056 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/pybind11-mkdoc.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.262061 depthai-2.9.0.0/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)      115 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/toolchain/msvc.cmake
+-rw-r--r--   0 root         (0) root         (0)       97 2021-08-07 07:37:16.000000 depthai-2.9.0.0/cmake/toolchain/pic.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.266061 depthai-2.9.0.0/depthai-core/
+-rw-r--r--   0 root         (0) root         (0)      388 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/.clang-format
+-rw-r--r--   0 root         (0) root         (0)    14785 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/.clang-tidy
+-rw-r--r--   0 root         (0) root         (0)       37 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/.git
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.254061 depthai-2.9.0.0/depthai-core/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.266061 depthai-2.9.0.0/depthai-core/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     8103 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/.github/workflows/main.workflow.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      245 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/.gitmodules
+-rw-r--r--   0 root         (0) root         (0)    21919 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1068 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5996 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.266061 depthai-2.9.0.0/depthai-core/ci/
+-rwxr-xr-x   0 root         (0) root         (0)      227 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/ci/check_format.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.266061 depthai-2.9.0.0/depthai-core/cmake/
+-rw-r--r--   0 root         (0) root         (0)    35978 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/CMakeRC.cmake
+-rw-r--r--   0 root         (0) root         (0)     1998 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/ClangFormat.cmake
+-rw-r--r--   0 root         (0) root         (0)      568 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/ClangTidy.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.266061 depthai-2.9.0.0/depthai-core/cmake/Depthai/
+-rw-r--r--   0 root         (0) root         (0)      151 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/Depthai/DepthaiBootloaderConfig.cmake
+-rw-r--r--   0 root         (0) root         (0)      267 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/Depthai/DepthaiDeviceSideConfig.cmake
+-rw-r--r--   0 root         (0) root         (0)     8402 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/DepthaiBootloaderDownloader.cmake
+-rw-r--r--   0 root         (0) root         (0)    12479 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/DepthaiDownloader.cmake
+-rw-r--r--   0 root         (0) root         (0)     3224 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/Flags.cmake
+-rw-r--r--   0 root         (0) root         (0)      464 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/GitCommitHash.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.266061 depthai-2.9.0.0/depthai-core/cmake/Hunter/
+-rw-r--r--   0 root         (0) root         (0)     2042 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/Hunter/config.cmake
+-rw-r--r--   0 root         (0) root         (0)    17070 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/HunterGate.cmake
+-rw-r--r--   0 root         (0) root         (0)      283 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/config.hpp.in
+-rw-r--r--   0 root         (0) root         (0)      518 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/depthaiConfig.cmake.in
+-rw-r--r--   0 root         (0) root         (0)     1637 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/depthaiDependencies.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/cmake/sanitizers/
+-rw-r--r--   0 root         (0) root         (0)     2144 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindASan.cmake
+-rw-r--r--   0 root         (0) root         (0)     2292 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindMSan.cmake
+-rwxr-xr-x   0 root         (0) root         (0)     3737 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindSanitizers.cmake
+-rw-r--r--   0 root         (0) root         (0)     2555 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindTSan.cmake
+-rw-r--r--   0 root         (0) root         (0)     1696 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindUBSan.cmake
+-rwxr-xr-x   0 root         (0) root         (0)     2011 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/asan-wrapper
+-rwxr-xr-x   0 root         (0) root         (0)     7684 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/sanitizers/sanitize-helpers.cmake
+-rw-r--r--   0 root         (0) root         (0)     2436 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/target-public-headers.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)      162 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/toolchain/pic.cmake
+-rw-r--r--   0 root         (0) root         (0)      710 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/cmake/version.hpp.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/docs/
+-rw-r--r--   0 root         (0) root         (0)     1670 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/docs/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)   112781 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/docs/Doxyfile.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.254061 depthai-2.9.0.0/depthai-core/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/include/depthai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/include/depthai/build/
+-rw-r--r--   0 root         (0) root         (0)      283 2021-08-07 07:39:27.000000 depthai-2.9.0.0/depthai-core/include/depthai/build/config.hpp
+-rw-r--r--   0 root         (0) root         (0)      662 2021-08-07 07:39:27.000000 depthai-2.9.0.0/depthai-core/include/depthai/build/version.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/include/depthai/common/
+-rw-r--r--   0 root         (0) root         (0)      594 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/common/CameraBoardSocket.hpp
+-rw-r--r--   0 root         (0) root         (0)      707 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/common/UsbSpeed.hpp
+-rw-r--r--   0 root         (0) root         (0)      570 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/depthai.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/include/depthai/device/
+-rw-r--r--   0 root         (0) root         (0)    20601 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/device/CalibrationHandler.hpp
+-rw-r--r--   0 root         (0) root         (0)      846 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/device/CallbackHandler.hpp
+-rw-r--r--   0 root         (0) root         (0)    14197 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/device/DataQueue.hpp
+-rw-r--r--   0 root         (0) root         (0)    20509 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/device/Device.hpp
+-rw-r--r--   0 root         (0) root         (0)     7844 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/device/DeviceBootloader.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.270061 depthai-2.9.0.0/depthai-core/include/depthai/openvino/
+-rw-r--r--   0 root         (0) root         (0)     2214 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/openvino/OpenVINO.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.274061 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     3335 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/AssetManager.hpp
+-rw-r--r--   0 root         (0) root         (0)     7648 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/Node.hpp
+-rw-r--r--   0 root         (0) root         (0)     7745 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/Pipeline.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.274061 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/
+-rw-r--r--   0 root         (0) root         (0)      530 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ADatatype.hpp
+-rw-r--r--   0 root         (0) root         (0)      722 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/Buffer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5118 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/CameraControl.hpp
+-rw-r--r--   0 root         (0) root         (0)     1242 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/EdgeDetectorConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)      602 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/IMUData.hpp
+-rw-r--r--   0 root         (0) root         (0)     5163 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ImageManipConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)      660 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ImgDetections.hpp
+-rw-r--r--   0 root         (0) root         (0)     4530 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ImgFrame.hpp
+-rw-r--r--   0 root         (0) root         (0)     3971 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/NNData.hpp
+-rw-r--r--   0 root         (0) root         (0)      795 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialImgDetections.hpp
+-rw-r--r--   0 root         (0) root         (0)     1446 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)     1029 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorData.hpp
+-rw-r--r--   0 root         (0) root         (0)     1827 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/StereoDepthConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)      917 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SystemInformation.hpp
+-rw-r--r--   0 root         (0) root         (0)     1264 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/Tracklets.hpp
+-rw-r--r--   0 root         (0) root         (0)      545 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatypes.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.278061 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/
+-rw-r--r--   0 root         (0) root         (0)     8920 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/ColorCamera.hpp
+-rw-r--r--   0 root         (0) root         (0)     2714 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/DetectionNetwork.hpp
+-rw-r--r--   0 root         (0) root         (0)     2179 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/EdgeDetector.hpp
+-rw-r--r--   0 root         (0) root         (0)     1942 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/IMU.hpp
+-rw-r--r--   0 root         (0) root         (0)     2918 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/ImageManip.hpp
+-rw-r--r--   0 root         (0) root         (0)     3093 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/MonoCamera.hpp
+-rw-r--r--   0 root         (0) root         (0)      670 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/MyProducer.hpp
+-rw-r--r--   0 root         (0) root         (0)     2683 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/NeuralNetwork.hpp
+-rw-r--r--   0 root         (0) root         (0)     3626 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/ObjectTracker.hpp
+-rw-r--r--   0 root         (0) root         (0)     1656 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SPIIn.hpp
+-rw-r--r--   0 root         (0) root         (0)     1480 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SPIOut.hpp
+-rw-r--r--   0 root         (0) root         (0)     2211 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/Script.hpp
+-rw-r--r--   0 root         (0) root         (0)     4335 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SpatialDetectionNetwork.hpp
+-rw-r--r--   0 root         (0) root         (0)     2369 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SpatialLocationCalculator.hpp
+-rw-r--r--   0 root         (0) root         (0)     8703 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/StereoDepth.hpp
+-rw-r--r--   0 root         (0) root         (0)     1008 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SystemLogger.hpp
+-rw-r--r--   0 root         (0) root         (0)     4446 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/VideoEncoder.hpp
+-rw-r--r--   0 root         (0) root         (0)     1539 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/XLinkIn.hpp
+-rw-r--r--   0 root         (0) root         (0)     1640 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/XLinkOut.hpp
+-rw-r--r--   0 root         (0) root         (0)      642 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/pipeline/nodes.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.278061 depthai-2.9.0.0/depthai-core/include/depthai/utility/
+-rw-r--r--   0 root         (0) root         (0)      121 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/utility/Initialization.hpp
+-rw-r--r--   0 root         (0) root         (0)     6267 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/utility/LockingQueue.hpp
+-rw-r--r--   0 root         (0) root         (0)      320 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/utility/Pimpl.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.278061 depthai-2.9.0.0/depthai-core/include/depthai/xlink/
+-rw-r--r--   0 root         (0) root         (0)     2920 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/xlink/XLinkConnection.hpp
+-rw-r--r--   0 root         (0) root         (0)     1950 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/include/depthai/xlink/XLinkStream.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.278061 depthai-2.9.0.0/depthai-core/shared/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.278061 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/
+-rw-r--r--   0 root         (0) root         (0)       84 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/.git
+-rw-r--r--   0 root         (0) root         (0)     1084 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/
+-rw-r--r--   0 root         (0) root         (0)     3688 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Bootloader.hpp
+-rw-r--r--   0 root         (0) root         (0)      181 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Memory.hpp
+-rw-r--r--   0 root         (0) root         (0)     1336 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/NetworkBootloaderConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)     2284 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/SBR.h
+-rw-r--r--   0 root         (0) root         (0)      222 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Section.hpp
+-rw-r--r--   0 root         (0) root         (0)      365 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Structure.hpp
+-rw-r--r--   0 root         (0) root         (0)      180 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Type.hpp
+-rw-r--r--   0 root         (0) root         (0)     1360 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/UsbBootloaderConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)      496 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/XLinkConstants.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/src/
+-rw-r--r--   0 root         (0) root         (0)     5807 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/src/SBR.c
+-rw-r--r--   0 root         (0) root         (0)     1621 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/
+-rw-r--r--   0 root         (0) root         (0)       73 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/.git
+-rw-r--r--   0 root         (0) root         (0)       85 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/invoke_hpp/
+-rw-r--r--   0 root         (0) root         (0)     8630 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/invoke_hpp/invoke.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/linb/
+-rw-r--r--   0 root         (0) root         (0)    15977 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/linb/any.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/
+-rw-r--r--   0 root         (0) root         (0)     4230 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/client.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/
+-rw-r--r--   0 root         (0) root         (0)      399 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/config.h
+-rw-r--r--   0 root         (0) root         (0)     1164 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/function_meta.h
+-rw-r--r--   0 root         (0) root         (0)      763 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/pack_meta.h
+-rw-r--r--   0 root         (0) root         (0)     1774 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/exception.h
+-rw-r--r--   0 root         (0) root         (0)      457 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/hash.h
+-rw-r--r--   0 root         (0) root         (0)     5263 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/server.h
+-rw-r--r--   0 root         (0) root         (0)      834 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/type.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/
+-rw-r--r--   0 root         (0) root         (0)     4785 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/cereal_binary.h
+-rw-r--r--   0 root         (0) root         (0)     3365 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_json.h
+-rw-r--r--   0 root         (0) root         (0)     3252 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_msgpack.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/version/
+-rw-r--r--   0 root         (0) root         (0)      594 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/version/core.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.282061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/tl/
+-rw-r--r--   0 root         (0) root         (0)    73553 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/tl/optional.hpp
+-rw-r--r--   0 root         (0) root         (0)     1068 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.286061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/
+-rw-r--r--   0 root         (0) root         (0)      252 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraBoardSocket.hpp
+-rw-r--r--   0 root         (0) root         (0)      443 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraImageOrientation.hpp
+-rw-r--r--   0 root         (0) root         (0)      631 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraInfo.hpp
+-rw-r--r--   0 root         (0) root         (0)      252 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraModel.hpp
+-rw-r--r--   0 root         (0) root         (0)      577 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/ChipTemperature.hpp
+-rw-r--r--   0 root         (0) root         (0)      483 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CpuUsage.hpp
+-rw-r--r--   0 root         (0) root         (0)      102 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/DetectionNetworkType.hpp
+-rw-r--r--   0 root         (0) root         (0)      928 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/EepromData.hpp
+-rw-r--r--   0 root         (0) root         (0)      726 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Extrinsics.hpp
+-rw-r--r--   0 root         (0) root         (0)      314 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/MemoryInfo.hpp
+-rw-r--r--   0 root         (0) root         (0)      394 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Point2f.hpp
+-rw-r--r--   0 root         (0) root         (0)      432 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Point3f.hpp
+-rw-r--r--   0 root         (0) root         (0)      226 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/ProcessorType.hpp
+-rw-r--r--   0 root         (0) root         (0)     3606 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Rect.hpp
+-rw-r--r--   0 root         (0) root         (0)      435 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/RotatedRect.hpp
+-rw-r--r--   0 root         (0) root         (0)      446 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Size2f.hpp
+-rw-r--r--   0 root         (0) root         (0)      528 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/StereoRectification.hpp
+-rw-r--r--   0 root         (0) root         (0)      525 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Timestamp.hpp
+-rw-r--r--   0 root         (0) root         (0)      184 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/UsbSpeed.hpp
+-rw-r--r--   0 root         (0) root         (0)      962 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/optional.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.290061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/
+-rw-r--r--   0 root         (0) root         (0)      481 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/DatatypeEnum.hpp
+-rw-r--r--   0 root         (0) root         (0)      485 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawBuffer.hpp
+-rw-r--r--   0 root         (0) root         (0)     8834 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawCameraControl.hpp
+-rw-r--r--   0 root         (0) root         (0)     1364 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawEdgeDetectorConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)     5995 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawIMUData.hpp
+-rw-r--r--   0 root         (0) root         (0)     3978 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImageManipConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)      801 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgDetections.hpp
+-rw-r--r--   0 root         (0) root         (0)     2988 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgFrame.hpp
+-rw-r--r--   0 root         (0) root         (0)     1479 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawNNData.hpp
+-rw-r--r--   0 root         (0) root         (0)      933 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialImgDetections.hpp
+-rw-r--r--   0 root         (0) root         (0)     1513 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocationCalculatorConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)     1979 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocations.hpp
+-rw-r--r--   0 root         (0) root         (0)     1866 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawStereoDepthConfig.hpp
+-rw-r--r--   0 root         (0) root         (0)     1304 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSystemInformation.hpp
+-rw-r--r--   0 root         (0) root         (0)     1809 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawTracklets.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.290061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/
+-rw-r--r--   0 root         (0) root         (0)      131 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/LogConstants.hpp
+-rw-r--r--   0 root         (0) root         (0)      236 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/LogLevel.hpp
+-rw-r--r--   0 root         (0) root         (0)      496 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/log/LogMessage.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.290061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1485 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/Assets.hpp
+-rw-r--r--   0 root         (0) root         (0)      378 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/NodeConnectionSchema.hpp
+-rw-r--r--   0 root         (0) root         (0)      404 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/NodeIoInfo.hpp
+-rw-r--r--   0 root         (0) root         (0)      401 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/NodeObjInfo.hpp
+-rw-r--r--   0 root         (0) root         (0)      804 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/PipelineSchema.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.294061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/
+-rw-r--r--   0 root         (0) root         (0)     3754 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ColorCameraProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     1326 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/DetectionNetworkProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      789 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/EdgeDetectorProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     1215 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/GlobalProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     6765 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/IMUProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      759 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ImageManipProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     1205 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MonoCameraProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      420 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyConsumerProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      591 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyProducerProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      867 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/NeuralNetworkProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     1085 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ObjectTrackerProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      614 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SPIInProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      355 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SPIOutProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      668 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ScriptProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     1337 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialDetectionNetworkProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      570 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialLocationCalculatorProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     4745 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/StereoDepthProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      451 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SystemLoggerProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)     2519 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/VideoEncoderProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      583 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkInProperties.hpp
+-rw-r--r--   0 root         (0) root         (0)      562 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkOutProperties.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.294061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/xlink/
+-rw-r--r--   0 root         (0) root         (0)      586 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/xlink/XLinkConstants.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.294061 depthai-2.9.0.0/depthai-core/shared/depthai-shared/src/datatype/
+-rw-r--r--   0 root         (0) root         (0)     3794 2021-08-07 07:37:18.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared/src/datatype/DatatypeEnum.cpp
+-rw-r--r--   0 root         (0) root         (0)     1622 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/shared/depthai-shared.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/depthai-core/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.294061 depthai-2.9.0.0/depthai-core/src/bspatch/
+-rw-r--r--   0 root         (0) root         (0)     7604 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/bspatch/bspatch.c
+-rw-r--r--   0 root         (0) root         (0)     1722 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/bspatch/bspatch.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.298061 depthai-2.9.0.0/depthai-core/src/device/
+-rw-r--r--   0 root         (0) root         (0)    33290 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/device/CalibrationHandler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1726 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/device/CallbackHandler.cpp
+-rw-r--r--   0 root         (0) root         (0)    10215 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/device/DataQueue.cpp
+-rw-r--r--   0 root         (0) root         (0)    40541 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/device/Device.cpp
+-rw-r--r--   0 root         (0) root         (0)    25899 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/device/DeviceBootloader.cpp
+-rw-r--r--   0 root         (0) root         (0)     1970 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/device/DeviceLogger.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.298061 depthai-2.9.0.0/depthai-core/src/opencv/
+-rw-r--r--   0 root         (0) root         (0)     4872 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/opencv/ImgFrame.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.298061 depthai-2.9.0.0/depthai-core/src/openvino/
+-rw-r--r--   0 root         (0) root         (0)     1690 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/openvino/BlobFormat.hpp
+-rw-r--r--   0 root         (0) root         (0)     5802 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/openvino/BlobReader.cpp
+-rw-r--r--   0 root         (0) root         (0)     1641 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/openvino/BlobReader.hpp
+-rw-r--r--   0 root         (0) root         (0)     4364 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/openvino/OpenVINO.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.298061 depthai-2.9.0.0/depthai-core/src/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     4267 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/AssetManager.cpp
+-rw-r--r--   0 root         (0) root         (0)     5257 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/Node.cpp
+-rw-r--r--   0 root         (0) root         (0)    14186 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/Pipeline.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.302061 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/
+-rw-r--r--   0 root         (0) root         (0)      491 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/Buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)     4475 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/CameraControl.cpp
+-rw-r--r--   0 root         (0) root         (0)      881 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/EdgeDetectorConfig.cpp
+-rw-r--r--   0 root         (0) root         (0)      448 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/IMUData.cpp
+-rw-r--r--   0 root         (0) root         (0)     5436 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/ImageManipConfig.cpp
+-rw-r--r--   0 root         (0) root         (0)      516 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/ImgDetections.cpp
+-rw-r--r--   0 root         (0) root         (0)     2417 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/ImgFrame.cpp
+-rw-r--r--   0 root         (0) root         (0)     8390 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/NNData.cpp
+-rw-r--r--   0 root         (0) root         (0)      590 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SpatialImgDetections.cpp
+-rw-r--r--   0 root         (0) root         (0)     1024 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorConfig.cpp
+-rw-r--r--   0 root         (0) root         (0)      796 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorData.cpp
+-rw-r--r--   0 root         (0) root         (0)     1362 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/StereoDepthConfig.cpp
+-rw-r--r--   0 root         (0) root         (0)     9822 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.cpp
+-rw-r--r--   0 root         (0) root         (0)      659 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.hpp
+-rw-r--r--   0 root         (0) root         (0)     1369 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SystemInformation.cpp
+-rw-r--r--   0 root         (0) root         (0)      484 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/datatype/Tracklets.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.302061 depthai-2.9.0.0/depthai-core/src/pipeline/node/
+-rw-r--r--   0 root         (0) root         (0)    11658 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/ColorCamera.cpp
+-rw-r--r--   0 root         (0) root         (0)     2826 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/DetectionNetwork.cpp
+-rw-r--r--   0 root         (0) root         (0)     1128 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/EdgeDetector.cpp
+-rw-r--r--   0 root         (0) root         (0)     1775 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/IMU.cpp
+-rw-r--r--   0 root         (0) root         (0)     2179 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/ImageManip.cpp
+-rw-r--r--   0 root         (0) root         (0)     3392 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/MonoCamera.cpp
+-rw-r--r--   0 root         (0) root         (0)      742 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/MyProducer.cpp
+-rw-r--r--   0 root         (0) root         (0)     2142 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/NeuralNetwork.cpp
+-rw-r--r--   0 root         (0) root         (0)     1363 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/ObjectTracker.cpp
+-rw-r--r--   0 root         (0) root         (0)     1204 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/SPIIn.cpp
+-rw-r--r--   0 root         (0) root         (0)     2191 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/Script.cpp
+-rw-r--r--   0 root         (0) root         (0)     3285 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/SpatialDetectionNetwork.cpp
+-rw-r--r--   0 root         (0) root         (0)     1035 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/SpatialLocationCalculator.cpp
+-rw-r--r--   0 root         (0) root         (0)     5224 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/StereoDepth.cpp
+-rw-r--r--   0 root         (0) root         (0)      677 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/SystemLogger.cpp
+-rw-r--r--   0 root         (0) root         (0)     5985 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/VideoEncoder.cpp
+-rw-r--r--   0 root         (0) root         (0)     1081 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/XLinkIn.cpp
+-rw-r--r--   0 root         (0) root         (0)     1091 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/pipeline/node/XLinkOut.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/depthai-core/src/utility/
+-rw-r--r--   0 root         (0) root         (0)     1870 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/utility/BootloaderHelper.hpp
+-rw-r--r--   0 root         (0) root         (0)     2277 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/utility/Initialization.cpp
+-rw-r--r--   0 root         (0) root         (0)      487 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/utility/PimplImpl.hpp
+-rw-r--r--   0 root         (0) root         (0)    14404 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/utility/Resources.cpp
+-rw-r--r--   0 root         (0) root         (0)     1132 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/utility/Resources.hpp
+-rw-r--r--   0 root         (0) root         (0)     4960 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/utility/matrixOps.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/depthai-core/src/xlink/
+-rw-r--r--   0 root         (0) root         (0)    11783 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/xlink/XLinkConnection.cpp
+-rw-r--r--   0 root         (0) root         (0)     6617 2021-08-07 07:37:17.000000 depthai-2.9.0.0/depthai-core/src/xlink/XLinkStream.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/depthai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8637 2021-08-07 07:41:06.000000 depthai-2.9.0.0/depthai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16868 2021-08-07 07:41:06.000000 depthai-2.9.0.0/depthai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-07 07:41:06.000000 depthai-2.9.0.0/depthai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-07 07:41:06.000000 depthai-2.9.0.0/depthai.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        8 2021-08-07 07:41:06.000000 depthai-2.9.0.0/depthai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/external/
+-rw-r--r--   0 root         (0) root         (0)       47 2021-08-07 07:37:16.000000 depthai-2.9.0.0/external/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/external/hedley/
+-rw-r--r--   0 root         (0) root         (0)      128 2021-08-07 07:37:16.000000 depthai-2.9.0.0/external/hedley/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.258061 depthai-2.9.0.0/external/hedley/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/external/hedley/include/hedley/
+-rw-r--r--   0 root         (0) root         (0)    74181 2021-08-07 07:37:16.000000 depthai-2.9.0.0/external/hedley/include/hedley/hedley.h
+-rw-r--r--   0 root         (0) root         (0)     1124 2021-08-07 07:37:16.000000 depthai-2.9.0.0/find_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.306061 depthai-2.9.0.0/generated/
+-rw-r--r--   0 root         (0) root         (0)       23 2021-08-07 07:41:06.000000 depthai-2.9.0.0/generated/version.py
+-rw-r--r--   0 root         (0) root         (0)       88 2021-08-07 07:37:16.000000 depthai-2.9.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-07 07:41:06.314061 depthai-2.9.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8263 2021-08-07 07:37:16.000000 depthai-2.9.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.310061 depthai-2.9.0.0/src/
+-rw-r--r--   0 root         (0) root         (0)     7074 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/CalibrationHandlerBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      156 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/CalibrationHandlerBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     7367 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DataQueueBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      147 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DataQueueBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)    58284 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DatatypeBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      146 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DatatypeBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)    17692 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DeviceBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      144 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DeviceBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     6168 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DeviceBootloaderBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      154 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/DeviceBootloaderBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     3464 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/XLinkConnectionBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      153 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/XLinkConnectionBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     4245 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/device_bindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      149 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/device_bindings.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.310061 depthai-2.9.0.0/src/log/
+-rw-r--r--   0 root         (0) root         (0)     1232 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/log/LogBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      141 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/log/LogBindings.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.310061 depthai-2.9.0.0/src/openvino/
+-rw-r--r--   0 root         (0) root         (0)     2817 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/openvino/OpenVINOBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      145 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/openvino/OpenVINOBindings.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.310061 depthai-2.9.0.0/src/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     3597 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/AssetManagerBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      150 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/AssetManagerBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     7392 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/CommonBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      144 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/CommonBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)    68681 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/NodeBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      354 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/NodeBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     7880 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/PipelineBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      146 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pipeline/PipelineBindings.hpp
+-rw-r--r--   0 root         (0) root         (0)     2214 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/py_bindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      671 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/pybind11_common.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-07 07:41:06.310061 depthai-2.9.0.0/src/utility/
+-rw-r--r--   0 root         (0) root         (0)      424 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/utility/ResourcesBindings.cpp
+-rw-r--r--   0 root         (0) root         (0)      146 2021-08-07 07:37:16.000000 depthai-2.9.0.0/src/utility/ResourcesBindings.hpp
```

### Comparing `depthai-2.8.0.0/CMakeLists.txt` & `depthai-2.9.0.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/LICENSE` & `depthai-2.9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/PKG-INFO` & `depthai-2.9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthai
-Version: 2.8.0.0
+Version: 2.9.0.0
 Summary: DepthAI Python Library
 Home-page: https://github.com/luxonis/depthai-python
 Author: Martin Peterlin
 Author-email: martin@luxonis.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `depthai-2.8.0.0/README.md` & `depthai-2.9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/ci/Dockerfile` & `depthai-2.9.0.0/ci/Dockerfile`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/ci/build-wheels.sh` & `depthai-2.9.0.0/ci/build-wheels.sh`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/ci/upload-pypi.sh` & `depthai-2.9.0.0/ci/upload-pypi.sh`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/cmake/HunterGate.cmake` & `depthai-2.9.0.0/cmake/HunterGate.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/cmake/pybind11-mkdoc.cmake` & `depthai-2.9.0.0/cmake/pybind11-mkdoc.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         # Execute mkdoc
         COMMAND
             ${PYTHON_EXECUTABLE}
             -m ${PYBIND11_MKDOC_MODULE_NAME}
             # Docstring wrap width
             -w 80
             -o "${output_path}"
+            # C++ standard
+            -std=c++14
             # List of include directories
             "-I$<JOIN:$<TARGET_PROPERTY:${target},INTERFACE_INCLUDE_DIRECTORIES>,;-I>"
             # List of compiler definitions
             "-D$<JOIN:$<TARGET_PROPERTY:${target},INTERFACE_COMPILE_DEFINITIONS>,;-D>"
             # List of headers for which to generate docstrings
             "${mkdoc_headers}"
             # Redirect stderr to not spam output
```

### Comparing `depthai-2.8.0.0/depthai-core/.clang-tidy` & `depthai-2.9.0.0/depthai-core/.clang-tidy`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/.github/workflows/main.workflow.yml` & `depthai-2.9.0.0/depthai-core/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/CMakeLists.txt` & `depthai-2.9.0.0/depthai-core/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # Move binary dir if windows, to shorten the path
 if(WIN32)
     set(HUNTER_BINARY_DIR "${HUNTER_GATE_ROOT}/_bin" CACHE STRING "Hunter binary directory")
 endif()
 
 # Create depthai project
-project(depthai VERSION "2.8.0" LANGUAGES CXX C)
+project(depthai VERSION "2.9.0" LANGUAGES CXX C)
 get_directory_property(has_parent PARENT_DIRECTORY)
 if(has_parent)
     set(DEPTHAI_VERSION ${PROJECT_VERSION} PARENT_SCOPE)
 endif()
 
 # Set default build type depending on context
 set(default_build_type "Release")
@@ -148,20 +148,22 @@
     src/pipeline/node/MonoCamera.cpp
     src/pipeline/node/StereoDepth.cpp
     src/pipeline/node/NeuralNetwork.cpp
     src/pipeline/node/ImageManip.cpp
     src/pipeline/node/MyProducer.cpp
     src/pipeline/node/VideoEncoder.cpp
     src/pipeline/node/DetectionNetwork.cpp
+    src/pipeline/node/Script.cpp
     src/pipeline/node/SpatialDetectionNetwork.cpp
     src/pipeline/node/SystemLogger.cpp
     src/pipeline/node/SpatialLocationCalculator.cpp
     src/pipeline/node/ObjectTracker.cpp
     src/pipeline/node/IMU.cpp
     src/pipeline/node/EdgeDetector.cpp
+    src/pipeline/node/SPIIn.cpp
     src/pipeline/datatype/Buffer.cpp
     src/pipeline/datatype/ImgFrame.cpp
     src/pipeline/datatype/ImageManipConfig.cpp
     src/pipeline/datatype/CameraControl.cpp
     src/pipeline/datatype/NNData.cpp
     src/pipeline/datatype/ImgDetections.cpp
     src/pipeline/datatype/SpatialImgDetections.cpp
```

### Comparing `depthai-2.8.0.0/depthai-core/LICENSE` & `depthai-2.9.0.0/depthai-core/LICENSE`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/README.md` & `depthai-2.9.0.0/depthai-core/README.md`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/CMakeRC.cmake` & `depthai-2.9.0.0/depthai-core/cmake/CMakeRC.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/ClangFormat.cmake` & `depthai-2.9.0.0/depthai-core/cmake/ClangFormat.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/ClangTidy.cmake` & `depthai-2.9.0.0/depthai-core/cmake/ClangTidy.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/DepthaiBootloaderDownloader.cmake` & `depthai-2.9.0.0/depthai-core/cmake/DepthaiBootloaderDownloader.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/DepthaiDownloader.cmake` & `depthai-2.9.0.0/depthai-core/cmake/DepthaiDownloader.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/Flags.cmake` & `depthai-2.9.0.0/depthai-core/cmake/Flags.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/Hunter/config.cmake` & `depthai-2.9.0.0/depthai-core/cmake/Hunter/config.cmake`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,17 @@
     VERSION "3.9.1"
     URL "https://github.com/nlohmann/json/archive/v3.9.1.tar.gz"
     SHA1 "f8a20a7e19227906d77de0ede97468fbcfea03e7"
 )
 
 hunter_config(
     XLink
-    VERSION "luxonis-2021.3-develop"
-    URL "https://github.com/luxonis/XLink/archive/1a89b3003529ccbed90a32cf7c13438be1901744.tar.gz"
-    SHA1 "5a0ce8016edf9a5092290b2971eba5e1f37059ee"
+    VERSION "luxonis-2021.3-master"
+    URL "https://github.com/luxonis/XLink/archive/2c6cdb857f3d21088b34ec172a0ea8df16528d00.tar.gz"
+    SHA1 "736da6528515d9c969008e2334f1387428f91a3b"
 )
 
 hunter_config(
     BZip2
     VERSION "1.0.8-p0"
 )
 
@@ -60,7 +60,18 @@
         ENABLE_TAR_SHARED=OFF
         ENABLE_TEST=OFF
         ENABLE_WERROR=OFF
         ENABLE_XATTR=OFF
         ENABLE_ZLIB=OFF
         ENABLE_ZSTD=OFF
 )
+
+# Luxonis FP16 fork which doesn't use git cloning for its dependencies
+hunter_config(
+    FP16
+    VERSION "luxonis-0.0.0"
+    URL "https://github.com/luxonis/FP16/archive/c911175d2717e562976e606c6e5f799bf40cf94e.tar.gz"
+    SHA1 "40e9723c87c2fe21781132c0f2f8b90338500e32"
+    CMAKE_ARGS
+        FP16_BUILD_BENCHMARKS=OFF
+        FP16_BUILD_TESTS=OFF
+)
```

### Comparing `depthai-2.8.0.0/depthai-core/cmake/HunterGate.cmake` & `depthai-2.9.0.0/depthai-core/cmake/HunterGate.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/depthaiConfig.cmake.in` & `depthai-2.9.0.0/depthai-core/cmake/depthaiConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/depthaiDependencies.cmake` & `depthai-2.9.0.0/depthai-core/cmake/depthaiDependencies.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindASan.cmake` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindASan.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindMSan.cmake` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindMSan.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindSanitizers.cmake` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindSanitizers.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindTSan.cmake` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindTSan.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/FindUBSan.cmake` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/FindUBSan.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/asan-wrapper` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/asan-wrapper`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/sanitizers/sanitize-helpers.cmake` & `depthai-2.9.0.0/depthai-core/cmake/sanitizers/sanitize-helpers.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/target-public-headers.cmake` & `depthai-2.9.0.0/depthai-core/cmake/target-public-headers.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/cmake/version.hpp.in` & `depthai-2.9.0.0/depthai-core/cmake/version.hpp.in`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/docs/CMakeLists.txt` & `depthai-2.9.0.0/depthai-core/docs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/docs/Doxyfile.in` & `depthai-2.9.0.0/depthai-core/docs/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/build/version.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/build/version.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,17 @@
  */
 #pragma once
 
 namespace dai
 {
 namespace build
 {
-    constexpr static const char* VERSION = "2.8.0";
+    constexpr static const char* VERSION = "2.9.0";
     constexpr static const int VERSION_MAJOR = 2;
-    constexpr static const int VERSION_MINOR = 8;
+    constexpr static const int VERSION_MINOR = 9;
     constexpr static const int VERSION_PATCH = 0;
 
-    constexpr static const char* COMMIT = "7d76a830ffc51512adae455ec28b1150eabec513";
-    constexpr static const char* COMMIT_DATETIME = "2021-07-23 15:42:59 +0300";
-    constexpr static const char* BUILD_DATETIME = "2021-07-23 13:43:47 +0000";
+    constexpr static const char* COMMIT = "119c29986e43a84f1a0d9d670f55a303d102fd1e";
+    constexpr static const char* COMMIT_DATETIME = "2021-08-07 03:07:40 +0200";
+    constexpr static const char* BUILD_DATETIME = "2021-08-07 07:39:27 +0000";
 } // namespace build
 } // namespace dai
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/common/CameraBoardSocket.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/common/CameraBoardSocket.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/common/UsbSpeed.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/common/UsbSpeed.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/depthai.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/depthai.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/device/CalibrationHandler.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/device/CalibrationHandler.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
      */
     std::tuple<std::vector<std::vector<float>>, int, int> getDefaultIntrinsics(CameraBoardSocket cameraId);
 
     /**
      * Get the Distortion Coefficients object
      *
      * @param cameraId Uses the cameraId to identify which distortion Coefficients to return.
-     * @return repesents the distortion coefficients of the requested camera.
+     * @return the distortion coefficients of the requested camera in this order: [k1,k2,p1,p2,k3,k4,k5,k6,s1,s2,s3,s4,τx,τy]
      */
     std::vector<float> getDistortionCoefficients(CameraBoardSocket cameraId);
 
     /**
      *  Get the Fov of the camera
      *
      * @param cameraId of the camera of which we are fetching fov.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/device/CallbackHandler.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/device/CallbackHandler.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/device/DataQueue.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/device/DataQueue.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/device/Device.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/device/Device.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/device/DeviceBootloader.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/device/DeviceBootloader.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
      * @returns Version of current running bootloader
      */
     Version getVersion();
 
     /**
      * @returns True whether the bootloader running is flashed or booted by library
      */
-    bool isEmbeddedVersion();
+    bool isEmbeddedVersion() const;
 
     /**
      * Explicitly closes connection to device.
      * @note This function does not need to be explicitly called
      * as destructor closes the device automatically
      */
     void close();
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/openvino/OpenVINO.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/openvino/OpenVINO.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/AssetManager.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/AssetManager.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
  */
 struct Asset {
     Asset() = default;
     explicit Asset(std::string k) : key(std::move(k)) {}
     const std::string key;
     std::vector<std::uint8_t> data;
     std::uint32_t alignment = 1;
+    std::string getRelativeUri();
 };
 
 class AssetsMutable : public Assets {
    public:
     void set(std::string, std::uint32_t offset, std::uint32_t size, std::uint32_t alignment);
 };
 
@@ -35,45 +36,56 @@
     /**
      * Adds all assets in an array to the AssetManager
      * @param assets Vector of assets to add
      */
     void addExisting(std::vector<std::shared_ptr<Asset>> assets);
 
     /**
-     * Adds an asset object to AssetManager.
+     * Adds or overwrites an asset object to AssetManager.
      * @param asset Asset to add
+     * @returns Shared pointer to asset
      */
-    void add(Asset asset);
+    std::shared_ptr<dai::Asset> set(Asset asset);
 
     /**
-     * Adds an asset object to AssetManager with a specificied key.
+     * Adds or overwrites an asset object to AssetManager with a specificied key.
      * Key value will be assigned to an Asset as well
      *
-     * If asset with key already exists, the function throws an error
-     *
      * @param key Key under which the asset should be stored
      * @param asset Asset to store
+     * @returns Shared pointer to asset
      */
-    void add(const std::string& key, Asset asset);
+    std::shared_ptr<dai::Asset> set(const std::string& key, Asset asset);
 
     /**
-     * Adds or overwrites existing asset with a specificied key.
+     * Loads file into asset manager under specified key.
      *
      * @param key Key under which the asset should be stored
-     * @param asset Asset to store
+     * @param path Path to file which to load as asset
+     * @param alignment [Optional] alignment of asset data in asset storage. Default is 64B
+     */
+    std::shared_ptr<dai::Asset> set(const std::string& key, const std::string& path, int alignment = 64);
+
+    /**
+     * Loads file into asset manager under specified key.
+     *
+     * @param key Key under which the asset should be stored
+     * @param data Asset data
+     * @param alignment [Optional] alignment of asset data in asset storage. Default is 64B
+     * @returns Shared pointer to asset
      */
-    void set(const std::string& key, Asset asset);
+    std::shared_ptr<dai::Asset> set(const std::string& key, const std::vector<std::uint8_t>& data, int alignment = 64);
 
     /**
-     * @returns Asset assigned to the specified key or throws an error otherwise
+     * @returns Asset assigned to the specified key or a nullptr otherwise
      */
     std::shared_ptr<const Asset> get(const std::string& key) const;
 
     /**
-     * @returns Asset assigned to the specified key or throws an error otherwise
+     * @returns Asset assigned to the specified key or a nullptr otherwise
      */
     std::shared_ptr<Asset> get(const std::string& key);
 
     /**
      * @returns All asset stored in the AssetManager
      */
     std::vector<std::shared_ptr<const Asset>> getAll() const;
@@ -91,11 +103,11 @@
     /**
      * Removes asset with key
      * @param key Key of asset to remove
      */
     void remove(const std::string& key);
 
     /// Serializes
-    void serialize(Assets& serAssets, std::vector<std::uint8_t>& assetStorage) const;
+    void serialize(AssetsMutable& assets, std::vector<std::uint8_t>& assetStorage, std::string prefix = "") const;
 };
 
 }  // namespace dai
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/Node.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/Node.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -33,18 +33,23 @@
     using Id = std::int64_t;
     struct Connection;
 
    protected:
     // fwd declare classes
     class Input;
     class Output;
+    class InputMap;
+    class OutputMap;
 
     std::vector<Output*> outputs;
     std::vector<Input*> inputs;
 
+    std::vector<OutputMap*> outputMaps;
+    std::vector<InputMap*> inputMaps;
+
     struct DatatypeHierarchy {
         DatatypeHierarchy(DatatypeEnum d, bool c) : datatype(d), descendants(c) {}
         DatatypeEnum datatype;
         bool descendants;
     };
 
     class Output {
@@ -96,14 +101,27 @@
          * Throws an error if not linked.
          *
          * @param in Input from which to unlink from
          */
         void unlink(const Input& in);
     };
 
+    /**
+     * Output map which keeps track of extra outputs assigned to a node
+     * Extends std::unordered_map<std::string, dai::Node::Output>
+     */
+    class OutputMap : public std::unordered_map<std::string, Output> {
+        Output defaultOutput;
+
+       public:
+        OutputMap(Output defaultOutput);
+        /// Create or modify an input
+        Output& operator[](const std::string& key);
+    };
+
     class Input {
         Node& parent;
 
        public:
         enum class Type { SReceiver, MReceiver };
         const std::string name;
         const Type type;
@@ -151,14 +169,27 @@
         /**
          * Get input queue size.
          * @returns Maximum input queue size
          */
         int getQueueSize() const;
     };
 
+    /**
+     * Input map which keeps track of inputs assigned to a node
+     * Extends std::unordered_map<std::string, dai::Node::Input>
+     */
+    class InputMap : public std::unordered_map<std::string, Input> {
+        Input defaultInput;
+
+       public:
+        InputMap(Input defaultInput);
+        /// Create or modify an input
+        Input& operator[](const std::string& key);
+    };
+
     // when Pipeline tries to serialize and construct on remote, it will check if all connected nodes are on same pipeline
     std::weak_ptr<PipelineImpl> parent;
     AssetManager assetManager;
 
     virtual nlohmann::json getProperties() = 0;
     virtual tl::optional<OpenVINO::Version> getRequiredOpenVINOVersion();
     virtual std::shared_ptr<Node> clone() = 0;
@@ -169,64 +200,52 @@
 
     // access
     Pipeline getParentPipeline();
     const Pipeline getParentPipeline() const;
 
     /// Retrieves nodes name
     virtual std::string getName() const = 0;
+
     /// Retrieves all nodes outputs
-    std::vector<Output> getOutputs() {
-        std::vector<Output> result;
-        for(auto* x : getOutputRefs()) {
-            result.push_back(*x);
-        }
-        return result;
-    }
+    std::vector<Output> getOutputs();
+
     /// Retrieves all nodes inputs
-    std::vector<Input> getInputs() {
-        std::vector<Input> result;
-        for(auto* x : getInputRefs()) {
-            result.push_back(*x);
-        }
-        return result;
-    }
-    /// Retrieves all nodes assets
-    virtual std::vector<std::shared_ptr<Asset>> getAssets();
+    std::vector<Input> getInputs();
 
     /// Retrieves reference to node outputs
-    std::vector<Output*> getOutputRefs() {
-        return outputs;
-    }
+    std::vector<Output*> getOutputRefs();
+
     /// Retrieves reference to node outputs
-    std::vector<const Output*> getOutputRefs() const {
-        return {outputs.begin(), outputs.end()};
-    }
+    std::vector<const Output*> getOutputRefs() const;
+
     /// Retrieves reference to node inputs
-    std::vector<Input*> getInputRefs() {
-        return inputs;
-    }
+    std::vector<Input*> getInputRefs();
+
     /// Retrieves reference to node inputs
-    std::vector<const Input*> getInputRefs() const {
-        return {inputs.begin(), inputs.end()};
-    }
+    std::vector<const Input*> getInputRefs() const;
 
     /// Connection between an Input and Output
     struct Connection {
         friend struct std::hash<Connection>;
         Connection(Output out, Input in);
         Id outputId;
         std::string outputName;
         Id inputId;
         std::string inputName;
         bool operator==(const Connection& rhs) const;
     };
 
     Node(const std::shared_ptr<PipelineImpl>& p, Id nodeId);
-
     virtual ~Node() = default;
+
+    /// Get node AssetManager as a const reference
+    const AssetManager& getAssetManager() const;
+
+    /// Get node AssetManager as a reference
+    AssetManager& getAssetManager();
 };
 
 }  // namespace dai
 
 // Specialization of std::hash for Node::Connection
 namespace std {
 template <>
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/Pipeline.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/Pipeline.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     static bool isSamePipeline(const Node::Output& out, const Node::Input& in);
     static bool canConnect(const Node::Output& out, const Node::Input& in);
 
     // Functions
     Node::Id getNextUniqueId();
     PipelineSchema getPipelineSchema() const;
     OpenVINO::Version getPipelineOpenVINOVersion() const;
-    AssetManager getAllAssets() const;
     void setCameraTuningBlobPath(const std::string& path);
 
     // Access to nodes
     std::vector<std::shared_ptr<const Node>> getAllNodes() const;
     std::vector<std::shared_ptr<Node>> getAllNodes();
     std::shared_ptr<const Node> getNode(Node::Id id) const;
     std::shared_ptr<Node> getNode(Node::Id id);
@@ -195,19 +194,14 @@
      * @param out Nodes output to unlink from
      * @param in Nodes input to unlink to
      */
     void unlink(const Node::Output& out, const Node::Input& in) {
         impl()->unlink(out, in);
     }
 
-    /// Get assets on the pipeline includes nodes assets
-    AssetManager getAllAssets() const {
-        return impl()->getAllAssets();
-    }
-
     /// Get pipelines AssetManager as reference
     const AssetManager& getAssetManager() const {
         return impl()->assetManager;
     }
 
     /// Get pipelines AssetManager as reference
     AssetManager& getAssetManager() {
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ADatatype.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ADatatype.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/Buffer.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/Buffer.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/CameraControl.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/CameraControl.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/EdgeDetectorConfig.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/EdgeDetectorConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/IMUData.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/IMUData.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ImageManipConfig.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ImageManipConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ImgDetections.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ImgDetections.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/ImgFrame.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/ImgFrame.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/NNData.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/NNData.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialImgDetections.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialImgDetections.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorConfig.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorData.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SpatialLocationCalculatorData.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/StereoDepthConfig.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/StereoDepthConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/SystemInformation.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/SystemInformation.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatype/Tracklets.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatype/Tracklets.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/datatypes.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/datatypes.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/ColorCamera.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/ColorCamera.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/DetectionNetwork.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/DetectionNetwork.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/EdgeDetector.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/EdgeDetector.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/IMU.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/IMU.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/ImageManip.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/ImageManip.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/MonoCamera.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/MonoCamera.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/MyProducer.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/MyProducer.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/NeuralNetwork.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/NeuralNetwork.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,14 @@
     std::shared_ptr<Node> clone() override;
     tl::optional<OpenVINO::Version> getRequiredOpenVINOVersion() override;
 
    private:
     Properties properties;
 
    protected:
-    struct BlobAssetInfo {
-        std::string uri;
-        uint32_t size;
-    };
-    std::string blobPath;
-    BlobAssetInfo loadBlob(const std::string& path);
     OpenVINO::Version networkOpenvinoVersion;
     virtual Properties& getPropertiesRef();
 
    public:
     NeuralNetwork(const std::shared_ptr<PipelineImpl>& par, int64_t nodeId);
 
     /**
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/ObjectTracker.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/ObjectTracker.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SPIOut.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SPIOut.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 namespace dai {
 namespace node {
 
 /**
  * @brief SPIOut node. Sends messages over SPI.
  */
 class SPIOut : public Node {
-    dai::SPIOutProperties properties;
+   public:
+    using Properties = dai::SPIOutProperties;
+
+   private:
+    Properties properties;
 
-    nlohmann::json getProperties() {
+    nlohmann::json getProperties() override {
         nlohmann::json j;
         nlohmann::to_json(j, properties);
         return j;
     }
 
-    std::shared_ptr<Node> clone() {
-        return std::make_shared<SPIOut>(*this);
+    std::shared_ptr<Node> clone() override {
+        return std::make_shared<std::decay<decltype(*this)>::type>(*this);
     }
 
    public:
-    std::string getName() const {
+    std::string getName() const override {
         return "SPIOut";
     }
 
     SPIOut(const std::shared_ptr<PipelineImpl>& par, int64_t nodeId) : Node(par, nodeId) {
         properties.busId = 0;
 
         inputs = {&input};
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SpatialDetectionNetwork.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SpatialDetectionNetwork.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SpatialLocationCalculator.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SpatialLocationCalculator.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/StereoDepth.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/StereoDepth.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/SystemLogger.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/SystemLogger.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/VideoEncoder.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/VideoEncoder.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/XLinkIn.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/XLinkIn.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/node/XLinkOut.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/node/XLinkOut.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/pipeline/nodes.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/pipeline/nodes.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 #include "node/EdgeDetector.hpp"
 #include "node/IMU.hpp"
 #include "node/ImageManip.hpp"
 #include "node/MonoCamera.hpp"
 #include "node/MyProducer.hpp"
 #include "node/NeuralNetwork.hpp"
 #include "node/ObjectTracker.hpp"
+#include "node/SPIIn.hpp"
 #include "node/SPIOut.hpp"
+#include "node/Script.hpp"
 #include "node/SpatialDetectionNetwork.hpp"
 #include "node/SpatialLocationCalculator.hpp"
 #include "node/StereoDepth.hpp"
 #include "node/SystemLogger.hpp"
 #include "node/VideoEncoder.hpp"
 #include "node/XLinkIn.hpp"
-#include "node/XLinkOut.hpp"
+#include "node/XLinkOut.hpp"
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/utility/LockingQueue.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/utility/LockingQueue.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #pragma once
+#include <atomic>
 #include <condition_variable>
 #include <functional>
 #include <limits>
 #include <mutex>
 #include <queue>
 
 namespace dai {
```

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/xlink/XLinkConnection.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/xlink/XLinkConnection.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/include/depthai/xlink/XLinkStream.hpp` & `depthai-2.9.0.0/depthai-core/include/depthai/xlink/XLinkStream.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/LICENSE` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/LICENSE`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Bootloader.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/Bootloader.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/NetworkBootloaderConfig.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/NetworkBootloaderConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/SBR.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/SBR.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/UsbBootloaderConfig.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/include/depthai-bootloader-shared/UsbBootloaderConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared/src/SBR.c` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared/src/SBR.c`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-bootloader-shared.cmake` & `depthai-2.9.0.0/depthai-core/shared/depthai-bootloader-shared.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/invoke_hpp/invoke.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/invoke_hpp/invoke.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/linb/any.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/linb/any.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/client.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/client.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/function_meta.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/function_meta.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/pack_meta.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/detail/pack_meta.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/exception.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/exception.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/server.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/server.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/type.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/core/type.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/cereal_binary.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/cereal_binary.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_json.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_json.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_msgpack.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/packer/nlohmann_msgpack.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/version/core.h` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/nanorpc/version/core.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/3rdparty/tl/optional.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/3rdparty/tl/optional.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/LICENSE` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/LICENSE`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraInfo.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/CameraInfo.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/ChipTemperature.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/ChipTemperature.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/EepromData.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/EepromData.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Extrinsics.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Extrinsics.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Rect.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Rect.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/StereoRectification.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/StereoRectification.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Timestamp.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/Timestamp.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/optional.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/common/optional.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawCameraControl.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawCameraControl.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawEdgeDetectorConfig.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawEdgeDetectorConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawIMUData.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawIMUData.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImageManipConfig.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImageManipConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgDetections.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgDetections.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgFrame.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawImgFrame.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawNNData.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawNNData.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialImgDetections.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialImgDetections.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocationCalculatorConfig.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocationCalculatorConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocations.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSpatialLocations.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawStereoDepthConfig.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawStereoDepthConfig.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSystemInformation.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawSystemInformation.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawTracklets.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/datatype/RawTracklets.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/Assets.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/Assets.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/PipelineSchema.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/pipeline/PipelineSchema.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ColorCameraProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ColorCameraProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/DetectionNetworkProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/DetectionNetworkProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/EdgeDetectorProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/EdgeDetectorProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/GlobalProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/GlobalProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/IMUProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/IMUProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ImageManipProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ImageManipProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MonoCameraProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MonoCameraProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyProducerProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyProducerProperties.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,13 @@
      * Message to be sent forward
      */
     tl::optional<std::string> message;
 
     /**
      * On which processor the node will be placed
      */
-    ProcessorType processorPlacement = ProcessorType::LOS;
+    ProcessorType processorPlacement = ProcessorType::LEON_CSS;
 };
 
 NLOHMANN_DEFINE_TYPE_NON_INTRUSIVE(MyProducerProperties, message, processorPlacement);
 
 }  // namespace dai
```

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/NeuralNetworkProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/NeuralNetworkProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ObjectTrackerProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/ObjectTrackerProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialDetectionNetworkProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialDetectionNetworkProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialLocationCalculatorProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialLocationCalculatorProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/StereoDepthProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/StereoDepthProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/VideoEncoderProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/VideoEncoderProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkInProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkInProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkOutProperties.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkOutProperties.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/xlink/XLinkConstants.hpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/include/depthai-shared/xlink/XLinkConstants.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared/src/datatype/DatatypeEnum.cpp` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared/src/datatype/DatatypeEnum.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/shared/depthai-shared.cmake` & `depthai-2.9.0.0/depthai-core/shared/depthai-shared.cmake`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/bspatch/bspatch.c` & `depthai-2.9.0.0/depthai-core/src/bspatch/bspatch.c`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/bspatch/bspatch.h` & `depthai-2.9.0.0/depthai-core/src/bspatch/bspatch.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/device/CalibrationHandler.cpp` & `depthai-2.9.0.0/depthai-core/src/device/CalibrationHandler.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/device/CallbackHandler.cpp` & `depthai-2.9.0.0/depthai-core/src/device/CallbackHandler.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/device/DataQueue.cpp` & `depthai-2.9.0.0/depthai-core/src/device/DataQueue.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/device/Device.cpp` & `depthai-2.9.0.0/depthai-core/src/device/Device.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -980,15 +980,15 @@
 
     pimpl->rpcClient->call("setSystemInformationLoggingRate", rateHz);
 }
 
 float Device::getSystemInformationLoggingRate() {
     checkClosed();
 
-    return pimpl->rpcClient->call("getSystemInformationLoggingrate").as<float>();
+    return pimpl->rpcClient->call("getSystemInformationLoggingRate").as<float>();
 }
 
 bool Device::flashCalibration(CalibrationHandler calibrationDataHandler) {
     if(!calibrationDataHandler.validateCameraArray()) {
         throw std::runtime_error("Failed to validate the extrinsics connection. Enable debug mode for more information.");
     }
     return pimpl->rpcClient->call("storeToEeprom", calibrationDataHandler.getEepromData()).as<bool>();
```

### Comparing `depthai-2.8.0.0/depthai-core/src/device/DeviceBootloader.cpp` & `depthai-2.9.0.0/depthai-core/src/device/DeviceBootloader.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -394,14 +394,20 @@
     std::ofstream outfile(path, std::ios::binary);
     outfile.write(reinterpret_cast<const char*>(dap.data()), dap.size());
 }
 
 std::tuple<bool, std::string> DeviceBootloader::flashDepthaiApplicationPackage(std::function<void(float)> progressCb, std::vector<uint8_t> package) {
     streamId_t streamId = stream->getStreamId();
 
+    // Bug in NETWORK bootloader in version 0.0.12 < 0.1.0 - flashing can cause a soft brick
+    auto version = getVersion();
+    if(bootloaderType == Type::NETWORK && version < Version(0, 1, 0)) {
+        throw std::invalid_argument("Network bootloader requires version 0.1.0 or higher to flash applications. Current version: " + version.toString());
+    }
+
     // send request to FLASH BOOTLOADER
     dai::bootloader::request::UpdateFlash updateFlash;
     updateFlash.storage = dai::bootloader::request::UpdateFlash::SBR;
     updateFlash.totalSize = static_cast<uint32_t>(package.size());
     updateFlash.numPackets = ((static_cast<uint32_t>(package.size()) - 1) / bootloader::XLINK_STREAM_MAX_SIZE) + 1;
     if(!sendBootloaderRequest(streamId, updateFlash)) return {false, "Couldn't send bootloader flash request"};
 
@@ -559,15 +565,15 @@
     } while(true);
 
     // Return if flashing was successful
     return {result.success, result.errorMsg};
 }
 */
 
-bool DeviceBootloader::isEmbeddedVersion() {
+bool DeviceBootloader::isEmbeddedVersion() const {
     return isEmbedded;
 }
 
 std::vector<std::uint8_t> DeviceBootloader::getEmbeddedBootloaderBinary(Type type) {
     return Resources::getInstance().getBootloaderFirmware(type);
 }
```

### Comparing `depthai-2.8.0.0/depthai-core/src/device/DeviceLogger.hpp` & `depthai-2.9.0.0/depthai-core/src/device/DeviceLogger.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/opencv/ImgFrame.cpp` & `depthai-2.9.0.0/depthai-core/src/opencv/ImgFrame.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/openvino/BlobFormat.hpp` & `depthai-2.9.0.0/depthai-core/src/openvino/BlobFormat.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/openvino/BlobReader.cpp` & `depthai-2.9.0.0/depthai-core/src/openvino/BlobReader.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/openvino/BlobReader.hpp` & `depthai-2.9.0.0/depthai-core/src/openvino/BlobReader.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/openvino/OpenVINO.cpp` & `depthai-2.9.0.0/depthai-core/src/openvino/OpenVINO.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/AssetManager.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/AssetManager.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,74 @@
 #include "depthai/pipeline/AssetManager.hpp"
 
+#include "spdlog/fmt/fmt.h"
+
+// std
+#include <fstream>
+
 namespace dai {
 
-void AssetManager::add(Asset asset) {
+std::string Asset::getRelativeUri() {
+    return fmt::format("{}:{}", "asset", key);
+}
+
+std::shared_ptr<dai::Asset> AssetManager::set(Asset asset) {
     // make sure that key doesn't exist already
     if(assetMap.count(asset.key) > 0) throw std::logic_error("An Asset with the key: " + asset.key + " already exists.");
     std::string key = asset.key;
     assetMap[key] = std::make_shared<Asset>(std::move(asset));
+    return assetMap[key];
 }
 
-void AssetManager::add(const std::string& key, Asset asset) {
+std::shared_ptr<dai::Asset> AssetManager::set(const std::string& key, Asset asset) {
     // Rename the asset with supplied key and store
     Asset a(key);
     a.data = std::move(asset.data);
     a.alignment = asset.alignment;
-    add(std::move(a));
+    return set(std::move(a));
 }
 
-void AssetManager::set(const std::string& key, Asset asset) {
-    // Rename the asset with supplied key and store
-    Asset a(key);
-    a.data = std::move(asset.data);
-    a.alignment = asset.alignment;
-    assetMap[key] = std::make_shared<Asset>(std::move(a));
+std::shared_ptr<dai::Asset> AssetManager::set(const std::string& key, const std::string& path, int alignment) {
+    // Load binary file at path
+    std::ifstream stream(path, std::ios::in | std::ios::binary);
+    if(!stream.is_open()) {
+        // Throw an error
+        // TODO(themarpe) - Unify exceptions into meaningful groups
+        throw std::runtime_error(fmt::format("Cannot load asset, file at path {} doesn't exist.", path));
+    }
+
+    // Create an asset
+    Asset binaryAsset(key);
+    binaryAsset.alignment = alignment;
+    binaryAsset.data = std::vector<std::uint8_t>(std::istreambuf_iterator<char>(stream), {});
+    // Store asset
+    return set(std::move(binaryAsset));
+}
+
+std::shared_ptr<dai::Asset> AssetManager::set(const std::string& key, const std::vector<std::uint8_t>& data, int alignment) {
+    // Create an asset
+    Asset binaryAsset(key);
+    binaryAsset.alignment = alignment;
+    binaryAsset.data = std::move(data);
+    // Store asset
+    return set(std::move(binaryAsset));
 }
 
 std::shared_ptr<const Asset> AssetManager::get(const std::string& key) const {
+    if(assetMap.count(key) == 0) {
+        return nullptr;
+    }
     return assetMap.at(key);
 }
 
 std::shared_ptr<Asset> AssetManager::get(const std::string& key) {
-    return assetMap[key];
+    if(assetMap.count(key) == 0) {
+        return nullptr;
+    }
+    return assetMap.at(key);
 }
 
 void AssetManager::addExisting(std::vector<std::shared_ptr<Asset>> assets) {
     // make sure that key doesn't exist already
     for(const auto& asset : assets) {
         if(assetMap.count(asset->key) > 0) throw std::logic_error("An Asset with the key: " + asset->key + " already exists.");
         std::string key = asset->key;
@@ -62,18 +96,16 @@
     return assetMap.size();
 }
 
 void AssetManager::remove(const std::string& key) {
     assetMap.erase(key);
 }
 
-void AssetManager::serialize(Assets& serAssets, std::vector<std::uint8_t>& assetStorage) const {
+void AssetManager::serialize(AssetsMutable& mutableAssets, std::vector<std::uint8_t>& storage, std::string prefix) const {
     using namespace std;
-    vector<uint8_t> storage;
-    AssetsMutable mutableAssets;
 
     for(auto& kv : assetMap) {
         auto& a = *kv.second;
 
         // calculate additional bytes needed to offset to alignment
         int toAdd = 0;
         if(a.alignment > 1 && storage.size() % a.alignment != 0) {
@@ -86,19 +118,16 @@
         // Add alignment bytes
         storage.resize(storage.size() + toAdd);
 
         // copy data
         storage.insert(storage.end(), a.data.begin(), a.data.end());
 
         // Add to map the currently added asset
-        mutableAssets.set(a.key, offset, static_cast<uint32_t>(a.data.size()), a.alignment);
+        mutableAssets.set(prefix + a.key, offset, static_cast<uint32_t>(a.data.size()), a.alignment);
     }
-
-    assetStorage = std::move(storage);
-    serAssets = Assets(mutableAssets);
 }
 
 void AssetsMutable::set(std::string key, std::uint32_t offset, std::uint32_t size, std::uint32_t alignment) {
     AssetInternal internal = {};
     internal.offset = offset;
     internal.size = size;
     internal.alignment = alignment;
```

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/Pipeline.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/Pipeline.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -50,34 +50,14 @@
     this->pimpl = pimpl;
 }
 
 GlobalProperties Pipeline::getGlobalProperties() const {
     return pimpl->globalProperties;
 }
 
-/*
-void Pipeline::loadAssets(AssetManager& assetManager) {
-    return pimpl->loadAssets(assetManager);
-}
-*/
-
-/*
-void PipelineImpl::loadAssets() {
-
-    // Load assets of nodes
-    for(const auto& node : nodes){
-        node->loadAssets(assetManager);
-    }
-
-    // Load assets of pipeline (if any)
-    // ...
-
-}
-*/
-
 std::shared_ptr<const Node> PipelineImpl::getNode(Node::Id id) const {
     if(nodeMap.count(id) > 0) {
         return nodeMap.at(id);
     }
     return nullptr;
 }
 std::shared_ptr<Node> PipelineImpl::getNode(Node::Id id) {
@@ -102,31 +82,27 @@
     return nodes;
 }
 
 void PipelineImpl::serialize(PipelineSchema& schema, Assets& assets, std::vector<std::uint8_t>& assetStorage, OpenVINO::Version& version) const {
     // Set schema
     schema = getPipelineSchema();
 
-    // set assets and generate asset storage
-    getAllAssets().serialize(assets, assetStorage);
-
-    // detect and set openvino version
-    version = getPipelineOpenVINOVersion();
-}
-
-AssetManager PipelineImpl::getAllAssets() const {
-    AssetManager am = assetManager;
-
+    // Serialize all asset managers into asset storage
+    assetStorage.clear();
+    AssetsMutable mutableAssets;
+    // Pipeline assets
+    assetManager.serialize(mutableAssets, assetStorage, "/pipeline/");
+    // Node assets
     for(const auto& kv : nodeMap) {
-        const auto& node = kv.second;
-        // Loop over all nodes and add any assets they have
-        am.addExisting(node->getAssets());
+        kv.second->getAssetManager().serialize(mutableAssets, assetStorage, fmt::format("/node/{}/", kv.second->id));
     }
+    assets = mutableAssets;
 
-    return am;
+    // detect and set openvino version
+    version = getPipelineOpenVINOVersion();
 }
 
 PipelineSchema PipelineImpl::getPipelineSchema() const {
     PipelineSchema schema;
     schema.globalProperties = globalProperties;
 
     // Loop over nodes, and add them to schema
@@ -155,14 +131,17 @@
                     io.type = NodeIoInfo::Type::MReceiver;
                     break;
                 case Node::Input::Type::SReceiver:
                     io.type = NodeIoInfo::Type::SReceiver;
                     break;
             }
 
+            if(info.ioInfo.count(io.name) > 0) {
+                throw std::invalid_argument(fmt::format("'{}.{}' redefined. Inputs and outputs must have unique names", info.name, io.name));
+            }
             info.ioInfo[io.name] = io;
         }
 
         // Add outputs
         for(const auto& output : outputs) {
             NodeIoInfo io;
             io.blocking = false;
@@ -172,14 +151,17 @@
                     io.type = NodeIoInfo::Type::MSender;
                     break;
                 case Node::Output::Type::SSender:
                     io.type = NodeIoInfo::Type::SSender;
                     break;
             }
 
+            if(info.ioInfo.count(io.name) > 0) {
+                throw std::invalid_argument(fmt::format("'{}.{}' redefined. Inputs and outputs must have unique names", info.name, io.name));
+            }
             info.ioInfo[io.name] = io;
         }
 
         // At the end, add the constructed node information to the schema
         schema.nodes[info.id] = info;
     }
 
@@ -253,27 +235,18 @@
 
     return openvinoVersion;
 }
 
 void PipelineImpl::setCameraTuningBlobPath(const std::string& path) {
     std::string assetKey = "camTuning";
 
-    std::ifstream blobStream(path, std::ios::binary);
-    if(!blobStream.is_open()) {
-        throw std::runtime_error("Pipeline | Couldn't open camera tuning blob at path: " + path);
-    }
-
-    Asset blobAsset;
-    blobAsset.alignment = 64;
-    blobAsset.data = std::vector<std::uint8_t>(std::istreambuf_iterator<char>(blobStream), {});
-
-    assetManager.set(assetKey, blobAsset);
+    auto asset = assetManager.set(assetKey, path);
 
-    globalProperties.cameraTuningBlobUri = std::string("asset:") + assetKey;
-    globalProperties.cameraTuningBlobSize = blobAsset.data.size();
+    globalProperties.cameraTuningBlobUri = asset->getRelativeUri();
+    globalProperties.cameraTuningBlobSize = asset->data.size();
 }
 
 // Remove node capability
 void PipelineImpl::remove(std::shared_ptr<Node> toRemove) {
     // Search for this node in 'nodes' vector.
     // If found, remove from vector
```

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/CameraControl.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/CameraControl.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/EdgeDetectorConfig.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/EdgeDetectorConfig.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/ImageManipConfig.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/ImageManipConfig.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 void ImageManipConfig::setCropRect(float xmin, float ymin, float xmax, float ymax) {
     // Enable crop stage
     cfg.enableCrop = true;
 
     // Disable center crop
     cfg.cropConfig.enableCenterCropRectangle = false;
 
-    // Set crop rect
-    cfg.cropConfig.cropRect.xmin = xmin;
-    cfg.cropConfig.cropRect.ymin = ymin;
-    cfg.cropConfig.cropRect.xmax = xmax;
-    cfg.cropConfig.cropRect.ymax = ymax;
+    // Set crop rect - limit to bounds beforehand
+    cfg.cropConfig.cropRect.xmin = std::max(xmin, 0.0f);
+    cfg.cropConfig.cropRect.ymin = std::max(ymin, 0.0f);
+    cfg.cropConfig.cropRect.xmax = std::min(xmax, 1.0f);
+    cfg.cropConfig.cropRect.ymax = std::min(ymax, 1.0f);
 }
 
 void ImageManipConfig::setCropRotatedRect(RotatedRect rr, bool normalizedCoords) {
     // Enable crop stage and extended flags
     cfg.enableCrop = true;
     cfg.cropConfig.enableRotatedRect = true;
 
@@ -73,14 +73,19 @@
     cfg.enableCrop = true;
 
     // Enable center center crop
     cfg.cropConfig.enableCenterCropRectangle = true;
 
     // Set crop center crop config
     cfg.cropConfig.cropRatio = ratio;
+    // Limit to max 1.0f and disallow setting zero ratio
+    if(ratio > 1.0f || ratio < 0.0f) {
+        cfg.cropConfig.cropRatio = 1.0f;
+    }
+
     cfg.cropConfig.widthHeightAspectRatio = whRatio;
 }
 
 void ImageManipConfig::setRotationDegrees(float deg) {
     cfg.enableResize = true;
     cfg.resizeConfig.rotationAngleDeg = deg;
     cfg.resizeConfig.enableRotation = true;
```

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/ImgDetections.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/ImgDetections.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/ImgFrame.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/ImgFrame.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/NNData.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/NNData.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SpatialImgDetections.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SpatialImgDetections.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorConfig.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorConfig.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorData.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SpatialLocationCalculatorData.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/StereoDepthConfig.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/StereoDepthConfig.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,18 @@
 
     if(serializedObjectSize < 0) {
         throw std::runtime_error("Bad packet, couldn't parse");
     }
     std::uint32_t bufferLength = packet->length - 8 - serializedObjectSize;
     auto* msgpackStart = packet->data + bufferLength;
 
-    nlohmann::json jser = nlohmann::json::from_msgpack(msgpackStart, msgpackStart + serializedObjectSize);
+    nlohmann::json jser;
+    if(serializedObjectSize > 0) {
+        jser = nlohmann::json::from_msgpack(msgpackStart, msgpackStart + serializedObjectSize);
+    }
 
     // copy data part
     std::vector<uint8_t> data(packet->data, packet->data + bufferLength);
 
     // Create corresponding object
     switch(objectType) {
         // RawBuffer is special case, no metadata is actually serialized
@@ -149,15 +152,18 @@
 
     if(serializedObjectSize < 0) {
         throw std::runtime_error("Bad packet, couldn't parse");
     }
     std::uint32_t bufferLength = packet->length - 8 - serializedObjectSize;
     auto* msgpackStart = packet->data + bufferLength;
 
-    nlohmann::json jser = nlohmann::json::from_msgpack(msgpackStart, msgpackStart + serializedObjectSize);
+    nlohmann::json jser;
+    if(serializedObjectSize > 0) {
+        jser = nlohmann::json::from_msgpack(msgpackStart, msgpackStart + serializedObjectSize);
+    }
 
     // copy data part
     std::vector<uint8_t> data(packet->data, packet->data + bufferLength);
 
     switch(objectType) {
         case DatatypeEnum::Buffer: {
             // RawBuffer is special case, no metadata is actually serialized
```

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.hpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/StreamPacketParser.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/datatype/SystemInformation.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/datatype/SystemInformation.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/ColorCamera.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/ColorCamera.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/DetectionNetwork.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/DetectionNetwork.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 //--------------------------------------------------------------------
 // Base Detection Network Class
 //--------------------------------------------------------------------
 DetectionNetwork::DetectionNetwork(const std::shared_ptr<PipelineImpl>& par, int64_t nodeId) : NeuralNetwork(par, nodeId) {
     inputs = {&input};
     outputs = {&out, &passthrough};
+
+    // Default confidence threshold
+    getPropertiesRef().confidenceThreshold = 0.5;
 }
 
 std::string DetectionNetwork::getName() const {
     return "DetectionNetwork";
 }
 
 DetectionNetwork::Properties& DetectionNetwork::getPropertiesRef() {
```

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/EdgeDetector.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/EdgeDetector.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/IMU.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/IMU.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/ImageManip.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/ImageManip.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/MonoCamera.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/MonoCamera.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/MyProducer.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/MyProducer.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/ObjectTracker.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/ObjectTracker.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/SpatialDetectionNetwork.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/SpatialDetectionNetwork.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/SpatialLocationCalculator.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/SpatialLocationCalculator.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/StereoDepth.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/StereoDepth.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -52,21 +52,19 @@
 
     Asset meshAsset;
     std::string assetKey;
     meshAsset.alignment = 64;
 
     meshAsset.data = dataLeft;
     assetKey = "meshLeft";
-    assetManager.set(assetKey, meshAsset);
-    properties.mesh.meshLeftUri = std::string("asset:") + assetKey;
+    properties.mesh.meshLeftUri = assetManager.set(assetKey, meshAsset)->getRelativeUri();
 
     meshAsset.data = dataRight;
     assetKey = "meshRight";
-    assetManager.set(assetKey, meshAsset);
-    properties.mesh.meshRightUri = std::string("asset:") + assetKey;
+    properties.mesh.meshRightUri = assetManager.set(assetKey, meshAsset)->getRelativeUri();
 
     properties.mesh.meshSize = meshAsset.data.size();
 }
 
 void StereoDepth::loadMeshFiles(const std::string& pathLeft, const std::string& pathRight) {
     std::ifstream streamLeft(pathLeft, std::ios::binary);
     if(!streamLeft.is_open()) {
```

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/SystemLogger.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/SystemLogger.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/VideoEncoder.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/VideoEncoder.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/XLinkIn.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/XLinkIn.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/pipeline/node/XLinkOut.cpp` & `depthai-2.9.0.0/depthai-core/src/pipeline/node/XLinkOut.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/utility/BootloaderHelper.hpp` & `depthai-2.9.0.0/depthai-core/src/utility/BootloaderHelper.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/utility/Initialization.cpp` & `depthai-2.9.0.0/depthai-core/src/utility/Initialization.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     static std::atomic<bool> initialized{false};
 
     if(initialized.exchange(true)) return true;
 
     // Set global logging level from ENV variable 'DEPTHAI_LEVEL'
     // Taken from spdlog, to replace with DEPTHAI_LEVEL instead of SPDLOG_LEVEL
     // spdlog::cfg::load_env_levels();
-    auto env_val = spdlog::details::os::getenv("DEPTHAI_LEVEL");
-    if(!env_val.empty()) {
-        spdlog::cfg::helpers::load_levels(env_val);
+    auto envLevel = spdlog::details::os::getenv("DEPTHAI_LEVEL");
+    if(!envLevel.empty()) {
+        spdlog::cfg::helpers::load_levels(envLevel);
     } else {
         // Otherwise set default level to WARN
         spdlog::set_level(spdlog::level::warn);
     }
 
     // auto debugger_val = spdlog::details::os::getenv("DEPTHAI_DEBUGGER");
     // if(!debugger_val.empty()){
```

### Comparing `depthai-2.8.0.0/depthai-core/src/utility/Resources.cpp` & `depthai-2.9.0.0/depthai-core/src/utility/Resources.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/utility/Resources.hpp` & `depthai-2.9.0.0/depthai-core/src/utility/Resources.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/utility/matrixOps.hpp` & `depthai-2.9.0.0/depthai-core/src/utility/matrixOps.hpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/xlink/XLinkConnection.cpp` & `depthai-2.9.0.0/depthai-core/src/xlink/XLinkConnection.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai-core/src/xlink/XLinkStream.cpp` & `depthai-2.9.0.0/depthai-core/src/xlink/XLinkStream.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/depthai.egg-info/PKG-INFO` & `depthai-2.9.0.0/depthai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthai
-Version: 2.8.0.0
+Version: 2.9.0.0
 Summary: DepthAI Python Library
 Home-page: https://github.com/luxonis/depthai-python
 Author: Martin Peterlin
 Author-email: martin@luxonis.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `depthai-2.8.0.0/depthai.egg-info/SOURCES.txt` & `depthai-2.9.0.0/depthai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,17 @@
 depthai-core/include/depthai/pipeline/node/EdgeDetector.hpp
 depthai-core/include/depthai/pipeline/node/IMU.hpp
 depthai-core/include/depthai/pipeline/node/ImageManip.hpp
 depthai-core/include/depthai/pipeline/node/MonoCamera.hpp
 depthai-core/include/depthai/pipeline/node/MyProducer.hpp
 depthai-core/include/depthai/pipeline/node/NeuralNetwork.hpp
 depthai-core/include/depthai/pipeline/node/ObjectTracker.hpp
+depthai-core/include/depthai/pipeline/node/SPIIn.hpp
 depthai-core/include/depthai/pipeline/node/SPIOut.hpp
+depthai-core/include/depthai/pipeline/node/Script.hpp
 depthai-core/include/depthai/pipeline/node/SpatialDetectionNetwork.hpp
 depthai-core/include/depthai/pipeline/node/SpatialLocationCalculator.hpp
 depthai-core/include/depthai/pipeline/node/StereoDepth.hpp
 depthai-core/include/depthai/pipeline/node/SystemLogger.hpp
 depthai-core/include/depthai/pipeline/node/VideoEncoder.hpp
 depthai-core/include/depthai/pipeline/node/XLinkIn.hpp
 depthai-core/include/depthai/pipeline/node/XLinkOut.hpp
@@ -189,15 +191,17 @@
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/IMUProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/ImageManipProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/MonoCameraProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyConsumerProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/MyProducerProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/NeuralNetworkProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/ObjectTrackerProperties.hpp
+depthai-core/shared/depthai-shared/include/depthai-shared/properties/SPIInProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/SPIOutProperties.hpp
+depthai-core/shared/depthai-shared/include/depthai-shared/properties/ScriptProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialDetectionNetworkProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/SpatialLocationCalculatorProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/StereoDepthProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/SystemLoggerProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/VideoEncoderProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkInProperties.hpp
 depthai-core/shared/depthai-shared/include/depthai-shared/properties/XLinkOutProperties.hpp
@@ -240,14 +244,16 @@
 depthai-core/src/pipeline/node/EdgeDetector.cpp
 depthai-core/src/pipeline/node/IMU.cpp
 depthai-core/src/pipeline/node/ImageManip.cpp
 depthai-core/src/pipeline/node/MonoCamera.cpp
 depthai-core/src/pipeline/node/MyProducer.cpp
 depthai-core/src/pipeline/node/NeuralNetwork.cpp
 depthai-core/src/pipeline/node/ObjectTracker.cpp
+depthai-core/src/pipeline/node/SPIIn.cpp
+depthai-core/src/pipeline/node/Script.cpp
 depthai-core/src/pipeline/node/SpatialDetectionNetwork.cpp
 depthai-core/src/pipeline/node/SpatialLocationCalculator.cpp
 depthai-core/src/pipeline/node/StereoDepth.cpp
 depthai-core/src/pipeline/node/SystemLogger.cpp
 depthai-core/src/pipeline/node/VideoEncoder.cpp
 depthai-core/src/pipeline/node/XLinkIn.cpp
 depthai-core/src/pipeline/node/XLinkOut.cpp
```

### Comparing `depthai-2.8.0.0/external/hedley/include/hedley/hedley.h` & `depthai-2.9.0.0/external/hedley/include/hedley/hedley.h`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/find_version.py` & `depthai-2.9.0.0/find_version.py`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/setup.py` & `depthai-2.9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/src/CalibrationHandlerBindings.cpp` & `depthai-2.9.0.0/src/CalibrationHandlerBindings.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 #include "CalibrationHandlerBindings.hpp"
 #include "depthai/device/CalibrationHandler.hpp"
 #include "depthai-shared/common/Point2f.hpp"
 #include <vector>
 
-void CalibrationHandlerBindings::bind(pybind11::module& m){
+void CalibrationHandlerBindings::bind(pybind11::module& m, void* pCallstack){
 
     using namespace dai;
 
-    // bind pipeline
-    py::class_<CalibrationHandler>(m, "CalibrationHandler", DOC(dai, CalibrationHandler))
+    // Type definitions
+    py::class_<CalibrationHandler> calibrationHandler(m, "CalibrationHandler", DOC(dai, CalibrationHandler));
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
+    // Bindings
+    calibrationHandler
         .def(py::init<>(), DOC(dai, CalibrationHandler, CalibrationHandler))
         .def(py::init<std::string>(), DOC(dai, CalibrationHandler, CalibrationHandler, 2))
         .def(py::init<std::string, std::string>(), DOC(dai, CalibrationHandler, CalibrationHandler, 3))
         .def(py::init<EepromData>(), DOC(dai, CalibrationHandler, CalibrationHandler, 4))
 
         .def("getEepromData", &CalibrationHandler::getEepromData, DOC(dai, CalibrationHandler, getEepromData))
```

### Comparing `depthai-2.8.0.0/src/DataQueueBindings.cpp` & `depthai-2.9.0.0/src/DataQueueBindings.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,38 @@
 
 // std
 #include <chrono>
 
 // depthai
 #include "depthai/device/DataQueue.hpp"
 
-void DataQueueBindings::bind(pybind11::module& m){
-
+void DataQueueBindings::bind(pybind11::module& m, void* pCallstack){
     using namespace dai;
     using namespace std::chrono;
 
+
+    // Type definitions
+    py::class_<DataOutputQueue, std::shared_ptr<DataOutputQueue>> dataOutputQueue(m, "DataOutputQueue", DOC(dai, DataOutputQueue));
+    py::class_<DataInputQueue, std::shared_ptr<DataInputQueue>> dataInputQueue(m, "DataInputQueue", DOC(dai, DataInputQueue));
+
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    // Actual bindings
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
+
     // To prevent blocking whole python interpreter, blocking functions like 'get' and 'send'
     // are pooled with a reasonable delay and check for python interrupt signal in between.
 
     // Bind DataOutputQueue
     auto addCallbackLambda = [](DataOutputQueue& q, py::function cb) -> int {
         pybind11::module inspect_module = pybind11::module::import("inspect");
         pybind11::object result = inspect_module.attr("signature")(cb).attr("parameters");
@@ -25,15 +44,15 @@
             return q.addCallback(cb.cast<std::function<void(std::shared_ptr<ADatatype>)>>());
         } else if (numParams == 0){
             return q.addCallback(cb.cast<std::function<void()>>());
         } else {
             throw py::value_error("Callback must take either zero, one or two arguments");
         }
     };
-    py::class_<DataOutputQueue, std::shared_ptr<DataOutputQueue>>(m, "DataOutputQueue", DOC(dai, DataOutputQueue))
+    dataOutputQueue
         .def("getName", &DataOutputQueue::getName, DOC(dai, DataOutputQueue, getName))
         .def("isClosed", &DataOutputQueue::isClosed, DOC(dai, DataOutputQueue, isClosed))
         .def("close", &DataOutputQueue::close, DOC(dai, DataOutputQueue, close))
 
         .def("addCallback", addCallbackLambda, py::arg("callback"), DOC(dai, DataOutputQueue, addCallback))
         .def("addCallback", addCallbackLambda, py::arg("callback"), DOC(dai, DataOutputQueue, addCallback, 2))
         .def("addCallback", addCallbackLambda, py::arg("callback"), DOC(dai, DataOutputQueue, addCallback, 3))
@@ -89,15 +108,15 @@
         }, DOC(dai, DataOutputQueue, get, 2))
         .def("has", static_cast<bool(DataOutputQueue::*)()>(&DataOutputQueue::has), DOC(dai, DataOutputQueue, has, 2))
         .def("tryGet", static_cast<std::shared_ptr<ADatatype>(DataOutputQueue::*)()>(&DataOutputQueue::tryGet), DOC(dai, DataOutputQueue, tryGet, 2))
         .def("tryGetAll", static_cast<std::vector<std::shared_ptr<ADatatype>>(DataOutputQueue::*)()>(&DataOutputQueue::tryGetAll), DOC(dai, DataOutputQueue, tryGetAll, 2))
         ;
 
     // Bind DataInputQueue
-    py::class_<DataInputQueue, std::shared_ptr<DataInputQueue>>(m, "DataInputQueue", DOC(dai, DataInputQueue))
+    dataInputQueue
         .def("isClosed", &DataInputQueue::isClosed, DOC(dai, DataInputQueue, isClosed))
         .def("close", &DataInputQueue::close, DOC(dai, DataInputQueue, close))
         .def("getName", &DataInputQueue::getName, DOC(dai, DataInputQueue, getName))
         .def("setBlocking", &DataInputQueue::setBlocking, py::arg("blocking"), DOC(dai, DataInputQueue, setBlocking))
         .def("getBlocking", &DataInputQueue::getBlocking, DOC(dai, DataInputQueue, getBlocking))
         .def("setMaxSize", &DataInputQueue::setMaxSize, py::arg("maxSize"), DOC(dai, DataInputQueue, setMaxSize))
         .def("getMaxSize", &DataInputQueue::getMaxSize, DOC(dai, DataInputQueue, getMaxSize))
```

### Comparing `depthai-2.8.0.0/src/DatatypeBindings.cpp` & `depthai-2.9.0.0/src/DatatypeBindings.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -40,34 +40,106 @@
 
 //pybind
 #include <pybind11/chrono.h>
 #include <pybind11/numpy.h>
 
 // #include "spdlog/spdlog.h"
 
-void DatatypeBindings::bind(pybind11::module& m){
+void DatatypeBindings::bind(pybind11::module& m, void* pCallstack){
 
 
     using namespace dai;
 
-    // Bind Raw datatypes
-    py::class_<RawBuffer, std::shared_ptr<RawBuffer>>(m, "RawBuffer", DOC(dai, RawBuffer))
+    py::class_<RawBuffer, std::shared_ptr<RawBuffer>> rawBuffer(m, "RawBuffer", DOC(dai, RawBuffer));
+    py::class_<RawImgFrame, RawBuffer, std::shared_ptr<RawImgFrame>> rawImgFrame(m, "RawImgFrame", DOC(dai, RawImgFrame));
+    py::enum_<RawImgFrame::Type> rawImgFrameType(rawImgFrame, "Type");
+    py::class_<RawImgFrame::Specs> rawImgFrameSpecs(rawImgFrame, "Specs", DOC(dai, RawImgFrame, Specs));
+    py::class_<RawNNData, RawBuffer, std::shared_ptr<RawNNData>> rawNnData(m, "RawNNData", DOC(dai, RawNNData));
+    py::class_<TensorInfo> tensorInfo(m, "TensorInfo", DOC(dai, TensorInfo));
+    py::enum_<TensorInfo::DataType>tensorInfoDataType(tensorInfo, "DataType");
+    py::enum_<TensorInfo::StorageOrder>tensorInfoStorageOrder(tensorInfo, "StorageOrder");
+    py::class_<ImgDetection> imgDetection(m, "ImgDetection", DOC(dai, ImgDetection));
+    py::class_<SpatialImgDetection, ImgDetection> spatialImgDetection(m, "SpatialImgDetection", DOC(dai, SpatialImgDetection));
+    py::class_<RawImgDetections, RawBuffer, std::shared_ptr<RawImgDetections>> rawImgDetections(m, "RawImgDetections", DOC(dai, RawImgDetections));
+    py::class_<RawSpatialImgDetections, RawBuffer, std::shared_ptr<RawSpatialImgDetections>> rawSpatialImgDetections(m, "RawSpatialImgDetections", DOC(dai, RawSpatialImgDetections));
+    py::class_<RawImageManipConfig, RawBuffer, std::shared_ptr<RawImageManipConfig>> rawImageManipConfig(m, "RawImageManipConfig", DOC(dai, RawImageManipConfig));
+    py::class_<RawImageManipConfig::CropRect> rawImageManipConfigCropRect(rawImageManipConfig, "CropRect", DOC(dai, RawImageManipConfig, CropRect));
+    py::class_<RawImageManipConfig::CropConfig> rawImageManipCropConfig(rawImageManipConfig, "CropConfig", DOC(dai, RawImageManipConfig, CropConfig));
+    py::class_<RawImageManipConfig::ResizeConfig>rawImageManipConfigResizeConfig(rawImageManipConfig, "ResizeConfig", DOC(dai, RawImageManipConfig, ResizeConfig));
+    py::class_<RawImageManipConfig::FormatConfig> rawImageManipConfigFormatConfig(rawImageManipConfig, "FormatConfig", DOC(dai, RawImageManipConfig, FormatConfig));
+    py::class_<RawCameraControl, RawBuffer, std::shared_ptr<RawCameraControl>> rawCameraControl(m, "RawCameraControl", DOC(dai, RawCameraControl));
+    py::class_<Tracklet> tracklet(m, "Tracklet", DOC(dai, Tracklet));
+    py::enum_<Tracklet::TrackingStatus> trackletTrackingStatus(tracklet, "TrackingStatus", DOC(dai, Tracklet, TrackingStatus));
+    py::class_<RawTracklets, RawBuffer, std::shared_ptr<RawTracklets>> rawTacklets(m, "RawTracklets", DOC(dai, RawTracklets));
+    py::class_<IMUReport, std::shared_ptr<IMUReport>> imuReport(m, "IMUReport", DOC(dai, IMUReport));
+    py::enum_<IMUReport::Accuracy> imuReportAccuracy(imuReport, "Accuracy");
+    py::class_<IMUReportAccelerometer, IMUReport, std::shared_ptr<IMUReportAccelerometer>> imuReportAccelerometer(m, "IMUReportAccelerometer", DOC(dai, IMUReportAccelerometer));
+    py::class_<IMUReportGyroscope, IMUReport, std::shared_ptr<IMUReportGyroscope>> imuReportGyroscope(m, "IMUReportGyroscope", DOC(dai, IMUReportGyroscope));
+    py::class_<IMUReportMagneticField, IMUReport, std::shared_ptr<IMUReportMagneticField>> imuReportMagneticField(m, "IMUReportMagneticField", DOC(dai, IMUReportMagneticField));
+    py::class_<IMUReportRotationVectorWAcc, IMUReport, std::shared_ptr<IMUReportRotationVectorWAcc>> imuReportRotationVectorWAcc(m, "IMUReportRotationVectorWAcc", DOC(dai, IMUReportRotationVectorWAcc));
+    py::class_<IMUPacket> imuPacket(m, "IMUPacket", DOC(dai, IMUPacket));
+    py::class_<RawIMUData, RawBuffer, std::shared_ptr<RawIMUData>> rawIMUPackets(m, "RawIMUData", DOC(dai, RawIMUData));
+    py::enum_<RawCameraControl::AutoFocusMode> rawCameraControlAutoFocusMode(rawCameraControl, "AutoFocusMode", DOC(dai, RawCameraControl, AutoFocusMode));
+    py::enum_<RawCameraControl::AutoWhiteBalanceMode> rawCameraControlAutoWhiteBalanceMode(rawCameraControl, "AutoWhiteBalanceMode", DOC(dai, RawCameraControl, AutoWhiteBalanceMode));
+    py::enum_<RawCameraControl::SceneMode> rawCameraControlSceneMode(rawCameraControl, "SceneMode", DOC(dai, RawCameraControl, SceneMode));
+    py::enum_<RawCameraControl::AntiBandingMode> rawCameraControlAntiBandingMode(rawCameraControl, "AntiBandingMode", DOC(dai, RawCameraControl, AntiBandingMode));
+    py::enum_<RawCameraControl::EffectMode> rawCameraControlEffectMode(rawCameraControl, "EffectMode", DOC(dai, RawCameraControl, EffectMode));
+    py::class_<RawSystemInformation, RawBuffer, std::shared_ptr<RawSystemInformation>> rawSystemInformation(m, "RawSystemInformation", DOC(dai, RawSystemInformation));
+    py::class_<ADatatype, std::shared_ptr<ADatatype>> adatatype(m, "ADatatype", DOC(dai, ADatatype));
+    py::class_<Buffer, ADatatype, std::shared_ptr<Buffer>> buffer(m, "Buffer", DOC(dai, Buffer));
+    py::class_<ImgFrame, Buffer, std::shared_ptr<ImgFrame>> imgFrame(m, "ImgFrame", DOC(dai, ImgFrame));
+    py::class_<RotatedRect> rotatedRect(m, "RotatedRect", DOC(dai, RotatedRect));
+    py::class_<NNData, Buffer, std::shared_ptr<NNData>> nnData(m, "NNData", DOC(dai, NNData));
+    py::class_<ImgDetections, Buffer, std::shared_ptr<ImgDetections>> imgDetections(m, "ImgDetections", DOC(dai, ImgDetections));
+    py::class_<SpatialImgDetections, Buffer, std::shared_ptr<SpatialImgDetections>> spatialImgDetections(m, "SpatialImgDetections", DOC(dai, SpatialImgDetections));
+    py::class_<ImageManipConfig, Buffer, std::shared_ptr<ImageManipConfig>> imageManipConfig(m, "ImageManipConfig", DOC(dai, ImageManipConfig));
+    py::class_<CameraControl, Buffer, std::shared_ptr<CameraControl>> cameraControl(m, "CameraControl", DOC(dai, CameraControl));
+    py::class_<SystemInformation, Buffer, std::shared_ptr<SystemInformation>> systemInformation(m, "SystemInformation", DOC(dai, SystemInformation));
+    py::class_<SpatialLocations> spatialLocations(m, "SpatialLocations", DOC(dai, SpatialLocations));
+    py::class_<Rect> rect(m, "Rect", DOC(dai, Rect));
+    py::class_<SpatialLocationCalculatorConfigThresholds> spatialLocationCalculatorConfigThresholds(m, "SpatialLocationCalculatorConfigThresholds", DOC(dai, SpatialLocationCalculatorConfigThresholds));
+    py::class_<SpatialLocationCalculatorConfigData> spatialLocationCalculatorConfigData(m, "SpatialLocationCalculatorConfigData", DOC(dai, SpatialLocationCalculatorConfigData));
+    py::class_<SpatialLocationCalculatorData, Buffer, std::shared_ptr<SpatialLocationCalculatorData>> spatialLocationCalculatorData(m, "SpatialLocationCalculatorData", DOC(dai, SpatialLocationCalculatorData));
+    py::class_<SpatialLocationCalculatorConfig, Buffer, std::shared_ptr<SpatialLocationCalculatorConfig>> spatialLocationCalculatorConfig(m, "SpatialLocationCalculatorConfig", DOC(dai, SpatialLocationCalculatorConfig));
+    py::class_<Tracklets, Buffer, std::shared_ptr<Tracklets>> tracklets(m, "Tracklets", DOC(dai, Tracklets));
+    py::class_<IMUData, Buffer, std::shared_ptr<IMUData>> imuData(m, "IMUData", DOC(dai, IMUData));
+    py::class_<RawStereoDepthConfig, RawBuffer, std::shared_ptr<RawStereoDepthConfig>> rawStereoDepthConfig(m, "RawStereoDepthConfig", DOC(dai, RawStereoDepthConfig));
+    py::class_<StereoDepthConfig, Buffer, std::shared_ptr<StereoDepthConfig>> stereoDepthConfig(m, "StereoDepthConfig", DOC(dai, StereoDepthConfig));
+    py::class_<EdgeDetectorConfigData> edgeDetectorConfigData(m, "EdgeDetectorConfigData", DOC(dai, EdgeDetectorConfigData));
+    py::class_<RawEdgeDetectorConfig, RawBuffer, std::shared_ptr<RawEdgeDetectorConfig>> rawEdgeDetectorConfig(m, "RawEdgeDetectorConfig", DOC(dai, RawEdgeDetectorConfig));
+    py::class_<EdgeDetectorConfig, Buffer, std::shared_ptr<EdgeDetectorConfig>> edgeDetectorConfig(m, "EdgeDetectorConfig", DOC(dai, EdgeDetectorConfig));
+
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    // Actual bindings
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
+
+    rawBuffer
         .def(py::init<>())
         .def_property("data", [](py::object &obj){
             dai::RawBuffer &a = obj.cast<dai::RawBuffer&>();
             return py::array_t<uint8_t>(a.data.size(), a.data.data(), obj);
         }, [](py::object &obj, py::array_t<std::uint8_t, py::array::c_style> array){
             dai::RawBuffer &a = obj.cast<dai::RawBuffer&>();
             a.data = {array.data(), array.data() + array.size()};
         })
         ;
 
 
-    // Bind RawImgFrame
-    py::class_<RawImgFrame, RawBuffer, std::shared_ptr<RawImgFrame>> rawImgFrame(m, "RawImgFrame", DOC(dai, RawImgFrame));
+
     rawImgFrame
         .def(py::init<>())
         .def_readwrite("fb", &RawImgFrame::fb)
         .def_readwrite("category", &RawImgFrame::category)
         .def_readwrite("instanceNum", &RawImgFrame::instanceNum)
         .def_readwrite("sequenceNum", &RawImgFrame::sequenceNum)
         .def_property("ts",
@@ -88,15 +160,16 @@
             [](RawImgFrame& o, double ts){
                 o.tsDevice.sec = ts;
                 o.tsDevice.nsec = (ts - o.tsDevice.sec) * 1000000000.0;
             }
         )
         ;
 
-    py::enum_<RawImgFrame::Type>(rawImgFrame, "Type")
+
+    rawImgFrameType
         .value("YUV422i", RawImgFrame::Type::YUV422i)
         .value("YUV444p", RawImgFrame::Type::YUV444p)
         .value("YUV420p", RawImgFrame::Type::YUV420p)
         .value("YUV422p", RawImgFrame::Type::YUV422p)
         .value("YUV400p", RawImgFrame::Type::YUV400p)
         .value("RGBA8888", RawImgFrame::Type::RGBA8888)
         .value("RGB161616", RawImgFrame::Type::RGB161616)
@@ -124,56 +197,53 @@
         .value("NV12", RawImgFrame::Type::NV12)
         .value("NV21", RawImgFrame::Type::NV21)
         .value("BITSTREAM", RawImgFrame::Type::BITSTREAM)
         .value("HDR", RawImgFrame::Type::HDR)
         .value("NONE", RawImgFrame::Type::NONE)
         ;
 
-    py::class_<RawImgFrame::Specs>(rawImgFrame, "Specs", DOC(dai, RawImgFrame, Specs))
+    rawImgFrameSpecs
         .def(py::init<>())
         .def_readwrite("type", &RawImgFrame::Specs::type)
         .def_readwrite("width", &RawImgFrame::Specs::width)
         .def_readwrite("height", &RawImgFrame::Specs::height)
         .def_readwrite("stride", &RawImgFrame::Specs::stride)
         .def_readwrite("bytesPP", &RawImgFrame::Specs::bytesPP)
         .def_readwrite("p1Offset", &RawImgFrame::Specs::p1Offset)
         .def_readwrite("p2Offset", &RawImgFrame::Specs::p2Offset)
         .def_readwrite("p3Offset", &RawImgFrame::Specs::p3Offset)
         ;
 
 
-    // NNData
-    py::class_<RawNNData, RawBuffer, std::shared_ptr<RawNNData>> rawNnData(m, "RawNNData", DOC(dai, RawNNData));
     rawNnData
         .def(py::init<>())
         .def_readwrite("tensors", &RawNNData::tensors)
         .def_readwrite("batchSize", &RawNNData::batchSize)
         ;
 
-    py::class_<TensorInfo> tensorInfo(m, "TensorInfo", DOC(dai, TensorInfo));
     tensorInfo
         .def(py::init<>())
         .def_readwrite("order", &TensorInfo::order)
         .def_readwrite("dataType", &TensorInfo::dataType)
         .def_readwrite("numDimensions", &TensorInfo::numDimensions)
         .def_readwrite("dims", &TensorInfo::dims)
         .def_readwrite("strides", &TensorInfo::strides)
         .def_readwrite("name", &TensorInfo::name)
         .def_readwrite("offset", &TensorInfo::offset)
         ;
 
-    py::enum_<TensorInfo::DataType>(tensorInfo, "DataType")
+    tensorInfoDataType
         .value("FP16", TensorInfo::DataType::FP16)
         .value("U8F", TensorInfo::DataType::U8F)
         .value("INT", TensorInfo::DataType::INT)
         .value("FP32", TensorInfo::DataType::FP32)
         .value("I8", TensorInfo::DataType::I8)
         ;
 
-    py::enum_<TensorInfo::StorageOrder>(tensorInfo, "StorageOrder")
+    tensorInfoStorageOrder
         .value("NHWC", TensorInfo::StorageOrder::NHWC)
         .value("NHCW", TensorInfo::StorageOrder::NHCW)
         .value("NCHW", TensorInfo::StorageOrder::NCHW)
         .value("HWC", TensorInfo::StorageOrder::HWC)
         .value("CHW", TensorInfo::StorageOrder::CHW)
         .value("WHC", TensorInfo::StorageOrder::WHC)
         .value("HCW", TensorInfo::StorageOrder::HCW)
@@ -182,73 +252,71 @@
         .value("NC", TensorInfo::StorageOrder::NC)
         .value("CN", TensorInfo::StorageOrder::CN)
         .value("C", TensorInfo::StorageOrder::C)
         .value("H", TensorInfo::StorageOrder::H)
         .value("W", TensorInfo::StorageOrder::W)
         ;
 
-    py::class_<ImgDetection>(m, "ImgDetection", DOC(dai, ImgDetection))
+    imgDetection
         .def(py::init<>())
         .def_readwrite("label", &ImgDetection::label)
         .def_readwrite("confidence", &ImgDetection::confidence)
         .def_readwrite("xmin", &ImgDetection::xmin)
         .def_readwrite("ymin", &ImgDetection::ymin)
         .def_readwrite("xmax", &ImgDetection::xmax)
         .def_readwrite("ymax", &ImgDetection::ymax)
         ;
 
-    py::class_<SpatialImgDetection, ImgDetection>(m, "SpatialImgDetection", DOC(dai, SpatialImgDetection))
+
+    spatialImgDetection
         .def(py::init<>())
         .def_readwrite("spatialCoordinates", &SpatialImgDetection::spatialCoordinates)
         ;
 
-    py::class_<RawImgDetections, RawBuffer, std::shared_ptr<RawImgDetections>> RawImgDetections(m, "RawImgDetections", DOC(dai, RawImgDetections));
-    RawImgDetections
+    rawImgDetections
         .def(py::init<>())
         .def_readwrite("detections", &RawImgDetections::detections)
         ;
 
-    py::class_<RawSpatialImgDetections, RawBuffer, std::shared_ptr<RawSpatialImgDetections>> RawSpatialImgDetections(m, "RawSpatialImgDetections", DOC(dai, RawSpatialImgDetections));
-    RawSpatialImgDetections
+    rawSpatialImgDetections
         .def(py::init<>())
         .def_readwrite("detections", &RawSpatialImgDetections::detections)
         ;
 
     // Bind RawImageManipConfig
-    py::class_<RawImageManipConfig, RawBuffer, std::shared_ptr<RawImageManipConfig>> rawImageManipConfig(m, "RawImageManipConfig", DOC(dai, RawImageManipConfig));
     rawImageManipConfig
         .def(py::init<>())
         .def_readwrite("enableFormat", &RawImageManipConfig::enableFormat)
         .def_readwrite("enableResize", &RawImageManipConfig::enableResize)
         .def_readwrite("enableCrop", &RawImageManipConfig::enableCrop)
         .def_readwrite("cropConfig", &RawImageManipConfig::cropConfig)
         .def_readwrite("resizeConfig", &RawImageManipConfig::resizeConfig)
         .def_readwrite("formatConfig", &RawImageManipConfig::formatConfig)
         ;
 
-    py::class_<RawImageManipConfig::CropRect>(rawImageManipConfig, "CropRect", DOC(dai, RawImageManipConfig, CropRect))
+    rawImageManipConfigCropRect
         .def(py::init<>())
         .def_readwrite("xmin", &RawImageManipConfig::CropRect::xmin)
         .def_readwrite("ymin", &RawImageManipConfig::CropRect::ymin)
         .def_readwrite("xmax", &RawImageManipConfig::CropRect::xmax)
         .def_readwrite("ymax", &RawImageManipConfig::CropRect::ymax)
         ;
 
-    py::class_<RawImageManipConfig::CropConfig>(rawImageManipConfig, "CropConfig", DOC(dai, RawImageManipConfig, CropConfig))
+    rawImageManipCropConfig
         .def(py::init<>())
         .def_readwrite("cropRect", &RawImageManipConfig::CropConfig::cropRect)
         .def_readwrite("cropRotatedRect", &RawImageManipConfig::CropConfig::cropRotatedRect)
         .def_readwrite("enableCenterCropRectangle", &RawImageManipConfig::CropConfig::enableCenterCropRectangle)
         .def_readwrite("cropRatio", &RawImageManipConfig::CropConfig::cropRatio)
         .def_readwrite("widthHeightAspectRatio", &RawImageManipConfig::CropConfig::widthHeightAspectRatio)
         .def_readwrite("enableRotatedRect", &RawImageManipConfig::CropConfig::enableRotatedRect)
         .def_readwrite("normalizedCoords", &RawImageManipConfig::CropConfig::normalizedCoords)
         ;
 
-    py::class_<RawImageManipConfig::ResizeConfig>(rawImageManipConfig, "ResizeConfig", DOC(dai, RawImageManipConfig, ResizeConfig))
+    rawImageManipConfigResizeConfig
         .def(py::init<>())
         .def_readwrite("width", &RawImageManipConfig::ResizeConfig::width)
         .def_readwrite("height", &RawImageManipConfig::ResizeConfig::height)
         .def_readwrite("lockAspectRatioFill", &RawImageManipConfig::ResizeConfig::lockAspectRatioFill)
         .def_readwrite("bgRed", &RawImageManipConfig::ResizeConfig::bgRed)
         .def_readwrite("bgGreen", &RawImageManipConfig::ResizeConfig::bgGreen)
         .def_readwrite("bgBlue", &RawImageManipConfig::ResizeConfig::bgBlue)
@@ -259,94 +327,91 @@
         .def_readwrite("enableWarpMatrix", &RawImageManipConfig::ResizeConfig::enableWarpMatrix)
         .def_readwrite("warpBorderReplicate", &RawImageManipConfig::ResizeConfig::warpBorderReplicate)
         .def_readwrite("rotationAngleDeg", &RawImageManipConfig::ResizeConfig::rotationAngleDeg)
         .def_readwrite("enableRotation", &RawImageManipConfig::ResizeConfig::enableRotation)
         .def_readwrite("keepAspectRatio", &RawImageManipConfig::ResizeConfig::keepAspectRatio)
         ;
 
-    py::class_<RawImageManipConfig::FormatConfig>(rawImageManipConfig, "FormatConfig", DOC(dai, RawImageManipConfig, FormatConfig))
+    rawImageManipConfigFormatConfig
         .def(py::init<>())
         .def_readwrite("type", &RawImageManipConfig::FormatConfig::type)
         .def_readwrite("flipHorizontal", &RawImageManipConfig::FormatConfig::flipHorizontal)
         ;
 
 
     // Bind RawCameraControl
-    py::class_<RawCameraControl, RawBuffer, std::shared_ptr<RawCameraControl>> rawCameraControl(m, "RawCameraControl", DOC(dai, RawCameraControl));
     rawCameraControl
         .def(py::init<>())
         .def_readwrite("cmdMask", &RawCameraControl::cmdMask)
         .def_readwrite("autoFocusMode", &RawCameraControl::autoFocusMode)
         .def_readwrite("lensPosition", &RawCameraControl::lensPosition)
         // TODO add more raw types here, not directly used
         ;
 
-    py::class_<Tracklet> tracklet(m, "Tracklet", DOC(dai, Tracklet));
     tracklet
         .def(py::init<>())
         .def_readwrite("roi", &Tracklet::roi)
         .def_readwrite("id", &Tracklet::id)
         .def_readwrite("label", &Tracklet::label)
         .def_readwrite("status", &Tracklet::status)
         .def_readwrite("srcImgDetection", &Tracklet::srcImgDetection)
         .def_readwrite("spatialCoordinates", &Tracklet::spatialCoordinates)
         ;
 
-    py::enum_<Tracklet::TrackingStatus>(tracklet, "TrackingStatus", DOC(dai, Tracklet, TrackingStatus))
+    trackletTrackingStatus
         .value("NEW", Tracklet::TrackingStatus::NEW)
         .value("TRACKED", Tracklet::TrackingStatus::TRACKED)
         .value("LOST", Tracklet::TrackingStatus::LOST)
         .value("REMOVED", Tracklet::TrackingStatus::REMOVED)
         ;
 
     // Bind RawTracklets
-    py::class_<RawTracklets, RawBuffer, std::shared_ptr<RawTracklets>> rawTacklets(m, "RawTracklets", DOC(dai, RawTracklets));
     rawTacklets
         .def(py::init<>())
         .def_readwrite("tracklets", &RawTracklets::tracklets)
         ;
 
 
-    py::class_<IMUReport, std::shared_ptr<IMUReport>> imureport(m, "IMUReport", DOC(dai, IMUReport));
-    imureport
+    imuReport
         .def(py::init<>())
         .def_readwrite("sequence", &IMUReport::sequence)
         .def_readwrite("accuracy", &IMUReport::accuracy)
         .def_readwrite("timestamp", &IMUReport::timestamp)
         ;
 
-    py::enum_<IMUReport::Accuracy>(imureport, "Accuracy")
+
+    imuReportAccuracy
         .value("UNRELIABLE", IMUReport::Accuracy::UNRELIABLE)
         .value("LOW", IMUReport::Accuracy::LOW)
         .value("MEDIUM", IMUReport::Accuracy::MEDIUM)
         .value("HIGH", IMUReport::Accuracy::HIGH)
         ;
 
-    py::class_<IMUReportAccelerometer, IMUReport, std::shared_ptr<IMUReportAccelerometer>>(m, "IMUReportAccelerometer", DOC(dai, IMUReportAccelerometer))
+    imuReportAccelerometer
         .def(py::init<>())
         .def_readwrite("x", &IMUReportAccelerometer::x)
         .def_readwrite("y", &IMUReportAccelerometer::y)
         .def_readwrite("z", &IMUReportAccelerometer::z)
         ;
 
-    py::class_<IMUReportGyroscope, IMUReport, std::shared_ptr<IMUReportGyroscope>>(m, "IMUReportGyroscope", DOC(dai, IMUReportGyroscope))
+    imuReportGyroscope
         .def(py::init<>())
         .def_readwrite("x", &IMUReportGyroscope::x)
         .def_readwrite("y", &IMUReportGyroscope::y)
         .def_readwrite("z", &IMUReportGyroscope::z)
         ;
 
-    py::class_<IMUReportMagneticField, IMUReport, std::shared_ptr<IMUReportMagneticField>>(m, "IMUReportMagneticField", DOC(dai, IMUReportMagneticField))
+    imuReportMagneticField
         .def(py::init<>())
         .def_readwrite("x", &IMUReportMagneticField::x)
         .def_readwrite("y", &IMUReportMagneticField::y)
         .def_readwrite("z", &IMUReportMagneticField::z)
         ;
 
-    py::class_<IMUReportRotationVectorWAcc, IMUReport, std::shared_ptr<IMUReportRotationVectorWAcc>>(m, "IMUReportRotationVectorWAcc", DOC(dai, IMUReportRotationVectorWAcc))
+    imuReportRotationVectorWAcc
         .def(py::init<>())
         .def_readwrite("i", &IMUReportRotationVectorWAcc::i)
         .def_readwrite("j", &IMUReportRotationVectorWAcc::j)
         .def_readwrite("k", &IMUReportRotationVectorWAcc::k)
         .def_readwrite("real", &IMUReportRotationVectorWAcc::real)
         .def_readwrite("rotationVectorAccuracy", &IMUReportRotationVectorWAcc::rotationVectorAccuracy)
         ;
@@ -389,16 +454,15 @@
         .def_readwrite("angVelX", &IMUReportGyroIntegratedRV::angVelX)
         .def_readwrite("angVelY", &IMUReportGyroIntegratedRV::angVelY)
         .def_readwrite("angVelZ", &IMUReportGyroIntegratedRV::angVelZ)
         ;
 
 #endif
 
-    py::class_<IMUPacket> imuPackets(m, "IMUPacket", DOC(dai, IMUPacket));
-    imuPackets
+    imuPacket
         .def(py::init<>())
         .def_readwrite("acceleroMeter", &IMUPacket::acceleroMeter)
         .def_readwrite("gyroscope", &IMUPacket::gyroscope)
         .def_readwrite("magneticField", &IMUPacket::magneticField)
         .def_readwrite("rotationVector", &IMUPacket::rotationVector)
 #if 0
         .def_readwrite("rawAcceleroMeter", &IMUPacket::rawAcceleroMeter)
@@ -414,48 +478,47 @@
         .def_readwrite("arvrStabilizedGameRotationVector", &IMUPacket::arvrStabilizedGameRotationVector)
         .def_readwrite("gyroIntegratedRotationVector", &IMUPacket::gyroIntegratedRotationVector)
 #endif
         ;
 
 
     // Bind RawIMUData
-    py::class_<RawIMUData, RawBuffer, std::shared_ptr<RawIMUData>> rawIMUPackets(m, "RawIMUData", DOC(dai, RawIMUData));
     rawIMUPackets
         .def(py::init<>())
         .def_readwrite("packets", &RawIMUData::packets)
         ;
 
     // RawCameraControl enum bindings
     // The enum fields will also be exposed in 'CameraControl', store them for later
     std::vector<const char *> camCtrlAttr;
     camCtrlAttr.push_back("AutoFocusMode");
-    py::enum_<RawCameraControl::AutoFocusMode>(rawCameraControl, "AutoFocusMode", DOC(dai, RawCameraControl, AutoFocusMode))
+    rawCameraControlAutoFocusMode
         .value("OFF", RawCameraControl::AutoFocusMode::OFF)
         .value("AUTO", RawCameraControl::AutoFocusMode::AUTO)
         .value("MACRO", RawCameraControl::AutoFocusMode::MACRO)
         .value("CONTINUOUS_VIDEO", RawCameraControl::AutoFocusMode::CONTINUOUS_VIDEO)
         .value("CONTINUOUS_PICTURE", RawCameraControl::AutoFocusMode::CONTINUOUS_PICTURE)
         .value("EDOF", RawCameraControl::AutoFocusMode::EDOF)
     ;
 
     camCtrlAttr.push_back("AutoWhiteBalanceMode");
-    py::enum_<RawCameraControl::AutoWhiteBalanceMode>(rawCameraControl, "AutoWhiteBalanceMode", DOC(dai, RawCameraControl, AutoWhiteBalanceMode))
+    rawCameraControlAutoWhiteBalanceMode
         .value("OFF", RawCameraControl::AutoWhiteBalanceMode::OFF)
         .value("AUTO", RawCameraControl::AutoWhiteBalanceMode::AUTO)
         .value("INCANDESCENT", RawCameraControl::AutoWhiteBalanceMode::INCANDESCENT)
         .value("FLUORESCENT", RawCameraControl::AutoWhiteBalanceMode::FLUORESCENT)
         .value("WARM_FLUORESCENT", RawCameraControl::AutoWhiteBalanceMode::WARM_FLUORESCENT)
         .value("DAYLIGHT", RawCameraControl::AutoWhiteBalanceMode::DAYLIGHT)
         .value("CLOUDY_DAYLIGHT", RawCameraControl::AutoWhiteBalanceMode::CLOUDY_DAYLIGHT)
         .value("TWILIGHT", RawCameraControl::AutoWhiteBalanceMode::TWILIGHT)
         .value("SHADE", RawCameraControl::AutoWhiteBalanceMode::SHADE)
     ;
 
     camCtrlAttr.push_back("SceneMode");
-    py::enum_<RawCameraControl::SceneMode>(rawCameraControl, "SceneMode", DOC(dai, RawCameraControl, SceneMode))
+    rawCameraControlSceneMode
         .value("UNSUPPORTED", RawCameraControl::SceneMode::UNSUPPORTED)
         .value("FACE_PRIORITY", RawCameraControl::SceneMode::FACE_PRIORITY)
         .value("ACTION", RawCameraControl::SceneMode::ACTION)
         .value("PORTRAIT", RawCameraControl::SceneMode::PORTRAIT)
         .value("LANDSCAPE", RawCameraControl::SceneMode::LANDSCAPE)
         .value("NIGHT", RawCameraControl::SceneMode::NIGHT)
         .value("NIGHT_PORTRAIT", RawCameraControl::SceneMode::NIGHT_PORTRAIT)
@@ -468,53 +531,53 @@
         .value("SPORTS", RawCameraControl::SceneMode::SPORTS)
         .value("PARTY", RawCameraControl::SceneMode::PARTY)
         .value("CANDLELIGHT", RawCameraControl::SceneMode::CANDLELIGHT)
         .value("BARCODE", RawCameraControl::SceneMode::BARCODE)
     ;
 
     camCtrlAttr.push_back("AntiBandingMode");
-    py::enum_<RawCameraControl::AntiBandingMode>(rawCameraControl, "AntiBandingMode", DOC(dai, RawCameraControl, AntiBandingMode))
+    rawCameraControlAntiBandingMode
         .value("OFF", RawCameraControl::AntiBandingMode::OFF)
         .value("MAINS_50_HZ", RawCameraControl::AntiBandingMode::MAINS_50_HZ)
         .value("MAINS_60_HZ", RawCameraControl::AntiBandingMode::MAINS_60_HZ)
         .value("AUTO", RawCameraControl::AntiBandingMode::AUTO)
     ;
 
     camCtrlAttr.push_back("EffectMode");
-    py::enum_<RawCameraControl::EffectMode>(rawCameraControl, "EffectMode", DOC(dai, RawCameraControl, EffectMode))
+    rawCameraControlEffectMode
         .value("OFF", RawCameraControl::EffectMode::OFF)
         .value("MONO", RawCameraControl::EffectMode::MONO)
         .value("NEGATIVE", RawCameraControl::EffectMode::NEGATIVE)
         .value("SOLARIZE", RawCameraControl::EffectMode::SOLARIZE)
         .value("SEPIA", RawCameraControl::EffectMode::SEPIA)
         .value("POSTERIZE", RawCameraControl::EffectMode::POSTERIZE)
         .value("WHITEBOARD", RawCameraControl::EffectMode::WHITEBOARD)
         .value("BLACKBOARD", RawCameraControl::EffectMode::BLACKBOARD)
         .value("AQUA", RawCameraControl::EffectMode::AQUA)
     ;
 
     // Bind RawSystemInformation
-    py::class_<RawSystemInformation, RawBuffer, std::shared_ptr<RawSystemInformation>> rawSystemInformation(m, "RawSystemInformation", DOC(dai, RawSystemInformation));
     rawSystemInformation
         .def(py::init<>())
         .def_readwrite("ddrMemoryUsage", &RawSystemInformation::ddrMemoryUsage)
         .def_readwrite("cmxMemoryUsage", &RawSystemInformation::cmxMemoryUsage)
         .def_readwrite("leonCssMemoryUsage", &RawSystemInformation::leonCssMemoryUsage)
         .def_readwrite("leonMssMemoryUsage", &RawSystemInformation::leonMssMemoryUsage)
         .def_readwrite("leonCssCpuUsage", &RawSystemInformation::leonCssCpuUsage)
         .def_readwrite("leonMssCpuUsage", &RawSystemInformation::leonMssCpuUsage)
         .def_readwrite("chipTemperature", &RawSystemInformation::chipTemperature)
         ;
 
 
     // Bind non-raw 'helper' datatypes
-    py::class_<ADatatype, std::shared_ptr<ADatatype>>(m, "ADatatype", DOC(dai, ADatatype))
+    adatatype
         .def("getRaw", &ADatatype::getRaw);
 
-    py::class_<Buffer, ADatatype, std::shared_ptr<Buffer>>(m, "Buffer", DOC(dai, Buffer))
+
+    buffer
         .def(py::init<>(), DOC(dai, Buffer, Buffer))
 
         // obj is "Python" object, which we used then to bind the numpy arrays lifespan to
         .def("getData", [](py::object &obj){
             // creates numpy array (zero-copy) which holds correct information such as shape, ...
             dai::Buffer &a = obj.cast<dai::Buffer&>();
             return py::array_t<uint8_t>(a.getData().size(), a.getData().data(), obj);
@@ -523,15 +586,15 @@
         .def("setData", [](Buffer& buffer, py::array_t<std::uint8_t, py::array::c_style | py::array::forcecast> array){
             buffer.getData().clear();
             buffer.getData().insert(buffer.getData().begin(), array.data(), array.data() + array.nbytes());
         }, DOC(dai, Buffer, setData))
         ;
 
     // Bind ImgFrame
-    py::class_<ImgFrame, Buffer, std::shared_ptr<ImgFrame>>(m, "ImgFrame", DOC(dai, ImgFrame))
+    imgFrame
         .def(py::init<>())
         // getters
         .def("getTimestamp", &ImgFrame::getTimestamp, DOC(dai, ImgFrame, getTimestamp))
         .def("getTimestampDevice", &ImgFrame::getTimestampDevice, DOC(dai, ImgFrame, getTimestampDevice))
         .def("getInstanceNum", &ImgFrame::getInstanceNum, DOC(dai, ImgFrame, getInstanceNum))
         .def("getCategory", &ImgFrame::getCategory, DOC(dai, ImgFrame, getCategory))
         .def("getSequenceNum", &ImgFrame::getSequenceNum, DOC(dai, ImgFrame, getSequenceNum))
@@ -731,23 +794,24 @@
         .def("setHeight", &ImgFrame::setHeight, py::arg("height"), DOC(dai, ImgFrame, setHeight))
         .def("setType", &ImgFrame::setType, py::arg("type"), DOC(dai, ImgFrame, setType))
         ;
     // add aliases dai.ImgFrame.Type and dai.ImgFrame.Specs
     m.attr("ImgFrame").attr("Type") = m.attr("RawImgFrame").attr("Type");
     m.attr("ImgFrame").attr("Specs") = m.attr("RawImgFrame").attr("Specs");
 
-    py::class_<RotatedRect>(m, "RotatedRect", DOC(dai, RotatedRect))
+    rotatedRect
         .def(py::init<>())
         .def_readwrite("center", &RotatedRect::center)
         .def_readwrite("size", &RotatedRect::size)
         .def_readwrite("angle", &RotatedRect::angle)
         ;
 
     // Bind NNData
-    py::class_<NNData, Buffer, std::shared_ptr<NNData>>(m, "NNData", DOC(dai, NNData))
+
+    nnData
         .def(py::init<>(), DOC(dai, NNData, NNData))
         // setters
         .def("setLayer", [](NNData& obj, const std::string& name, py::array_t<std::uint8_t, py::array::c_style | py::array::forcecast> data){
             std::vector<std::uint8_t> vec(data.data(), data.data() + data.size());
             obj.setLayer(name, std::move(vec));
         }, py::arg("name"), py::arg("data"), DOC(dai, NNData, setLayer))
         .def("setLayer", static_cast<void(NNData::*)(const std::string&, const std::vector<int>&)>(&NNData::setLayer), py::arg("name"), py::arg("data"), DOC(dai, NNData, setLayer, 2))
@@ -763,27 +827,30 @@
         .def("getLayerInt32", &NNData::getLayerInt32, py::arg("name"), DOC(dai, NNData, getLayerInt32))
         .def("getFirstLayerUInt8", &NNData::getFirstLayerUInt8, DOC(dai, NNData, getFirstLayerUInt8))
         .def("getFirstLayerFp16", &NNData::getFirstLayerFp16, DOC(dai, NNData, getFirstLayerFp16))
         .def("getFirstLayerInt32", &NNData::getFirstLayerInt32, DOC(dai, NNData, getFirstLayerInt32))
         ;
 
     // Bind ImgDetections
-    py::class_<ImgDetections, Buffer, std::shared_ptr<ImgDetections>>(m, "ImgDetections", DOC(dai, ImgDetections))
+
+    imgDetections
         .def(py::init<>(), DOC(dai, ImgDetections, ImgDetections))
         .def_property("detections", [](ImgDetections& det) { return &det.detections; }, [](ImgDetections& det, std::vector<ImgDetection> val) { det.detections = val; }, DOC(dai, ImgDetections, detections))
         ;
 
     // Bind SpatialImgDetections
-    py::class_<SpatialImgDetections, Buffer, std::shared_ptr<SpatialImgDetections>>(m, "SpatialImgDetections", DOC(dai, SpatialImgDetections))
+
+    spatialImgDetections
         .def(py::init<>())
         .def_property("detections", [](SpatialImgDetections& det) { return &det.detections; }, [](SpatialImgDetections& det, std::vector<SpatialImgDetection> val) { det.detections = val; })
         ;
 
      // Bind ImageManipConfig
-    py::class_<ImageManipConfig, Buffer, std::shared_ptr<ImageManipConfig>>(m, "ImageManipConfig", DOC(dai, ImageManipConfig))
+
+    imageManipConfig
         .def(py::init<>())
         // setters
         .def("setCropRect", &ImageManipConfig::setCropRect, py::arg("xmin"), py::arg("ymin"), py::arg("xmax"), py::arg("xmax"), DOC(dai, ImageManipConfig, setCropRect))
         .def("setCropRotatedRect", &ImageManipConfig::setCropRotatedRect, py::arg("rr"), py::arg("normalizedCoords") = true, DOC(dai, ImageManipConfig, setCropRotatedRect))
         .def("setCenterCrop", &ImageManipConfig::setCenterCrop, py::arg("ratio"), py::arg("whRatio")=1.0f, DOC(dai, ImageManipConfig, setCenterCrop))
         .def("setWarpTransformFourPoints", &ImageManipConfig::setWarpTransformFourPoints, py::arg("pt"), py::arg("normalizedCoords"), DOC(dai, ImageManipConfig, setWarpTransformFourPoints))
         .def("setWarpTransformMatrix3x3", &ImageManipConfig::setWarpTransformMatrix3x3, py::arg("mat"), DOC(dai, ImageManipConfig, setWarpTransformMatrix3x3))
@@ -806,15 +873,16 @@
         .def("getCropYMax", &ImageManipConfig::getCropYMax, DOC(dai, ImageManipConfig, getCropYMax))
         .def("getResizeWidth", &ImageManipConfig::getResizeWidth, DOC(dai, ImageManipConfig, getResizeWidth))
         .def("getResizeHeight", &ImageManipConfig::getResizeHeight, DOC(dai, ImageManipConfig, getResizeHeight))
         .def("isResizeThumbnail", &ImageManipConfig::isResizeThumbnail, DOC(dai, ImageManipConfig, isResizeThumbnail))
         ;
 
     // Bind CameraControl
-    py::class_<CameraControl, Buffer, std::shared_ptr<CameraControl>>(m, "CameraControl", DOC(dai, CameraControl))
+
+    cameraControl
         .def(py::init<>(), DOC(dai, CameraControl, CameraControl))
         // setters
         .def("setCaptureStill", &CameraControl::setCaptureStill, py::arg("capture"), DOC(dai, CameraControl, setCaptureStill))
         .def("setStartStreaming", &CameraControl::setStartStreaming, DOC(dai, CameraControl, setStartStreaming))
         .def("setStopStreaming", &CameraControl::setStopStreaming, DOC(dai, CameraControl, setStopStreaming))
         .def("setAutoFocusMode", &CameraControl::setAutoFocusMode, py::arg("mode"), DOC(dai, CameraControl, setAutoFocusMode))
         .def("setAutoFocusTrigger", &CameraControl::setAutoFocusTrigger, DOC(dai, CameraControl, setAutoFocusTrigger))
@@ -841,37 +909,40 @@
         ;
     // Add also enum attributes from RawCameraControl
     for (const auto& a : camCtrlAttr) {
         m.attr("CameraControl").attr(a) = m.attr("RawCameraControl").attr(a);
     }
 
     // Bind SystemInformation
-    py::class_<SystemInformation, Buffer, std::shared_ptr<SystemInformation>>(m, "SystemInformation", DOC(dai, SystemInformation))
+
+    systemInformation
         .def(py::init<>())
         .def_property("ddrMemoryUsage", [](SystemInformation& i) { return &i.ddrMemoryUsage; }, [](SystemInformation& i, MemoryInfo val) { i.ddrMemoryUsage = val; } )
         .def_property("cmxMemoryUsage", [](SystemInformation& i) { return &i.cmxMemoryUsage; }, [](SystemInformation& i, MemoryInfo val) { i.cmxMemoryUsage = val; } )
         .def_property("leonCssMemoryUsage", [](SystemInformation& i) { return &i.leonCssMemoryUsage; }, [](SystemInformation& i, MemoryInfo val) { i.leonCssMemoryUsage = val; } )
         .def_property("leonMssMemoryUsage", [](SystemInformation& i) { return &i.leonMssMemoryUsage; }, [](SystemInformation& i, MemoryInfo val) { i.leonMssMemoryUsage = val; } )
         .def_property("leonCssCpuUsage", [](SystemInformation& i) { return &i.leonCssCpuUsage; }, [](SystemInformation& i, CpuUsage val) { i.leonCssCpuUsage = val; } )
         .def_property("leonMssCpuUsage", [](SystemInformation& i) { return &i.leonMssCpuUsage; }, [](SystemInformation& i, CpuUsage val) { i.leonMssCpuUsage = val; } )
         .def_property("chipTemperature", [](SystemInformation& i) { return &i.chipTemperature; }, [](SystemInformation& i, ChipTemperature val) { i.chipTemperature = val; } )
         ;
 
-    py::class_<SpatialLocations> (m, "SpatialLocations", DOC(dai, SpatialLocations))
+
+    spatialLocations
         .def(py::init<>())
         .def_readwrite("config", &SpatialLocations::config, DOC(dai, SpatialLocations, config))
         .def_readwrite("depthAverage", &SpatialLocations::depthAverage, DOC(dai, SpatialLocations, depthAverage))
         .def_readwrite("depthMin", &SpatialLocations::depthMin, DOC(dai, SpatialLocations, depthMin))
         .def_readwrite("depthMax", &SpatialLocations::depthMax, DOC(dai, SpatialLocations, depthMax))
         .def_readwrite("depthAveragePixelCount", &SpatialLocations::depthAveragePixelCount, DOC(dai, SpatialLocations, depthAveragePixelCount))
         .def_readwrite("spatialCoordinates", &SpatialLocations::spatialCoordinates, DOC(dai, SpatialLocations, spatialCoordinates))
         ;
 
 
-    py::class_<Rect> (m, "Rect", DOC(dai, Rect))
+
+    rect
         .def(py::init<>())
         .def(py::init<float, float, float, float>())
         .def(py::init<Point2f, Point2f>())
         .def(py::init<Point2f, Size2f>())
 
         .def("topLeft", &Rect::topLeft, DOC(dai, Rect, topLeft))
         .def("bottomRight", &Rect::bottomRight, DOC(dai, Rect, bottomRight))
@@ -884,89 +955,91 @@
         .def("normalize", &Rect::normalize, py::arg("width"), py::arg("height"), DOC(dai, Rect, normalize))
         .def_readwrite("x", &Rect::x)
         .def_readwrite("y", &Rect::y)
         .def_readwrite("width", &Rect::width)
         .def_readwrite("height", &Rect::height)
         ;
 
-    py::class_<SpatialLocationCalculatorConfigThresholds> (m, "SpatialLocationCalculatorConfigThresholds", DOC(dai, SpatialLocationCalculatorConfigThresholds))
+
+    spatialLocationCalculatorConfigThresholds
         .def(py::init<>())
         .def_readwrite("lowerThreshold", &SpatialLocationCalculatorConfigThresholds::lowerThreshold)
         .def_readwrite("upperThreshold", &SpatialLocationCalculatorConfigThresholds::upperThreshold)
         ;
 
-    py::class_<SpatialLocationCalculatorConfigData> (m, "SpatialLocationCalculatorConfigData", DOC(dai, SpatialLocationCalculatorConfigData))
+
+    spatialLocationCalculatorConfigData
         .def(py::init<>())
         .def_readwrite("roi", &SpatialLocationCalculatorConfigData::roi)
         .def_readwrite("depthThresholds", &SpatialLocationCalculatorConfigData::depthThresholds)
         ;
 
     // Bind SpatialLocationCalculatorData
-    py::class_<SpatialLocationCalculatorData, Buffer, std::shared_ptr<SpatialLocationCalculatorData>>(m, "SpatialLocationCalculatorData", DOC(dai, SpatialLocationCalculatorData))
+
+    spatialLocationCalculatorData
         .def(py::init<>())
         .def("getSpatialLocations", &SpatialLocationCalculatorData::getSpatialLocations, DOC(dai, SpatialLocationCalculatorData, getSpatialLocations))
         ;
 
     // SpatialLocationCalculatorConfig (after ConfigData)
-    py::class_<SpatialLocationCalculatorConfig, Buffer, std::shared_ptr<SpatialLocationCalculatorConfig>>(m, "SpatialLocationCalculatorConfig", DOC(dai, SpatialLocationCalculatorConfig))
+
+    spatialLocationCalculatorConfig
         .def(py::init<>())
         // setters
         .def("setROIs", &SpatialLocationCalculatorConfig::setROIs, py::arg("ROIs"), DOC(dai, SpatialLocationCalculatorConfig, setROIs))
         .def("addROI", &SpatialLocationCalculatorConfig::addROI, py::arg("ROI"), DOC(dai, SpatialLocationCalculatorConfig, addROI))
         .def("getConfigData", &SpatialLocationCalculatorConfig::getConfigData, DOC(dai, SpatialLocationCalculatorConfig, getConfigData))
         ;
 
     // Tracklets (after ConfigData)
-    py::class_<Tracklets, Buffer, std::shared_ptr<Tracklets>>(m, "Tracklets", DOC(dai, Tracklets))
+
+    tracklets
         .def(py::init<>())
         .def_property("tracklets", [](Tracklets& track) { return &track.tracklets; }, [](Tracklets& track, std::vector<Tracklet> val) { track.tracklets = val; }, DOC(dai, Tracklets, tracklets))
         ;
 
 
-    // IMUData (after ConfigData)
-    py::class_<IMUData, Buffer, std::shared_ptr<IMUData>>(m, "IMUData", DOC(dai, IMUData))
+
+    imuData
         .def(py::init<>())
         .def_property("packets", [](IMUData& imuDta) { return &imuDta.packets; }, [](IMUData& imuDta, std::vector<IMUPacket> val) { imuDta.packets = val; }, DOC(dai, IMUData, packets))
         ;
 
-    // Bind RawStereoDepthConfig
-    py::class_<RawStereoDepthConfig, RawBuffer, std::shared_ptr<RawStereoDepthConfig>> rawStereoDepthConfig(m, "RawStereoDepthConfig", DOC(dai, RawStereoDepthConfig));
+
     rawStereoDepthConfig
         .def(py::init<>())
         .def_readwrite("config", &RawStereoDepthConfig::config)
         ;
 
-    // StereoDepthConfig (after ConfigData)
-    py::class_<StereoDepthConfig, Buffer, std::shared_ptr<StereoDepthConfig>>(m, "StereoDepthConfig", DOC(dai, StereoDepthConfig))
+
+    stereoDepthConfig
         .def(py::init<>())
         .def("setConfidenceThreshold",  &StereoDepthConfig::setConfidenceThreshold, py::arg("confThr"), DOC(dai, StereoDepthConfig, setConfidenceThreshold))
         .def("setMedianFilter",         &StereoDepthConfig::setMedianFilter, py::arg("median"), DOC(dai, StereoDepthConfig, setMedianFilter))
         .def("setBilateralFilterSigma", &StereoDepthConfig::setBilateralFilterSigma, py::arg("sigma"), DOC(dai, StereoDepthConfig, setBilateralFilterSigma))
         .def("setLeftRightCheckThreshold", &StereoDepthConfig::setLeftRightCheckThreshold, py::arg("sigma"), DOC(dai, StereoDepthConfig, setLeftRightCheckThreshold))
         .def("getConfidenceThreshold",  &StereoDepthConfig::getConfidenceThreshold, DOC(dai, StereoDepthConfig, getConfidenceThreshold))
         .def("getMedianFilter",         &StereoDepthConfig::getMedianFilter, DOC(dai, StereoDepthConfig, getMedianFilter))
         .def("getBilateralFilterSigma", &StereoDepthConfig::getBilateralFilterSigma, DOC(dai, StereoDepthConfig, getBilateralFilterSigma))
         .def("getLeftRightCheckThreshold",         &StereoDepthConfig::getLeftRightCheckThreshold, DOC(dai, StereoDepthConfig, getLeftRightCheckThreshold))
         ;
 
-
-    py::class_<EdgeDetectorConfigData> (m, "EdgeDetectorConfigData", DOC(dai, EdgeDetectorConfigData))
+    edgeDetectorConfigData
         .def(py::init<>())
         .def_readwrite("sobelFilterHorizontalKernel", &EdgeDetectorConfigData::sobelFilterHorizontalKernel, DOC(dai, EdgeDetectorConfigData, sobelFilterHorizontalKernel))
         .def_readwrite("sobelFilterVerticalKernel", &EdgeDetectorConfigData::sobelFilterVerticalKernel, DOC(dai, EdgeDetectorConfigData, sobelFilterVerticalKernel))
         ;
 
-    // Bind RawEdgeDetectorConfig
-    py::class_<RawEdgeDetectorConfig, RawBuffer, std::shared_ptr<RawEdgeDetectorConfig>> rawEdgeDetectorConfig(m, "RawEdgeDetectorConfig", DOC(dai, RawEdgeDetectorConfig));
+
     rawEdgeDetectorConfig
         .def(py::init<>())
         .def_readwrite("config", &RawEdgeDetectorConfig::config)
         ;
 
-    // EdgeDetectorConfig (after ConfigData)
-    py::class_<EdgeDetectorConfig, Buffer, std::shared_ptr<EdgeDetectorConfig>>(m, "EdgeDetectorConfig", DOC(dai, EdgeDetectorConfig))
+
+    edgeDetectorConfig
         .def(py::init<>())
         .def("setSobelFilterKernels",  &EdgeDetectorConfig::setSobelFilterKernels, py::arg("horizontalKernel"), py::arg("verticalKernel"), DOC(dai, EdgeDetectorConfig, setSobelFilterKernels))
         .def("getConfigData",         &EdgeDetectorConfig::getConfigData, DOC(dai, EdgeDetectorConfig, getConfigData))
         ;
 
 }
```

### Comparing `depthai-2.8.0.0/src/DeviceBindings.cpp` & `depthai-2.9.0.0/src/DeviceBindings.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -108,25 +108,45 @@
         if (PyErr_CheckSignals() != 0) throw py::error_already_set();
     } while(unlimitedTimeout || steady_clock::now() - startTime < timeout);
 
     return std::vector<std::string>();
 }
 
 
-void DeviceBindings::bind(pybind11::module& m){
+void DeviceBindings::bind(pybind11::module& m, void* pCallstack){
 
     using namespace dai;
 
+    // Type definitions
+    py::class_<Device> device(m, "Device", DOC(dai, Device));
+
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
+
 
     // Bind Device, using DeviceWrapper to be able to destruct the object by calling close()
-    py::class_<Device>(m, "Device", DOC(dai, Device))
+    device
         // Python only methods
         .def("__enter__", [](py::object obj){ return obj; })
-        .def("__exit__", [](Device& d, py::object type, py::object value, py::object traceback) { d.close(); })
-        .def("close", &Device::close, "Closes the connection to device. Better alternative is the usage of context manager: `with depthai.Device(pipeline) as device:`")
+        .def("__exit__", [](Device& d, py::object type, py::object value, py::object traceback) {
+            py::gil_scoped_release release;
+            d.close();
+        })
+        .def("close", [](Device& d) { py::gil_scoped_release release; d.close(); }, "Closes the connection to device. Better alternative is the usage of context manager: `with depthai.Device(pipeline) as device:`")
         .def("isClosed", &Device::isClosed, "Check if the device is still connected`")
 
         //dai::Device methods
         //static
         .def_static("getAnyAvailableDevice", [](std::chrono::microseconds us){ return Device::getAnyAvailableDevice(us); }, py::arg("timeout"), DOC(dai, Device, getAnyAvailableDevice))
         .def_static("getAnyAvailableDevice", [](){ return Device::getAnyAvailableDevice(); }, DOC(dai, Device, getAnyAvailableDevice, 2))
         .def_static("getFirstAvailableDevice", &Device::getFirstAvailableDevice, DOC(dai, Device, getFirstAvailableDevice))
@@ -151,15 +171,14 @@
             return std::unique_ptr<Device>(new Device(pipeline, deviceInfo, usb2Mode));
         }), py::arg("pipeline"), py::arg("deviceDesc"), py::arg("usb2Mode") = false, DOC(dai, Device, Device, 4))
         .def(py::init([](const Pipeline& pipeline, const DeviceInfo& deviceInfo, std::string pathToCmd){
             // Non blocking constructor
             return std::unique_ptr<Device>(new Device(pipeline, deviceInfo, pathToCmd));
         }), py::arg("pipeline"), py::arg("deviceDesc"), py::arg("pathToCmd"), DOC(dai, Device, Device, 5))
 
-
         // Device constructor - OpenVINO version
         .def(py::init([](OpenVINO::Version version){ return deviceConstructorHelper(version); }), py::arg("version") = Pipeline::DEFAULT_OPENVINO_VERSION, DOC(dai, Device, Device, 6))
         .def(py::init([](OpenVINO::Version version, bool usb2Mode){
             // Blocking constructor
             return deviceConstructorHelper(version, std::string(""), usb2Mode);
         }), py::arg("version"), py::arg("usb2Mode"), DOC(dai, Device, Device, 7))
         .def(py::init([](OpenVINO::Version version, const std::string& pathToCmd){
@@ -171,24 +190,25 @@
             return std::unique_ptr<Device>(new Device(version, deviceInfo, usb2Mode));
         }), py::arg("version"), py::arg("deviceDesc"), py::arg("usb2Mode") = false, DOC(dai, Device, Device, 9))
         .def(py::init([](OpenVINO::Version version, const DeviceInfo& deviceInfo, std::string pathToCmd){
             // Non blocking constructor
             return std::unique_ptr<Device>(new Device(version, deviceInfo, pathToCmd));
         }), py::arg("version"), py::arg("deviceDesc"), py::arg("pathToCmd"), DOC(dai, Device, Device, 10))
 
-        .def("isPipelineRunning", &Device::isPipelineRunning, DOC(dai, Device, isPipelineRunning))
+        .def("isPipelineRunning", [](Device& d) { py::gil_scoped_release release; return d.isPipelineRunning(); }, DOC(dai, Device, isPipelineRunning))
         .def("startPipeline", [](Device& d){
             // Issue an deprecation warning
             PyErr_WarnEx(PyExc_DeprecationWarning, "Device(pipeline) starts the pipeline automatically. Use Device() and startPipeline(pipeline) otherwise", 1);
             HEDLEY_DIAGNOSTIC_PUSH
             HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED
+            py::gil_scoped_release release;
             d.startPipeline();
             HEDLEY_DIAGNOSTIC_POP
         }, DOC(dai, Device, startPipeline))
-        .def("startPipeline", py::overload_cast<const Pipeline&>(&Device::startPipeline), DOC(dai, Device, startPipeline, 2))
+        .def("startPipeline", [](Device& d, const Pipeline& pipeline) { py::gil_scoped_release release; return d.startPipeline(pipeline); }, DOC(dai, Device, startPipeline, 2))
 
         .def("getOutputQueue", static_cast<std::shared_ptr<DataOutputQueue>(Device::*)(const std::string&)>(&Device::getOutputQueue), py::arg("name"), DOC(dai, Device, getOutputQueue))
         .def("getOutputQueue", static_cast<std::shared_ptr<DataOutputQueue>(Device::*)(const std::string&, unsigned int, bool)>(&Device::getOutputQueue), py::arg("name"), py::arg("maxSize"), py::arg("blocking") = true, DOC(dai, Device, getOutputQueue, 2))
         .def("getOutputQueueNames", &Device::getOutputQueueNames, DOC(dai, Device, getOutputQueueNames))
 
         .def("getInputQueue", static_cast<std::shared_ptr<DataInputQueue>(Device::*)(const std::string&)>(&Device::getInputQueue), py::arg("name"), DOC(dai, Device, getInputQueue))
         .def("getInputQueue", static_cast<std::shared_ptr<DataInputQueue>(Device::*)(const std::string&, unsigned int, bool)>(&Device::getInputQueue), py::arg("name"), py::arg("maxSize"), py::arg("blocking") = true, DOC(dai, Device, getInputQueue, 2))
@@ -222,29 +242,33 @@
         .def("getQueueEvent", [](Device& d, std::chrono::microseconds timeout) {
             auto events = deviceGetQueueEventsHelper(d, d.getOutputQueueNames(), std::numeric_limits<std::size_t>::max(), timeout);
             if(events.empty()) return std::string("");
             return events[0];
         }, py::arg("timeout") = std::chrono::microseconds(-1), DOC(dai, Device, getQueueEvent, 4))
 
         //.def("setCallback", DeviceWrapper::wrap(&Device::setCallback), py::arg("name"), py::arg("callback"))
-        .def("setLogLevel", &Device::setLogLevel, py::arg("level"), DOC(dai, Device, setLogLevel))
-        .def("getLogLevel", &Device::getLogLevel, DOC(dai, Device, getLogLevel))
-        .def("getDeviceInfo", &Device::getDeviceInfo, DOC(dai, Device, getDeviceInfo))
-        .def("setSystemInformationLoggingRate", &Device::setSystemInformationLoggingRate, py::arg("rateHz"), DOC(dai, Device, setSystemInformationLoggingRate))
-        .def("getSystemInformationLoggingRate", &Device::getSystemInformationLoggingRate, DOC(dai, Device, getSystemInformationLoggingRate))
-        .def("getMxId", &Device::getMxId, DOC(dai, Device, getMxId))
-        .def("getConnectedCameras", &Device::getConnectedCameras, DOC(dai, Device, getConnectedCameras))
-        .def("getDdrMemoryUsage", &Device::getDdrMemoryUsage, DOC(dai, Device, getDdrMemoryUsage))
-        .def("getCmxMemoryUsage", &Device::getCmxMemoryUsage, DOC(dai, Device, getCmxMemoryUsage))
-        .def("getLeonCssHeapUsage", &Device::getLeonCssHeapUsage, DOC(dai, Device, getLeonCssHeapUsage))
-        .def("getLeonMssHeapUsage", &Device::getLeonMssHeapUsage, DOC(dai, Device, getLeonMssHeapUsage))
-        .def("getChipTemperature", &Device::getChipTemperature, DOC(dai, Device, getChipTemperature))
-        .def("getLeonCssCpuUsage", &Device::getLeonCssCpuUsage, DOC(dai, Device, getLeonCssCpuUsage))
-        .def("getLeonMssCpuUsage", &Device::getLeonMssCpuUsage, DOC(dai, Device, getLeonMssCpuUsage))
-        .def("getUsbSpeed", &Device::getUsbSpeed, DOC(dai, Device, getUsbSpeed))
+
+        // Doesn't require GIL release (eg, don't do RPC or long blocking things in background)
         .def("setLogOutputLevel", &Device::setLogOutputLevel, py::arg("level"), DOC(dai, Device, setLogOutputLevel))
         .def("getLogOutputLevel", &Device::getLogOutputLevel, DOC(dai, Device, getLogOutputLevel))
-        .def("addLogCallback", &Device::addLogCallback, py::arg("callback"), DOC(dai, Device, addLogCallback))
-        .def("removeLogCallback", &Device::removeLogCallback, py::arg("callbackId"), DOC(dai, Device, removeLogCallback))
-        ;
+
+        // Requires GIL release
+        .def("setLogLevel", [](Device& d, LogLevel l) { py::gil_scoped_release release; d.setLogLevel(l); }, py::arg("level"), DOC(dai, Device, setLogLevel))
+        .def("getLogLevel", [](Device& d) { py::gil_scoped_release release; return d.getLogLevel(); }, DOC(dai, Device, getLogLevel))
+        .def("setSystemInformationLoggingRate", [](Device& d, float hz) { py::gil_scoped_release release; d.setSystemInformationLoggingRate(hz); }, py::arg("rateHz"), DOC(dai, Device, setSystemInformationLoggingRate))
+        .def("getSystemInformationLoggingRate", [](Device& d) { py::gil_scoped_release release; return d.getSystemInformationLoggingRate(); }, DOC(dai, Device, getSystemInformationLoggingRate))
+        .def("getConnectedCameras", [](Device& d) { py::gil_scoped_release release; return d.getConnectedCameras(); }, DOC(dai, Device, getConnectedCameras))
+        .def("getDdrMemoryUsage", [](Device& d) { py::gil_scoped_release release; return d.getDdrMemoryUsage(); }, DOC(dai, Device, getDdrMemoryUsage))
+        .def("getCmxMemoryUsage", [](Device& d) { py::gil_scoped_release release; return d.getCmxMemoryUsage(); }, DOC(dai, Device, getCmxMemoryUsage))
+        .def("getLeonCssHeapUsage", [](Device& d) { py::gil_scoped_release release; return d.getLeonCssHeapUsage(); }, DOC(dai, Device, getLeonCssHeapUsage))
+        .def("getLeonMssHeapUsage", [](Device& d) { py::gil_scoped_release release; return d.getLeonMssHeapUsage(); }, DOC(dai, Device, getLeonMssHeapUsage))
+        .def("getChipTemperature", [](Device& d) { py::gil_scoped_release release; return d.getChipTemperature(); }, DOC(dai, Device, getChipTemperature))
+        .def("getLeonCssCpuUsage", [](Device& d) { py::gil_scoped_release release; return d.getLeonCssCpuUsage(); }, DOC(dai, Device, getLeonCssCpuUsage))
+        .def("getLeonMssCpuUsage", [](Device& d) { py::gil_scoped_release release; return d.getLeonMssCpuUsage(); }, DOC(dai, Device, getLeonMssCpuUsage))
+        .def("addLogCallback", [](Device& d, std::function<void(LogMessage)> callback) { py::gil_scoped_release release; return d.addLogCallback(callback); }, py::arg("callback"), DOC(dai, Device, addLogCallback))
+        .def("removeLogCallback", [](Device& d, int cbId) { py::gil_scoped_release release; return d.removeLogCallback(cbId); }, py::arg("callbackId"), DOC(dai, Device, removeLogCallback))
+        .def("getUsbSpeed", [](Device& d) { py::gil_scoped_release release; return d.getUsbSpeed(); }, DOC(dai, Device, getUsbSpeed))
+        .def("getDeviceInfo", [](Device& d) { py::gil_scoped_release release; return d.getDeviceInfo(); }, DOC(dai, Device, getDeviceInfo))
+        .def("getMxId", [](Device& d) { py::gil_scoped_release release; return d.getMxId(); }, DOC(dai, Device, getMxId));
+    ;
 
 }
```

### Comparing `depthai-2.8.0.0/src/DeviceBootloaderBindings.cpp` & `depthai-2.9.0.0/src/DeviceBootloaderBindings.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 #include "DeviceBootloaderBindings.hpp"
 
 // depthai
 #include "depthai/device/DeviceBootloader.hpp"
 
-void DeviceBootloaderBindings::bind(pybind11::module& m){
+void DeviceBootloaderBindings::bind(pybind11::module& m, void* pCallstack){
 
     using namespace dai;
 
-    // Bind DeviceBootloader
+    // Type definitions
     py::class_<DeviceBootloader> deviceBootloader(m, "DeviceBootloader", DOC(dai, DeviceBootloader));
+    py::class_<DeviceBootloader::Version> deviceBootloaderVersion(deviceBootloader, "Version", DOC(dai, DeviceBootloader, Version));
+    py::enum_<DeviceBootloader::Type> deviceBootloaderType(deviceBootloader, "Type");
+    py::enum_<DeviceBootloader::Memory> deviceBootloaderMemory(deviceBootloader, "Memory");
+    py::enum_<DeviceBootloader::Section> deviceBootloaderSection(deviceBootloader, "Section");
+
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
 
-    py::class_<DeviceBootloader::Version>(deviceBootloader, "Version", DOC(dai, DeviceBootloader, Version))
+    // Bind DeviceBootloader
+    deviceBootloaderVersion
         .def(py::init<const std::string&>(), py::arg("v"), DOC(dai, DeviceBootloader, Version, Version))
         .def(py::init<unsigned, unsigned, unsigned>(), py::arg("major"), py::arg("minor"), py::arg("patch"), DOC(dai, DeviceBootloader, Version, Version, 2))
         .def("__str__", &DeviceBootloader::Version::toString)
         .def("__eq__", &DeviceBootloader::Version::operator==)
         .def("__lt__", &DeviceBootloader::Version::operator<)
         .def("__gt__", &DeviceBootloader::Version::operator>)
         ;
 
-    py::enum_<DeviceBootloader::Type>(deviceBootloader, "Type")
+    deviceBootloaderType
         .value("USB", DeviceBootloader::Type::USB)
         .value("NETWORK", DeviceBootloader::Type::NETWORK)
         ;
-    py::enum_<DeviceBootloader::Memory>(deviceBootloader, "Memory")
+    deviceBootloaderMemory
         .value("FLASH", DeviceBootloader::Memory::FLASH)
         .value("EMMC", DeviceBootloader::Memory::EMMC)
         ;
-    py::enum_<DeviceBootloader::Section>(deviceBootloader, "Section")
+    deviceBootloaderSection
         .value("HEADER", DeviceBootloader::Section::HEADER)
         .value("BOOTLOADER", DeviceBootloader::Section::BOOTLOADER)
         .value("BOOTLOADER_CONFIG", DeviceBootloader::Section::BOOTLOADER_CONFIG)
         .value("APPLICATION", DeviceBootloader::Section::APPLICATION)
         ;
 
     deviceBootloader
@@ -45,17 +64,18 @@
         .def_static("saveDepthaiApplicationPackage", &DeviceBootloader::saveDepthaiApplicationPackage, py::arg("path"), py::arg("pipeline"), py::arg("pathToCmd") = "", DOC(dai, DeviceBootloader, saveDepthaiApplicationPackage))
         .def_static("createDepthaiApplicationPackage", &DeviceBootloader::createDepthaiApplicationPackage, py::arg("pipeline"), py::arg("pathToCmd") = "", DOC(dai, DeviceBootloader, createDepthaiApplicationPackage))
         .def_static("getEmbeddedBootloaderVersion", &DeviceBootloader::getEmbeddedBootloaderVersion, DOC(dai, DeviceBootloader, getEmbeddedBootloaderVersion))
         .def_static("getEmbeddedBootloaderBinary", &DeviceBootloader::getEmbeddedBootloaderBinary, DOC(dai, DeviceBootloader, getEmbeddedBootloaderBinary))
 
         .def(py::init<const DeviceInfo&>(), py::arg("deviceDesc"), DOC(dai, DeviceBootloader, DeviceBootloader))
         .def(py::init<const DeviceInfo&, std::string>(), py::arg("deviceDesc"), py::arg("pathToCmd"), DOC(dai, DeviceBootloader, DeviceBootloader, 2))
-        .def("flash", &DeviceBootloader::flash, py::arg("progressCallback"), py::arg("pipeline"), DOC(dai, DeviceBootloader, flash))
-        .def("flashDepthaiApplicationPackage", &DeviceBootloader::flashDepthaiApplicationPackage, py::arg("progressCallback"), py::arg("package"), DOC(dai, DeviceBootloader, flashDepthaiApplicationPackage))
-        .def("flashBootloader", py::overload_cast<std::function<void(float)>, std::string>(&DeviceBootloader::flashBootloader), py::arg("progressCallback"), py::arg("path") = "", DOC(dai, DeviceBootloader, flashBootloader))
-        .def("flashBootloader", py::overload_cast<DeviceBootloader::Memory, DeviceBootloader::Type, std::function<void(float)>, std::string>(&DeviceBootloader::flashBootloader), py::arg("memory"), py::arg("type"), py::arg("progressCallback"), py::arg("path") = "", DOC(dai, DeviceBootloader, flashBootloader, 2))
+        .def("flash", [](DeviceBootloader& db, std::function<void(float)> progressCallback, Pipeline& pipeline) { py::gil_scoped_release release; return db.flash(progressCallback, pipeline); }, py::arg("progressCallback"), py::arg("pipeline"), DOC(dai, DeviceBootloader, flash))
+        .def("flashDepthaiApplicationPackage", [](DeviceBootloader& db, std::function<void(float)> progressCallback, std::vector<uint8_t> package) { py::gil_scoped_release release; return db.flashDepthaiApplicationPackage(progressCallback, package); }, py::arg("progressCallback"), py::arg("package"), DOC(dai, DeviceBootloader, flashDepthaiApplicationPackage))
+        .def("flashBootloader", [](DeviceBootloader& db, std::function<void(float)> progressCallback, std::string path) { py::gil_scoped_release release; return db.flashBootloader(progressCallback, path); }, py::arg("progressCallback"), py::arg("path") = "", DOC(dai, DeviceBootloader, flashBootloader))
+        .def("flashBootloader", [](DeviceBootloader& db, DeviceBootloader::Memory memory, DeviceBootloader::Type type, std::function<void(float)> progressCallback, std::string path) { py::gil_scoped_release release; return db.flashBootloader(memory, type, progressCallback, path); }, py::arg("memory"), py::arg("type"), py::arg("progressCallback"), py::arg("path") = "", DOC(dai, DeviceBootloader, flashBootloader, 2))
         //.def("flashCustom", &DeviceBootloader::flashCustom, py::arg("memory"), py::arg("offset"), py::arg("progressCallback"), py::arg("data"), DOC(dai, DeviceBootloader, flashCustom))
-        .def("getVersion", &DeviceBootloader::getVersion, DOC(dai, DeviceBootloader, getVersion))
+        .def("getVersion", [](DeviceBootloader& db) { py::gil_scoped_release release; return db.getVersion(); }, DOC(dai, DeviceBootloader, getVersion))
+
         .def("isEmbeddedVersion", &DeviceBootloader::isEmbeddedVersion, DOC(dai, DeviceBootloader, isEmbeddedVersion))
         ;
 
 }
```

### Comparing `depthai-2.8.0.0/src/device_bindings.cpp` & `depthai-2.9.0.0/src/device_bindings.cpp`

 * *Files identical despite different names*

### Comparing `depthai-2.8.0.0/src/pipeline/CommonBindings.cpp` & `depthai-2.9.0.0/src/pipeline/CommonBindings.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -3,146 +3,185 @@
 // depthai-shared
 #include "depthai-shared/common/CameraBoardSocket.hpp"
 #include "depthai-shared/common/EepromData.hpp"
 #include "depthai-shared/common/CameraImageOrientation.hpp"
 #include "depthai-shared/common/MemoryInfo.hpp"
 #include "depthai-shared/common/ChipTemperature.hpp"
 #include "depthai-shared/common/CpuUsage.hpp"
+#include "depthai-shared/common/ProcessorType.hpp"
 #include "depthai-shared/common/Timestamp.hpp"
 #include "depthai-shared/common/Point2f.hpp"
 #include "depthai-shared/common/Point3f.hpp"
 #include "depthai-shared/common/Size2f.hpp"
 #include "depthai-shared/common/UsbSpeed.hpp"
 
-void CommonBindings::bind(pybind11::module& m){
+void CommonBindings::bind(pybind11::module& m, void* pCallstack){
 
     using namespace dai;
 
-    py::class_<Timestamp>(m, "Timestamp", DOC(dai, Timestamp))
+    py::class_<Timestamp> timestamp(m, "Timestamp", DOC(dai, Timestamp));
+    py::class_<Point2f> point2f(m, "Point2f", DOC(dai, Point2f));
+    py::class_<Point3f> point3f(m, "Point3f", DOC(dai, Point3f));
+    py::class_<Size2f> size2f(m, "Size2f", DOC(dai, Size2f));
+    py::enum_<CameraBoardSocket> cameraBoardSocket(m, "CameraBoardSocket", DOC(dai, CameraBoardSocket));
+    py::enum_<CameraImageOrientation> cameraImageOrientation(m, "CameraImageOrientation", DOC(dai, CameraImageOrientation));
+    py::class_<MemoryInfo> memoryInfo(m, "MemoryInfo", DOC(dai, MemoryInfo));
+    py::class_<ChipTemperature> chipTemperature(m, "ChipTemperature", DOC(dai, ChipTemperature));
+    py::class_<CpuUsage> cpuUsage(m, "CpuUsage", DOC(dai, CpuUsage));
+    py::enum_<CameraModel> cameraModel(m, "CameraModel", DOC(dai, CameraModel));
+    py::class_<StereoRectification> stereoRectification(m, "StereoRectification", DOC(dai, StereoRectification));
+    py::class_<Extrinsics> extrinsics(m, "Extrinsics", DOC(dai, Extrinsics));
+    py::class_<CameraInfo> cameraInfo(m, "CameraInfo", DOC(dai, CameraInfo));
+    py::class_<EepromData> eepromData(m, "EepromData", DOC(dai, EepromData));
+    py::enum_<UsbSpeed> usbSpeed(m, "UsbSpeed", DOC(dai, UsbSpeed));
+    py::enum_<ProcessorType> processorType(m, "ProcessorType");
+
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    // Actual bindings
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
+
+    timestamp
         .def(py::init<>())
         .def_readwrite("sec", &Timestamp::sec)
         .def_readwrite("nsec", &Timestamp::nsec)
         .def("get", &Timestamp::get)
         ;
 
-    py::class_<Point2f>(m, "Point2f", DOC(dai, Point2f))
+    point2f
         .def(py::init<>())
         .def(py::init<float, float>())
         .def_readwrite("x", &Point2f::x)
         .def_readwrite("y", &Point2f::y)
         ;
 
-    py::class_<Point3f>(m, "Point3f", DOC(dai, Point3f))
+    point3f
         .def(py::init<>())
         .def(py::init<float, float, float>())
         .def_readwrite("x", &Point3f::x)
         .def_readwrite("y", &Point3f::y)
         .def_readwrite("z", &Point3f::z)
         ;
 
-    py::class_<Size2f>(m, "Size2f", DOC(dai, Size2f))
+    size2f
         .def(py::init<>())
         .def(py::init<float, float>())
         .def_readwrite("width", &Size2f::width)
         .def_readwrite("height", &Size2f::height)
         ;
 
     // CameraBoardSocket enum bindings
-    py::enum_<CameraBoardSocket>(m, "CameraBoardSocket", DOC(dai, CameraBoardSocket))
+    cameraBoardSocket
         .value("AUTO", CameraBoardSocket::AUTO)
         .value("RGB", CameraBoardSocket::RGB)
         .value("LEFT", CameraBoardSocket::LEFT)
         .value("RIGHT", CameraBoardSocket::RIGHT)
     ;
 
     // CameraImageOrientation enum bindings
-    py::enum_<CameraImageOrientation>(m, "CameraImageOrientation", DOC(dai, CameraImageOrientation))
+    cameraImageOrientation
         .value("AUTO", CameraImageOrientation::AUTO)
         .value("NORMAL", CameraImageOrientation::NORMAL)
         .value("HORIZONTAL_MIRROR", CameraImageOrientation::HORIZONTAL_MIRROR)
         .value("VERTICAL_FLIP", CameraImageOrientation::VERTICAL_FLIP)
         .value("ROTATE_180_DEG", CameraImageOrientation::ROTATE_180_DEG)
     ;
 
     // MemoryInfo
-    py::class_<MemoryInfo>(m, "MemoryInfo", DOC(dai, MemoryInfo))
+    memoryInfo
         .def(py::init<>())
         .def_readwrite("remaining", &MemoryInfo::remaining)
         .def_readwrite("used", &MemoryInfo::used)
         .def_readwrite("total", &MemoryInfo::total)
     ;
 
     // ChipTemperature
-    py::class_<ChipTemperature>(m, "ChipTemperature", DOC(dai, ChipTemperature))
+    chipTemperature
         .def(py::init<>())
         .def_readwrite("css", &ChipTemperature::css)
         .def_readwrite("mss", &ChipTemperature::mss)
         .def_readwrite("upa", &ChipTemperature::upa)
         .def_readwrite("dss", &ChipTemperature::dss)
         .def_readwrite("average", &ChipTemperature::average)
     ;
 
     // CpuUsage
-    py::class_<CpuUsage>(m, "CpuUsage", DOC(dai, CpuUsage))
+    cpuUsage
         .def(py::init<>())
         .def_readwrite("average", &CpuUsage::average)
         .def_readwrite("msTime", &CpuUsage::msTime)
     ;
     // CameraModel enum bindings
-    py::enum_<CameraModel>(m, "CameraModel", DOC(dai, CameraModel))
+    cameraModel
         .value("Perspective", CameraModel::Perspective)
         .value("Fisheye", CameraModel::Fisheye)
         .value("Equirectangular", CameraModel::Equirectangular)
         .value("RadialDivision", CameraModel::RadialDivision)
     ;
 
     // StereoRectification
-    py::class_<StereoRectification> (m, "StereoRectification", DOC(dai, StereoRectification))
+    stereoRectification
         .def(py::init<>())
         .def_readwrite("rectifiedRotationLeft", &StereoRectification::rectifiedRotationLeft)
         .def_readwrite("rectifiedRotationRight", &StereoRectification::rectifiedRotationRight)
         .def_readwrite("leftCameraSocket", &StereoRectification::leftCameraSocket)
         .def_readwrite("rightCameraSocket", &StereoRectification::rightCameraSocket)
         ;
 
     // Extrinsics
-    py::class_<Extrinsics> (m, "Extrinsics", DOC(dai, Extrinsics))
+    extrinsics
         .def(py::init<>())
         .def_readwrite("rotationMatrix", &Extrinsics::rotationMatrix)
         .def_readwrite("translation", &Extrinsics::translation)
         .def_readwrite("specTranslation", &Extrinsics::specTranslation)
         .def_readwrite("toCameraSocket", &Extrinsics::toCameraSocket)
         ;
 
     // CameraInfo
-    py::class_<CameraInfo> (m, "CameraInfo", DOC(dai, CameraInfo))
+    cameraInfo
         .def(py::init<>())
         .def_readwrite("width", &CameraInfo::width)
         .def_readwrite("height", &CameraInfo::height)
         .def_readwrite("intrinsicMatrix", &CameraInfo::intrinsicMatrix)
         .def_readwrite("distortionCoeff", &CameraInfo::distortionCoeff)
         .def_readwrite("extrinsics", &CameraInfo::extrinsics)
         .def_readwrite("cameraType", &CameraInfo::cameraType)
         .def_readwrite("specHfovDeg", &CameraInfo::specHfovDeg)
         ;
 
     // EepromData
-    py::class_<EepromData> (m, "EepromData", DOC(dai, EepromData))
+    eepromData
         .def(py::init<>())
         .def_readwrite("version", &EepromData::version)
         .def_readwrite("boardName", &EepromData::boardName)
         .def_readwrite("boardRev", &EepromData::boardRev)
         .def_readwrite("cameraData", &EepromData::cameraData)
         .def_readwrite("stereoRectificationData", &EepromData::stereoRectificationData)
         .def_readwrite("imuExtrinsics", &EepromData::imuExtrinsics)
         ;
     // UsbSpeed
-    py::enum_<UsbSpeed>(m, "UsbSpeed", DOC(dai, UsbSpeed))
+    usbSpeed
         .value("UNKNOWN", UsbSpeed::UNKNOWN)
         .value("LOW", UsbSpeed::LOW)
         .value("FULL", UsbSpeed::FULL)
         .value("HIGH", UsbSpeed::HIGH)
         .value("SUPER", UsbSpeed::SUPER)
         .value("SUPER_PLUS", UsbSpeed::SUPER_PLUS)
     ;
 
+    // ProcessorType
+    processorType
+        .value("LEON_CSS", ProcessorType::LEON_CSS)
+        .value("LEON_MSS", ProcessorType::LEON_MSS)
+    ;
+
 }
```

### Comparing `depthai-2.8.0.0/src/pipeline/NodeBindings.cpp` & `depthai-2.9.0.0/src/pipeline/NodeBindings.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,129 +1,564 @@
 #include "NodeBindings.hpp"
 
+#include "depthai/pipeline/Pipeline.hpp"
 #include "depthai/pipeline/Node.hpp"
 #include "depthai/pipeline/Pipeline.hpp"
 #include "depthai/pipeline/node/XLinkIn.hpp"
 #include "depthai/pipeline/node/XLinkOut.hpp"
 #include "depthai/pipeline/node/ColorCamera.hpp"
 #include "depthai/pipeline/node/MonoCamera.hpp"
 #include "depthai/pipeline/node/StereoDepth.hpp"
 #include "depthai/pipeline/node/NeuralNetwork.hpp"
 #include "depthai/pipeline/node/VideoEncoder.hpp"
 #include "depthai/pipeline/node/ImageManip.hpp"
 #include "depthai/pipeline/node/SPIOut.hpp"
+#include "depthai/pipeline/node/SPIIn.hpp"
 #include "depthai/pipeline/node/DetectionNetwork.hpp"
 #include "depthai/pipeline/node/SystemLogger.hpp"
+#include "depthai/pipeline/node/Script.hpp"
 #include "depthai/pipeline/node/SpatialLocationCalculator.hpp"
 #include "depthai/pipeline/node/SpatialDetectionNetwork.hpp"
 #include "depthai/pipeline/node/ObjectTracker.hpp"
 #include "depthai/pipeline/node/IMU.hpp"
 #include "depthai/pipeline/node/EdgeDetector.hpp"
 
 // Libraries
 #include "hedley/hedley.h"
 
-void NodeBindings::bind(pybind11::module& m){
+// pybind11
+#include "pybind11/stl_bind.h"
+
+// Map of python node classes and call to pipeline to create it
+std::vector<std::pair<py::handle, std::function<std::shared_ptr<dai::Node>(dai::Pipeline&, py::object class_)>>> pyNodeCreateMap;
+
+py::handle daiNodeModule;
+
+template<typename T, typename DERIVED = dai::Node>
+py::class_<T> addNode(const char* name, const char* docstring = nullptr){
+    auto node = py::class_<T, DERIVED, std::shared_ptr<T>>(daiNodeModule, name, docstring);
+    pyNodeCreateMap.push_back(std::make_pair(node, [](dai::Pipeline& p, py::object class_){
+        return p.create<T>();
+    }));
+    return node;
+}
+
+template<typename T, typename DERIVED = dai::Node>
+py::class_<T> addNodeAbstract(const char* name, const char* docstring = nullptr){
+    auto node = py::class_<T, DERIVED, std::shared_ptr<T>>(daiNodeModule, name, docstring);
+    pyNodeCreateMap.push_back(std::make_pair(node, [](dai::Pipeline& p, py::object class_) -> std::shared_ptr<dai::Node> {
+        throw std::invalid_argument(std::string(py::str(class_)) + " is an abstract node. Choose an appropriate derived node instead");
+        return nullptr;
+    }));
+    return node;
+}
+
+std::vector<std::pair<py::handle, std::function<std::shared_ptr<dai::Node>(dai::Pipeline&, py::object class_)>>> NodeBindings::getNodeCreateMap(){
+    return pyNodeCreateMap;
+}
+
+// Macro helpers
+#define ADD_NODE(NodeName) addNode<NodeName>(#NodeName, DOC(dai, node, NodeName))
+#define ADD_NODE_DERIVED(NodeName, Derived) addNode<NodeName, Derived>(#NodeName, DOC(dai, node, NodeName))
+#define ADD_NODE_ABSTRACT(NodeName) addNodeAbstract<NodeName>(#NodeName, DOC(dai, node, NodeName))
+#define ADD_NODE_DERIVED_ABSTRACT(NodeName, Derived) addNodeAbstract<NodeName, Derived>(#NodeName, DOC(dai, node, NodeName))
+#define ADD_NODE_DOC(NodeName, docstring) addNode<NodeName>(#NodeName, docstring)
+#define ADD_NODE_DERIVED_DOC(NodeName, Derived, docstring) addNode<NodeName, Derived>(#NodeName, docstring)
+
+
+// Bind map - without init method
+template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
+py::class_<Map, holder_type> bindNodeMap(py::handle scope, const std::string &name, Args&&... args) {
+    using namespace py;
+    using KeyType = typename Map::key_type;
+    using MappedType = typename Map::mapped_type;
+    using Class_ = class_<Map, holder_type>;
+
+    // If either type is a non-module-local bound type then make the map binding non-local as well;
+    // otherwise (e.g. both types are either module-local or converting) the map will be
+    // module-local.
+    auto tinfo = py::detail::get_type_info(typeid(MappedType));
+    bool local = !tinfo || tinfo->module_local;
+    if (local) {
+        tinfo = py::detail::get_type_info(typeid(KeyType));
+        local = !tinfo || tinfo->module_local;
+    }
+
+    Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
+
+    // Register stream insertion operator (if possible)
+    detail::map_if_insertion_operator<Map, Class_>(cl, name);
+
+    cl.def("__bool__",
+        [](const Map &m) -> bool { return !m.empty(); },
+        "Check whether the map is nonempty"
+    );
+
+    cl.def("__iter__",
+           [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
+           keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
+    );
+
+    cl.def("items",
+           [](Map &m) { return make_iterator(m.begin(), m.end()); },
+           keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
+    );
+
+    // Modified __getitem__. Uses operator[] underneath
+    cl.def("__getitem__",
+        [](Map &m, const KeyType &k) -> MappedType & {
+            return m[k];
+        },
+        return_value_policy::reference_internal // ref + keepalive
+    );
+
+    cl.def("__contains__",
+        [](Map &m, const KeyType &k) -> bool {
+            auto it = m.find(k);
+            if (it == m.end())
+              return false;
+           return true;
+        }
+    );
+
+    // Assignment provided only if the type is copyable
+    detail::map_assignment<Map, Class_>(cl);
+
+    cl.def("__delitem__",
+           [](Map &m, const KeyType &k) {
+               auto it = m.find(k);
+               if (it == m.end())
+                   throw key_error();
+               m.erase(it);
+           }
+    );
+
+    cl.def("__len__", &Map::size);
+
+    return cl;
+}
+
+
+void NodeBindings::bind(pybind11::module& m, void* pCallstack){
 
     using namespace dai;
+    //// Bindings for actual nodes
+    // Create "namespace" (python submodule) for nodes
     using namespace dai::node;
+    // Move properties into nodes and nodes under 'node' submodule
+    daiNodeModule = m.def_submodule("node");
 
-
-    // Base 'Node' class binding
+    // Properties
+    py::class_<ColorCameraProperties> colorCameraProperties(m, "ColorCameraProperties", DOC(dai, ColorCameraProperties));
+    py::enum_<ColorCameraProperties::SensorResolution> colorCameraPropertiesSensorResolution(colorCameraProperties, "SensorResolution", DOC(dai, ColorCameraProperties, SensorResolution));
+    py::enum_<ColorCameraProperties::ColorOrder> colorCameraPropertiesColorOrder(colorCameraProperties, "ColorOrder", DOC(dai, ColorCameraProperties, ColorOrder));
+    py::class_<MonoCameraProperties> monoCameraProperties(m, "MonoCameraProperties", DOC(dai, MonoCameraProperties));
+    py::enum_<MonoCameraProperties::SensorResolution> monoCameraPropertiesSensorResolution(monoCameraProperties, "SensorResolution", DOC(dai, MonoCameraProperties, SensorResolution));
+    py::class_<StereoDepthProperties> stereoDepthProperties(m, "StereoDepthProperties", DOC(dai, StereoDepthProperties));
+    py::enum_<MedianFilter> medianFilter(m, "MedianFilter", DOC(dai, MedianFilter));
+    py::class_<StereoDepthConfigData> stereoDepthConfigData(m, "StereoDepthConfigData", DOC(dai, StereoDepthConfigData));
+    py::class_<VideoEncoderProperties> videoEncoderProperties(m, "VideoEncoderProperties", DOC(dai, VideoEncoderProperties));
+    py::enum_<VideoEncoderProperties::Profile> videoEncoderPropertiesProfile(videoEncoderProperties, "Profile", DOC(dai, VideoEncoderProperties, Profile));
+    py::enum_<VideoEncoderProperties::RateControlMode> videoEncoderPropertiesProfileRateControlMode(videoEncoderProperties, "RateControlMode", DOC(dai, VideoEncoderProperties, RateControlMode));
+    py::class_<SystemLoggerProperties> systemLoggerProperties(m, "SystemLoggerProperties", DOC(dai, SystemLoggerProperties));
+    py::class_<NeuralNetworkProperties, std::shared_ptr<NeuralNetworkProperties>> neuralNetworkProperties(m, "NeuralNetworkProperties", DOC(dai, NeuralNetworkProperties));
+    py::class_<DetectionNetworkProperties, NeuralNetworkProperties, std::shared_ptr<DetectionNetworkProperties>> detectionNetworkProperties(m, "DetectionNetworkProperties", DOC(dai, DetectionNetworkProperties));
+    py::class_<SpatialDetectionNetworkProperties, DetectionNetworkProperties, std::shared_ptr<SpatialDetectionNetworkProperties>> spatialDetectionNetworkProperties(m, "SpatialDetectionNetworkProperties", DOC(dai, SpatialDetectionNetworkProperties));
+    py::class_<SpatialLocationCalculatorProperties> spatialLocationCalculatorProperties(m, "SpatialLocationCalculatorProperties", DOC(dai, SpatialLocationCalculatorProperties));
+    py::enum_<TrackerType> trackerType(m, "TrackerType");
+    py::enum_<TrackerIdAssigmentPolicy> trackerIdAssigmentPolicy(m, "TrackerIdAssigmentPolicy");
+    py::class_<ObjectTrackerProperties, std::shared_ptr<ObjectTrackerProperties>> objectTrackerProperties(m, "ObjectTrackerProperties", DOC(dai, ObjectTrackerProperties));
+    py::enum_<IMUSensor> imuSensor(m, "IMUSensor", DOC(dai, IMUSensor));
+    py::class_<IMUSensorConfig, std::shared_ptr<IMUSensorConfig>> imuSensorConfig(m, "IMUSensorConfig", DOC(dai, IMUSensorConfig));
+    py::class_<IMUProperties> imuProperties(m, "IMUProperties", DOC(dai, IMUProperties));
+    py::class_<EdgeDetectorProperties> edgeDetectorProperties(m, "EdgeDetectorProperties", DOC(dai, EdgeDetectorProperties));
+    py::class_<SPIOutProperties> spiOutProperties(m, "SPIOutProperties", DOC(dai, SPIOutProperties));
+    py::class_<SPIInProperties> spiInProperties(m, "SPIInProperties", DOC(dai, SPIInProperties));
     py::class_<Node, std::shared_ptr<Node>> pyNode(m, "Node", DOC(dai, Node));
+    py::class_<Node::Input> pyInput(pyNode, "Input", DOC(dai, Node, Input));
+    py::enum_<Node::Input::Type> nodeInputType(pyInput, "Type");
+    py::class_<Node::Output> pyOutput(pyNode, "Output", DOC(dai, Node, Output));
+    py::enum_<Node::Output::Type> nodeOutputType(pyOutput, "Type");
+    py::class_<ScriptProperties> scriptProperties(m, "ScriptProperties", DOC(dai, ScriptProperties));
+
+
+    // Node::Id bindings
+    py::class_<Node::Id>(pyNode, "Id", "Node identificator. Unique for every node on a single Pipeline");
+    // Node::Connection bindings
+    py::class_<Node::Connection> nodeConnection(pyNode, "Connection", DOC(dai, Node, Connection));
+    // Node::InputMap bindings
+    bindNodeMap<Node::InputMap>(pyNode, "InputMap");
+    // Node::OutputMap bindings
+    bindNodeMap<Node::OutputMap>(pyNode, "OutputMap");
+    auto xlinkIn = ADD_NODE(XLinkIn);
+    auto xlinkOut = ADD_NODE(XLinkOut);
+    auto colorCamera = ADD_NODE(ColorCamera);
+    auto neuralNetwork = ADD_NODE(NeuralNetwork);
+    auto imageManip = ADD_NODE(ImageManip);
+    auto monoCamera = ADD_NODE(MonoCamera);
+    auto stereoDepth = ADD_NODE(StereoDepth);
+    auto videoEncoder = ADD_NODE(VideoEncoder);
+    auto spiOut = ADD_NODE(SPIOut);
+    auto spiIn = ADD_NODE(SPIIn);
+    auto detectionNetwork = ADD_NODE_DERIVED_ABSTRACT(DetectionNetwork, NeuralNetwork);
+    auto mobileNetDetectionNetwork = ADD_NODE_DERIVED(MobileNetDetectionNetwork, DetectionNetwork);
+    auto yoloDetectionNetwork = ADD_NODE_DERIVED(YoloDetectionNetwork, DetectionNetwork);
+    auto spatialDetectionNetwork = ADD_NODE_DERIVED_ABSTRACT(SpatialDetectionNetwork, DetectionNetwork);
+    auto mobileNetSpatialDetectionNetwork = ADD_NODE_DERIVED(MobileNetSpatialDetectionNetwork, SpatialDetectionNetwork);
+    auto yoloSpatialDetectionNetwork = ADD_NODE_DERIVED(YoloSpatialDetectionNetwork, SpatialDetectionNetwork);
+    auto spatialLocationCalculator = ADD_NODE(SpatialLocationCalculator);
+    auto systemLogger = ADD_NODE(SystemLogger);
+    auto objectTracker = ADD_NODE(ObjectTracker);
+    auto script = ADD_NODE(Script);
+    auto imu = ADD_NODE(IMU);
+    auto edgeDetector = ADD_NODE(EdgeDetector);
+
+
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    // Actual bindings
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
+
+
+    colorCameraPropertiesSensorResolution
+        .value("THE_1080_P", ColorCameraProperties::SensorResolution::THE_1080_P)
+        .value("THE_4_K", ColorCameraProperties::SensorResolution::THE_4_K)
+        .value("THE_12_MP", ColorCameraProperties::SensorResolution::THE_12_MP)
+        ;
 
+    colorCameraPropertiesColorOrder
+        .value("BGR", ColorCameraProperties::ColorOrder::BGR)
+        .value("RGB", ColorCameraProperties::ColorOrder::RGB)
+        ;
+
+    colorCameraProperties
+        .def_readwrite("initialControl", &ColorCameraProperties::initialControl)
+        .def_readwrite("boardSocket", &ColorCameraProperties::boardSocket)
+        .def_readwrite("colorOrder", &ColorCameraProperties::colorOrder)
+        .def_readwrite("interleaved", &ColorCameraProperties::interleaved)
+        .def_readwrite("previewHeight", &ColorCameraProperties::previewHeight)
+        .def_readwrite("previewWidth", &ColorCameraProperties::previewWidth)
+        .def_readwrite("videoHeight", &ColorCameraProperties::videoHeight)
+        .def_readwrite("videoWidth", &ColorCameraProperties::videoWidth)
+        .def_readwrite("stillHeight", &ColorCameraProperties::stillHeight)
+        .def_readwrite("stillWidth", &ColorCameraProperties::stillWidth)
+        .def_readwrite("resolution", &ColorCameraProperties::resolution)
+        .def_readwrite("fps", &ColorCameraProperties::fps)
+        .def_readwrite("sensorCropX", &ColorCameraProperties::sensorCropX)
+        .def_readwrite("sensorCropY", &ColorCameraProperties::sensorCropY)
+    ;
+
+
+
+    // MonoCamera props
+
+    monoCameraPropertiesSensorResolution
+        .value("THE_720_P", MonoCameraProperties::SensorResolution::THE_720_P)
+        .value("THE_800_P", MonoCameraProperties::SensorResolution::THE_800_P)
+        .value("THE_400_P", MonoCameraProperties::SensorResolution::THE_400_P)
+        ;
+
+    monoCameraProperties
+        .def_readwrite("initialControl", &MonoCameraProperties::initialControl)
+        .def_readwrite("boardSocket", &MonoCameraProperties::boardSocket)
+        .def_readwrite("resolution", &MonoCameraProperties::resolution)
+        .def_readwrite("fps",  &MonoCameraProperties::fps)
+    ;
+
+
+    // StereoDepth props
+
+    // MedianFilter
+    medianFilter
+        .value("MEDIAN_OFF", MedianFilter::MEDIAN_OFF)
+        .value("KERNEL_3x3", MedianFilter::KERNEL_3x3)
+        .value("KERNEL_5x5", MedianFilter::KERNEL_5x5)
+        .value("KERNEL_7x7", MedianFilter::KERNEL_7x7)
+        ;
+
+    stereoDepthProperties
+        .def_readwrite("calibration",             &StereoDepthProperties::calibration)
+        .def_readwrite("initialConfig",           &StereoDepthProperties::initialConfig)
+        .def_readwrite("inputConfigSync",         &StereoDepthProperties::inputConfigSync)
+        .def_readwrite("depthAlign",              &StereoDepthProperties::depthAlign)
+        .def_readwrite("depthAlignCamera",        &StereoDepthProperties::depthAlignCamera)
+        .def_readwrite("enableLeftRightCheck",    &StereoDepthProperties::enableLeftRightCheck)
+        .def_readwrite("enableSubpixel",          &StereoDepthProperties::enableSubpixel)
+        .def_readwrite("enableExtendedDisparity", &StereoDepthProperties::enableExtendedDisparity)
+        .def_readwrite("rectifyMirrorFrame",      &StereoDepthProperties::rectifyMirrorFrame)
+        .def_readwrite("rectifyEdgeFillColor",    &StereoDepthProperties::rectifyEdgeFillColor)
+        .def_readwrite("width",                   &StereoDepthProperties::width)
+        .def_readwrite("height",                  &StereoDepthProperties::height)
+        .def_readwrite("outWidth",                &StereoDepthProperties::outWidth, DOC(dai, StereoDepthProperties, outWidth))
+        .def_readwrite("outHeight",               &StereoDepthProperties::outHeight, DOC(dai, StereoDepthProperties, outHeight))
+        .def_readwrite("outKeepAspectRatio",      &StereoDepthProperties::outKeepAspectRatio, DOC(dai, StereoDepthProperties, outKeepAspectRatio))
+        .def_readwrite("mesh",                    &StereoDepthProperties::mesh, DOC(dai, StereoDepthProperties, mesh))
+        ;
+    m.attr("StereoDepthProperties").attr("MedianFilter") = medianFilter;
+
+    stereoDepthConfigData
+        .def(py::init<>())
+        .def_readwrite("median", &StereoDepthConfigData::median,  DOC(dai, StereoDepthConfigData, median))
+        .def_readwrite("confidenceThreshold", &StereoDepthConfigData::confidenceThreshold,  DOC(dai, StereoDepthConfigData, confidenceThreshold))
+        .def_readwrite("bilateralSigmaValue", &StereoDepthConfigData::bilateralSigmaValue,  DOC(dai, StereoDepthConfigData, bilateralSigmaValue))
+        .def_readwrite("leftRightCheckThreshold", &StereoDepthConfigData::leftRightCheckThreshold,  DOC(dai, StereoDepthConfigData, leftRightCheckThreshold))
+        ;
+    m.attr("StereoDepthConfigData").attr("MedianFilter") = medianFilter;
+
+
+    // VideoEncoder props
+
+    videoEncoderPropertiesProfile
+        .value("H264_BASELINE", VideoEncoderProperties::Profile::H264_BASELINE)
+        .value("H264_HIGH", VideoEncoderProperties::Profile::H264_HIGH)
+        .value("H264_MAIN", VideoEncoderProperties::Profile::H264_MAIN)
+        .value("H265_MAIN", VideoEncoderProperties::Profile::H265_MAIN)
+        .value("MJPEG", VideoEncoderProperties::Profile::MJPEG)
+        ;
+
+    videoEncoderPropertiesProfileRateControlMode
+        .value("CBR", VideoEncoderProperties::RateControlMode::CBR)
+        .value("VBR", VideoEncoderProperties::RateControlMode::VBR)
+        ;
+
+    videoEncoderProperties
+        .def_readwrite("bitrate", &VideoEncoderProperties::bitrate)
+        .def_readwrite("keyframeFrequency", &VideoEncoderProperties::keyframeFrequency)
+        .def_readwrite("maxBitrate", &VideoEncoderProperties::maxBitrate)
+        .def_readwrite("numBFrames", &VideoEncoderProperties::numBFrames)
+        .def_readwrite("numFramesPool", &VideoEncoderProperties::numFramesPool)
+        .def_readwrite("profile", &VideoEncoderProperties::profile)
+        .def_readwrite("quality", &VideoEncoderProperties::quality)
+        .def_readwrite("rateCtrlMode", &VideoEncoderProperties::rateCtrlMode)
+        .def_readwrite("width", &VideoEncoderProperties::width)
+        .def_readwrite("height", &VideoEncoderProperties::height)
+        ;
+
+
+    // System logger
+    systemLoggerProperties
+        .def_readwrite("rateHz", &SystemLoggerProperties::rateHz)
+        ;
+
+    neuralNetworkProperties
+        .def_readwrite("blobSize", &NeuralNetworkProperties::blobSize)
+        .def_readwrite("blobUri", &NeuralNetworkProperties::blobUri)
+        .def_readwrite("numFrames", &NeuralNetworkProperties::numFrames)
+        .def_readwrite("numThreads", &NeuralNetworkProperties::numThreads)
+        .def_readwrite("numNCEPerThread", &NeuralNetworkProperties::numNCEPerThread)
+        ;
+
+
+    detectionNetworkProperties
+        .def_readwrite("nnFamily", &DetectionNetworkProperties::nnFamily)
+        .def_readwrite("confidenceThreshold", &DetectionNetworkProperties::confidenceThreshold)
+        .def_readwrite("classes", &DetectionNetworkProperties::classes)
+        .def_readwrite("coordinates", &DetectionNetworkProperties::coordinates)
+        .def_readwrite("anchors", &DetectionNetworkProperties::anchors)
+        .def_readwrite("anchorMasks", &DetectionNetworkProperties::anchorMasks)
+        .def_readwrite("iouThreshold", &DetectionNetworkProperties::iouThreshold)
+        ;
+
+
+    spatialDetectionNetworkProperties
+        .def_readwrite("detectedBBScaleFactor", &SpatialDetectionNetworkProperties::detectedBBScaleFactor)
+        .def_readwrite("depthThresholds", &SpatialDetectionNetworkProperties::depthThresholds)
+        ;
+
+    spatialLocationCalculatorProperties
+        .def_readwrite("roiConfig", &SpatialLocationCalculatorProperties::roiConfig)
+        .def_readwrite("inputConfigSync", &SpatialLocationCalculatorProperties::inputConfigSync)
+        ;
+
+
+    trackerType
+        .value("ZERO_TERM_IMAGELESS", TrackerType::ZERO_TERM_IMAGELESS)
+        .value("ZERO_TERM_COLOR_HISTOGRAM", TrackerType::ZERO_TERM_COLOR_HISTOGRAM)
+    ;
+
+    trackerIdAssigmentPolicy
+        .value("UNIQUE_ID", TrackerIdAssigmentPolicy::UNIQUE_ID)
+        .value("SMALLEST_ID", TrackerIdAssigmentPolicy::SMALLEST_ID)
+    ;
+
+    objectTrackerProperties
+        .def_readwrite("trackerThreshold", &ObjectTrackerProperties::trackerThreshold)
+        .def_readwrite("maxObjectsToTrack", &ObjectTrackerProperties::maxObjectsToTrack)
+        .def_readwrite("detectionLabelsToTrack", &ObjectTrackerProperties::detectionLabelsToTrack)
+        .def_readwrite("trackerType", &ObjectTrackerProperties::trackerType)
+        .def_readwrite("trackerIdAssigmentPolicy", &ObjectTrackerProperties::trackerIdAssigmentPolicy)
+        ;
+
+    // IMU node properties
+    imuSensor
+        .value("ACCELEROMETER_RAW", IMUSensor::ACCELEROMETER_RAW, DOC(dai, IMUSensor, ACCELEROMETER_RAW))
+        .value("ACCELEROMETER", IMUSensor::ACCELEROMETER, DOC(dai, IMUSensor, ACCELEROMETER))
+        .value("LINEAR_ACCELERATION", IMUSensor::LINEAR_ACCELERATION, DOC(dai, IMUSensor, LINEAR_ACCELERATION))
+        .value("GRAVITY", IMUSensor::GRAVITY, DOC(dai, IMUSensor, GRAVITY))
+        .value("GYROSCOPE_RAW", IMUSensor::GYROSCOPE_RAW, DOC(dai, IMUSensor, GYROSCOPE_RAW))
+        .value("GYROSCOPE_CALIBRATED", IMUSensor::GYROSCOPE_CALIBRATED, DOC(dai, IMUSensor, GYROSCOPE_CALIBRATED))
+        .value("GYROSCOPE_UNCALIBRATED", IMUSensor::GYROSCOPE_UNCALIBRATED, DOC(dai, IMUSensor, GYROSCOPE_UNCALIBRATED))
+        .value("MAGNETOMETER_RAW", IMUSensor::MAGNETOMETER_RAW, DOC(dai, IMUSensor, MAGNETOMETER_RAW))
+        .value("MAGNETOMETER_CALIBRATED", IMUSensor::MAGNETOMETER_CALIBRATED, DOC(dai, IMUSensor, MAGNETOMETER_CALIBRATED))
+        .value("MAGNETOMETER_UNCALIBRATED", IMUSensor::MAGNETOMETER_UNCALIBRATED, DOC(dai, IMUSensor, MAGNETOMETER_UNCALIBRATED))
+        .value("ROTATION_VECTOR", IMUSensor::ROTATION_VECTOR, DOC(dai, IMUSensor, ROTATION_VECTOR))
+        .value("GAME_ROTATION_VECTOR", IMUSensor::GAME_ROTATION_VECTOR, DOC(dai, IMUSensor, GAME_ROTATION_VECTOR))
+        .value("GEOMAGNETIC_ROTATION_VECTOR", IMUSensor::GEOMAGNETIC_ROTATION_VECTOR, DOC(dai, IMUSensor, GEOMAGNETIC_ROTATION_VECTOR))
+        .value("ARVR_STABILIZED_ROTATION_VECTOR", IMUSensor::ARVR_STABILIZED_ROTATION_VECTOR, DOC(dai, IMUSensor, ARVR_STABILIZED_ROTATION_VECTOR))
+        .value("ARVR_STABILIZED_GAME_ROTATION_VECTOR", IMUSensor::ARVR_STABILIZED_GAME_ROTATION_VECTOR, DOC(dai, IMUSensor, ARVR_STABILIZED_GAME_ROTATION_VECTOR))
+        // .value("GYRO_INTEGRATED_ROTATION_VECTOR", IMUSensor::GYRO_INTEGRATED_ROTATION_VECTOR)
+    ;
+
+    imuSensorConfig
+        .def(py::init<>())
+        .def_readwrite("sensitivityEnabled", &IMUSensorConfig::sensitivityEnabled)
+        .def_readwrite("sensitivityRelative", &IMUSensorConfig::sensitivityRelative)
+        .def_readwrite("changeSensitivity", &IMUSensorConfig::changeSensitivity)
+        .def_readwrite("reportRate", &IMUSensorConfig::reportRate)
+        .def_readwrite("sensorId", &IMUSensorConfig::sensorId)
+        ;
+
+    imuProperties
+        .def_readwrite("imuSensors", &IMUProperties::imuSensors, DOC(dai, IMUProperties, imuSensors))
+        .def_readwrite("batchReportThreshold", &IMUProperties::batchReportThreshold, DOC(dai, IMUProperties, batchReportThreshold))
+        .def_readwrite("maxBatchReports", &IMUProperties::maxBatchReports, DOC(dai, IMUProperties, maxBatchReports))
+    ;
+
+    // EdgeDetector node properties
+    edgeDetectorProperties
+        .def_readwrite("initialConfig", &EdgeDetectorProperties::initialConfig, DOC(dai, EdgeDetectorProperties, initialConfig))
+        .def_readwrite("inputConfigSync", &EdgeDetectorProperties::inputConfigSync, DOC(dai, EdgeDetectorProperties, inputConfigSync))
+        .def_readwrite("outputFrameSize", &EdgeDetectorProperties::outputFrameSize, DOC(dai, EdgeDetectorProperties, outputFrameSize))
+        .def_readwrite("numFramesPool", &EdgeDetectorProperties::numFramesPool, DOC(dai, EdgeDetectorProperties, numFramesPool))
+    ;
+
+    // SPIOut properties
+    spiOutProperties
+        .def_readwrite("streamName", &SPIOutProperties::streamName)
+        .def_readwrite("busId", &SPIOutProperties::busId)
+    ;
+
+    // SPIIn properties
+    spiInProperties
+        .def_readwrite("streamName", &SPIInProperties::streamName)
+        .def_readwrite("busId", &SPIInProperties::busId)
+        .def_readwrite("maxDataSize", &SPIInProperties::maxDataSize)
+        .def_readwrite("numFrames", &SPIInProperties::numFrames)
+    ;
+
+    // Script properties
+    scriptProperties
+        .def_readwrite("scriptUri", &ScriptProperties::scriptUri, DOC(dai, ScriptProperties, scriptUri))
+        .def_readwrite("scriptName", &ScriptProperties::scriptName, DOC(dai, ScriptProperties, scriptName))
+        .def_readwrite("processor", &ScriptProperties::processor, DOC(dai, ScriptProperties, processor))
+    ;
+
+
+    ////////////////////////////////////////////////////////////////////////////////////////
+    ////////////////////////////////////////////////////////////////////////////////////////
+    // Node Bindings after properties, so types are resolved
+    ////////////////////////////////////////////////////////////////////////////////////////
+    ////////////////////////////////////////////////////////////////////////////////////////
+
+    // Base 'Node' class binding
 
     // Node::Input bindings
-    py::class_<Node::Input> pyInput(pyNode, "Input", DOC(dai, Node, Input));
-    py::enum_<Node::Input::Type>(pyInput, "Type")
+    nodeInputType
         .value("SReceiver", Node::Input::Type::SReceiver)
         .value("MReceiver", Node::Input::Type::MReceiver)
     ;
     pyInput
         .def_property_readonly("name", [](const Node::Input& input){ return input.name; })
         .def_property_readonly("type", [](const Node::Input& input){ return input.type; })
         .def("setBlocking", &Node::Input::setBlocking, py::arg("blocking"), DOC(dai, Node, Input, setBlocking))
         .def("getBlocking", &Node::Input::getBlocking, DOC(dai, Node, Input, getBlocking))
         .def("setQueueSize", &Node::Input::setQueueSize, py::arg("size"), DOC(dai, Node, Input, setQueueSize))
         .def("getQueueSize", &Node::Input::getQueueSize, DOC(dai, Node, Input, getQueueSize))
     ;
 
     // Node::Output bindings
-    py::class_<Node::Output> pyOutput(pyNode, "Output", DOC(dai, Node, Output));
-    py::enum_<Node::Output::Type>(pyOutput, "Type")
+    nodeOutputType
         .value("MSender", Node::Output::Type::MSender)
         .value("SSender", Node::Output::Type::SSender)
     ;
     pyOutput
         .def("canConnect", &Node::Output::canConnect, py::arg("in"), DOC(dai, Node, Output, canConnect))
         .def("link", &Node::Output::link, py::arg("in"), DOC(dai, Node, Output, link))
         .def("unlink", &Node::Output::unlink, py::arg("in"), DOC(dai, Node, Output, unlink))
         .def("getConnections", &Node::Output::getConnections, DOC(dai, Node, Output, getConnections))
     ;
-    // Node::Id bindings
-    py::class_<Node::Id>(pyNode, "Id", "Node identificator. Unique for every node on a single Pipeline");
 
-    // Node::Connection bindings
-    py::class_<Node::Connection>(pyNode, "Connection", DOC(dai, Node, Connection))
+
+    nodeConnection
         .def_property("outputId", [](Node::Connection& conn) { return conn.outputId; }, [](Node::Connection& conn, Node::Id id) {conn.outputId = id; }, DOC(dai, Node, Connection, outputId))
         .def_property("outputName", [](Node::Connection& conn) { return conn.outputName; }, [](Node::Connection& conn, std::string name) {conn.outputName = name; }, DOC(dai, Node, Connection, outputName))
         .def_property("inputId", [](Node::Connection& conn) { return conn.inputId; }, [](Node::Connection& conn, Node::Id id) {conn.inputId = id; }, DOC(dai, Node, Connection, inputId))
         .def_property("inputName", [](Node::Connection& conn) { return conn.inputName; }, [](Node::Connection& conn, std::string name) {conn.inputName = name; }, DOC(dai, Node, Connection, inputName))
     ;
 
     pyNode
         .def_readonly("id", &Node::id, DOC(dai, Node, id))
         .def("getName", &Node::getName, DOC(dai, Node, getName))
         .def("getOutputs", &Node::getOutputs, DOC(dai, Node, getOutputs))
         .def("getInputs", &Node::getInputs, DOC(dai, Node, getInputs))
-        .def("getAssets", &Node::getAssets, DOC(dai, Node, getAssets))
         .def("getOutputRefs", static_cast<std::vector< Node::Output*> (Node::*)()>(&Node::getOutputRefs), DOC(dai, Node, getOutputRefs), py::return_value_policy::reference_internal)
         .def("getInputRefs", static_cast<std::vector<Node::Input*> (Node::*)()>(&Node::getInputRefs), DOC(dai, Node, getInputRefs), py::return_value_policy::reference_internal)
         .def("getOutputRefs", static_cast<std::vector<const Node::Output*> (Node::*)() const>(&Node::getOutputRefs), DOC(dai, Node, getOutputRefs), py::return_value_policy::reference_internal)
         .def("getInputRefs", static_cast<std::vector<const Node::Input*> (Node::*)() const>(&Node::getInputRefs), DOC(dai, Node, getInputRefs), py::return_value_policy::reference_internal)
         .def("getParentPipeline", py::overload_cast<>(&Node::getParentPipeline), DOC(dai, Node, getParentPipeline))
         .def("getParentPipeline", py::overload_cast<>(&Node::getParentPipeline, py::const_), DOC(dai, Node, getParentPipeline))
+        .def("getAssetManager", static_cast<const AssetManager& (Node::*)() const>(&Node::getAssetManager), py::return_value_policy::reference_internal, DOC(dai, Node, getAssetManager))
+        .def("getAssetManager", static_cast<AssetManager& (Node::*)()>(&Node::getAssetManager), py::return_value_policy::reference_internal, DOC(dai, Node, getAssetManager))
     ;
 
     // MSVC errors out with:
     // Error C2326 'void NodeBindings::bind(pybind11::module &)': function cannot access 'dai::Node::Connection::outputId'
     // ...
     // py::class_<Node::Connection>(pyNode, "Connection")
     //     .def_readwrite("outputId", &dai::Node::Connection::outputId)
     //     .def_readwrite("outputName", &dai::Node::Connection::outputName)
     //     .def_readwrite("inputId", &dai::Node::Connection::inputId)
     //     .def_readwrite("inputName", &dai::Node::Connection::inputName)
     // ;
 
-    //// Bindings for actual nodes
 
     // XLinkIn node
-    py::class_<XLinkIn, Node, std::shared_ptr<XLinkIn>>(m, "XLinkIn", DOC(dai, node, XLinkIn))
+    xlinkIn
         .def_readonly("out", &XLinkIn::out, DOC(dai, node, XLinkIn, out))
         .def("setStreamName", &XLinkIn::setStreamName, py::arg("streamName"), DOC(dai, node, XLinkIn, setStreamName))
         .def("setMaxDataSize", &XLinkIn::setMaxDataSize, py::arg("maxDataSize"), DOC(dai, node, XLinkIn, setMaxDataSize))
         .def("setNumFrames",  &XLinkIn::setNumFrames, py::arg("numFrames"), DOC(dai, node, XLinkIn, setNumFrames))
         .def("getStreamName", &XLinkIn::getStreamName, DOC(dai, node, XLinkIn, getStreamName))
         .def("getMaxDataSize", &XLinkIn::getMaxDataSize, DOC(dai, node, XLinkIn, getMaxDataSize))
         .def("getNumFrames",  &XLinkIn::getNumFrames, DOC(dai, node, XLinkIn, getNumFrames))
         ;
 
     // XLinkOut node
-    py::class_<XLinkOut, Node, std::shared_ptr<XLinkOut>>(m, "XLinkOut", DOC(dai, node, XLinkOut))
+    xlinkOut
         .def_readonly("input", &XLinkOut::input, DOC(dai, node, XLinkOut, input))
         .def("setStreamName", &XLinkOut::setStreamName, py::arg("streamName"), DOC(dai, node, XLinkOut, setStreamName))
         .def("setFpsLimit", &XLinkOut::setFpsLimit, py::arg("fpsLimit"), DOC(dai, node, XLinkOut, setFpsLimit))
         .def("getStreamName", &XLinkOut::getStreamName, DOC(dai, node, XLinkOut, getStreamName))
         .def("getFpsLimit", &XLinkOut::getFpsLimit, DOC(dai, node, XLinkOut, getFpsLimit))
         .def("setMetadataOnly", &XLinkOut::setMetadataOnly, DOC(dai, node, XLinkOut, setMetadataOnly))
         .def("getMetadataOnly", &XLinkOut::getMetadataOnly, DOC(dai, node, XLinkOut, getMetadataOnly))
         ;
 
     // ColorCamera node
-    py::class_<ColorCamera, Node, std::shared_ptr<ColorCamera>>(m, "ColorCamera", DOC(dai, node, ColorCamera))
+    colorCamera
         .def_readonly("inputConfig", &ColorCamera::inputConfig, DOC(dai, node, ColorCamera, inputConfig))
         .def_readonly("inputControl", &ColorCamera::inputControl, DOC(dai, node, ColorCamera, inputControl))
         .def_readonly("initialControl", &ColorCamera::initialControl, DOC(dai, node, ColorCamera, initialControl))
         .def_readonly("video", &ColorCamera::video, DOC(dai, node, ColorCamera, video))
         .def_readonly("preview", &ColorCamera::preview, DOC(dai, node, ColorCamera, preview))
         .def_readonly("still", &ColorCamera::still, DOC(dai, node, ColorCamera, still))
         .def_readonly("isp", &ColorCamera::isp, DOC(dai, node, ColorCamera, isp))
@@ -189,32 +624,36 @@
         .def("setIspScale", static_cast<void(ColorCamera::*)(std::tuple<int,int>)>(&ColorCamera::setIspScale), py::arg("scale"), DOC(dai, node, ColorCamera, setIspScale, 2))
         .def("setIspScale", static_cast<void(ColorCamera::*)(int,int,int,int)>(&ColorCamera::setIspScale), py::arg("horizNum"), py::arg("horizDenom"), py::arg("vertNum"), py::arg("vertDenom"), DOC(dai, node, ColorCamera, setIspScale, 3))
         .def("setIspScale", static_cast<void(ColorCamera::*)(std::tuple<int,int>,std::tuple<int,int>)>(&ColorCamera::setIspScale), py::arg("horizScale"), py::arg("vertScale"), DOC(dai, node, ColorCamera, setIspScale, 4))
         .def("getIspSize", &ColorCamera::getIspSize, DOC(dai, node, ColorCamera, getIspSize))
         .def("getIspWidth", &ColorCamera::getIspWidth, DOC(dai, node, ColorCamera, getIspWidth))
         .def("getIspHeight", &ColorCamera::getIspHeight, DOC(dai, node, ColorCamera, getIspHeight))
         ;
+    // ALIAS
+    daiNodeModule.attr("ColorCamera").attr("Properties") = colorCameraProperties;
 
 
 
     // NeuralNetwork node
-    py::class_<NeuralNetwork, Node, std::shared_ptr<NeuralNetwork>>(m, "NeuralNetwork", DOC(dai, node, NeuralNetwork))
+    neuralNetwork
         .def_readonly("input", &NeuralNetwork::input, DOC(dai, node, NeuralNetwork, input))
         .def_readonly("out", &NeuralNetwork::out, DOC(dai, node, NeuralNetwork, out))
         .def_readonly("passthrough", &NeuralNetwork::passthrough, DOC(dai, node, NeuralNetwork, passthrough))
         .def("setBlobPath", &NeuralNetwork::setBlobPath, py::arg("path"), DOC(dai, node, NeuralNetwork, setBlobPath))
         .def("setNumPoolFrames", &NeuralNetwork::setNumPoolFrames, py::arg("numFrames"), DOC(dai, node, NeuralNetwork, setNumPoolFrames))
         .def("setNumInferenceThreads", &NeuralNetwork::setNumInferenceThreads, py::arg("numThreads"), DOC(dai, node, NeuralNetwork, setNumInferenceThreads))
         .def("setNumNCEPerInferenceThread", &NeuralNetwork::setNumNCEPerInferenceThread, py::arg("numNCEPerThread"), DOC(dai, node, NeuralNetwork, setNumNCEPerInferenceThread))
         .def("getNumInferenceThreads", &NeuralNetwork::getNumInferenceThreads, DOC(dai, node, NeuralNetwork, getNumInferenceThreads))
         ;
+    // Properties alias
+    daiNodeModule.attr("NeuralNetwork").attr("Properties") = neuralNetworkProperties;
 
 
     // ImageManip node
-    py::class_<ImageManip, Node, std::shared_ptr<ImageManip>>(m, "ImageManip", DOC(dai, node, ImageManip))
+    imageManip
         .def_readonly("inputConfig", &ImageManip::inputConfig, DOC(dai, node, ImageManip, inputConfig))
         .def_readonly("inputImage", &ImageManip::inputImage, DOC(dai, node, ImageManip, inputImage))
         .def_readonly("out", &ImageManip::out, DOC(dai, node, ImageManip, out))
         .def_readonly("initialConfig", &ImageManip::initialConfig, DOC(dai, node, ImageManip, initialConfig))
         // setters
 
         .def("setCropRect", [](ImageManip& im, float xmin, float ymin, float xmax, float ymax) {
@@ -274,15 +713,15 @@
 
         .def("setWaitForConfigInput", &ImageManip::setWaitForConfigInput, DOC(dai, node, ImageManip, setWaitForConfigInput))
         .def("setNumFramesPool", &ImageManip::setNumFramesPool, DOC(dai, node, ImageManip, setNumFramesPool))
         .def("setMaxOutputFrameSize", &ImageManip::setMaxOutputFrameSize, DOC(dai, node, ImageManip, setMaxOutputFrameSize))
         ;
 
      // MonoCamera node
-    py::class_<MonoCamera, Node, std::shared_ptr<MonoCamera>>(m, "MonoCamera", DOC(dai, node, MonoCamera))
+    monoCamera
         .def_readonly("inputControl", &MonoCamera::inputControl, DOC(dai, node, MonoCamera, inputControl))
         .def_readonly("out",  &MonoCamera::out, DOC(dai, node, MonoCamera, out))
         .def_readonly("raw",  &MonoCamera::raw, DOC(dai, node, MonoCamera, raw))
         .def_readonly("initialControl",  &MonoCamera::initialControl, DOC(dai, node, MonoCamera, initialControl))
         .def("setCamId", [](MonoCamera& c, int64_t id) {
             // Issue an deprecation warning
             PyErr_WarnEx(PyExc_DeprecationWarning, "setCamId() is deprecated, use setBoardSocket() instead.", 1);
@@ -307,19 +746,20 @@
         .def("getResolution", &MonoCamera::getResolution, DOC(dai, node, MonoCamera, getResolution))
         .def("setFps",        &MonoCamera::setFps, py::arg("fps"), DOC(dai, node, MonoCamera, setFps))
         .def("getFps",        &MonoCamera::getFps, DOC(dai, node, MonoCamera, getFps))
         .def("getResolutionSize", &MonoCamera::getResolutionSize, DOC(dai, node, MonoCamera, getResolutionSize))
         .def("getResolutionWidth", &MonoCamera::getResolutionWidth, DOC(dai, node, MonoCamera, getResolutionWidth))
         .def("getResolutionHeight", &MonoCamera::getResolutionHeight, DOC(dai, node, MonoCamera, getResolutionHeight))
         ;
-
+    // ALIAS
+    daiNodeModule.attr("MonoCamera").attr("Properties") = monoCameraProperties;
 
 
     // StereoDepth node
-    py::class_<StereoDepth, Node, std::shared_ptr<StereoDepth>>(m, "StereoDepth", DOC(dai, node, StereoDepth))
+    stereoDepth
         .def_readonly("initialConfig",  &StereoDepth::initialConfig, DOC(dai, node, StereoDepth, initialConfig))
         .def_readonly("inputConfig",    &StereoDepth::inputConfig, DOC(dai, node, StereoDepth, inputConfig))
         .def_readonly("left",           &StereoDepth::left, DOC(dai, node, StereoDepth, left))
         .def_readonly("right",          &StereoDepth::right, DOC(dai, node, StereoDepth, right))
         .def_readonly("depth",          &StereoDepth::depth, DOC(dai, node, StereoDepth, depth))
         .def_readonly("disparity",      &StereoDepth::disparity, DOC(dai, node, StereoDepth, disparity))
         .def_readonly("syncedLeft",     &StereoDepth::syncedLeft, DOC(dai, node, StereoDepth, syncedLeft))
@@ -391,17 +831,19 @@
             HEDLEY_DIAGNOSTIC_PUSH
             HEDLEY_DIAGNOSTIC_DISABLE_DEPRECATED
             s.setEmptyCalibration();
             HEDLEY_DIAGNOSTIC_POP
         }, DOC(dai, node, StereoDepth, setEmptyCalibration))
         .def("getMaxDisparity", &StereoDepth::getMaxDisparity, DOC(dai, node, StereoDepth, getMaxDisparity))
         ;
+    // ALIAS
+    daiNodeModule.attr("StereoDepth").attr("Properties") = stereoDepthProperties;
 
     // VideoEncoder node
-    py::class_<VideoEncoder, Node, std::shared_ptr<VideoEncoder>>(m, "VideoEncoder", DOC(dai, node, VideoEncoder))
+    videoEncoder
         .def_readonly("input", &VideoEncoder::input, DOC(dai, node, VideoEncoder, input), DOC(dai, node, VideoEncoder, input))
         .def_readonly("bitstream", &VideoEncoder::bitstream, DOC(dai, node, VideoEncoder, bitstream), DOC(dai, node, VideoEncoder, bitstream))
         .def("setDefaultProfilePreset", static_cast<void(VideoEncoder::*)(int, int, float, VideoEncoderProperties::Profile)>(&VideoEncoder::setDefaultProfilePreset), py::arg("width"), py::arg("height"), py::arg("fps"), py::arg("profile"), DOC(dai, node, VideoEncoder, setDefaultProfilePreset))
         .def("setDefaultProfilePreset", static_cast<void(VideoEncoder::*)(std::tuple<int,int>, float, VideoEncoderProperties::Profile)>(&VideoEncoder::setDefaultProfilePreset), py::arg("size"), py::arg("fps"), py::arg("profile"), DOC(dai, node, VideoEncoder, setDefaultProfilePreset, 2))
         .def("setNumFramesPool", &VideoEncoder::setNumFramesPool, py::arg("frames"), DOC(dai, node, VideoEncoder, setNumFramesPool))
         .def("getNumFramesPool", &VideoEncoder::getNumFramesPool, DOC(dai, node, VideoEncoder, getNumFramesPool))
         .def("setRateControlMode", &VideoEncoder::setRateControlMode, py::arg("mode"), DOC(dai, node, VideoEncoder, setRateControlMode))
@@ -425,373 +867,164 @@
         .def("getQuality", &VideoEncoder::getQuality, DOC(dai, node, VideoEncoder, getQuality))
         .def("getWidth", &VideoEncoder::getWidth, DOC(dai, node, VideoEncoder, getWidth))
         .def("getHeight", &VideoEncoder::getHeight, DOC(dai, node, VideoEncoder, getHeight))
         .def("getFrameRate", &VideoEncoder::getFrameRate, DOC(dai, node, VideoEncoder, getFrameRate))
         .def("getSize", &VideoEncoder::getSize, DOC(dai, node, VideoEncoder, getSize))
         .def("getLossless", &VideoEncoder::getLossless, DOC(dai, node, VideoEncoder, getLossless))
     ;
+    // ALIAS
+    daiNodeModule.attr("VideoEncoder").attr("Properties") = videoEncoderProperties;
+
 
-    // SPIOut node
-    py::class_<SPIOut, Node, std::shared_ptr<SPIOut>>(m, "SPIOut", DOC(dai, node, SPIOut))
+    spiOut
         .def_readonly("input", &SPIOut::input, DOC(dai, node, SPIOut, input))
         .def("setStreamName", &SPIOut::setStreamName, py::arg("name"), DOC(dai, node, SPIOut, setStreamName))
         .def("setBusId", &SPIOut::setBusId, py::arg("id"), DOC(dai, node, SPIOut, setBusId))
         ;
+    // ALIAS
+    daiNodeModule.attr("SPIOut").attr("Properties") = spiOutProperties;
+
+
+    // SPIIn node
+    spiIn
+        .def_readonly("out", &SPIIn::out, DOC(dai, node, SPIIn, out))
+        .def("setStreamName", &SPIIn::setStreamName, py::arg("name"), DOC(dai, node, SPIIn, setStreamName))
+        .def("setBusId", &SPIIn::setBusId, py::arg("id"), DOC(dai, node, SPIIn, setBusId))
+        .def("setMaxDataSize", &SPIIn::setMaxDataSize, py::arg("maxDataSize"), DOC(dai, node, SPIIn, setMaxDataSize))
+        .def("setNumFrames", &SPIIn::setNumFrames, py::arg("numFrames"), DOC(dai, node, SPIIn, setNumFrames))
+        .def("getStreamName", &SPIIn::getStreamName, DOC(dai, node, SPIIn, getStreamName))
+        .def("getBusId", &SPIIn::getBusId, DOC(dai, node, SPIIn, getBusId))
+        .def("getMaxDataSize", &SPIIn::getMaxDataSize, DOC(dai, node, SPIIn, getMaxDataSize))
+        .def("getNumFrames", &SPIIn::getNumFrames, DOC(dai, node, SPIIn, getNumFrames))
+        ;
+    // ALIAS
+    daiNodeModule.attr("SPIIn").attr("Properties") = spiInProperties;
 
-    py::class_<DetectionNetwork, NeuralNetwork, std::shared_ptr<DetectionNetwork>>(m, "DetectionNetwork", DOC(dai, node, DetectionNetwork))
+    // DetectionNetwork node
+    detectionNetwork
         .def_readonly("input", &DetectionNetwork::input, DOC(dai, node, DetectionNetwork, input))
         .def_readonly("out", &DetectionNetwork::out, DOC(dai, node, DetectionNetwork, out))
         .def_readonly("passthrough", &DetectionNetwork::passthrough, DOC(dai, node, DetectionNetwork, passthrough))
         .def("setConfidenceThreshold", &DetectionNetwork::setConfidenceThreshold, py::arg("thresh"), DOC(dai, node, DetectionNetwork, setConfidenceThreshold))
         ;
+    // ALIAS
+    daiNodeModule.attr("DetectionNetwork").attr("Properties") = detectionNetworkProperties;
+
 
-    // MobileNetDetectionNetwork node
-    py::class_<MobileNetDetectionNetwork, DetectionNetwork, std::shared_ptr<MobileNetDetectionNetwork>>(m, "MobileNetDetectionNetwork", DOC(dai, node, MobileNetDetectionNetwork))
-        ;
 
     // YoloDetectionNetwork node
-    py::class_<YoloDetectionNetwork, DetectionNetwork, std::shared_ptr<YoloDetectionNetwork>>(m, "YoloDetectionNetwork", DOC(dai, node, YoloDetectionNetwork))
+    yoloDetectionNetwork
         .def("setNumClasses", &YoloDetectionNetwork::setNumClasses, py::arg("numClasses"), DOC(dai, node, YoloDetectionNetwork, setNumClasses))
         .def("setCoordinateSize", &YoloDetectionNetwork::setCoordinateSize, py::arg("coordinates"), DOC(dai, node, YoloDetectionNetwork, setCoordinateSize))
         .def("setAnchors", &YoloDetectionNetwork::setAnchors, py::arg("anchors"), DOC(dai, node, YoloDetectionNetwork, setAnchors))
         .def("setAnchorMasks", &YoloDetectionNetwork::setAnchorMasks, py::arg("anchorMasks"), DOC(dai, node, YoloDetectionNetwork, setAnchorMasks))
         .def("setIouThreshold", &YoloDetectionNetwork::setIouThreshold, py::arg("thresh"), DOC(dai, node, YoloDetectionNetwork, setIouThreshold))
         ;
 
-    py::class_<SpatialDetectionNetwork, DetectionNetwork, std::shared_ptr<SpatialDetectionNetwork>>(m, "SpatialDetectionNetwork", DOC(dai, node, SpatialDetectionNetwork))
+    spatialDetectionNetwork
         .def_readonly("input", &SpatialDetectionNetwork::input, DOC(dai, node, SpatialDetectionNetwork, input))
         .def_readonly("inputDepth", &SpatialDetectionNetwork::inputDepth, DOC(dai, node, SpatialDetectionNetwork, inputDepth))
         .def_readonly("out", &SpatialDetectionNetwork::out, DOC(dai, node, SpatialDetectionNetwork, out))
         .def_readonly("boundingBoxMapping", &SpatialDetectionNetwork::boundingBoxMapping, DOC(dai, node, SpatialDetectionNetwork, boundingBoxMapping))
         .def_readonly("passthrough", &SpatialDetectionNetwork::passthrough, DOC(dai, node, SpatialDetectionNetwork, passthrough))
         .def_readonly("passthroughDepth", &SpatialDetectionNetwork::passthroughDepth, DOC(dai, node, SpatialDetectionNetwork, passthroughDepth))
 
         .def("setBoundingBoxScaleFactor", &SpatialDetectionNetwork::setBoundingBoxScaleFactor, py::arg("scaleFactor"), DOC(dai, node, SpatialDetectionNetwork, setBoundingBoxScaleFactor))
         .def("setDepthLowerThreshold", &SpatialDetectionNetwork::setDepthLowerThreshold, py::arg("lowerThreshold"), DOC(dai, node, SpatialDetectionNetwork, setDepthLowerThreshold))
         .def("setDepthUpperThreshold", &SpatialDetectionNetwork::setDepthUpperThreshold, py::arg("upperThreshold"), DOC(dai, node, SpatialDetectionNetwork, setDepthUpperThreshold))
         ;
+     // ALIAS
+    daiNodeModule.attr("SpatialDetectionNetwork").attr("Properties") = spatialDetectionNetworkProperties;
 
-    py::class_<MobileNetSpatialDetectionNetwork, SpatialDetectionNetwork, std::shared_ptr<MobileNetSpatialDetectionNetwork>>(m, "MobileNetSpatialDetectionNetwork", DOC(dai, node, MobileNetSpatialDetectionNetwork))
-        ;
+    // MobileNetSpatialDetectionNetwork
 
     // YoloSpatialDetectionNetwork node
-    py::class_<YoloSpatialDetectionNetwork, SpatialDetectionNetwork, std::shared_ptr<YoloSpatialDetectionNetwork>>(m, "YoloSpatialDetectionNetwork", DOC(dai, node, YoloSpatialDetectionNetwork))
+    yoloSpatialDetectionNetwork
         .def("setNumClasses", &YoloSpatialDetectionNetwork::setNumClasses, py::arg("numClasses"), DOC(dai, node, YoloSpatialDetectionNetwork, setNumClasses))
         .def("setCoordinateSize", &YoloSpatialDetectionNetwork::setCoordinateSize, py::arg("coordinates"), DOC(dai, node, YoloSpatialDetectionNetwork, setCoordinateSize))
         .def("setAnchors", &YoloSpatialDetectionNetwork::setAnchors, py::arg("anchors"), DOC(dai, node, YoloSpatialDetectionNetwork, setAnchors))
         .def("setAnchorMasks", &YoloSpatialDetectionNetwork::setAnchorMasks, py::arg("anchorMasks"), DOC(dai, node, YoloSpatialDetectionNetwork, setAnchorMasks))
         .def("setIouThreshold", &YoloSpatialDetectionNetwork::setIouThreshold, py::arg("thresh"), DOC(dai, node, YoloSpatialDetectionNetwork, setIouThreshold))
         ;
 
     // SpatialLocationCalculator node
-    py::class_<SpatialLocationCalculator, Node, std::shared_ptr<SpatialLocationCalculator>>(m, "SpatialLocationCalculator", DOC(dai, node, SpatialLocationCalculator))
+
+    spatialLocationCalculator
         .def_readonly("inputConfig", &SpatialLocationCalculator::inputConfig, DOC(dai, node, SpatialLocationCalculator, inputConfig))
         .def_readonly("inputDepth", &SpatialLocationCalculator::inputDepth, DOC(dai, node, SpatialLocationCalculator, inputDepth))
         .def_readonly("out", &SpatialLocationCalculator::out, DOC(dai, node, SpatialLocationCalculator, out))
         .def_readonly("passthroughDepth", &SpatialLocationCalculator::passthroughDepth, DOC(dai, node, SpatialLocationCalculator, passthroughDepth))
         .def_readonly("initialConfig", &SpatialLocationCalculator::initialConfig, DOC(dai, node, SpatialLocationCalculator, initialConfig))
         .def("setWaitForConfigInput", &SpatialLocationCalculator::setWaitForConfigInput, py::arg("wait"), DOC(dai, node, SpatialLocationCalculator, setWaitForConfigInput))
         ;
+    // ALIAS
+    daiNodeModule.attr("SpatialLocationCalculator").attr("Properties") = spatialLocationCalculatorProperties;
 
     // SystemLogger node
-    py::class_<SystemLogger, Node, std::shared_ptr<SystemLogger>>(m, "SystemLogger", DOC(dai, node, SystemLogger))
+    systemLogger
         .def_readonly("out", &SystemLogger::out, DOC(dai, node, SystemLogger, out))
         .def("setRate", &SystemLogger::setRate, py::arg("hz"), DOC(dai, node, SystemLogger, setRate))
         ;
 
     // NeuralNetwork node
-    py::class_<ObjectTracker, Node, std::shared_ptr<ObjectTracker>>(m, "ObjectTracker", DOC(dai, node, ObjectTracker))
+    objectTracker
         .def_readonly("inputTrackerFrame", &ObjectTracker::inputTrackerFrame, DOC(dai, node, ObjectTracker, inputTrackerFrame))
         .def_readonly("inputDetectionFrame", &ObjectTracker::inputDetectionFrame, DOC(dai, node, ObjectTracker, inputDetectionFrame))
         .def_readonly("inputDetections", &ObjectTracker::inputDetections, DOC(dai, node, ObjectTracker, inputDetections))
         .def_readonly("out", &ObjectTracker::out, DOC(dai, node, ObjectTracker, out))
         .def_readonly("passthroughTrackerFrame", &ObjectTracker::passthroughTrackerFrame, DOC(dai, node, ObjectTracker, passthroughTrackerFrame))
         .def_readonly("passthroughDetectionFrame", &ObjectTracker::passthroughDetectionFrame, DOC(dai, node, ObjectTracker, passthroughDetectionFrame))
         .def_readonly("passthroughDetections", &ObjectTracker::passthroughDetections, DOC(dai, node, ObjectTracker, passthroughDetections))
 
         .def("setTrackerThreshold", &ObjectTracker::setTrackerThreshold, py::arg("threshold"), DOC(dai, node, ObjectTracker, setTrackerThreshold))
         .def("setMaxObjectsToTrack", &ObjectTracker::setMaxObjectsToTrack, py::arg("maxObjectsToTrack"), DOC(dai, node, ObjectTracker, setMaxObjectsToTrack))
         .def("setDetectionLabelsToTrack", &ObjectTracker::setDetectionLabelsToTrack, py::arg("labels"), DOC(dai, node, ObjectTracker, setDetectionLabelsToTrack))
         .def("setTrackerType", &ObjectTracker::setTrackerType, py::arg("type"), DOC(dai, node, ObjectTracker, setTrackerType))
         .def("setTrackerIdAssigmentPolicy", &ObjectTracker::setTrackerIdAssigmentPolicy, py::arg("type"), DOC(dai, node, ObjectTracker, setTrackerIdAssigmentPolicy))
         ;
+    daiNodeModule.attr("ObjectTracker").attr("Properties") = objectTrackerProperties;
+
+    // Script node
+    script
+        .def_readonly("inputs", &Script::inputs)
+        .def_readonly("outputs", &Script::outputs)
+        .def("setScriptPath", &Script::setScriptPath, DOC(dai, node, Script, setScriptPath))
+        .def("setScript", py::overload_cast<const std::string&, const std::string&>(&Script::setScript), py::arg("script"), py::arg("name") = "", DOC(dai, node, Script, setScript))
+        .def("setScript", py::overload_cast<const std::vector<std::uint8_t>&, const std::string&>(&Script::setScript), py::arg("data"), py::arg("name") = "", DOC(dai, node, Script, setScript, 2))
+        .def("getScriptPath", &Script::getScriptPath, DOC(dai, node, Script, getScriptPath))
+        .def("getScriptName", &Script::getScriptName, DOC(dai, node, Script, getScriptName))
+        .def("setProcessor", &Script::setProcessor, DOC(dai, node, Script, setProcessor))
+        .def("getProcessor", &Script::getProcessor, DOC(dai, node, Script, getProcessor))
+        ;
+    daiNodeModule.attr("Script").attr("Properties") = scriptProperties;
+
 
     // IMU node
-    py::class_<IMU, Node, std::shared_ptr<IMU>>(m, "IMU", DOC(dai, node, IMU))
+    imu
         .def_readonly("out", &IMU::out, DOC(dai, node, IMU, out))
         .def("enableIMUSensor", static_cast<void(IMU::*)(IMUSensorConfig imuSensor)>(&IMU::enableIMUSensor), py::arg("sensorConfig"), DOC(dai, node, IMU, enableIMUSensor))
         .def("enableIMUSensor", static_cast<void(IMU::*)(const std::vector<IMUSensorConfig>& imuSensors)>(&IMU::enableIMUSensor), py::arg("sensorConfigs"), DOC(dai, node, IMU, enableIMUSensor, 2))
         .def("enableIMUSensor", static_cast<void(IMU::*)(IMUSensor sensor, uint32_t reportRate)>(&IMU::enableIMUSensor), py::arg("sensor"), py::arg("reportRate"), DOC(dai, node, IMU, enableIMUSensor, 3))
         .def("enableIMUSensor", static_cast<void(IMU::*)(const std::vector<IMUSensor>& sensors, uint32_t reportRate)>(&IMU::enableIMUSensor), py::arg("sensors"), py::arg("reportRate"), DOC(dai, node, IMU, enableIMUSensor, 4))
         .def("setBatchReportThreshold", &IMU::setBatchReportThreshold, py::arg("batchReportThreshold"), DOC(dai, node, IMU, setBatchReportThreshold))
         .def("getBatchReportThreshold", &IMU::getBatchReportThreshold, DOC(dai, node, IMU, getBatchReportThreshold))
         .def("setMaxBatchReports", &IMU::setMaxBatchReports, py::arg("maxBatchReports"), DOC(dai, node, IMU, setMaxBatchReports))
         .def("getMaxBatchReports", &IMU::getMaxBatchReports, DOC(dai, node, IMU, getMaxBatchReports))
         ;
+    daiNodeModule.attr("IMU").attr("Properties") = imuProperties;
 
     // EdgeDetector node
-    py::class_<EdgeDetector, Node, std::shared_ptr<EdgeDetector>>(m, "EdgeDetector", DOC(dai, node, EdgeDetector))
+
+    edgeDetector
         .def_readonly("initialConfig", &EdgeDetector::initialConfig, DOC(dai, node, EdgeDetector, initialConfig))
         .def_readonly("inputConfig", &EdgeDetector::inputConfig, DOC(dai, node, EdgeDetector, inputConfig))
         .def_readonly("inputImage", &EdgeDetector::inputImage, DOC(dai, node, EdgeDetector, inputImage))
         .def_readonly("outputImage", &EdgeDetector::outputImage, DOC(dai, node, EdgeDetector, outputImage))
         .def("setWaitForConfigInput", &EdgeDetector::setWaitForConfigInput, DOC(dai, node, EdgeDetector, setWaitForConfigInput))
         .def("setNumFramesPool", &EdgeDetector::setNumFramesPool, DOC(dai, node, EdgeDetector, setNumFramesPool))
         .def("setMaxOutputFrameSize", &EdgeDetector::setMaxOutputFrameSize, DOC(dai, node, EdgeDetector, setMaxOutputFrameSize))
         ;
-
-    ////////////////////////////////////
-    // Node properties bindings
-    ////////////////////////////////////
-    py::class_<ColorCameraProperties> colorCameraProperties(m, "ColorCameraProperties", DOC(dai, ColorCameraProperties));
-    colorCameraProperties
-        .def_readwrite("initialControl", &ColorCameraProperties::initialControl)
-        .def_readwrite("boardSocket", &ColorCameraProperties::boardSocket)
-        .def_readwrite("colorOrder", &ColorCameraProperties::colorOrder)
-        .def_readwrite("interleaved", &ColorCameraProperties::interleaved)
-        .def_readwrite("previewHeight", &ColorCameraProperties::previewHeight)
-        .def_readwrite("previewWidth", &ColorCameraProperties::previewWidth)
-        .def_readwrite("videoHeight", &ColorCameraProperties::videoHeight)
-        .def_readwrite("videoWidth", &ColorCameraProperties::videoWidth)
-        .def_readwrite("stillHeight", &ColorCameraProperties::stillHeight)
-        .def_readwrite("stillWidth", &ColorCameraProperties::stillWidth)
-        .def_readwrite("resolution", &ColorCameraProperties::resolution)
-        .def_readwrite("fps", &ColorCameraProperties::fps)
-        .def_readwrite("sensorCropX", &ColorCameraProperties::sensorCropX)
-        .def_readwrite("sensorCropY", &ColorCameraProperties::sensorCropY)
-    ;
-
-    py::enum_<ColorCameraProperties::SensorResolution>(colorCameraProperties, "SensorResolution", DOC(dai, ColorCameraProperties, SensorResolution))
-        .value("THE_1080_P", ColorCameraProperties::SensorResolution::THE_1080_P)
-        .value("THE_4_K", ColorCameraProperties::SensorResolution::THE_4_K)
-        .value("THE_12_MP", ColorCameraProperties::SensorResolution::THE_12_MP)
-        ;
-
-    py::enum_<ColorCameraProperties::ColorOrder>(colorCameraProperties, "ColorOrder", DOC(dai, ColorCameraProperties, ColorOrder))
-        .value("BGR", ColorCameraProperties::ColorOrder::BGR)
-        .value("RGB", ColorCameraProperties::ColorOrder::RGB)
-        ;
-    // ALIAS
-    m.attr("ColorCamera").attr("Properties") = colorCameraProperties;
-
-
-
-    // MonoCamera props
-    py::class_<MonoCameraProperties> monoCameraProperties(m, "MonoCameraProperties", DOC(dai, MonoCameraProperties));
-    monoCameraProperties
-        .def_readwrite("initialControl", &MonoCameraProperties::initialControl)
-        .def_readwrite("boardSocket", &MonoCameraProperties::boardSocket)
-        .def_readwrite("resolution", &MonoCameraProperties::resolution)
-        .def_readwrite("fps",  &MonoCameraProperties::fps)
-    ;
-
-    py::enum_<MonoCameraProperties::SensorResolution>(monoCameraProperties, "SensorResolution", DOC(dai, MonoCameraProperties, SensorResolution))
-        .value("THE_720_P", MonoCameraProperties::SensorResolution::THE_720_P)
-        .value("THE_800_P", MonoCameraProperties::SensorResolution::THE_800_P)
-        .value("THE_400_P", MonoCameraProperties::SensorResolution::THE_400_P)
-        ;
-    // ALIAS
-    m.attr("MonoCamera").attr("Properties") = monoCameraProperties;
-
-
-    // StereoDepth props
-    py::class_<StereoDepthProperties> stereoDepthProperties(m, "StereoDepthProperties", DOC(dai, StereoDepthProperties));
-    stereoDepthProperties
-        .def_readwrite("calibration",             &StereoDepthProperties::calibration)
-        .def_readwrite("initialConfig",           &StereoDepthProperties::initialConfig)
-        .def_readwrite("inputConfigSync",         &StereoDepthProperties::inputConfigSync)
-        .def_readwrite("depthAlign",              &StereoDepthProperties::depthAlign)
-        .def_readwrite("depthAlignCamera",        &StereoDepthProperties::depthAlignCamera)
-        .def_readwrite("enableLeftRightCheck",    &StereoDepthProperties::enableLeftRightCheck)
-        .def_readwrite("enableSubpixel",          &StereoDepthProperties::enableSubpixel)
-        .def_readwrite("enableExtendedDisparity", &StereoDepthProperties::enableExtendedDisparity)
-        .def_readwrite("rectifyMirrorFrame",      &StereoDepthProperties::rectifyMirrorFrame)
-        .def_readwrite("rectifyEdgeFillColor",    &StereoDepthProperties::rectifyEdgeFillColor)
-        .def_readwrite("width",                   &StereoDepthProperties::width)
-        .def_readwrite("height",                  &StereoDepthProperties::height)
-        .def_readwrite("outWidth",                &StereoDepthProperties::outWidth, DOC(dai, StereoDepthProperties, outWidth))
-        .def_readwrite("outHeight",               &StereoDepthProperties::outHeight, DOC(dai, StereoDepthProperties, outHeight))
-        .def_readwrite("outKeepAspectRatio",      &StereoDepthProperties::outKeepAspectRatio, DOC(dai, StereoDepthProperties, outKeepAspectRatio))
-        .def_readwrite("mesh",                    &StereoDepthProperties::mesh, DOC(dai, StereoDepthProperties, mesh))
-        ;
-
-    py::enum_<MedianFilter> medianFilter(m, "MedianFilter", DOC(dai, MedianFilter));
-    medianFilter
-        .value("MEDIAN_OFF", MedianFilter::MEDIAN_OFF)
-        .value("KERNEL_3x3", MedianFilter::KERNEL_3x3)
-        .value("KERNEL_5x5", MedianFilter::KERNEL_5x5)
-        .value("KERNEL_7x7", MedianFilter::KERNEL_7x7)
-        ;
-
-    py::enum_<StereoDepthProperties::DepthAlign>(stereoDepthProperties, "DepthAlign")
-        .value("RECTIFIED_RIGHT", StereoDepthProperties::DepthAlign::RECTIFIED_RIGHT)
-        .value("RECTIFIED_LEFT",  StereoDepthProperties::DepthAlign::RECTIFIED_LEFT)
-        .value("CENTER",          StereoDepthProperties::DepthAlign::CENTER)
-        ;
-
-    py::class_<StereoDepthConfigData> stereoDepthConfigData(m, "StereoDepthConfigData", DOC(dai, StereoDepthConfigData));
-    stereoDepthConfigData
-        .def(py::init<>())
-        .def_readwrite("median", &StereoDepthConfigData::median,  DOC(dai, StereoDepthConfigData, median))
-        .def_readwrite("confidenceThreshold", &StereoDepthConfigData::confidenceThreshold,  DOC(dai, StereoDepthConfigData, confidenceThreshold))
-        .def_readwrite("bilateralSigmaValue", &StereoDepthConfigData::bilateralSigmaValue,  DOC(dai, StereoDepthConfigData, bilateralSigmaValue))
-        .def_readwrite("leftRightCheckThreshold", &StereoDepthConfigData::leftRightCheckThreshold,  DOC(dai, StereoDepthConfigData, leftRightCheckThreshold))
-        ;
-
-    m.attr("StereoDepthProperties").attr("MedianFilter") = medianFilter;
-    m.attr("StereoDepthConfigData").attr("MedianFilter") = medianFilter;
-
-    // ALIAS
-    m.attr("StereoDepth").attr("Properties") = stereoDepthProperties;
-
-
-
-    // VideoEncoder props
-    py::class_<VideoEncoderProperties> videoEncoderProperties(m, "VideoEncoderProperties", DOC(dai, VideoEncoderProperties));
-    videoEncoderProperties
-        .def_readwrite("bitrate", &VideoEncoderProperties::bitrate)
-        .def_readwrite("keyframeFrequency", &VideoEncoderProperties::keyframeFrequency)
-        .def_readwrite("maxBitrate", &VideoEncoderProperties::maxBitrate)
-        .def_readwrite("numBFrames", &VideoEncoderProperties::numBFrames)
-        .def_readwrite("numFramesPool", &VideoEncoderProperties::numFramesPool)
-        .def_readwrite("profile", &VideoEncoderProperties::profile)
-        .def_readwrite("quality", &VideoEncoderProperties::quality)
-        .def_readwrite("rateCtrlMode", &VideoEncoderProperties::rateCtrlMode)
-        .def_readwrite("width", &VideoEncoderProperties::width)
-        .def_readwrite("height", &VideoEncoderProperties::height)
-        ;
-
-    py::enum_<VideoEncoderProperties::Profile>(videoEncoderProperties, "Profile", DOC(dai, VideoEncoderProperties, Profile))
-        .value("H264_BASELINE", VideoEncoderProperties::Profile::H264_BASELINE)
-        .value("H264_HIGH", VideoEncoderProperties::Profile::H264_HIGH)
-        .value("H264_MAIN", VideoEncoderProperties::Profile::H264_MAIN)
-        .value("H265_MAIN", VideoEncoderProperties::Profile::H265_MAIN)
-        .value("MJPEG", VideoEncoderProperties::Profile::MJPEG)
-        ;
-
-    py::enum_<VideoEncoderProperties::RateControlMode>(videoEncoderProperties, "RateControlMode", DOC(dai, VideoEncoderProperties, RateControlMode))
-        .value("CBR", VideoEncoderProperties::RateControlMode::CBR)
-        .value("VBR", VideoEncoderProperties::RateControlMode::VBR)
-        ;
-    // ALIAS
-    m.attr("VideoEncoder").attr("Properties") = videoEncoderProperties;
-
-
-
-
-    py::class_<SystemLoggerProperties>(m, "SystemLoggerProperties", DOC(dai, SystemLoggerProperties))
-        .def_readwrite("rateHz", &SystemLoggerProperties::rateHz)
-        ;
-
-    py::class_<NeuralNetworkProperties, std::shared_ptr<NeuralNetworkProperties>> neuralNetworkProperties(m, "NeuralNetworkProperties", DOC(dai, NeuralNetworkProperties));
-    neuralNetworkProperties
-        .def_readwrite("blobSize", &NeuralNetworkProperties::blobSize)
-        .def_readwrite("blobUri", &NeuralNetworkProperties::blobUri)
-        .def_readwrite("numFrames", &NeuralNetworkProperties::numFrames)
-        .def_readwrite("numThreads", &NeuralNetworkProperties::numThreads)
-        .def_readwrite("numNCEPerThread", &NeuralNetworkProperties::numNCEPerThread)
-        ;
-    m.attr("NeuralNetwork").attr("Properties") = neuralNetworkProperties;
-
-
-    py::class_<DetectionNetworkProperties, NeuralNetworkProperties, std::shared_ptr<DetectionNetworkProperties>> detectionNetworkProperties(m, "DetectionNetworkProperties", DOC(dai, DetectionNetworkProperties));
-    detectionNetworkProperties
-        .def_readwrite("nnFamily", &DetectionNetworkProperties::nnFamily)
-        .def_readwrite("confidenceThreshold", &DetectionNetworkProperties::confidenceThreshold)
-        .def_readwrite("classes", &DetectionNetworkProperties::classes)
-        .def_readwrite("coordinates", &DetectionNetworkProperties::coordinates)
-        .def_readwrite("anchors", &DetectionNetworkProperties::anchors)
-        .def_readwrite("anchorMasks", &DetectionNetworkProperties::anchorMasks)
-        .def_readwrite("iouThreshold", &DetectionNetworkProperties::iouThreshold)
-        ;
-    // ALIAS
-    m.attr("DetectionNetwork").attr("Properties") = detectionNetworkProperties;
-
-
-    py::class_<SpatialDetectionNetworkProperties, DetectionNetworkProperties, std::shared_ptr<SpatialDetectionNetworkProperties>> spatialDetectionNetworkProperties(m, "SpatialDetectionNetworkProperties", DOC(dai, SpatialDetectionNetworkProperties));
-    spatialDetectionNetworkProperties
-        .def_readwrite("detectedBBScaleFactor", &SpatialDetectionNetworkProperties::detectedBBScaleFactor)
-        .def_readwrite("depthThresholds", &SpatialDetectionNetworkProperties::depthThresholds)
-        ;
-    // ALIAS
-    m.attr("SpatialDetectionNetwork").attr("Properties") = spatialDetectionNetworkProperties;
-
-
-    py::class_<SpatialLocationCalculatorProperties> spatialLocationCalculatorProperties(m, "SpatialLocationCalculatorProperties", DOC(dai, SpatialLocationCalculatorProperties));
-    spatialLocationCalculatorProperties
-        .def_readwrite("roiConfig", &SpatialLocationCalculatorProperties::roiConfig)
-        .def_readwrite("inputConfigSync", &SpatialLocationCalculatorProperties::inputConfigSync)
-        ;
-    m.attr("SpatialLocationCalculator").attr("Properties") = spatialLocationCalculatorProperties;
-
-
-    py::enum_<TrackerType>(m, "TrackerType")
-        .value("ZERO_TERM_IMAGELESS", TrackerType::ZERO_TERM_IMAGELESS)
-        .value("ZERO_TERM_COLOR_HISTOGRAM", TrackerType::ZERO_TERM_COLOR_HISTOGRAM)
-    ;
-
-    py::enum_<TrackerIdAssigmentPolicy>(m, "TrackerIdAssigmentPolicy")
-        .value("UNIQUE_ID", TrackerIdAssigmentPolicy::UNIQUE_ID)
-        .value("SMALLEST_ID", TrackerIdAssigmentPolicy::SMALLEST_ID)
-    ;
-
-
-    py::class_<ObjectTrackerProperties, std::shared_ptr<ObjectTrackerProperties>> objectTrackerProperties(m, "ObjectTrackerProperties", DOC(dai, ObjectTrackerProperties));
-    objectTrackerProperties
-        .def_readwrite("trackerThreshold", &ObjectTrackerProperties::trackerThreshold)
-        .def_readwrite("maxObjectsToTrack", &ObjectTrackerProperties::maxObjectsToTrack)
-        .def_readwrite("detectionLabelsToTrack", &ObjectTrackerProperties::detectionLabelsToTrack)
-        .def_readwrite("trackerType", &ObjectTrackerProperties::trackerType)
-        .def_readwrite("trackerIdAssigmentPolicy", &ObjectTrackerProperties::trackerIdAssigmentPolicy)
-        ;
-    m.attr("ObjectTracker").attr("Properties") = objectTrackerProperties;
-
-    py::enum_<IMUSensor>(m, "IMUSensor", DOC(dai, IMUSensor))
-        .value("ACCELEROMETER_RAW", IMUSensor::ACCELEROMETER_RAW, DOC(dai, IMUSensor, ACCELEROMETER_RAW))
-        .value("ACCELEROMETER", IMUSensor::ACCELEROMETER, DOC(dai, IMUSensor, ACCELEROMETER))
-        .value("LINEAR_ACCELERATION", IMUSensor::LINEAR_ACCELERATION, DOC(dai, IMUSensor, LINEAR_ACCELERATION))
-        .value("GRAVITY", IMUSensor::GRAVITY, DOC(dai, IMUSensor, GRAVITY))
-        .value("GYROSCOPE_RAW", IMUSensor::GYROSCOPE_RAW, DOC(dai, IMUSensor, GYROSCOPE_RAW))
-        .value("GYROSCOPE_CALIBRATED", IMUSensor::GYROSCOPE_CALIBRATED, DOC(dai, IMUSensor, GYROSCOPE_CALIBRATED))
-        .value("GYROSCOPE_UNCALIBRATED", IMUSensor::GYROSCOPE_UNCALIBRATED, DOC(dai, IMUSensor, GYROSCOPE_UNCALIBRATED))
-        .value("MAGNETOMETER_RAW", IMUSensor::MAGNETOMETER_RAW, DOC(dai, IMUSensor, MAGNETOMETER_RAW))
-        .value("MAGNETOMETER_CALIBRATED", IMUSensor::MAGNETOMETER_CALIBRATED, DOC(dai, IMUSensor, MAGNETOMETER_CALIBRATED))
-        .value("MAGNETOMETER_UNCALIBRATED", IMUSensor::MAGNETOMETER_UNCALIBRATED, DOC(dai, IMUSensor, MAGNETOMETER_UNCALIBRATED))
-        .value("ROTATION_VECTOR", IMUSensor::ROTATION_VECTOR, DOC(dai, IMUSensor, ROTATION_VECTOR))
-        .value("GAME_ROTATION_VECTOR", IMUSensor::GAME_ROTATION_VECTOR, DOC(dai, IMUSensor, GAME_ROTATION_VECTOR))
-        .value("GEOMAGNETIC_ROTATION_VECTOR", IMUSensor::GEOMAGNETIC_ROTATION_VECTOR, DOC(dai, IMUSensor, GEOMAGNETIC_ROTATION_VECTOR))
-        .value("ARVR_STABILIZED_ROTATION_VECTOR", IMUSensor::ARVR_STABILIZED_ROTATION_VECTOR, DOC(dai, IMUSensor, ARVR_STABILIZED_ROTATION_VECTOR))
-        .value("ARVR_STABILIZED_GAME_ROTATION_VECTOR", IMUSensor::ARVR_STABILIZED_GAME_ROTATION_VECTOR, DOC(dai, IMUSensor, ARVR_STABILIZED_GAME_ROTATION_VECTOR))
-        // .value("GYRO_INTEGRATED_ROTATION_VECTOR", IMUSensor::GYRO_INTEGRATED_ROTATION_VECTOR)
-    ;
-
-    py::class_<IMUSensorConfig, std::shared_ptr<IMUSensorConfig>>(m, "IMUSensorConfig", DOC(dai, IMUSensorConfig))
-        .def(py::init<>())
-        .def_readwrite("sensitivityEnabled", &IMUSensorConfig::sensitivityEnabled)
-        .def_readwrite("sensitivityRelative", &IMUSensorConfig::sensitivityRelative)
-        .def_readwrite("changeSensitivity", &IMUSensorConfig::changeSensitivity)
-        .def_readwrite("reportRate", &IMUSensorConfig::reportRate)
-        .def_readwrite("sensorId", &IMUSensorConfig::sensorId)
-        ;
-
-    py::class_<IMUProperties> imuProperties(m, "IMUProperties", DOC(dai, IMUProperties));
-    imuProperties
-        .def_readwrite("imuSensors", &IMUProperties::imuSensors, DOC(dai, IMUProperties, imuSensors))
-        .def_readwrite("batchReportThreshold", &IMUProperties::batchReportThreshold, DOC(dai, IMUProperties, batchReportThreshold))
-        .def_readwrite("maxBatchReports", &IMUProperties::maxBatchReports, DOC(dai, IMUProperties, maxBatchReports))
-    ;
-    m.attr("IMU").attr("Properties") = imuProperties;
-
-
-    py::class_<EdgeDetectorProperties> edgeDetectorProperties(m, "EdgeDetectorProperties", DOC(dai, EdgeDetectorProperties));
-    edgeDetectorProperties
-        .def_readwrite("initialConfig", &EdgeDetectorProperties::initialConfig, DOC(dai, EdgeDetectorProperties, initialConfig))
-        .def_readwrite("inputConfigSync", &EdgeDetectorProperties::inputConfigSync, DOC(dai, EdgeDetectorProperties, inputConfigSync))
-        .def_readwrite("outputFrameSize", &EdgeDetectorProperties::outputFrameSize, DOC(dai, EdgeDetectorProperties, outputFrameSize))
-        .def_readwrite("numFramesPool", &EdgeDetectorProperties::numFramesPool, DOC(dai, EdgeDetectorProperties, numFramesPool))
-
-    ;
-    m.attr("EdgeDetector").attr("Properties") = edgeDetectorProperties;
-
+    daiNodeModule.attr("EdgeDetector").attr("Properties") = edgeDetectorProperties;
 
 
 }
+
```

### Comparing `depthai-2.8.0.0/src/pipeline/PipelineBindings.cpp` & `depthai-2.9.0.0/src/pipeline/PipelineBindings.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,122 @@
+
 #include "PipelineBindings.hpp"
+#include "NodeBindings.hpp"
 
 // depthai
 #include "depthai/pipeline/Pipeline.hpp"
 
 // depthai - nodes
 #include "depthai/pipeline/node/XLinkIn.hpp"
 #include "depthai/pipeline/node/XLinkOut.hpp"
 #include "depthai/pipeline/node/NeuralNetwork.hpp"
 #include "depthai/pipeline/node/ColorCamera.hpp"
 #include "depthai/pipeline/node/VideoEncoder.hpp"
 #include "depthai/pipeline/node/SPIOut.hpp"
+#include "depthai/pipeline/node/SPIIn.hpp"
 #include "depthai/pipeline/node/ImageManip.hpp"
 #include "depthai/pipeline/node/MonoCamera.hpp"
 #include "depthai/pipeline/node/StereoDepth.hpp"
 #include "depthai/pipeline/node/DetectionNetwork.hpp"
+#include "depthai/pipeline/node/Script.hpp"
 #include "depthai/pipeline/node/SystemLogger.hpp"
 #include "depthai/pipeline/node/SpatialLocationCalculator.hpp"
 #include "depthai/pipeline/node/SpatialDetectionNetwork.hpp"
 #include "depthai/pipeline/node/ObjectTracker.hpp"
 #include "depthai/pipeline/node/IMU.hpp"
 #include "depthai/pipeline/node/EdgeDetector.hpp"
 
 // depthai-shared
 #include "depthai-shared/properties/GlobalProperties.hpp"
 
-void PipelineBindings::bind(pybind11::module& m){
 
+
+std::shared_ptr<dai::Node> createNode(dai::Pipeline& p, py::object class_){
+    auto nodeCreateMap = NodeBindings::getNodeCreateMap();
+    for(auto& kv : nodeCreateMap){
+        auto& node = kv.first;
+        auto& create = kv.second;
+        if(node.is(class_)){
+            return create(p, class_);
+        }
+    }
+    return nullptr;
+}
+
+void PipelineBindings::bind(pybind11::module& m, void* pCallstack){
     using namespace dai;
 
+    // Type definitions
+    py::class_<GlobalProperties> globalProperties(m, "GlobalProperties", DOC(dai, GlobalProperties));
+    py::class_<Pipeline> pipeline(m, "Pipeline", DOC(dai, Pipeline, 2));
+
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    // Call the rest of the type defines, then perform the actual bindings
+    Callstack* callstack = (Callstack*) pCallstack;
+    auto cb = callstack->top();
+    callstack->pop();
+    cb(m, pCallstack);
+    // Actual bindings
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+    ///////////////////////////////////////////////////////////////////////
+
 
     // Bind global properties
-    py::class_<GlobalProperties>(m, "GlobalProperties", DOC(dai, GlobalProperties))
+    globalProperties
         .def_readwrite("leonOsFrequencyHz", &GlobalProperties::leonCssFrequencyHz)
         .def_readwrite("leonRtFrequencyHz", &GlobalProperties::leonMssFrequencyHz)
         .def_readwrite("pipelineName", &GlobalProperties::pipelineName)
         .def_readwrite("pipelineVersion", &GlobalProperties::pipelineVersion)
         .def_readwrite("cameraTuningBlobSize", &GlobalProperties::cameraTuningBlobSize, DOC(dai, GlobalProperties, cameraTuningBlobSize))
         .def_readwrite("cameraTuningBlobUri", &GlobalProperties::cameraTuningBlobUri, DOC(dai, GlobalProperties, cameraTuningBlobUri))
         ;
 
     // bind pipeline
-    py::class_<Pipeline>(m, "Pipeline", DOC(dai, Pipeline, 2))
+    pipeline
         .def(py::init<>(), DOC(dai, Pipeline, Pipeline))
         //.def(py::init<const Pipeline&>())
         .def("getGlobalProperties", &Pipeline::getGlobalProperties, DOC(dai, Pipeline, getGlobalProperties))
         //.def("create", &Pipeline::create<node::XLinkIn>)
         .def("remove", &Pipeline::remove, py::arg("node"), DOC(dai, Pipeline, remove))
         .def("getAllNodes", static_cast<std::vector<std::shared_ptr<const Node>> (Pipeline::*)() const>(&Pipeline::getAllNodes), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getAllNodes))
         .def("getAllNodes", static_cast<std::vector<std::shared_ptr< Node>> (Pipeline::*)()>(&Pipeline::getAllNodes), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getAllNodes))
         .def("getNode", static_cast<std::shared_ptr<const Node> (Pipeline::*)(Node::Id) const>(&Pipeline::getNode), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getNode))
         .def("getNode", static_cast<std::shared_ptr<Node> (Pipeline::*)(Node::Id)>(&Pipeline::getNode), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getNode))
         .def("getConnections", &Pipeline::getConnections, DOC(dai, Pipeline, getConnections), DOC(dai, Pipeline, getConnections))
         .def("getConnectionMap", &Pipeline::getConnectionMap, DOC(dai, Pipeline, getConnectionMap), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getConnectionMap))
         .def("getNodeMap", &Pipeline::getNodeMap, DOC(dai, Pipeline, getNodeMap), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getNodeMap))
         .def("link", &Pipeline::link, DOC(dai, Pipeline, link), DOC(dai, Pipeline, link))
         .def("unlink", &Pipeline::unlink, DOC(dai, Pipeline, unlink), DOC(dai, Pipeline, unlink))
-        .def("getAllAssets", &Pipeline::getAllAssets, DOC(dai, Pipeline, getAllAssets))
         .def("getAssetManager", static_cast<const AssetManager& (Pipeline::*)() const>(&Pipeline::getAssetManager), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getAssetManager))
         .def("getAssetManager", static_cast<AssetManager& (Pipeline::*)()>(&Pipeline::getAssetManager), py::return_value_policy::reference_internal, DOC(dai, Pipeline, getAssetManager))
         .def("setOpenVINOVersion", &Pipeline::setOpenVINOVersion, py::arg("version") = Pipeline::DEFAULT_OPENVINO_VERSION, DOC(dai, Pipeline, setOpenVINOVersion))
         .def("getOpenVINOVersion", &Pipeline::getOpenVINOVersion, DOC(dai, Pipeline, getOpenVINOVersion))
         .def("setCameraTuningBlobPath", &Pipeline::setCameraTuningBlobPath, py::arg("path"), DOC(dai, Pipeline, setCameraTuningBlobPath))
         .def("setCalibrationData", &Pipeline::setCalibrationData, py::arg("calibrationDataHandler"), DOC(dai, Pipeline, setCalibrationData))
         .def("getCalibrationData", &Pipeline::getCalibrationData, DOC(dai, Pipeline, getCalibrationData))
-         // templated create<NODE> function
+        // 'Template' create function
+        .def("create", [](dai::Pipeline& p, py::object class_) {
+            auto node = createNode(p, class_);
+            if(node == nullptr){
+                throw std::invalid_argument(std::string(py::str(class_)) + " is not a subclass of depthai.node");
+            }
+            return node;
+        })
+        // TODO(themarpe) DEPRECATE, use pipeline.create([class name])
+        // templated create<NODE> function
         .def("createXLinkIn", &Pipeline::create<node::XLinkIn>)
         .def("createXLinkOut", &Pipeline::create<node::XLinkOut>)
         .def("createNeuralNetwork", &Pipeline::create<node::NeuralNetwork>)
         .def("createColorCamera", &Pipeline::create<node::ColorCamera>)
         .def("createVideoEncoder", &Pipeline::create<node::VideoEncoder>)
         .def("createSPIOut", &Pipeline::create<node::SPIOut>)
+        .def("createSPIIn", &Pipeline::create<node::SPIIn>)
         .def("createImageManip", &Pipeline::create<node::ImageManip>)
         .def("createMonoCamera", &Pipeline::create<node::MonoCamera>)
         .def("createStereoDepth", &Pipeline::create<node::StereoDepth>)
         .def("createMobileNetDetectionNetwork", &Pipeline::create<node::MobileNetDetectionNetwork>)
         .def("createYoloDetectionNetwork", &Pipeline::create<node::YoloDetectionNetwork>)
         .def("createSystemLogger", &Pipeline::create<node::SystemLogger>)
         .def("createSpatialLocationCalculator", &Pipeline::create<node::SpatialLocationCalculator>)
```


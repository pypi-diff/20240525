# Comparing `tmp/whisper_cpp_python_smr-0.2.tar.gz` & `tmp/whisper_cpp_python_smr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_cpp_python_smr-0.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "whisper_cpp_python_smr-0.2.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `whisper_cpp_python_smr-0.2.tar` & `whisper_cpp_python_smr-0.2.1.tar`

### file list

```diff
@@ -1,570 +1,570 @@
--rw-r--r--   0        0        0     1657 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/.gitignore
--rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/.gitmodules
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/CMakeLists.txt
--rw-r--r--   0        0        0    11358 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/LICENSE
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/README.md
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/pyproject.toml
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.devops/cublas.Dockerfile
--rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.devops/main-cuda.Dockerfile
--rw-r--r--   0        0        0      402 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.devops/main.Dockerfile
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.git
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/bindings-go.yml
--rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/bindings-ruby.yml
--rw-r--r--   0        0        0    19410 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/build.yml
--rw-r--r--   0        0        0     1715 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/examples.yml
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.gitignore
--rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.gitmodules
--rw-r--r--   0        0        0    12824 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/AUTHORS
--rw-r--r--   0        0        0    29517 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/CMakeLists.txt
--rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/LICENSE
--rw-r--r--   0        0        0    18797 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/Makefile
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/Package.swift
--rw-r--r--   0        0        0    39837 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/README.md
--rw-r--r--   0        0        0     6835 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/README_sycl.md
--rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/CMakeLists.txt
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/.gitignore
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/LICENSE
--rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/Makefile
--rw-r--r--   0        0        0     2825 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/README.md
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/doc.go
--rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go
--rw-r--r--   0        0        0     5343 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go
--rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go
--rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go
--rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go
--rw-r--r--   0        0        0     3295 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/go.mod
--rw-r--r--   0        0        0     2019 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/go.sum
--rw-r--r--   0        0        0     3812 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/params.go
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go
--rw-r--r--   0        0        0     8443 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go
--rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/doc.go
--rw-r--r--   0        0        0     3280 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go
--rw-r--r--   0        0        0   352078 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/samples/jfk.wav
--rw-r--r--   0        0        0    16147 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/whisper.go
--rw-r--r--   0        0        0     2815 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/whisper_test.go
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/.git
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/.github/workflows/swift.yml
--rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/.gitignore
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/LICENSE
--rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Makefile
--rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Makefile-tmpl
--rw-r--r--   0        0        0     2754 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Package.swift
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/README.md
--rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m
--rw-r--r--   0        0        0      937 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift
--rw-r--r--   0        0        0     7458 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.h
--rw-r--r--   0        0        0     8817 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.m
--rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.h
--rw-r--r--   0        0        0     8522 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.m
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.h
--rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.mm
--rw-r--r--   0        0        0    36901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.c
--rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.h
--rw-r--r--   0        0        0     7001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend-impl.h
--rw-r--r--   0        0        0    77427 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.c
--rw-r--r--   0        0        0    13346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.h
--rw-r--r--   0        0        0   133178 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-common.h
--rw-r--r--   0        0        0    16658 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-impl.h
--rw-r--r--   0        0        0     2316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.h
--rw-r--r--   0        0        0   187040 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.m
--rw-r--r--   0        0        0   633755 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.c
--rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.h
--rw-r--r--   0        0        0   758065 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c
--rw-r--r--   0        0        0    89614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/ggml.h
--rw-r--r--   0        0        0    31901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h
--rw-r--r--   0        0        0   262486 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp
--rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/publish-trigger
--rw-r--r--   0        0        0     8915 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/.idea/uiDesigner.xml
--rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/README.md
--rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/build.gradle
--rw-r--r--   0        0        0    61608 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradle.properties
--rw-r--r--   0        0        0     8495 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradlew
--rw-r--r--   0        0        0     2868 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradlew.bat
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/settings.gradle
--rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperContext.java
--rw-r--r--   0        0        0     7464 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCpp.java
--rw-r--r--   0        0        0    16263 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCppJnaLibrary.java
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/bean/WhisperSegment.java
--rw-r--r--   0        0        0      801 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperEncoderBeginCallback.java
--rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperLogitsFilterCallback.java
--rw-r--r--   0        0        0      811 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperNewSegmentCallback.java
--rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperProgressCallback.java
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/ggml/GgmlTensor.java
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/ggml/GgmlType.java
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/EModel.java
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModel.java
--rw-r--r--   0        0        0     1605 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModelLoader.java
--rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperState.java
--rw-r--r--   0        0        0     1194 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperTokenData.java
--rw-r--r--   0        0        0      586 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/BeamSearchParams.java
--rw-r--r--   0        0        0      676 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/CBool.java
--rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/GreedyParams.java
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperContextParams.java
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperFilters.java
--rw-r--r--   0        0        0    11673 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperFullParams.java
--rw-r--r--   0        0        0      406 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperHParams.java
--rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperSamplingStrategy.java
--rw-r--r--   0        0        0     5968 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperCppTest.java
--rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperJnaLibraryTest.java
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/.gitignore
--rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt
--rw-r--r--   0        0        0     2546 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/README.md
--rw-r--r--   0        0        0     3048 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/emscripten.cpp
--rw-r--r--   0        0        0     2907 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js
--rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/package-tmpl.json
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/package.json
--rw-r--r--   0        0        0   960825 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/whisper.js
--rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/Rakefile
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/.gitignore
--rw-r--r--   0        0        0     1532 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb
--rw-r--r--   0        0        0     7001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend-impl.h
--rw-r--r--   0        0        0    77241 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.c
--rw-r--r--   0        0        0    13346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.h
--rw-r--r--   0        0        0   133178 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-common.h
--rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-cuda.h
--rw-r--r--   0        0        0     8298 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-impl.h
--rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-kompute.h
--rw-r--r--   0        0        0     2316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-metal.h
--rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-opencl.h
--rw-r--r--   0        0        0   526217 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.c
--rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.h
--rw-r--r--   0        0        0     1909 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-sycl.h
--rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-vulkan.h
--rw-r--r--   0        0        0    15354 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
--rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
--rw-r--r--   0        0        0     3444 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/whispercpp.gemspec
--rw-r--r--   0        0        0     2037 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/BuildTypes.cmake
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/DefaultTargetOptions.cmake
--rw-r--r--   0        0        0     6234 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/FindFFmpeg.cmake
--rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/GitVars.cmake
--rw-r--r--   0        0        0     7458 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-decoder-impl.h
--rw-r--r--   0        0        0     8817 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-decoder-impl.m
--rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder-impl.h
--rw-r--r--   0        0        0     8522 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder-impl.m
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder.h
--rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder.mm
--rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/CMakeLists.txt
--rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/.gitignore
--rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/README.md
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
--rw-r--r--   0        0        0    13407 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/addon.cpp
--rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/index.js
--rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/package.json
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench/CMakeLists.txt
--rw-r--r--   0        0        0     1978 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench/README.md
--rw-r--r--   0        0        0     6313 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench/bench.cpp
--rw-r--r--   0        0        0     1161 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/README.md
--rw-r--r--   0        0        0     2713 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp
--rw-r--r--   0        0        0    12516 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command/CMakeLists.txt
--rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command/README.md
--rw-r--r--   0        0        0    30594 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command/command.cpp
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command/commands.txt
--rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/README.md
--rw-r--r--   0        0        0    10458 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp
--rw-r--r--   0        0        0    16219 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html
--rw-r--r--   0        0        0     8467 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-ggml.cpp
--rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-ggml.h
--rw-r--r--   0        0        0     6670 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-sdl.cpp
--rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-sdl.h
--rw-r--r--   0        0        0    31348 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common.cpp
--rw-r--r--   0        0        0     9571 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common.h
--rw-r--r--   0        0        0   241358 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/dr_wav.h
--rw-r--r--   0        0        0     9366 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/ffmpeg-transcode.cpp
--rwxr-xr-x   0        0        0     1197 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/generate-karaoke.sh
--rw-r--r--   0        0        0    17665 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/grammar-parser.cpp
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/grammar-parser.h
--rw-r--r--   0        0        0     6521 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/helpers.js
--rw-r--r--   0        0        0   907858 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/json.hpp
--rwxr-xr-x   0        0        0     2969 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/livestream.sh
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/CMakeLists.txt
--rw-r--r--   0        0        0     6120 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/README.md
--rw-r--r--   0        0        0    21186 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/lsp.cpp
--rw-r--r--   0        0        0    15906 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/whisper.vim
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/main/CMakeLists.txt
--rw-r--r--   0        0        0     3479 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/main/README.md
--rw-r--r--   0        0        0    54197 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/main/main.cpp
--rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/python/test_whisper_processor.py
--rw-r--r--   0        0        0     1775 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/python/whisper_processor.py
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/quantize/CMakeLists.txt
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/quantize/README.md
--rw-r--r--   0        0        0     8150 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/quantize/quantize.cpp
--rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/CMakeLists.txt
--rw-r--r--   0        0        0     3414 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/README.md
--rw-r--r--   0        0        0   302116 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/httplib.h
--rw-r--r--   0        0        0    44370 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/server.cpp
--rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream/CMakeLists.txt
--rw-r--r--   0        0        0     2281 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream/README.md
--rw-r--r--   0        0        0    18179 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream/stream.cpp
--rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/README.md
--rw-r--r--   0        0        0     6197 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp
--rw-r--r--   0        0        0    16188 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/CMakeLists.txt
--rw-r--r--   0        0        0     1510 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/README.md
--rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/build.sh
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/ls-sycl-device.cpp
--rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/run-whisper.sh
--rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/.gitignore
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/CMakeLists.txt
--rw-r--r--   0        0        0     1423 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/README.md
--rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/eleven-labs.py
--rw-r--r--   0        0        0    27930 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/gpt-2.cpp
--rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/gpt-2.h
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/speak
--rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/speak.bat
--rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/speak.ps1
--rw-r--r--   0        0        0    15579 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/talk.cpp
--rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/.gitignore
--rw-r--r--   0        0        0      643 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt
--rw-r--r--   0        0        0     2801 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/README.md
--rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py
--rw-r--r--   0        0        0   739022 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/llama.cpp
--rw-r--r--   0        0        0    53493 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/llama.h
--rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
--rwxr-xr-x   0        0        0     1494 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/speak
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/speak.bat
--rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/speak.ps1
--rw-r--r--   0        0        0    33891 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp
--rw-r--r--   0        0        0   223121 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode-data.cpp
--rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode-data.h
--rw-r--r--   0        0        0    30620 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode.cpp
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode.h
--rw-r--r--   0        0        0     1171 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt
--rw-r--r--   0        0        0     3341 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/README.md
--rw-r--r--   0        0        0    11996 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp
--rw-r--r--   0        0        0    27895 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp
--rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h
--rw-r--r--   0        0        0    33143 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html
--rwxr-xr-x   0        0        0     2771 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/twitch.sh
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/CMakeLists.txt
--rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/README.md
--rw-r--r--   0        0        0      344 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/CMakeLists.txt
--rw-r--r--   0        0        0    26777 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.cpp
--rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.h
--rw-r--r--   0        0        0     6625 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/WChess.cpp
--rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/WChess.h
--rw-r--r--   0        0        0     4362 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/test-chessboard.cpp
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.cmd/CMakeLists.txt
--rw-r--r--   0        0        0    10826 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.cmd/wchess.cmd.cpp
--rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/CMakeLists.txt
--rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.css
--rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.min.css
--rw-r--r--   0        0        0     1405 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bB.png
--rw-r--r--   0        0        0     3009 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bK.png
--rw-r--r--   0        0        0     1875 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bN.png
--rw-r--r--   0        0        0      777 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bP.png
--rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bQ.png
--rw-r--r--   0        0        0      748 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bR.png
--rw-r--r--   0        0        0     2374 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wB.png
--rw-r--r--   0        0        0     2823 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wK.png
--rw-r--r--   0        0        0     2388 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wN.png
--rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wP.png
--rw-r--r--   0        0        0     3812 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wQ.png
--rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wR.png
--rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     2605 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/README.md
--rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/package.json
--rw-r--r--   0        0        0    53836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.js
--rw-r--r--   0        0        0    14470 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.min.js
--rw-r--r--   0        0        0    19233 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/index-tmpl.html
--rw-r--r--   0        0        0    87533 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/jquery-3.7.1.min.js
--rw-r--r--   0        0        0     4173 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/wchess.wasm.cpp
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.gitignore
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/.gitignore
--rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/.name
--rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/compiler.xml
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml
--rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/misc.xml
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/vcs.xml
--rw-r--r--   0        0        0     2367 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/README.md
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/.gitignore
--rw-r--r--   0        0        0     1966 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/build.gradle
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
--rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
--rw-r--r--   0        0        0     1124 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
--rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
--rw-r--r--   0        0        0     2259 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
--rw-r--r--   0        0        0     2711 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
--rw-r--r--   0        0        0     7396 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
--rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
--rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
--rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
--rw-r--r--   0        0        0     5606 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
--rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
--rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
--rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
--rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
--rw-r--r--   0        0        0      342 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/build.gradle
--rw-r--r--   0        0        0    59203 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradle.properties
--rwxr-xr-x   0        0        0     5766 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradlew
--rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradlew.bat
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/.gitignore
--rw-r--r--   0        0        0     2170 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/build.gradle
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/AndroidManifest.xml
--rw-r--r--   0        0        0     6498 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/LibWhisper.kt
--rw-r--r--   0        0        0     2523 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/WhisperCpuConfig.kt
--rw-r--r--   0        0        0     2364 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/CMakeLists.txt
--rw-r--r--   0        0        0     8974 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/jni.c
--rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/settings.gradle
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/.gitignore
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/README.md
--rw-r--r--   0        0        0    68988 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/README_files/1.jpg
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/.gitignore
--rw-r--r--   0        0        0     1505 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/build.gradle
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/proguard-rules.pro
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/androidTest/java/com/litongjava/whisper/android/java/ExampleInstrumentedTest.java
--rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/AndroidManifest.xml
--rw-r--r--   0        0        0     1960 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/assets/logback.xml
--rw-r--r--   0        0        0     3266 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/MainActivity.java
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/app/App.java
--rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/bean/WhisperSegment.java
--rw-r--r--   0        0        0     3001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/services/WhisperService.java
--rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/single/LocalWhisper.java
--rw-r--r--   0        0        0      947 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/LoadModelTask.java
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/TranscriptionTask.java
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/AssetUtils.java
--rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/WaveEncoder.java
--rw-r--r--   0        0        0     3838 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/CpuInfo.java
--rw-r--r--   0        0        0     4788 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperContext.java
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperCpuConfig.java
--rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperLib.java
--rw-r--r--   0        0        0      792 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperUtils.java
--rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/CMakeLists.txt
--rw-r--r--   0        0        0     8810 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/jni.c
--rw-r--r--   0        0        0     5012 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0        0        0     1550 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable-v24/ic_launcher_foreground.xml
--rw-r--r--   0        0        0     1735 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/layout/activity_main.xml
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-anydpi-v26/ic_launcher.xml
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-anydpi-v26/ic_launcher_round.xml
--rw-r--r--   0        0        0     3593 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher.png
--rw-r--r--   0        0        0     5339 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher_round.png
--rw-r--r--   0        0        0     2636 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher.png
--rw-r--r--   0        0        0     3388 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher_round.png
--rw-r--r--   0        0        0     4926 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher.png
--rw-r--r--   0        0        0     7472 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png
--rw-r--r--   0        0        0     7909 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
--rw-r--r--   0        0        0    11873 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png
--rw-r--r--   0        0        0    10652 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
--rw-r--r--   0        0        0    16570 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png
--rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/colors.xml
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/strings.xml
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/themes.xml
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values-night/themes.xml
--rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/test/java/com/litongjava/whisper/android/java/ExampleUnitTest.java
--rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/build.gradle
--rw-r--r--   0        0        0    54329 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradle.properties
--rw-r--r--   0        0        0     5296 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradlew
--rw-r--r--   0        0        0     2176 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradlew.bat
--rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/settings.gradle
--rw-r--r--   0        0        0     3766 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.nvim/README.md
--rwxr-xr-x   0        0        0     2035 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim
--rw-r--r--   0        0        0     2278 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/README.md
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
--rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
--rw-r--r--   0        0        0     1665 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0        0        0     8419 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
--rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
--rw-r--r--   0        0        0     2138 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
--rw-r--r--   0        0        0      761 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
--rw-r--r--   0        0        0     9653 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
--rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
--rw-r--r--   0        0        0    24327 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/.gitignore
--rw-r--r--   0        0        0     1410 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/README.md
--rw-r--r--   0        0        0     2492 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
--rw-r--r--   0        0        0     4966 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/Contents.json
--rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/Contents.json
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/Contents.json
--rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/WhisperCppDemo.entitlements
--rw-r--r--   0        0        0     1323 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
--rw-r--r--   0        0        0     1065 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
--rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
--rw-r--r--   0        0        0    19593 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
--rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
--rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0        0        0     3896 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
--rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
--rw-r--r--   0        0        0     1802 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/README.md
--rw-r--r--   0        0        0     3660 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp
--rw-r--r--   0        0        0    33017 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html
--rwxr-xr-x   0        0        0     6932 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/yt-wsp.sh
--rw-r--r--   0        0        0    36901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-alloc.c
--rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-alloc.h
--rw-r--r--   0        0        0     7001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-backend-impl.h
--rw-r--r--   0        0        0    77427 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-backend.c
--rw-r--r--   0        0        0    13346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-backend.h
--rw-r--r--   0        0        0   133178 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-common.h
--rw-r--r--   0        0        0     1974 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/acc.cu
--rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/acc.cuh
--rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/arange.cu
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/arange.cuh
--rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/argsort.cu
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/argsort.cuh
--rw-r--r--   0        0        0    10529 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/binbcast.cu
--rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/binbcast.cuh
--rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/clamp.cu
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/clamp.cuh
--rw-r--r--   0        0        0    23537 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/common.cuh
--rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/concat.cu
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/concat.cuh
--rw-r--r--   0        0        0    29213 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/convert.cu
--rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/convert.cuh
--rw-r--r--   0        0        0    20414 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/cpy.cu
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/cpy.cuh
--rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/dequantize.cuh
--rw-r--r--   0        0        0     1760 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/diagmask.cu
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/diagmask.cuh
--rw-r--r--   0        0        0    32890 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/dmmv.cu
--rw-r--r--   0        0        0      584 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/dmmv.cuh
--rw-r--r--   0        0        0     1884 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-common.cuh
--rw-r--r--   0        0        0    15023 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-vec-f16.cu
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-vec-f16.cuh
--rw-r--r--   0        0        0    13073 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-vec-f32.cu
--rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-vec-f32.cuh
--rw-r--r--   0        0        0    28733 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn.cu
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn.cuh
--rw-r--r--   0        0        0     7032 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/getrows.cu
--rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/getrows.cuh
--rw-r--r--   0        0        0     4554 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/im2col.cu
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/im2col.cuh
--rw-r--r--   0        0        0    86698 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/mmq.cu
--rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/mmq.cuh
--rw-r--r--   0        0        0    18193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/mmvq.cu
--rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/mmvq.cuh
--rw-r--r--   0        0        0     7011 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/norm.cu
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/norm.cuh
--rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/pad.cu
--rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/pad.cuh
--rw-r--r--   0        0        0     3306 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/pool2d.cu
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/pool2d.cuh
--rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/quantize.cu
--rw-r--r--   0        0        0      200 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/quantize.cuh
--rw-r--r--   0        0        0    12159 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/rope.cu
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/rope.cuh
--rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/scale.cu
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/scale.cuh
--rw-r--r--   0        0        0     7831 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/softmax.cu
--rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/softmax.cuh
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/sumrows.cu
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/sumrows.cuh
--rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/tsembd.cu
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/tsembd.cuh
--rw-r--r--   0        0        0     9476 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/unary.cu
--rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/unary.cuh
--rw-r--r--   0        0        0     1866 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/upscale.cu
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/upscale.cuh
--rw-r--r--   0        0        0    45188 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/vecdotq.cuh
--rw-r--r--   0        0        0   120299 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda.cu
--rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda.h
--rw-r--r--   0        0        0    16658 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-impl.h
--rw-r--r--   0        0        0    79907 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-kompute.cpp
--rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-kompute.h
--rw-r--r--   0        0        0     2316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-metal.h
--rw-r--r--   0        0        0   187040 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-metal.m
--rw-r--r--   0        0        0    85950 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-opencl.cpp
--rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-opencl.h
--rw-r--r--   0        0        0   633755 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-quants.c
--rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-quants.h
--rw-r--r--   0        0        0    39412 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-rpc.cpp
--rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-rpc.h
--rw-r--r--   0        0        0   698932 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-sycl.cpp
--rw-r--r--   0        0        0     1909 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-sycl.h
--rw-r--r--   0        0        0   390265 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-vulkan.cpp
--rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-vulkan.h
--rw-r--r--   0        0        0   758065 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml.c
--rw-r--r--   0        0        0    89614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml.h
--rw-r--r--   0        0        0     2329 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/grammars/assistant.gbnf
--rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/grammars/chess.gbnf
--rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/grammars/colors.gbnf
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/.gitignore
--rw-r--r--   0        0        0     5505 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/README.md
--rw-r--r--   0        0        0     4863 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-h5-to-coreml.py
--rw-r--r--   0        0        0     7376 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-h5-to-ggml.py
--rw-r--r--   0        0        0    10613 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-pt-to-ggml.py
--rw-r--r--   0        0        0    12443 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-whisper-to-coreml.py
--rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-whisper-to-openvino.py
--rwxr-xr-x   0        0        0     2283 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/download-coreml-model.sh
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/download-ggml-model.cmd
--rwxr-xr-x   0        0        0     2917 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/download-ggml-model.sh
--rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-base.bin
--rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin
--rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-large.bin
--rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-medium.bin
--rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin
--rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-small.bin
--rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin
--rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin
--rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin
--rwxr-xr-x   0        0        0     1477 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/generate-coreml-interface.sh
--rwxr-xr-x   0        0        0     1319 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/generate-coreml-model.sh
--rw-r--r--   0        0        0     3602 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/ggml_to_pt.py
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/requirements-coreml.txt
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/requirements-openvino.txt
--rw-r--r--   0        0        0     3988 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/openvino/whisper-openvino-encoder.cpp
--rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/openvino/whisper-openvino-encoder.h
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/samples/.gitignore
--rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/samples/README.md
--rw-r--r--   0        0        0    76447 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/samples/jfk.mp3
--rw-r--r--   0        0        0   352078 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/samples/jfk.wav
--rw-r--r--   0        0        0    20521 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench-all-gg.txt
--rwxr-xr-x   0        0        0     3487 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench-all.sh
--rwxr-xr-x   0        0        0     2113 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench-wts.sh
--rw-r--r--   0        0        0     6850 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench.py
--rwxr-xr-x   0        0        0      311 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/convert-all.sh
--rwxr-xr-x   0        0        0     1154 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/deploy-wasm.sh
--rwxr-xr-x   0        0        0      337 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/gen-authors.sh
--rwxr-xr-x   0        0        0      843 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/quantize-all.sh
--rwxr-xr-x   0        0        0      134 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sha-all.sh
--rwxr-xr-x   0        0        0     7114 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sync-ggml-am.sh
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sync-ggml.last
--rwxr-xr-x   0        0        0     2481 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sync-ggml.sh
--rwxr-xr-x   0        0        0      445 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sync-llama.sh
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/spm-headers/ggml.h -> ../ggml.h
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/spm-headers/whisper.h -> ../whisper.h
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/.gitignore
--rw-r--r--   0        0        0     3125 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/CMakeLists.txt
--rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/en-0-ref.txt
--rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/en-1-ref.txt
--rw-r--r--   0        0        0      957 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/en-2-ref.txt
--rw-r--r--   0        0        0     1945 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/es-0-ref.txt
--rwxr-xr-x   0        0        0     3446 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/run-tests.sh
--rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/test-whisper.js
--rw-r--r--   0        0        0   262486 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/whisper.cpp
--rw-r--r--   0        0        0    31901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/vendor/whisper.cpp/whisper.h
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/whisper_cpp/__init__.py
--rw-r--r--   0        0        0     7375 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/whisper_cpp/whisper.py
--rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1657 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/.gitignore
+-rw-r--r--   0        0        0      108 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/.gitmodules
+-rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/CMakeLists.txt
+-rw-r--r--   0        0        0    11358 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/LICENSE
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/README.md
+-rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.devops/cublas.Dockerfile
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.devops/main-cuda.Dockerfile
+-rw-r--r--   0        0        0      402 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.devops/main.Dockerfile
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.git
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/bindings-go.yml
+-rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/bindings-ruby.yml
+-rw-r--r--   0        0        0    19410 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1715 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/examples.yml
+-rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.gitignore
+-rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.gitmodules
+-rw-r--r--   0        0        0    12824 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/AUTHORS
+-rw-r--r--   0        0        0    29517 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/CMakeLists.txt
+-rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/LICENSE
+-rw-r--r--   0        0        0    18797 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/Makefile
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/Package.swift
+-rw-r--r--   0        0        0    39837 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/README.md
+-rw-r--r--   0        0        0     6835 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/README_sycl.md
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/CMakeLists.txt
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/.gitignore
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/LICENSE
+-rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/Makefile
+-rw-r--r--   0        0        0     2825 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/README.md
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/doc.go
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go
+-rw-r--r--   0        0        0     5343 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go
+-rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go
+-rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go
+-rw-r--r--   0        0        0      878 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go
+-rw-r--r--   0        0        0     3295 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/go.mod
+-rw-r--r--   0        0        0     2019 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/go.sum
+-rw-r--r--   0        0        0     3812 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/params.go
+-rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go
+-rw-r--r--   0        0        0     8443 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go
+-rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/doc.go
+-rw-r--r--   0        0        0     3280 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go
+-rw-r--r--   0        0        0   352078 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/samples/jfk.wav
+-rw-r--r--   0        0        0    16147 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/whisper.go
+-rw-r--r--   0        0        0     2815 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/whisper_test.go
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/.git
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/.github/workflows/swift.yml
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/.gitignore
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/LICENSE
+-rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Makefile
+-rw-r--r--   0        0        0     1453 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Makefile-tmpl
+-rw-r--r--   0        0        0     2754 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Package.swift
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/README.md
+-rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m
+-rw-r--r--   0        0        0      937 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift
+-rw-r--r--   0        0        0     7458 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.h
+-rw-r--r--   0        0        0     8817 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.m
+-rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.h
+-rw-r--r--   0        0        0     8522 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.m
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.h
+-rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.mm
+-rw-r--r--   0        0        0    36901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.c
+-rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.h
+-rw-r--r--   0        0        0     7001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend-impl.h
+-rw-r--r--   0        0        0    77427 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.c
+-rw-r--r--   0        0        0    13346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.h
+-rw-r--r--   0        0        0   133178 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-common.h
+-rw-r--r--   0        0        0    16658 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-impl.h
+-rw-r--r--   0        0        0     2316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.h
+-rw-r--r--   0        0        0   187040 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.m
+-rw-r--r--   0        0        0   633755 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.c
+-rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.h
+-rw-r--r--   0        0        0   758065 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c
+-rw-r--r--   0        0        0    89614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/ggml.h
+-rw-r--r--   0        0        0    31901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h
+-rw-r--r--   0        0        0   262486 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp
+-rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/publish-trigger
+-rw-r--r--   0        0        0     8915 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/.idea/uiDesigner.xml
+-rw-r--r--   0        0        0     2354 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/README.md
+-rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/build.gradle
+-rw-r--r--   0        0        0    61608 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradle.properties
+-rw-r--r--   0        0        0     8495 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradlew
+-rw-r--r--   0        0        0     2868 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradlew.bat
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/settings.gradle
+-rw-r--r--   0        0        0     1338 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperContext.java
+-rw-r--r--   0        0        0     7464 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCpp.java
+-rw-r--r--   0        0        0    16263 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCppJnaLibrary.java
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/bean/WhisperSegment.java
+-rw-r--r--   0        0        0      801 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperEncoderBeginCallback.java
+-rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperLogitsFilterCallback.java
+-rw-r--r--   0        0        0      811 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperNewSegmentCallback.java
+-rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperProgressCallback.java
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/ggml/GgmlTensor.java
+-rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/ggml/GgmlType.java
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/EModel.java
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModel.java
+-rw-r--r--   0        0        0     1605 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModelLoader.java
+-rw-r--r--   0        0        0       81 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperState.java
+-rw-r--r--   0        0        0     1194 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperTokenData.java
+-rw-r--r--   0        0        0      586 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/BeamSearchParams.java
+-rw-r--r--   0        0        0      676 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/CBool.java
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/GreedyParams.java
+-rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperContextParams.java
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperFilters.java
+-rw-r--r--   0        0        0    11673 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperFullParams.java
+-rw-r--r--   0        0        0      406 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperHParams.java
+-rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperSamplingStrategy.java
+-rw-r--r--   0        0        0     5968 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperCppTest.java
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperJnaLibraryTest.java
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/.gitignore
+-rw-r--r--   0        0        0      991 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt
+-rw-r--r--   0        0        0     2546 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/README.md
+-rw-r--r--   0        0        0     3048 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/emscripten.cpp
+-rw-r--r--   0        0        0     2907 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/package-tmpl.json
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/package.json
+-rw-r--r--   0        0        0   960825 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/whisper.js
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/Rakefile
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/.gitignore
+-rw-r--r--   0        0        0     1532 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb
+-rw-r--r--   0        0        0     7001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend-impl.h
+-rw-r--r--   0        0        0    77241 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.c
+-rw-r--r--   0        0        0    13346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.h
+-rw-r--r--   0        0        0   133178 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-common.h
+-rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-cuda.h
+-rw-r--r--   0        0        0     8298 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-impl.h
+-rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-kompute.h
+-rw-r--r--   0        0        0     2316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-metal.h
+-rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-opencl.h
+-rw-r--r--   0        0        0   526217 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.c
+-rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.h
+-rw-r--r--   0        0        0     1909 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-sycl.h
+-rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-vulkan.h
+-rw-r--r--   0        0        0    15354 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
+-rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
+-rw-r--r--   0        0        0     3444 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/whispercpp.gemspec
+-rw-r--r--   0        0        0     2037 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/BuildTypes.cmake
+-rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/DefaultTargetOptions.cmake
+-rw-r--r--   0        0        0     6234 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/FindFFmpeg.cmake
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/GitVars.cmake
+-rw-r--r--   0        0        0     7458 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-decoder-impl.h
+-rw-r--r--   0        0        0     8817 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-decoder-impl.m
+-rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder-impl.h
+-rw-r--r--   0        0        0     8522 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder-impl.m
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder.h
+-rw-r--r--   0        0        0     2224 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder.mm
+-rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/CMakeLists.txt
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/.gitignore
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/README.md
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
+-rw-r--r--   0        0        0    13407 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/addon.cpp
+-rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/index.js
+-rw-r--r--   0        0        0      285 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/package.json
+-rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench/CMakeLists.txt
+-rw-r--r--   0        0        0     1978 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench/README.md
+-rw-r--r--   0        0        0     6313 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench/bench.cpp
+-rw-r--r--   0        0        0     1161 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/README.md
+-rw-r--r--   0        0        0     2713 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp
+-rw-r--r--   0        0        0    12516 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command/CMakeLists.txt
+-rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command/README.md
+-rw-r--r--   0        0        0    30594 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command/command.cpp
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command/commands.txt
+-rw-r--r--   0        0        0     1181 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt
+-rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/README.md
+-rw-r--r--   0        0        0    10458 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp
+-rw-r--r--   0        0        0    16219 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html
+-rw-r--r--   0        0        0     8467 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-ggml.cpp
+-rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-ggml.h
+-rw-r--r--   0        0        0     6670 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-sdl.cpp
+-rw-r--r--   0        0        0      975 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-sdl.h
+-rw-r--r--   0        0        0    31348 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common.cpp
+-rw-r--r--   0        0        0     9571 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common.h
+-rw-r--r--   0        0        0   241358 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/dr_wav.h
+-rw-r--r--   0        0        0     9366 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/ffmpeg-transcode.cpp
+-rwxr-xr-x   0        0        0     1197 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/generate-karaoke.sh
+-rw-r--r--   0        0        0    17665 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/grammar-parser.cpp
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/grammar-parser.h
+-rw-r--r--   0        0        0     6521 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/helpers.js
+-rw-r--r--   0        0        0   907858 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/json.hpp
+-rwxr-xr-x   0        0        0     2969 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/livestream.sh
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/CMakeLists.txt
+-rw-r--r--   0        0        0     6120 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/README.md
+-rw-r--r--   0        0        0    21186 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/lsp.cpp
+-rw-r--r--   0        0        0    15906 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/whisper.vim
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/main/CMakeLists.txt
+-rw-r--r--   0        0        0     3479 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/main/README.md
+-rw-r--r--   0        0        0    54197 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/main/main.cpp
+-rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/python/test_whisper_processor.py
+-rw-r--r--   0        0        0     1775 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/python/whisper_processor.py
+-rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/quantize/CMakeLists.txt
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/quantize/README.md
+-rw-r--r--   0        0        0     8150 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/quantize/quantize.cpp
+-rw-r--r--   0        0        0      261 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/CMakeLists.txt
+-rw-r--r--   0        0        0     3414 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/README.md
+-rw-r--r--   0        0        0   302116 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/httplib.h
+-rw-r--r--   0        0        0    44370 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/server.cpp
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream/CMakeLists.txt
+-rw-r--r--   0        0        0     2281 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream/README.md
+-rw-r--r--   0        0        0    18179 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream/stream.cpp
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt
+-rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/README.md
+-rw-r--r--   0        0        0     6197 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp
+-rw-r--r--   0        0        0    16188 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/CMakeLists.txt
+-rw-r--r--   0        0        0     1510 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/README.md
+-rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/build.sh
+-rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/ls-sycl-device.cpp
+-rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/run-whisper.sh
+-rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/.gitignore
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/CMakeLists.txt
+-rw-r--r--   0        0        0     1423 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/README.md
+-rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/eleven-labs.py
+-rw-r--r--   0        0        0    27930 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/gpt-2.cpp
+-rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/gpt-2.h
+-rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/speak
+-rw-r--r--   0        0        0       70 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/speak.bat
+-rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/speak.ps1
+-rw-r--r--   0        0        0    15579 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/talk.cpp
+-rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/.gitignore
+-rw-r--r--   0        0        0      643 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt
+-rw-r--r--   0        0        0     2801 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/README.md
+-rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py
+-rw-r--r--   0        0        0   739022 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/llama.cpp
+-rw-r--r--   0        0        0    53493 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/llama.h
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
+-rwxr-xr-x   0        0        0     1494 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/speak
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/speak.bat
+-rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/speak.ps1
+-rw-r--r--   0        0        0    33891 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp
+-rw-r--r--   0        0        0   223121 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode-data.cpp
+-rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode-data.h
+-rw-r--r--   0        0        0    30620 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode.cpp
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode.h
+-rw-r--r--   0        0        0     1171 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt
+-rw-r--r--   0        0        0     3341 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/README.md
+-rw-r--r--   0        0        0    11996 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp
+-rw-r--r--   0        0        0    27895 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp
+-rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h
+-rw-r--r--   0        0        0    33143 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html
+-rwxr-xr-x   0        0        0     2771 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/twitch.sh
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/CMakeLists.txt
+-rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/README.md
+-rw-r--r--   0        0        0      344 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/CMakeLists.txt
+-rw-r--r--   0        0        0    26777 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.cpp
+-rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.h
+-rw-r--r--   0        0        0     6625 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/WChess.cpp
+-rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/WChess.h
+-rw-r--r--   0        0        0     4362 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/test-chessboard.cpp
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.cmd/CMakeLists.txt
+-rw-r--r--   0        0        0    10826 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.cmd/wchess.cmd.cpp
+-rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/CMakeLists.txt
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.css
+-rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.min.css
+-rw-r--r--   0        0        0     1405 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bB.png
+-rw-r--r--   0        0        0     3009 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bK.png
+-rw-r--r--   0        0        0     1875 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bN.png
+-rw-r--r--   0        0        0      777 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bP.png
+-rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bQ.png
+-rw-r--r--   0        0        0      748 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bR.png
+-rw-r--r--   0        0        0     2374 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wB.png
+-rw-r--r--   0        0        0     2823 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wK.png
+-rw-r--r--   0        0        0     2388 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wN.png
+-rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wP.png
+-rw-r--r--   0        0        0     3812 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wQ.png
+-rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wR.png
+-rw-r--r--   0        0        0     1064 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2605 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/README.md
+-rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/package.json
+-rw-r--r--   0        0        0    53836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.js
+-rw-r--r--   0        0        0    14470 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.min.js
+-rw-r--r--   0        0        0    19233 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/index-tmpl.html
+-rw-r--r--   0        0        0    87533 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/jquery-3.7.1.min.js
+-rw-r--r--   0        0        0     4173 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/wchess.wasm.cpp
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.gitignore
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/.gitignore
+-rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/.name
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/compiler.xml
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml
+-rw-r--r--   0        0        0      448 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/misc.xml
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/vcs.xml
+-rw-r--r--   0        0        0     2367 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/README.md
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/.gitignore
+-rw-r--r--   0        0        0     1966 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/build.gradle
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
+-rw-r--r--   0        0        0      663 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
+-rw-r--r--   0        0        0     1124 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
+-rw-r--r--   0        0        0     2259 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
+-rw-r--r--   0        0        0     2711 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
+-rw-r--r--   0        0        0     7396 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
+-rw-r--r--   0        0        0      282 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
+-rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
+-rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
+-rw-r--r--   0        0        0     5606 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
+-rw-r--r--   0        0        0      272 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
+-rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
+-rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
+-rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
+-rw-r--r--   0        0        0      342 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/build.gradle
+-rw-r--r--   0        0        0    59203 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradle.properties
+-rwxr-xr-x   0        0        0     5766 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradlew
+-rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradlew.bat
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/.gitignore
+-rw-r--r--   0        0        0     2170 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/build.gradle
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/AndroidManifest.xml
+-rw-r--r--   0        0        0     6498 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/LibWhisper.kt
+-rw-r--r--   0        0        0     2523 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/WhisperCpuConfig.kt
+-rw-r--r--   0        0        0     2364 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/CMakeLists.txt
+-rw-r--r--   0        0        0     8974 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/jni.c
+-rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/settings.gradle
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/.gitignore
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/README.md
+-rw-r--r--   0        0        0    68988 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/README_files/1.jpg
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/.gitignore
+-rw-r--r--   0        0        0     1505 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/build.gradle
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/proguard-rules.pro
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/androidTest/java/com/litongjava/whisper/android/java/ExampleInstrumentedTest.java
+-rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/AndroidManifest.xml
+-rw-r--r--   0        0        0     1960 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/assets/logback.xml
+-rw-r--r--   0        0        0     3266 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/MainActivity.java
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/app/App.java
+-rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/bean/WhisperSegment.java
+-rw-r--r--   0        0        0     3001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/services/WhisperService.java
+-rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/single/LocalWhisper.java
+-rw-r--r--   0        0        0      947 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/LoadModelTask.java
+-rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/TranscriptionTask.java
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/AssetUtils.java
+-rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/WaveEncoder.java
+-rw-r--r--   0        0        0     3838 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/CpuInfo.java
+-rw-r--r--   0        0        0     4788 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperContext.java
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperCpuConfig.java
+-rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperLib.java
+-rw-r--r--   0        0        0      792 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperUtils.java
+-rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/CMakeLists.txt
+-rw-r--r--   0        0        0     8810 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/jni.c
+-rw-r--r--   0        0        0     5012 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-r--r--   0        0        0     1550 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable-v24/ic_launcher_foreground.xml
+-rw-r--r--   0        0        0     1735 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/layout/activity_main.xml
+-rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-anydpi-v26/ic_launcher.xml
+-rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-anydpi-v26/ic_launcher_round.xml
+-rw-r--r--   0        0        0     3593 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher.png
+-rw-r--r--   0        0        0     5339 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher_round.png
+-rw-r--r--   0        0        0     2636 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher.png
+-rw-r--r--   0        0        0     3388 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher_round.png
+-rw-r--r--   0        0        0     4926 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher.png
+-rw-r--r--   0        0        0     7472 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png
+-rw-r--r--   0        0        0     7909 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher.png
+-rw-r--r--   0        0        0    11873 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png
+-rw-r--r--   0        0        0    10652 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png
+-rw-r--r--   0        0        0    16570 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/colors.xml
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/strings.xml
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/themes.xml
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values-night/themes.xml
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/test/java/com/litongjava/whisper/android/java/ExampleUnitTest.java
+-rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/build.gradle
+-rw-r--r--   0        0        0    54329 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0        0        0     1093 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradle.properties
+-rw-r--r--   0        0        0     5296 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradlew
+-rw-r--r--   0        0        0     2176 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradlew.bat
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/settings.gradle
+-rw-r--r--   0        0        0     3766 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.nvim/README.md
+-rwxr-xr-x   0        0        0     2035 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim
+-rw-r--r--   0        0        0     2278 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/README.md
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
+-rw-r--r--   0        0        0     1320 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
+-rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
+-rw-r--r--   0        0        0     1665 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
+-rw-r--r--   0        0        0     8419 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
+-rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
+-rw-r--r--   0        0        0     2138 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
+-rw-r--r--   0        0        0      761 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
+-rw-r--r--   0        0        0     9653 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
+-rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
+-rw-r--r--   0        0        0    24327 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/.gitignore
+-rw-r--r--   0        0        0     1410 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/README.md
+-rw-r--r--   0        0        0     2492 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
+-rw-r--r--   0        0        0     4966 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/Contents.json
+-rw-r--r--   0        0        0      999 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/Contents.json
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/Contents.json
+-rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/WhisperCppDemo.entitlements
+-rw-r--r--   0        0        0     1323 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
+-rw-r--r--   0        0        0     1065 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
+-rw-r--r--   0        0        0      394 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
+-rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
+-rw-r--r--   0        0        0    19593 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0        0        0     3896 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
+-rw-r--r--   0        0        0     1802 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/README.md
+-rw-r--r--   0        0        0     3660 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp
+-rw-r--r--   0        0        0    33017 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html
+-rwxr-xr-x   0        0        0     6932 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/yt-wsp.sh
+-rw-r--r--   0        0        0    36901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-alloc.c
+-rw-r--r--   0        0        0     2995 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-alloc.h
+-rw-r--r--   0        0        0     7001 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-backend-impl.h
+-rw-r--r--   0        0        0    77427 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-backend.c
+-rw-r--r--   0        0        0    13346 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-backend.h
+-rw-r--r--   0        0        0   133178 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-common.h
+-rw-r--r--   0        0        0     1974 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/acc.cu
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/acc.cuh
+-rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/arange.cu
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/arange.cuh
+-rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/argsort.cu
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/argsort.cuh
+-rw-r--r--   0        0        0    10529 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/binbcast.cu
+-rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/binbcast.cuh
+-rw-r--r--   0        0        0     1164 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/clamp.cu
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/clamp.cuh
+-rw-r--r--   0        0        0    23537 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/common.cuh
+-rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/concat.cu
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/concat.cuh
+-rw-r--r--   0        0        0    29213 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/convert.cu
+-rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/convert.cuh
+-rw-r--r--   0        0        0    20414 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/cpy.cu
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/cpy.cuh
+-rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/dequantize.cuh
+-rw-r--r--   0        0        0     1760 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/diagmask.cu
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/diagmask.cuh
+-rw-r--r--   0        0        0    32890 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/dmmv.cu
+-rw-r--r--   0        0        0      584 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/dmmv.cuh
+-rw-r--r--   0        0        0     1884 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-common.cuh
+-rw-r--r--   0        0        0    15023 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-vec-f16.cu
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-vec-f16.cuh
+-rw-r--r--   0        0        0    13073 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-vec-f32.cu
+-rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-vec-f32.cuh
+-rw-r--r--   0        0        0    28733 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn.cu
+-rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn.cuh
+-rw-r--r--   0        0        0     7032 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/getrows.cu
+-rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/getrows.cuh
+-rw-r--r--   0        0        0     4554 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/im2col.cu
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/im2col.cuh
+-rw-r--r--   0        0        0    86698 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/mmq.cu
+-rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/mmq.cuh
+-rw-r--r--   0        0        0    18193 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/mmvq.cu
+-rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/mmvq.cuh
+-rw-r--r--   0        0        0     7011 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/norm.cu
+-rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/norm.cuh
+-rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/pad.cu
+-rw-r--r--   0        0        0      131 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/pad.cuh
+-rw-r--r--   0        0        0     3306 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/pool2d.cu
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/pool2d.cuh
+-rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/quantize.cu
+-rw-r--r--   0        0        0      200 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/quantize.cuh
+-rw-r--r--   0        0        0    12159 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/rope.cu
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/rope.cuh
+-rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/scale.cu
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/scale.cuh
+-rw-r--r--   0        0        0     7831 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/softmax.cu
+-rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/softmax.cuh
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/sumrows.cu
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/sumrows.cuh
+-rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/tsembd.cu
+-rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/tsembd.cuh
+-rw-r--r--   0        0        0     9476 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/unary.cu
+-rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/unary.cuh
+-rw-r--r--   0        0        0     1866 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/upscale.cu
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/upscale.cuh
+-rw-r--r--   0        0        0    45188 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/vecdotq.cuh
+-rw-r--r--   0        0        0   120299 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda.cu
+-rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda.h
+-rw-r--r--   0        0        0    16658 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-impl.h
+-rw-r--r--   0        0        0    79907 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-kompute.cpp
+-rw-r--r--   0        0        0     1029 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-kompute.h
+-rw-r--r--   0        0        0     2316 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-metal.h
+-rw-r--r--   0        0        0   187040 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-metal.m
+-rw-r--r--   0        0        0    85950 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-opencl.cpp
+-rw-r--r--   0        0        0     1386 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-opencl.h
+-rw-r--r--   0        0        0   633755 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-quants.c
+-rw-r--r--   0        0        0    11794 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-quants.h
+-rw-r--r--   0        0        0    39412 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-rpc.cpp
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-rpc.h
+-rw-r--r--   0        0        0   698932 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-sycl.cpp
+-rw-r--r--   0        0        0     1909 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-sycl.h
+-rw-r--r--   0        0        0   390265 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-vulkan.cpp
+-rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-vulkan.h
+-rw-r--r--   0        0        0   758065 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml.c
+-rw-r--r--   0        0        0    89614 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml.h
+-rw-r--r--   0        0        0     2329 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/grammars/assistant.gbnf
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/grammars/chess.gbnf
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/grammars/colors.gbnf
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/.gitignore
+-rw-r--r--   0        0        0     5505 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/README.md
+-rw-r--r--   0        0        0     4863 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-h5-to-coreml.py
+-rw-r--r--   0        0        0     7376 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-h5-to-ggml.py
+-rw-r--r--   0        0        0    10613 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-pt-to-ggml.py
+-rw-r--r--   0        0        0    12443 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-whisper-to-coreml.py
+-rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-whisper-to-openvino.py
+-rwxr-xr-x   0        0        0     2283 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/download-coreml-model.sh
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/download-ggml-model.cmd
+-rwxr-xr-x   0        0        0     2917 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/download-ggml-model.sh
+-rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-base.bin
+-rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin
+-rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-large.bin
+-rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-medium.bin
+-rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin
+-rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-small.bin
+-rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin
+-rw-r--r--   0        0        0   575451 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin
+-rw-r--r--   0        0        0   586836 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin
+-rwxr-xr-x   0        0        0     1477 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/generate-coreml-interface.sh
+-rwxr-xr-x   0        0        0     1319 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/generate-coreml-model.sh
+-rw-r--r--   0        0        0     3602 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/ggml_to_pt.py
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/requirements-coreml.txt
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/requirements-openvino.txt
+-rw-r--r--   0        0        0     3988 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/openvino/whisper-openvino-encoder.cpp
+-rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/openvino/whisper-openvino-encoder.h
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/samples/.gitignore
+-rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/samples/README.md
+-rw-r--r--   0        0        0    76447 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/samples/jfk.mp3
+-rw-r--r--   0        0        0   352078 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/samples/jfk.wav
+-rw-r--r--   0        0        0    20521 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench-all-gg.txt
+-rwxr-xr-x   0        0        0     3487 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench-all.sh
+-rwxr-xr-x   0        0        0     2113 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench-wts.sh
+-rw-r--r--   0        0        0     6850 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench.py
+-rwxr-xr-x   0        0        0      311 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/convert-all.sh
+-rwxr-xr-x   0        0        0     1154 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/deploy-wasm.sh
+-rwxr-xr-x   0        0        0      337 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/gen-authors.sh
+-rwxr-xr-x   0        0        0      843 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/quantize-all.sh
+-rwxr-xr-x   0        0        0      134 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sha-all.sh
+-rwxr-xr-x   0        0        0     7114 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sync-ggml-am.sh
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sync-ggml.last
+-rwxr-xr-x   0        0        0     2481 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sync-ggml.sh
+-rwxr-xr-x   0        0        0      445 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sync-llama.sh
+lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/spm-headers/ggml.h -> ../ggml.h
+lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/spm-headers/whisper.h -> ../whisper.h
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/.gitignore
+-rw-r--r--   0        0        0     3125 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/en-0-ref.txt
+-rw-r--r--   0        0        0     2221 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/en-1-ref.txt
+-rw-r--r--   0        0        0      957 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/en-2-ref.txt
+-rw-r--r--   0        0        0     1945 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/es-0-ref.txt
+-rwxr-xr-x   0        0        0     3446 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/run-tests.sh
+-rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/test-whisper.js
+-rw-r--r--   0        0        0   262486 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/whisper.cpp
+-rw-r--r--   0        0        0    31901 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/whisper.h
+-rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/whisper_cpp/__init__.py
+-rw-r--r--   0        0        0     7375 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/whisper_cpp/whisper.py
+-rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 whisper_cpp_python_smr-0.2.1/PKG-INFO
```

### Comparing `whisper_cpp_python_smr-0.2/.github/workflows/wheels.yml` & `whisper_cpp_python_smr-0.2.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/LICENSE` & `whisper_cpp_python_smr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.devops/cublas.Dockerfile` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.devops/cublas.Dockerfile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.devops/main-cuda.Dockerfile` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.devops/main-cuda.Dockerfile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/build.yml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/docker.yml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.github/workflows/examples.yml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/.gitignore` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/.gitignore`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/AUTHORS` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/AUTHORS`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/LICENSE` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/Makefile` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/Package.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/Package.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/README_sycl.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/README_sycl.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/LICENSE` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/Makefile` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-model-download/context.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-model-download/main.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/color.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/flags.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/main.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/examples/go-whisper/process.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/go.sum` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/go.sum`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/params.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/params.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/consts.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/context.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/context_test.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/interface.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/pkg/whisper/model.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/samples/jfk.wav` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/whisper.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/whisper.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/go/whisper_test.go` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/go/whisper_test.go`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/LICENSE` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Makefile` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Makefile`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Makefile-tmpl` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Makefile-tmpl`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Package.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Package.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/test-objc/main.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/test-swift/main.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-decoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.mm` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/coreml/whisper-encoder.mm`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-alloc.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-backend.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-common.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-common.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-metal.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml-quants.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/ggml.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/ggml.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/ggml.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/include/whisper.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/Sources/whisper/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ios/models/for-tests-ggml-base.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/.idea/uiDesigner.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/.idea/uiDesigner.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/build.gradle` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/build.gradle`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradle/wrapper/gradle-wrapper.jar` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradlew` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradlew`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/gradlew.bat` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/gradlew.bat`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperContext.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperContext.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCpp.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCpp.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCppJnaLibrary.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/WhisperCppJnaLibrary.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/bean/WhisperSegment.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/bean/WhisperSegment.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperEncoderBeginCallback.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperEncoderBeginCallback.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperLogitsFilterCallback.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperLogitsFilterCallback.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperNewSegmentCallback.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperNewSegmentCallback.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperProgressCallback.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/callbacks/WhisperProgressCallback.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModel.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModel.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModelLoader.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperModelLoader.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperTokenData.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/model/WhisperTokenData.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/BeamSearchParams.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/BeamSearchParams.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/CBool.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/CBool.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperContextParams.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperContextParams.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperFullParams.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/main/java/io/github/ggerganov/whispercpp/params/WhisperFullParams.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperCppTest.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperCppTest.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperJnaLibraryTest.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/java/src/test/java/io/github/ggerganov/whispercpp/WhisperJnaLibraryTest.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/emscripten.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/libwhisper.worker.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/package-tmpl.json` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/package-tmpl.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/package.json` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/package.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/javascript/whisper.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/javascript/whisper.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/extconf.rb`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-backend.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-common.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-common.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-cuda.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-kompute.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-kompute.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-metal.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-metal.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-opencl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-quants.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-sycl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-sycl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ggml-vulkan.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ggml-vulkan.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/tests/test_whisper.rb`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/bindings/ruby/whispercpp.gemspec` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/bindings/ruby/whispercpp.gemspec`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/BuildTypes.cmake` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/FindFFmpeg.cmake` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/FindFFmpeg.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/cmake/GitVars.cmake` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-decoder-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-decoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-decoder-impl.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-decoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder-impl.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder-impl.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/coreml/whisper-encoder.mm` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/coreml/whisper-encoder.mm`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/__test__/whisper.spec.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/addon.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/addon.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/addon.node/index.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/addon.node/index.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench/bench.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench/bench.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/bench.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command/command.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command/command.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/command.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-ggml.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-ggml.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-sdl.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-sdl.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common-sdl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common-sdl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/common.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/common.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/dr_wav.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/ffmpeg-transcode.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/ffmpeg-transcode.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/generate-karaoke.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/generate-karaoke.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/grammar-parser.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/grammar-parser.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/grammar-parser.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/grammar-parser.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/helpers.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/helpers.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/json.hpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/json.hpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/livestream.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/livestream.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/lsp.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/lsp.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/lsp/whisper.vim` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/lsp/whisper.vim`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/main/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/main/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/main/main.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/main/main.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/python/whisper_processor.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/python/whisper_processor.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/quantize/quantize.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/quantize/quantize.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/httplib.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/httplib.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/server/server.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/server/server.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream/stream.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream/stream.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/stream.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/sycl/build.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/sycl/build.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/eleven-labs.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/gpt-2.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/gpt-2.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/speak` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/speak`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk/talk.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk/talk.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/llama.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/llama.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/llama.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/llama.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/speak` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/speak`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/talk-llama.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode-data.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode-data.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode-data.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode-data.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk-llama/unicode.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk-llama/unicode.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/talk.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/twitch.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/twitch.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/Chessboard.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/WChess.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/WChess.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/WChess.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/WChess.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/libwchess/test-chessboard.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/libwchess/test-chessboard.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.cmd/wchess.cmd.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.cmd/wchess.cmd.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.css` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.css`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.min.css` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/css/chessboard-1.0.0.min.css`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bB.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bB.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bK.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bK.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bN.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bN.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bP.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bP.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bQ.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bQ.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bR.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/bR.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wB.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wB.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wK.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wK.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wN.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wN.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wP.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wP.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wQ.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wQ.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wR.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/img/chesspieces/wikipedia/wR.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/CHANGELOG.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/LICENSE.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/package.json` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0/package.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.min.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/chessboardjs-1.0.0/js/chessboard-1.0.0.min.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/index-tmpl.html` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/jquery-3.7.1.min.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/wchess/wchess.wasm/wchess.wasm.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/wchess/wchess.wasm/wchess.wasm.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/.idea/gradle.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/build.gradle` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradle.properties` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradle.properties`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradlew` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradlew`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/gradlew.bat` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/gradlew.bat`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/build.gradle` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/build.gradle`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/LibWhisper.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/LibWhisper.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/WhisperCpuConfig.kt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/java/com/whispercpp/whisper/WhisperCpuConfig.kt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/jni.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android/lib/src/main/jni/whisper/jni.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/README_files/1.jpg` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/README_files/1.jpg`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/build.gradle` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/build.gradle`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/proguard-rules.pro` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/androidTest/java/com/litongjava/whisper/android/java/ExampleInstrumentedTest.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/androidTest/java/com/litongjava/whisper/android/java/ExampleInstrumentedTest.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/AndroidManifest.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/assets/logback.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/assets/logback.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/MainActivity.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/MainActivity.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/bean/WhisperSegment.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/bean/WhisperSegment.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/services/WhisperService.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/services/WhisperService.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/single/LocalWhisper.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/single/LocalWhisper.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/LoadModelTask.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/LoadModelTask.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/TranscriptionTask.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/task/TranscriptionTask.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/AssetUtils.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/AssetUtils.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/WaveEncoder.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/litongjava/whisper/android/java/utils/WaveEncoder.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/CpuInfo.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/CpuInfo.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperContext.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperContext.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperLib.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperLib.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperUtils.java` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/java/com/whispercpp/java/whisper/WhisperUtils.java`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/jni.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/jni/whisper/jni.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable/ic_launcher_background.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable-v24/ic_launcher_foreground.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/drawable-v24/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/layout/activity_main.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/layout/activity_main.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher_round.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-hdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher_round.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-mdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.png`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/themes.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values/themes.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values-night/themes.xml` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/app/src/main/res/values-night/themes.xml`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradle/wrapper/gradle-wrapper.jar` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradle.properties` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradle.properties`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradlew` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradlew`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.android.java/gradlew.bat` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.android.java/gradlew.bat`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.nvim/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.nvim/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.nvim/whisper.nvim`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/whisper.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/examples/yt-wsp.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/examples/yt-wsp.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-alloc.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-alloc.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-alloc.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-alloc.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-backend-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-backend-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-backend.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-backend.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-backend.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-backend.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-common.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-common.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/acc.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/acc.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/arange.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/arange.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/argsort.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/argsort.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/binbcast.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/binbcast.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/clamp.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/clamp.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/common.cuh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/common.cuh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/concat.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/concat.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/convert.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/convert.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/cpy.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/cpy.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/dequantize.cuh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/dequantize.cuh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/diagmask.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/diagmask.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/dmmv.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/dmmv.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/dmmv.cuh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/dmmv.cuh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-common.cuh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-common.cuh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-vec-f16.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-vec-f16.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn-vec-f32.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn-vec-f32.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/fattn.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/fattn.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/getrows.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/getrows.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/im2col.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/im2col.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/mmq.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/mmq.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/mmvq.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/mmvq.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/norm.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/norm.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/pad.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/pad.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/pool2d.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/pool2d.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/quantize.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/quantize.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/rope.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/rope.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/scale.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/scale.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/softmax.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/softmax.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/sumrows.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/sumrows.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/tsembd.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/tsembd.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/unary.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/unary.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/unary.cuh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/unary.cuh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/upscale.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/upscale.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda/vecdotq.cuh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda/vecdotq.cuh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda.cu` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-cuda.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-impl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-impl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-kompute.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-kompute.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-kompute.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-kompute.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-metal.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-metal.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-metal.m` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-metal.m`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-opencl.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-opencl.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-opencl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-quants.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-quants.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-quants.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-quants.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-rpc.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-rpc.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-rpc.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-rpc.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-sycl.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-sycl.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-sycl.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-sycl.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-vulkan.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-vulkan.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml-vulkan.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml-vulkan.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml.c` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml.c`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/ggml.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/ggml.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/grammars/assistant.gbnf` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/grammars/assistant.gbnf`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/grammars/chess.gbnf` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/grammars/chess.gbnf`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/README.md` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/README.md`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-h5-to-coreml.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-h5-to-coreml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-h5-to-ggml.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-pt-to-ggml.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-pt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-whisper-to-coreml.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-whisper-to-coreml.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/convert-whisper-to-openvino.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/convert-whisper-to-openvino.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/download-coreml-model.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/download-coreml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/download-ggml-model.cmd` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/download-ggml-model.cmd`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/download-ggml-model.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-base.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-base.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-base.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-large.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-large.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-medium.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-medium.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-medium.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-small.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-small.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-small.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-tiny.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/for-tests-ggml-tiny.en.bin`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/generate-coreml-interface.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/generate-coreml-interface.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/generate-coreml-model.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/generate-coreml-model.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/models/ggml_to_pt.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/models/ggml_to_pt.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/openvino/whisper-openvino-encoder.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/openvino/whisper-openvino-encoder.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/openvino/whisper-openvino-encoder.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/openvino/whisper-openvino-encoder.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/samples/jfk.mp3` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/samples/jfk.mp3`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/samples/jfk.wav` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench-all-gg.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench-all-gg.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench-all.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench-all.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench-wts.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench-wts.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/bench.py` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/bench.py`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/deploy-wasm.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/deploy-wasm.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/quantize-all.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/quantize-all.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sync-ggml-am.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sync-ggml-am.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/scripts/sync-ggml.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/scripts/sync-ggml.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/CMakeLists.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/en-0-ref.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/en-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/en-1-ref.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/en-1-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/en-2-ref.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/en-2-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/es-0-ref.txt` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/es-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/run-tests.sh` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/run-tests.sh`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/tests/test-whisper.js` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/tests/test-whisper.js`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/whisper.cpp` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/vendor/whisper.cpp/whisper.h` & `whisper_cpp_python_smr-0.2.1/vendor/whisper.cpp/whisper.h`

 * *Files identical despite different names*

### Comparing `whisper_cpp_python_smr-0.2/whisper_cpp/whisper.py` & `whisper_cpp_python_smr-0.2.1/whisper_cpp/whisper.py`

 * *Files identical despite different names*


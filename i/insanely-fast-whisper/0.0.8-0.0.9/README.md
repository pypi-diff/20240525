# Comparing `tmp/insanely_fast_whisper-0.0.8.tar.gz` & `tmp/insanely_fast_whisper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insanely_fast_whisper-0.0.8.tar", last modified: Wed Nov 22 19:29:54 2023, max compression
+gzip compressed data, was "insanely_fast_whisper-0.0.9.tar", last modified: Mon Nov 27 20:49:10 2023, max compression
```

## Comparing `insanely_fast_whisper-0.0.8.tar` & `insanely_fast_whisper-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-11-12 20:03:55.236316 insanely_fast_whisper-0.0.8/LICENSE
--rw-r--r--   0        0        0     6536 2023-11-22 19:29:00.892710 insanely_fast_whisper-0.0.8/README.md
--rw-r--r--   0        0        0      608 2023-11-22 19:29:54.424515 insanely_fast_whisper-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-05 17:51:43.860503 insanely_fast_whisper-0.0.8/src/insanely_fast_whisper/__init__.py
--rw-r--r--   0        0        0     3346 2023-11-22 19:29:00.892710 insanely_fast_whisper-0.0.8/src/insanely_fast_whisper/cli.py
--rw-r--r--   0        0        0        0 2023-11-05 17:51:43.860503 insanely_fast_whisper-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     6945 1970-01-01 00:00:00.000000 insanely_fast_whisper-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-12 20:03:55.236316 insanely_fast_whisper-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6736 2023-11-27 19:57:57.672665 insanely_fast_whisper-0.0.9/README.md
+-rw-r--r--   0        0        0      644 2023-11-27 20:49:10.739644 insanely_fast_whisper-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-05 17:51:43.860503 insanely_fast_whisper-0.0.9/src/insanely_fast_whisper/__init__.py
+-rw-r--r--   0        0        0     4962 2023-11-27 20:43:04.553293 insanely_fast_whisper-0.0.9/src/insanely_fast_whisper/cli.py
+-rw-r--r--   0        0        0     5567 2023-11-27 19:58:23.820550 insanely_fast_whisper-0.0.9/src/insanely_fast_whisper/utils.py
+-rw-r--r--   0        0        0        0 2023-11-05 17:51:43.860503 insanely_fast_whisper-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     7189 1970-01-01 00:00:00.000000 insanely_fast_whisper-0.0.9/PKG-INFO
```

### Comparing `insanely_fast_whisper-0.0.8/LICENSE` & `insanely_fast_whisper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `insanely_fast_whisper-0.0.8/README.md` & `insanely_fast_whisper-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Insanely Fast Whisper
 
-Powered by 🤗 *Transformers*, *Optimum* & *flash-attn*
+An opinionated CLI to transcribe Audio files w/ Whisper on-device! Powered by 🤗 *Transformers*, *Optimum* & *flash-attn*
 
 **TL;DR** - Transcribe **150** minutes (2.5 hours) of audio in less than **98** seconds - with [OpenAI's Whisper Large v3](https://huggingface.co/openai/whisper-large-v3). Blazingly fast transcription is now a reality!⚡️
 
 Not convinced? Here are some benchmarks we ran on a Nvidia A100 - 80GB 👇
 
 | Optimisation type    | Time to Transcribe (150 mins of Audio) |
 |------------------|------------------|
-| Transformers (`fp32`)             | ~31 (*31 min 1 sec*)             |
-| Transformers (`fp16` + `batching [24]` + `bettertransformer`) | ~5 (*5 min 2 sec*)            |
-| **Transformers (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~2 (*1 min 38 sec*)**            |
-| distil-whisper (`fp16` + `batching [24]` + `bettertransformer`) | ~3 (*3 min 16 sec*)            |
-| **distil-whisper (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~1 (*1 min 18 sec*)**           |
-| Faster Whisper (`fp16` + `beam_size [1]`) | ~9.23 (*9 min 23 sec*)            |
-| Faster Whisper (`8-bit` + `beam_size [1]`) | ~8 (*8 min 15 sec*)            |
+| large-v3 (Transformers) (`fp32`)             | ~31 (*31 min 1 sec*)             |
+| large-v3 (Transformers) (`fp16` + `batching [24]` + `bettertransformer`) | ~5 (*5 min 2 sec*)            |
+| **large-v3 (Transformers) (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~2 (*1 min 38 sec*)**            |
+| distil-large-v2 (Transformers) (`fp16` + `batching [24]` + `bettertransformer`) | ~3 (*3 min 16 sec*)            |
+| **distil-large-v2 (Transformers) (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~1 (*1 min 18 sec*)**           |
+| large-v2 (Faster Whisper) (`fp16` + `beam_size [1]`) | ~9.23 (*9 min 23 sec*)            |
+| large-v2 (Faster Whisper) (`8-bit` + `beam_size [1]`) | ~8 (*8 min 15 sec*)            |
 
 P.S. We also ran the benchmarks on a [Google Colab T4 GPU](/notebooks/) instance too!
 
 ## 🆕 Blazingly fast transcriptions via your terminal! ⚡️
 
 We've added a CLI to enable fast transcriptions. Here's how you can use it:
 
-Install `insanely-fast-whisper` with `pipx`:
+Install `insanely-fast-whisper` with `pipx` (`pip install pipx` or `brew install pipx`):
 
 ```bash
 pipx install insanely-fast-whisper
 ```
 
 Run inference from any path on your computer:
 
@@ -48,26 +48,27 @@
 
 Don't want to install `insanely-fast-whisper`? Just use `pipx run`:
 
 ```bash
 pipx run insanely-fast-whisper --file-name <filename or URL>
 ```
 
-Note: The CLI is opinionated and currently only works for Nvidia GPUs. Make sure to check out the defaults and the list of options you can play around with to maximise your transcription throughput. Run `insanely-fast-whisper --help` or `pipx run insanely-fast-whisper --help` to get all the CLI arguments and defaults. 
+> [!NOTE]
+> The CLI is highly opinionate and only works on NVIDIA GPUs & Mac. Make sure to check out the defaults and the list of options you can play around with to maximise your transcription throughput. Run `insanely-fast-whisper --help` or `pipx run insanely-fast-whisper --help` to get all the CLI arguments along with their defaults. 
 
 
 ## CLI Options
 
-The `insanely-fast-whisper` repo provides an all round support for running Whisper in various settings. Note that as of today 20th Nov, `insanely-fast-whisper` only works on CUDA enabled devices.
+The `insanely-fast-whisper` repo provides an all round support for running Whisper in various settings. Note that as of today 26th Nov, `insanely-fast-whisper` works on both CUDA and mps (mac) enabled devices.
 ```
   -h, --help            show this help message and exit
   --file-name FILE_NAME
                         Path or URL to the audio file to be transcribed.
   --device-id DEVICE_ID
-                        Device ID for your GPU (just pass the device ID number). (default: "0")
+                        Device ID for your GPU. Just pass the device number when using CUDA, or "mps" for Macs with Apple Silicon. (default: "0")
   --transcript-path TRANSCRIPT_PATH
                         Path to save the transcription output. (default: output.json)
   --model-name MODEL_NAME
                         Name of the pretrained model/ checkpoint to perform ASR. (default: openai/whisper-large-v3)
   --task {transcribe,translate}
                         Task to perform: transcribe or translate to another language. (default: transcribe)
   --language LANGUAGE   
@@ -86,65 +87,50 @@
 
 Make sure to install it via `pipx runpip insanely-fast-whisper install flash-attn --no-build-isolation`. Massive kudos to @li-yifei for helping with this.
 
 **How to solve an `AssertionError: Torch not compiled with CUDA enabled` error on Windows?**
 
 The root cause of this problem is still unkown, however, you can resolve this by manually installing torch in the virtualenv like `python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121`. Thanks to @pto2k for all tdebugging this.
 
-## How to use Whisper without a CLI?
-
-<details>
-<summary>For older GPUs, all you need to run is:</summary>
-
-```python
-import torch
-from transformers import pipeline
-
-pipe = pipeline("automatic-speech-recognition",
-                "openai/whisper-large-v3",
-                torch_dtype=torch.float16,
-                device="cuda:0")
-
-pipe.model = pipe.model.to_bettertransformer()
+**How to avoid Out-Of-Memory (OOM) exceptions on Mac?**
 
-outputs = pipe("<FILE_NAME>",
-               chunk_length_s=30,
-               batch_size=24,
-               return_timestamps=True)
+The *mps* backend isn't as optimised as CUDA, hence is way more memory hungry. Typically you can run with `--batch-size 4` without any issues (should use roughly 12GB GPU VRAM). Don't forget to set `--device mps`.
 
-outputs["text"]
-```
-</details>
+## How to use Whisper without a CLI?
 
 <details>
-
-<summary>For newer (A10, A100, H100s), use [Flash Attention](https://github.com/Dao-AILab/flash-attention):</summary>
+<summary>All you need to run is the below snippet:</summary>
 
 ```python
 import torch
 from transformers import pipeline
 
-pipe = pipeline("automatic-speech-recognition",
-                "openai/whisper-large-v3",
-                torch_dtype=torch.float16,
-                model_kwargs={"use_flash_attention_2": True},
-                device="cuda:0")
+pipe = pipeline(
+    "automatic-speech-recognition",
+    model=args.model_name,
+    torch_dtype=torch.float16,
+    device="cuda", # or mps for Mac devices
+    model_kwargs={"use_flash_attention_2": True}, # set to False for old GPUs
+)
+
+pipe.model = pipe.model.to_bettertransformer() # only if `use_flash_attention_2` is set to False
 
 outputs = pipe("<FILE_NAME>",
                chunk_length_s=30,
                batch_size=24,
                return_timestamps=True)
 
-outputs["text"]                
+outputs
 ```
 </details>
 
 ## Acknowledgements
 
 1. [OpenAI Whisper](https://github.com/openai/whisper) team for open sourcing such a brilliant check point.
 2. Hugging Face Transformers team, specifically [Arthur](https://github.com/ArthurZucker), [Patrick](https://github.com/patrickvonplaten), [Sanchit](https://github.com/sanchit-gandhi) & [Yoach](https://github.com/ylacombe)  (alphabetical order) for continuing to maintain Whisper in Transformers.
 3. Hugging Face [Optimum](https://github.com/huggingface/optimum) team for making the BetterTransformer API so easily accessible.
 4. [Patrick Arminio](https://github.com/patrick91) for helping me tremendously to put together this CLI.
 
 ## Community showcase
 
-@ochen1 created a brilliant MVP for a CLI here: https://github.com/ochen1/insanely-fast-whisper-cli (Try it out now!)
+1. @ochen1 created a brilliant MVP for a CLI here: https://github.com/ochen1/insanely-fast-whisper-cli (Try it out now!)
+2. @arihanv created a an app (Shush) using NextJS (Frontend) & Modal (Backend): https://github.com/arihanv/Shush (Check it outtt!)
```

### Comparing `insanely_fast_whisper-0.0.8/src/insanely_fast_whisper/cli.py` & `insanely_fast_whisper-0.0.9/src/insanely_fast_whisper/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import json
 
 import argparse
 import torch
 from transformers import pipeline
+from pyannote.audio import Pipeline
+
+from utils import (
+    preprocess_inputs,
+    diarize_audio,
+    post_process_segments_and_transcripts,
+)
 from rich.progress import Progress, TimeElapsedColumn, BarColumn, TextColumn
 
+
 parser = argparse.ArgumentParser(description="Automatic Speech Recognition")
 parser.add_argument(
     "--file-name",
     required=True,
     type=str,
     help="Path or URL to the audio file to be transcribed.",
 )
@@ -66,14 +74,21 @@
     "--timestamp",
     required=False,
     type=str,
     default="chunk",
     choices=["chunk", "word"],
     help="Whisper supports both chunked as well as word level timestamps. (default: chunk)",
 )
+parser.add_argument(
+    "--hf_token",
+    required=False,
+    default="no_token",
+    type=str,
+    help="Provide a hf.co/settings/token for Pyannote.audio to diarise the audio clips",
+)
 
 
 def main():
     args = parser.parse_args()
 
     pipe = pipeline(
         "automatic-speech-recognition",
@@ -103,13 +118,44 @@
             args.file_name,
             chunk_length_s=30,
             batch_size=args.batch_size,
             generate_kwargs={"task": args.task, "language": language},
             return_timestamps=ts,
         )
 
-    with open(args.transcript_path, "w", encoding="utf8") as fp:
-        json.dump(outputs, fp, ensure_ascii=False)
+    if args.hf_token != "no_token":
+        diarization_pipeline = Pipeline.from_pretrained(
+            "pyannote/speaker-diarization-3.1", use_auth_token=args.hf_token
+        )
+        diarization_pipeline.to(
+            torch.device("mps" if args.device_id == "mps" else f"cuda:{args.device_id}")
+        )
+        with Progress(
+            TextColumn("🤗 [progress.description]{task.description}"),
+            BarColumn(style="yellow1", pulse_style="white"),
+            TimeElapsedColumn(),
+        ) as progress:
+            progress.add_task("[yellow]Segmenting...", total=None)
+
+            inputs, diarizer_inputs = preprocess_inputs(inputs=args.file_name)
 
-    print(
-        f"Voila! Your file has been transcribed go check it out over here! {args.transcript_path}"
-    )
+            segments = diarize_audio(diarizer_inputs, diarization_pipeline)
+
+            segmented_transcript = post_process_segments_and_transcripts(
+                segments, outputs["chunks"], group_by_speaker=False
+            )
+
+        segmented_transcript.append(outputs)
+
+        with open(args.transcript_path, "w", encoding="utf8") as fp:
+            json.dump(segmented_transcript, fp, ensure_ascii=False)
+
+        print(
+            f"Voila!✨ Your file has been transcribed & speaker segmented go check it out over here 👉 {args.transcript_path}"
+        )
+    else:
+        with open(args.transcript_path, "w", encoding="utf8") as fp:
+            json.dump(outputs, fp, ensure_ascii=False)
+
+        print(
+            f"Voila!✨ Your file has been transcribed go check it out over here 👉 {args.transcript_path}"
+        )
```

### Comparing `insanely_fast_whisper-0.0.8/PKG-INFO` & `insanely_fast_whisper-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: insanely-fast-whisper
-Version: 0.0.8
+Version: 0.0.9
 Summary: An insanely fast whisper CLI
 Author-Email: VB <reachvaibhavs10@gmail.com>, Patrick Arminio <patrick.arminio@gmail.com>
 License: MIT
-Requires-Python: >=3.8
+Requires-Python: <=3.11,>=3.8
 Requires-Dist: transformers
 Requires-Dist: optimum
 Requires-Dist: accelerate
+Requires-Dist: pyannote-audio>=3.1.0
 Requires-Dist: setuptools>=68.2.2
 Requires-Dist: rich>=13.7.0
 Description-Content-Type: text/markdown
 
 # Insanely Fast Whisper
 
-Powered by 🤗 *Transformers*, *Optimum* & *flash-attn*
+An opinionated CLI to transcribe Audio files w/ Whisper on-device! Powered by 🤗 *Transformers*, *Optimum* & *flash-attn*
 
 **TL;DR** - Transcribe **150** minutes (2.5 hours) of audio in less than **98** seconds - with [OpenAI's Whisper Large v3](https://huggingface.co/openai/whisper-large-v3). Blazingly fast transcription is now a reality!⚡️
 
 Not convinced? Here are some benchmarks we ran on a Nvidia A100 - 80GB 👇
 
 | Optimisation type    | Time to Transcribe (150 mins of Audio) |
 |------------------|------------------|
-| Transformers (`fp32`)             | ~31 (*31 min 1 sec*)             |
-| Transformers (`fp16` + `batching [24]` + `bettertransformer`) | ~5 (*5 min 2 sec*)            |
-| **Transformers (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~2 (*1 min 38 sec*)**            |
-| distil-whisper (`fp16` + `batching [24]` + `bettertransformer`) | ~3 (*3 min 16 sec*)            |
-| **distil-whisper (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~1 (*1 min 18 sec*)**           |
-| Faster Whisper (`fp16` + `beam_size [1]`) | ~9.23 (*9 min 23 sec*)            |
-| Faster Whisper (`8-bit` + `beam_size [1]`) | ~8 (*8 min 15 sec*)            |
+| large-v3 (Transformers) (`fp32`)             | ~31 (*31 min 1 sec*)             |
+| large-v3 (Transformers) (`fp16` + `batching [24]` + `bettertransformer`) | ~5 (*5 min 2 sec*)            |
+| **large-v3 (Transformers) (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~2 (*1 min 38 sec*)**            |
+| distil-large-v2 (Transformers) (`fp16` + `batching [24]` + `bettertransformer`) | ~3 (*3 min 16 sec*)            |
+| **distil-large-v2 (Transformers) (`fp16` + `batching [24]` + `Flash Attention 2`)** | **~1 (*1 min 18 sec*)**           |
+| large-v2 (Faster Whisper) (`fp16` + `beam_size [1]`) | ~9.23 (*9 min 23 sec*)            |
+| large-v2 (Faster Whisper) (`8-bit` + `beam_size [1]`) | ~8 (*8 min 15 sec*)            |
 
 P.S. We also ran the benchmarks on a [Google Colab T4 GPU](/notebooks/) instance too!
 
 ## 🆕 Blazingly fast transcriptions via your terminal! ⚡️
 
 We've added a CLI to enable fast transcriptions. Here's how you can use it:
 
-Install `insanely-fast-whisper` with `pipx`:
+Install `insanely-fast-whisper` with `pipx` (`pip install pipx` or `brew install pipx`):
 
 ```bash
 pipx install insanely-fast-whisper
 ```
 
 Run inference from any path on your computer:
 
@@ -62,26 +63,27 @@
 
 Don't want to install `insanely-fast-whisper`? Just use `pipx run`:
 
 ```bash
 pipx run insanely-fast-whisper --file-name <filename or URL>
 ```
 
-Note: The CLI is opinionated and currently only works for Nvidia GPUs. Make sure to check out the defaults and the list of options you can play around with to maximise your transcription throughput. Run `insanely-fast-whisper --help` or `pipx run insanely-fast-whisper --help` to get all the CLI arguments and defaults. 
+> [!NOTE]
+> The CLI is highly opinionate and only works on NVIDIA GPUs & Mac. Make sure to check out the defaults and the list of options you can play around with to maximise your transcription throughput. Run `insanely-fast-whisper --help` or `pipx run insanely-fast-whisper --help` to get all the CLI arguments along with their defaults. 
 
 
 ## CLI Options
 
-The `insanely-fast-whisper` repo provides an all round support for running Whisper in various settings. Note that as of today 20th Nov, `insanely-fast-whisper` only works on CUDA enabled devices.
+The `insanely-fast-whisper` repo provides an all round support for running Whisper in various settings. Note that as of today 26th Nov, `insanely-fast-whisper` works on both CUDA and mps (mac) enabled devices.
 ```
   -h, --help            show this help message and exit
   --file-name FILE_NAME
                         Path or URL to the audio file to be transcribed.
   --device-id DEVICE_ID
-                        Device ID for your GPU (just pass the device ID number). (default: "0")
+                        Device ID for your GPU. Just pass the device number when using CUDA, or "mps" for Macs with Apple Silicon. (default: "0")
   --transcript-path TRANSCRIPT_PATH
                         Path to save the transcription output. (default: output.json)
   --model-name MODEL_NAME
                         Name of the pretrained model/ checkpoint to perform ASR. (default: openai/whisper-large-v3)
   --task {transcribe,translate}
                         Task to perform: transcribe or translate to another language. (default: transcribe)
   --language LANGUAGE   
@@ -100,65 +102,50 @@
 
 Make sure to install it via `pipx runpip insanely-fast-whisper install flash-attn --no-build-isolation`. Massive kudos to @li-yifei for helping with this.
 
 **How to solve an `AssertionError: Torch not compiled with CUDA enabled` error on Windows?**
 
 The root cause of this problem is still unkown, however, you can resolve this by manually installing torch in the virtualenv like `python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121`. Thanks to @pto2k for all tdebugging this.
 
-## How to use Whisper without a CLI?
-
-<details>
-<summary>For older GPUs, all you need to run is:</summary>
-
-```python
-import torch
-from transformers import pipeline
-
-pipe = pipeline("automatic-speech-recognition",
-                "openai/whisper-large-v3",
-                torch_dtype=torch.float16,
-                device="cuda:0")
-
-pipe.model = pipe.model.to_bettertransformer()
+**How to avoid Out-Of-Memory (OOM) exceptions on Mac?**
 
-outputs = pipe("<FILE_NAME>",
-               chunk_length_s=30,
-               batch_size=24,
-               return_timestamps=True)
+The *mps* backend isn't as optimised as CUDA, hence is way more memory hungry. Typically you can run with `--batch-size 4` without any issues (should use roughly 12GB GPU VRAM). Don't forget to set `--device mps`.
 
-outputs["text"]
-```
-</details>
+## How to use Whisper without a CLI?
 
 <details>
-
-<summary>For newer (A10, A100, H100s), use [Flash Attention](https://github.com/Dao-AILab/flash-attention):</summary>
+<summary>All you need to run is the below snippet:</summary>
 
 ```python
 import torch
 from transformers import pipeline
 
-pipe = pipeline("automatic-speech-recognition",
-                "openai/whisper-large-v3",
-                torch_dtype=torch.float16,
-                model_kwargs={"use_flash_attention_2": True},
-                device="cuda:0")
+pipe = pipeline(
+    "automatic-speech-recognition",
+    model=args.model_name,
+    torch_dtype=torch.float16,
+    device="cuda", # or mps for Mac devices
+    model_kwargs={"use_flash_attention_2": True}, # set to False for old GPUs
+)
+
+pipe.model = pipe.model.to_bettertransformer() # only if `use_flash_attention_2` is set to False
 
 outputs = pipe("<FILE_NAME>",
                chunk_length_s=30,
                batch_size=24,
                return_timestamps=True)
 
-outputs["text"]                
+outputs
 ```
 </details>
 
 ## Acknowledgements
 
 1. [OpenAI Whisper](https://github.com/openai/whisper) team for open sourcing such a brilliant check point.
 2. Hugging Face Transformers team, specifically [Arthur](https://github.com/ArthurZucker), [Patrick](https://github.com/patrickvonplaten), [Sanchit](https://github.com/sanchit-gandhi) & [Yoach](https://github.com/ylacombe)  (alphabetical order) for continuing to maintain Whisper in Transformers.
 3. Hugging Face [Optimum](https://github.com/huggingface/optimum) team for making the BetterTransformer API so easily accessible.
 4. [Patrick Arminio](https://github.com/patrick91) for helping me tremendously to put together this CLI.
 
 ## Community showcase
 
-@ochen1 created a brilliant MVP for a CLI here: https://github.com/ochen1/insanely-fast-whisper-cli (Try it out now!)
+1. @ochen1 created a brilliant MVP for a CLI here: https://github.com/ochen1/insanely-fast-whisper-cli (Try it out now!)
+2. @arihanv created a an app (Shush) using NextJS (Frontend) & Modal (Backend): https://github.com/arihanv/Shush (Check it outtt!)
```


# Comparing `tmp/alabamaencoder-0.4.1.tar.gz` & `tmp/alabamaencoder-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alabamaencoder-0.4.1.tar", last modified: Mon May 13 18:44:50 2024, max compression
+gzip compressed data, was "alabamaencoder-0.4.2.tar", last modified: Sat May 25 14:13:37 2024, max compression
```

## Comparing `alabamaencoder-0.4.1.tar` & `alabamaencoder-0.4.2.tar`

### file list

```diff
@@ -1,161 +1,168 @@
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.088802 alabamaencoder-0.4.1/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      299 2024-05-13 18:44:50.088802 alabamaencoder-0.4.1/PKG-INFO
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.052801 alabamaencoder-0.4.1/alabamaEncode/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.4.1/alabamaEncode/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.052801 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/aom_firstpass.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/perdict.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.052801 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/train/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/train/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/train/train.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.052801 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.052801 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.056801 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10661 2024-04-29 21:50:58.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-03 21:10:20.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.056801 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-04-22 19:10:58.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-03-05 22:27:27.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      859 2024-02-02 15:57:21.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2256 2024-04-26 22:44:56.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/opinionated_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5927 2024-03-05 22:32:37.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/pipelines.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.060801 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4955 2024-03-05 20:43:08.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_steps/multires_package.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.060801 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1498 2024-05-04 17:39:06.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/args_tune.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4687 2024-04-27 00:03:05.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/autocrop.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-04 17:38:16.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/ideal_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5986 2024-03-05 22:00:10.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2777 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/x264_tune.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.064801 alabamaencoder-0.4.1/alabamaEncode/core/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.4.1/alabamaEncode/core/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10800 2024-05-04 17:37:43.000000 alabamaencoder-0.4.1/alabamaEncode/core/alabama.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2879 2024-02-21 15:17:46.000000 alabamaencoder-0.4.1/alabamaEncode/core/bin_utils.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3878 2024-05-02 23:47:10.000000 alabamaencoder-0.4.1/alabamaEncode/core/chunk_job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.4.1/alabamaEncode/core/cli_executor.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13706 2024-03-22 06:24:59.000000 alabamaencoder-0.4.1/alabamaEncode/core/ffmpeg.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5661 2024-05-07 20:56:31.000000 alabamaencoder-0.4.1/alabamaEncode/core/final_touches.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19276 2024-05-04 17:36:30.000000 alabamaencoder-0.4.1/alabamaEncode/core/job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.4.1/alabamaEncode/core/kv.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.4.1/alabamaEncode/core/path.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.4.1/alabamaEncode/core/timer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.4.1/alabamaEncode/core/ws_update.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.068801 alabamaencoder-0.4.1/alabamaEncode/encoder/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/codec.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11438 2024-04-26 23:55:50.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/encoder.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/encoder_factory.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.072801 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/Aomenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/Nvenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/SvtAvif.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7642 2024-04-26 23:56:02.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/Svtenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/VaapiH264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2114 2024-03-23 06:39:42.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/VaapiH265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/X264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/X265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/rav1e.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/impl/vp9.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/rate_dist.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.4.1/alabamaEncode/encoder/stats.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.076802 alabamaencoder-0.4.1/alabamaEncode/experiments/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/Aq.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/Overlays.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/Svtav1Speed.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/Svtav1Tunes.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/TemporalFiltering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/ai_feature_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/aom_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/convexhull.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/crf_vmaf_relation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/denoise.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/sequence_convex.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/serialise_context.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/streaming_output.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/superres.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/target_vmaf.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.076802 alabamaencoder-0.4.1/alabamaEncode/experiments/util/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/util/ExperimentUtil.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.4.1/alabamaEncode/experiments/util/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.080802 alabamaencoder-0.4.1/alabamaEncode/metrics/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/calculate.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/comparison_display.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/exception.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/image.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.080802 alabamaencoder-0.4.1/alabamaEncode/metrics/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/impl/psnr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/impl/ssim.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/impl/ssimu2.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9052 2024-02-05 00:40:43.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/impl/vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/metric.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/options.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.4.1/alabamaEncode/metrics/result.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.080802 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/CeleryApp.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/command.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12819 2024-04-21 00:03:18.000000 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/execute_commands.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/worker.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.084802 alabamaencoder-0.4.1/alabamaEncode/scene/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.4.1/alabamaEncode/scene/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.4.1/alabamaEncode/scene/annel.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9690 2024-05-04 17:06:53.000000 alabamaencoder-0.4.1/alabamaEncode/scene/chunk.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13305 2024-05-13 18:43:21.000000 alabamaencoder-0.4.1/alabamaEncode/scene/concat.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4451 2024-05-04 17:06:53.000000 alabamaencoder-0.4.1/alabamaEncode/scene/sequence.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11219 2024-05-04 17:23:39.000000 alabamaencoder-0.4.1/alabamaEncode/scene/split.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.084802 alabamaencoder-0.4.1/alabamaEncode_frontends/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.084802 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/__init__.py
--rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4366 2024-03-22 06:30:36.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/__main__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.084802 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-03-05 20:36:01.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/autopaths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    20157 2024-03-29 15:04:00.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/cli_args.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/paths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/res_preset.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1987 2024-05-04 17:19:56.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/validate_files.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1177 2024-03-17 23:12:31.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/video_filters.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.084802 alabamaencoder-0.4.1/alabamaEncode_frontends/demon/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/demon/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.4.1/alabamaEncode_frontends/demon/demon.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-13 18:44:50.088802 alabamaencoder-0.4.1/alabamaEncoder.egg-info/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      299 2024-05-13 18:44:50.000000 alabamaencoder-0.4.1/alabamaEncoder.egg-info/PKG-INFO
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5965 2024-05-13 18:44:50.000000 alabamaencoder-0.4.1/alabamaEncoder.egg-info/SOURCES.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-13 18:44:50.000000 alabamaencoder-0.4.1/alabamaEncoder.egg-info/dependency_links.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-05-13 18:44:50.000000 alabamaencoder-0.4.1/alabamaEncoder.egg-info/entry_points.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       91 2024-05-13 18:44:50.000000 alabamaencoder-0.4.1/alabamaEncoder.egg-info/requires.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-13 18:44:50.000000 alabamaencoder-0.4.1/alabamaEncoder.egg-info/top_level.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-13 18:44:50.088802 alabamaencoder-0.4.1/setup.cfg
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      482 2024-05-13 18:44:39.000000 alabamaencoder-0.4.1/setup.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/PKG-INFO
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.142367 alabamaencoder-0.4.2/alabamaEncode/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.4.2/alabamaEncode/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.142367 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/aom_firstpass.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/perdict.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/train.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10661 2024-04-29 21:50:58.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-03 21:10:20.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-04-22 19:10:58.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-03-05 22:27:27.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      859 2024-02-02 15:57:21.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2362 2024-05-20 19:14:36.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/opinionated_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5927 2024-03-05 22:32:37.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/pipelines.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4955 2024-03-05 20:43:08.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_package.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-20 13:32:49.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/args_tune.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4687 2024-04-27 00:03:05.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/autocrop.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-04 17:38:16.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/ideal_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5986 2024-03-05 22:00:10.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2777 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/x264_tune.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/core/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.4.2/alabamaEncode/core/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10800 2024-05-04 17:37:43.000000 alabamaencoder-0.4.2/alabamaEncode/core/alabama.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2879 2024-02-21 15:17:46.000000 alabamaencoder-0.4.2/alabamaEncode/core/bin_utils.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3878 2024-05-02 23:47:10.000000 alabamaencoder-0.4.2/alabamaEncode/core/chunk_job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.4.2/alabamaEncode/core/cli_executor.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/core/extras/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.4.2/alabamaEncode/core/extras/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11151 2024-05-25 13:48:52.000000 alabamaencoder-0.4.2/alabamaEncode/core/extras/auto_thumbnailer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13706 2024-03-22 06:24:59.000000 alabamaencoder-0.4.2/alabamaEncode/core/ffmpeg.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5661 2024-05-07 20:56:31.000000 alabamaencoder-0.4.2/alabamaEncode/core/final_touches.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19276 2024-05-04 17:36:30.000000 alabamaencoder-0.4.2/alabamaEncode/core/job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.4.2/alabamaEncode/core/kv.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.4.2/alabamaEncode/core/path.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.4.2/alabamaEncode/core/timer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.4.2/alabamaEncode/core/ws_update.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/encoder/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/codec.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11438 2024-04-26 23:55:50.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/encoder.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/encoder_factory.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Aomenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Nvenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/SvtAvif.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7642 2024-04-26 23:56:02.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Svtenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2114 2024-03-23 06:39:42.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/rav1e.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/vp9.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/rate_dist.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/stats.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/experiments/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Aq.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Overlays.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Speed.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Tunes.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/TemporalFiltering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/ai_feature_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/aom_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/convexhull.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/crf_vmaf_relation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/denoise.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/sequence_convex.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/serialise_context.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/streaming_output.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/superres.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/target_vmaf.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/experiments/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/util/ExperimentUtil.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/util/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-21 17:50:35.000000 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      837 2024-05-24 18:46:29.000000 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/ffmpeg_src.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-22 16:28:12.000000 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/yuv.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/metrics/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/calculate.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/comparison_display.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/exception.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/image.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/psnr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssim.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssimu2.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9052 2024-02-05 00:40:43.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/metric.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/options.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/result.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryApp.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/command.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12819 2024-04-21 00:03:18.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/execute_commands.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/worker.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/scene/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.4.2/alabamaEncode/scene/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.4.2/alabamaEncode/scene/annel.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9690 2024-05-04 17:06:53.000000 alabamaencoder-0.4.2/alabamaEncode/scene/chunk.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13305 2024-05-13 18:43:21.000000 alabamaencoder-0.4.2/alabamaEncode/scene/concat.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4451 2024-05-04 17:06:53.000000 alabamaencoder-0.4.2/alabamaEncode/scene/sequence.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11219 2024-05-04 17:23:39.000000 alabamaencoder-0.4.2/alabamaEncode/scene/split.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode_frontends/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/__init__.py
+-rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4366 2024-03-22 06:30:36.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/__main__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-03-05 20:36:01.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/autopaths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    20157 2024-03-29 15:04:00.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/cli_args.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/paths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/res_preset.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1987 2024-05-04 17:19:56.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/validate_files.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1177 2024-03-17 23:12:31.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/video_filters.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncode_frontends/demon/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/demon/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/demon/demon.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncoder.egg-info/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/PKG-INFO
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6166 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/entry_points.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      124 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/requires.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/top_level.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/setup.cfg
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      548 2024-05-25 14:12:58.000000 alabamaencoder-0.4.2/setup.py
```

### Comparing `alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/aom_firstpass.py` & `alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/aom_firstpass.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/perdict.py` & `alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/perdict.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/ai_vmaf/train/train.py` & `alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/train.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_step.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_step.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/opinionated_vmaf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/opinionated_vmaf.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         case Codec.vp9:
             return 0, 63
         case _:
             raise ValueError(f"FATAL: Unknown codec: {codec}")
 
 
 def get_vmaf_probe_speed(encoder: Encoder) -> int:
+    env_name = "VMAF_PROBE_SPEED"
+    if env_name in os.environ:
+        return int(os.environ[env_name])
     match encoder:
         case EncoderSvt():
             return 13
         case _:
             # TODO: pick other values
             return 5
```

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/pipelines.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/pipelines.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_steps/multires_package.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_package.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/args_tune.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/args_tune.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
                 for _ in range(3):
                     ctx.log(
                         "YOU ARE USING SIMPLE DENOISE, THIS IS NOT RECOMMENDED FOR FIDELITY TUNING",
                         category="analyzing_content_logs"
                     )
             ctx.prototype_encoder.svt_tune = 1
             ctx.prototype_encoder.svt_tf = 0
+            ctx.prototype_encoder.svt_enable_variance_boost = 1
+
         case "appeal":
             ctx.log("Tuning for appeal", category="analyzing_content_logs")
             ctx.prototype_encoder.qm_max = 8
             ctx.prototype_encoder.qm_min = 0
             ctx.prototype_encoder.svt_tune = 0
             ctx.prototype_encoder.svt_enable_variance_boost = 0
         case "balanced":
```

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/autocrop.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/autocrop.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/denoise_filtering.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/denoise_filtering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/encoding_tiles.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/encoding_tiles.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/ideal_crf.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/ideal_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/sequence_autograin.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/sequence_autograin.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/conent_analysis/sequence/x264_tune.py` & `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/x264_tune.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/alabama.py` & `alabamaencoder-0.4.2/alabamaEncode/core/alabama.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/bin_utils.py` & `alabamaencoder-0.4.2/alabamaEncode/core/bin_utils.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/chunk_job.py` & `alabamaencoder-0.4.2/alabamaEncode/core/chunk_job.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/cli_executor.py` & `alabamaencoder-0.4.2/alabamaEncode/core/cli_executor.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/ffmpeg.py` & `alabamaencoder-0.4.2/alabamaEncode/core/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/final_touches.py` & `alabamaencoder-0.4.2/alabamaEncode/core/final_touches.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/job.py` & `alabamaencoder-0.4.2/alabamaEncode/core/job.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/kv.py` & `alabamaencoder-0.4.2/alabamaEncode/core/kv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/path.py` & `alabamaencoder-0.4.2/alabamaEncode/core/path.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/timer.py` & `alabamaencoder-0.4.2/alabamaEncode/core/timer.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/core/ws_update.py` & `alabamaencoder-0.4.2/alabamaEncode/core/ws_update.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/codec.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/codec.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/encoder.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/encoder_factory.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/encoder_factory.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/Aomenc.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Aomenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/Nvenc.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Nvenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/SvtAvif.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/SvtAvif.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/Svtenc.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Svtenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/VaapiH264.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH264.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/VaapiH265.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH265.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/X264.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X264.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/X265.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X265.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/rav1e.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/rav1e.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/impl/vp9.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/vp9.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/encoder/stats.py` & `alabamaencoder-0.4.2/alabamaEncode/encoder/stats.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/Aq.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/Aq.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/Overlays.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/Overlays.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/Svtav1Speed.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Speed.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/Svtav1Tunes.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Tunes.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/TemporalFiltering.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/TemporalFiltering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/ai_feature_extract.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/ai_feature_extract.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/convexhull.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/convexhull.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/crf_vmaf_relation.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/crf_vmaf_relation.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/denoise.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/denoise.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/sequence_convex.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/sequence_convex.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/streaming_output.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/streaming_output.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/superres.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/superres.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/target_vmaf.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/experiments/util/ExperimentUtil.py` & `alabamaencoder-0.4.2/alabamaEncode/experiments/util/ExperimentUtil.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/calculate.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/calculate.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/comparison_display.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/comparison_display.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/image.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/image.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/impl/psnr.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/psnr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/impl/ssim.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssim.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/impl/ssimu2.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssimu2.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/metrics/impl/vmaf.py` & `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/CeleryApp.py` & `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryApp.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/CeleryAutoscaler.py` & `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryAutoscaler.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/execute_commands.py` & `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/execute_commands.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/parallelEncoding/worker.py` & `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/worker.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/scene/annel.py` & `alabamaencoder-0.4.2/alabamaEncode/scene/annel.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/scene/chunk.py` & `alabamaencoder-0.4.2/alabamaEncode/scene/chunk.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/scene/concat.py` & `alabamaencoder-0.4.2/alabamaEncode/scene/concat.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/scene/sequence.py` & `alabamaencoder-0.4.2/alabamaEncode/scene/sequence.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode/scene/split.py` & `alabamaencoder-0.4.2/alabamaEncode/scene/split.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/__main__.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/autopaths.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/autopaths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/cli_args.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/cli_args.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/paths.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/paths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/res_preset.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/res_preset.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/validate_files.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/validate_files.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/cli/cli_setup/video_filters.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/video_filters.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncode_frontends/demon/demon.py` & `alabamaencoder-0.4.2/alabamaEncode_frontends/demon/demon.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.1/alabamaEncoder.egg-info/SOURCES.txt` & `alabamaencoder-0.4.2/alabamaEncoder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 alabamaEncode/core/ffmpeg.py
 alabamaEncode/core/final_touches.py
 alabamaEncode/core/job.py
 alabamaEncode/core/kv.py
 alabamaEncode/core/path.py
 alabamaEncode/core/timer.py
 alabamaEncode/core/ws_update.py
+alabamaEncode/core/extras/__init__.py
+alabamaEncode/core/extras/auto_thumbnailer.py
 alabamaEncode/encoder/__init__.py
 alabamaEncode/encoder/codec.py
 alabamaEncode/encoder/encoder.py
 alabamaEncode/encoder/encoder_factory.py
 alabamaEncode/encoder/rate_dist.py
 alabamaEncode/encoder/stats.py
 alabamaEncode/encoder/impl/Aomenc.py
@@ -85,14 +87,17 @@
 alabamaEncode/experiments/sequence_convex.py
 alabamaEncode/experiments/serialise_context.py
 alabamaEncode/experiments/streaming_output.py
 alabamaEncode/experiments/superres.py
 alabamaEncode/experiments/target_vmaf.py
 alabamaEncode/experiments/util/ExperimentUtil.py
 alabamaEncode/experiments/util/__init__.py
+alabamaEncode/ffmpeg_source/__init__.py
+alabamaEncode/ffmpeg_source/ffmpeg_src.py
+alabamaEncode/ffmpeg_source/yuv.py
 alabamaEncode/metrics/__init__.py
 alabamaEncode/metrics/calculate.py
 alabamaEncode/metrics/comparison_display.py
 alabamaEncode/metrics/exception.py
 alabamaEncode/metrics/image.py
 alabamaEncode/metrics/metric.py
 alabamaEncode/metrics/options.py
```


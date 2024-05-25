# Comparing `tmp/athina-1.3.0.tar.gz` & `tmp/athina-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina-1.3.0.tar", max compression
+gzip compressed data, was "athina-1.3.1.tar", max compression
```

## Comparing `athina-1.3.0.tar` & `athina-1.3.1.tar`

### file list

```diff
@@ -1,143 +1,144 @@
--rw-r--r--   0        0        0     8595 2024-05-03 15:41:49.406642 athina-1.3.0/README.md
--rw-r--r--   0        0        0      169 2024-05-03 15:41:49.406999 athina-1.3.0/athina/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.3.0/athina/cli/__init__.py
--rw-r--r--   0        0        0     5390 2024-05-05 12:00:16.321612 athina-1.3.0/athina/cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.3.0/athina/constants/__init__.py
--rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.3.0/athina/constants/messages.py
--rw-r--r--   0        0        0       72 2024-05-03 15:41:49.407935 athina-1.3.0/athina/datasets/__init__.py
--rw-r--r--   0        0        0   218970 2024-05-03 15:41:49.408467 athina-1.3.0/athina/datasets/conversations.json
--rw-r--r--   0        0        0     3230 2024-05-19 14:25:58.792810 athina-1.3.0/athina/datasets/dataset.py
--rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.3.0/athina/datasets/summarization_sample.py
--rw-r--r--   0        0        0     2675 2024-05-03 15:41:49.409340 athina-1.3.0/athina/datasets/yc_query_mini.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.3.0/athina/errors/__init__.py
--rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.3.0/athina/errors/exceptions.py
--rw-r--r--   0        0        0     4069 2024-05-03 15:41:49.409717 athina-1.3.0/athina/evals/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-16 19:27:48.886844 athina-1.3.0/athina/evals/base_evaluator.py
--rw-r--r--   0        0        0     4259 2024-05-16 19:27:48.887245 athina-1.3.0/athina/evals/conversation/conversation_coherence/evaluator.py
--rw-r--r--   0        0        0     1198 2024-05-03 15:41:49.410542 athina-1.3.0/athina/evals/conversation/conversation_coherence/prompt.py
--rw-r--r--   0        0        0     4414 2024-05-16 19:27:48.887449 athina-1.3.0/athina/evals/conversation/conversation_resolution/evaluator.py
--rw-r--r--   0        0        0     1104 2024-05-03 15:41:49.410767 athina-1.3.0/athina/evals/conversation/conversation_resolution/prompt.py
--rw-r--r--   0        0        0     2579 2024-05-03 15:41:49.411157 athina-1.3.0/athina/evals/eval_type.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.3.0/athina/evals/function/__init__.py
--rw-r--r--   0        0        0     3780 2024-05-16 19:27:48.888106 athina-1.3.0/athina/evals/function/function_evaluator.py
--rw-r--r--   0        0        0    18806 2024-05-03 15:41:49.412956 athina-1.3.0/athina/evals/function/functions.py
--rw-r--r--   0        0        0    10216 2024-05-03 15:41:49.414039 athina-1.3.0/athina/evals/function/wrapper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.3.0/athina/evals/grounded/__init__.py
--rw-r--r--   0        0        0     4298 2024-05-16 19:27:48.888364 athina-1.3.0/athina/evals/grounded/grounded_evaluator.py
--rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.3.0/athina/evals/grounded/similarity.py
--rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.3.0/athina/evals/grounded/wrapper.py
--rw-r--r--   0        0        0     3041 2024-05-16 19:27:48.889059 athina-1.3.0/athina/evals/guardrails/gibberish_text/evaluator.py
--rw-r--r--   0        0        0     3797 2024-05-16 19:27:48.889242 athina-1.3.0/athina/evals/guardrails/sensitive_topics/evaluator.py
--rw-r--r--   0        0        0     2965 2024-05-16 19:27:48.889409 athina-1.3.0/athina/evals/guardrails/sfw/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.3.0/athina/evals/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.3.0/athina/evals/llm/context_contains_enough_information/__init__.py
--rw-r--r--   0        0        0     3004 2024-05-16 19:27:48.889580 athina-1.3.0/athina/evals/llm/context_contains_enough_information/evaluator.py
--rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.3.0/athina/evals/llm/context_contains_enough_information/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.3.0/athina/evals/llm/custom_prompt/__init__.py
--rw-r--r--   0        0        0     2483 2024-05-16 19:27:48.889741 athina-1.3.0/athina/evals/llm/custom_prompt/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.3.0/athina/evals/llm/does_response_answer_query/__init__.py
--rw-r--r--   0        0        0     2632 2024-05-03 15:41:49.417364 athina-1.3.0/athina/evals/llm/does_response_answer_query/evaluator.py
--rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.3.0/athina/evals/llm/does_response_answer_query/examples.py
--rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.3.0/athina/evals/llm/example.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.3.0/athina/evals/llm/faithfulness/__init__.py
--rw-r--r--   0        0        0     2599 2024-05-03 15:41:49.417490 athina-1.3.0/athina/evals/llm/faithfulness/evaluator.py
--rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.3.0/athina/evals/llm/faithfulness/examples.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.3.0/athina/evals/llm/grading_criteria/__init__.py
--rw-r--r--   0        0        0     2209 2024-05-16 19:27:48.889913 athina-1.3.0/athina/evals/llm/grading_criteria/evaluator.py
--rw-r--r--   0        0        0     5821 2024-05-03 15:41:49.418273 athina-1.3.0/athina/evals/llm/groundedness/evaluator.py
--rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.3.0/athina/evals/llm/groundedness/prompt.py
--rw-r--r--   0        0        0     4982 2024-05-05 09:24:29.466550 athina-1.3.0/athina/evals/llm/llm_evaluator.py
--rw-r--r--   0        0        0    10915 2024-05-03 15:41:49.418745 athina-1.3.0/athina/evals/llm/summary_accuracy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.3.0/athina/evals/ragas/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.3.0/athina/evals/ragas/answer_correctness/__init__.py
--rw-r--r--   0        0        0     2383 2024-05-03 15:41:49.419035 athina-1.3.0/athina/evals/ragas/answer_correctness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.3.0/athina/evals/ragas/answer_relevancy/__init__.py
--rw-r--r--   0        0        0     2441 2024-05-03 15:41:49.419202 athina-1.3.0/athina/evals/ragas/answer_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.3.0/athina/evals/ragas/answer_semantic_similarity/__init__.py
--rw-r--r--   0        0        0     2440 2024-05-03 15:41:49.419340 athina-1.3.0/athina/evals/ragas/answer_semantic_similarity/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.3.0/athina/evals/ragas/coherence/__init__.py
--rw-r--r--   0        0        0     2187 2024-05-03 15:41:49.419789 athina-1.3.0/athina/evals/ragas/coherence/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.3.0/athina/evals/ragas/conciseness/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-03 15:41:49.420084 athina-1.3.0/athina/evals/ragas/conciseness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.3.0/athina/evals/ragas/context_precision/__init__.py
--rw-r--r--   0        0        0     2521 2024-05-03 15:41:49.420494 athina-1.3.0/athina/evals/ragas/context_precision/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.3.0/athina/evals/ragas/context_recall/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-03 15:41:49.420634 athina-1.3.0/athina/evals/ragas/context_recall/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.3.0/athina/evals/ragas/context_relevancy/__init__.py
--rw-r--r--   0        0        0     2159 2024-05-03 15:41:49.420776 athina-1.3.0/athina/evals/ragas/context_relevancy/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.3.0/athina/evals/ragas/faithfulness/__init__.py
--rw-r--r--   0        0        0     2370 2024-05-03 15:41:49.420918 athina-1.3.0/athina/evals/ragas/faithfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.3.0/athina/evals/ragas/harmfulness/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-03 15:41:49.421222 athina-1.3.0/athina/evals/ragas/harmfulness/evaluator.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.3.0/athina/evals/ragas/maliciousness/__init__.py
--rw-r--r--   0        0        0     2127 2024-05-03 15:41:49.421640 athina-1.3.0/athina/evals/ragas/maliciousness/evaluator.py
--rw-r--r--   0        0        0     3298 2024-05-03 15:41:49.421803 athina-1.3.0/athina/evals/ragas/ragas_evaluator.py
--rw-r--r--   0        0        0     5154 2024-05-03 15:41:49.422152 athina-1.3.0/athina/evals/safety/content_moderation/evaluator.py
--rw-r--r--   0        0        0     3387 2024-05-03 15:41:49.422800 athina-1.3.0/athina/evals/safety/pii_detection/evaluator.py
--rw-r--r--   0        0        0     4370 2024-05-03 15:41:49.424028 athina-1.3.0/athina/evals/safety/prompt_injection/evaluator.py
--rw-r--r--   0        0        0      106 2024-05-03 15:41:49.424321 athina-1.3.0/athina/guard/exception.py
--rw-r--r--   0        0        0     1404 2024-05-03 15:41:49.424686 athina-1.3.0/athina/guard/guard.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.3.0/athina/helpers/__init__.py
--rw-r--r--   0        0        0     5739 2024-05-16 19:27:48.890218 athina-1.3.0/athina/helpers/athina_logging_helper.py
--rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.3.0/athina/helpers/config.py
--rw-r--r--   0        0        0      122 2024-03-19 22:27:57.184730 athina-1.3.0/athina/helpers/constants.py
--rw-r--r--   0        0        0      790 2024-05-16 19:27:48.890420 athina-1.3.0/athina/helpers/dataset_helper.py
--rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.3.0/athina/helpers/eval_helper.py
--rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.3.0/athina/helpers/function_eval_util.py
--rw-r--r--   0        0        0     4591 2024-05-03 15:41:49.425070 athina-1.3.0/athina/helpers/get_evaluator.py
--rw-r--r--   0        0        0     2469 2024-05-22 07:52:50.227484 athina-1.3.0/athina/helpers/json.py
--rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.3.0/athina/helpers/kwparser.py
--rw-r--r--   0        0        0      894 2024-05-03 15:41:49.425348 athina-1.3.0/athina/helpers/loader_helper.py
--rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.3.0/athina/helpers/logger.py
--rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.3.0/athina/helpers/package_helper.py
--rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.3.0/athina/helpers/run_helper.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.3.0/athina/interfaces/__init__.py
--rw-r--r--   0        0        0     3905 2024-05-03 15:41:49.425463 athina-1.3.0/athina/interfaces/athina.py
--rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.3.0/athina/interfaces/data.py
--rw-r--r--   0        0        0     2065 2024-05-14 15:59:10.451321 athina-1.3.0/athina/interfaces/model.py
--rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.3.0/athina/interfaces/openai.py
--rw-r--r--   0        0        0     2944 2024-05-05 12:12:32.954417 athina-1.3.0/athina/interfaces/result.py
--rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.3.0/athina/keys/__init__.py
--rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.3.0/athina/keys/athina_api_key.py
--rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.3.0/athina/keys/openai_api_key.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.3.0/athina/llms/__init__.py
--rw-r--r--   0        0        0     1368 2024-05-22 07:52:50.227988 athina-1.3.0/athina/llms/abstract_llm_service.py
--rw-r--r--   0        0        0     1524 2024-05-22 07:52:50.228405 athina-1.3.0/athina/llms/litellm_service.py
--rw-r--r--   0        0        0     3461 2024-05-22 07:52:50.228694 athina-1.3.0/athina/llms/openai_service.py
--rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.3.0/athina/llms/question_answerer.py
--rw-r--r--   0        0        0     2874 2024-05-21 13:33:12.522927 athina-1.3.0/athina/llms/question_answerer_bulk.py
--rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.3.0/athina/llms/question_answerer_cot.py
--rw-r--r--   0        0        0     6674 2024-05-03 15:41:49.426272 athina-1.3.0/athina/llms/question_answerer_with_retrieval.py
--rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.3.0/athina/llms/question_generator.py
--rw-r--r--   0        0        0      323 2024-05-03 15:41:49.426530 athina-1.3.0/athina/loaders/__init__.py
--rw-r--r--   0        0        0     2326 2024-05-16 23:56:49.987467 athina-1.3.0/athina/loaders/base_loader.py
--rw-r--r--   0        0        0     2179 2024-05-16 19:27:48.890989 athina-1.3.0/athina/loaders/conversation_loader.py
--rw-r--r--   0        0        0     6507 2024-05-17 01:08:19.006440 athina-1.3.0/athina/loaders/loader.py
--rw-r--r--   0        0        0     3597 2024-05-16 19:27:48.892946 athina-1.3.0/athina/loaders/response_loader.py
--rw-r--r--   0        0        0     2970 2024-05-03 17:07:59.624449 athina-1.3.0/athina/loaders/summary_loader.py
--rw-r--r--   0        0        0     2380 2024-05-03 15:41:49.427400 athina-1.3.0/athina/loaders/text_loader.py
--rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.3.0/athina/metrics/agreement_score.py
--rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.3.0/athina/metrics/contradiction_score.py
--rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.3.0/athina/metrics/groundedness.py
--rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.3.0/athina/metrics/hallucination_score.py
--rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.3.0/athina/metrics/metric.py
--rw-r--r--   0        0        0     3000 2024-05-03 15:41:49.427514 athina-1.3.0/athina/metrics/metric_type.py
--rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.3.0/athina/metrics/passed.py
--rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.3.0/athina/metrics/ragas_metric.py
--rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.3.0/athina/metrics/similarity_score.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.3.0/athina/runner/__init__.py
--rw-r--r--   0        0        0     6940 2024-05-16 19:27:48.893298 athina-1.3.0/athina/runner/run.py
--rw-r--r--   0        0        0      341 2024-05-03 15:41:49.427983 athina-1.3.0/athina/runner/run_wrapper.py
--rw-r--r--   0        0        0     1781 2024-05-03 15:41:49.428243 athina-1.3.0/athina/scripts/guardrails.py
--rw-r--r--   0        0        0    13804 2024-05-19 14:25:58.794110 athina-1.3.0/athina/services/athina_api_service.py
--rw-r--r--   0        0        0      472 2024-05-22 07:52:50.229087 athina-1.3.0/athina/steps/__init__.py
--rw-r--r--   0        0        0     1582 2024-05-22 07:52:50.229307 athina-1.3.0/athina/steps/api.py
--rw-r--r--   0        0        0     4456 2024-05-22 07:52:50.229580 athina-1.3.0/athina/steps/base.py
--rw-r--r--   0        0        0     1729 2024-05-22 07:52:50.229864 athina-1.3.0/athina/steps/chain.py
--rw-r--r--   0        0        0     1501 2024-05-22 07:52:50.230002 athina-1.3.0/athina/steps/conditional.py
--rw-r--r--   0        0        0        0 2024-05-22 07:52:50.230033 athina-1.3.0/athina/steps/debug.py
--rw-r--r--   0        0        0      646 2024-05-22 07:52:50.230202 athina-1.3.0/athina/steps/iterator.py
--rw-r--r--   0        0        0     3187 2024-05-22 07:52:50.230415 athina-1.3.0/athina/steps/llm.py
--rw-r--r--   0        0        0      787 2024-05-22 07:52:50.230543 athina-1.3.0/athina/steps/transform.py
--rw-r--r--   0        0        0      978 2024-05-22 07:52:50.232786 athina-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     9705 1970-01-01 00:00:00.000000 athina-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     8595 2024-05-03 15:41:49.406642 athina-1.3.1/README.md
+-rw-r--r--   0        0        0      169 2024-05-03 15:41:49.406999 athina-1.3.1/athina/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.176900 athina-1.3.1/athina/cli/__init__.py
+-rw-r--r--   0        0        0     5390 2024-05-05 12:00:16.321612 athina-1.3.1/athina/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177123 athina-1.3.1/athina/constants/__init__.py
+-rw-r--r--   0        0        0      517 2024-03-19 22:27:57.177236 athina-1.3.1/athina/constants/messages.py
+-rw-r--r--   0        0        0       72 2024-05-03 15:41:49.407935 athina-1.3.1/athina/datasets/__init__.py
+-rw-r--r--   0        0        0   218970 2024-05-03 15:41:49.408467 athina-1.3.1/athina/datasets/conversations.json
+-rw-r--r--   0        0        0     3342 2024-05-25 05:42:57.982961 athina-1.3.1/athina/datasets/dataset.py
+-rw-r--r--   0        0        0     3355 2024-03-19 22:27:57.177821 athina-1.3.1/athina/datasets/summarization_sample.py
+-rw-r--r--   0        0        0     2675 2024-05-03 15:41:49.409340 athina-1.3.1/athina/datasets/yc_query_mini.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.177993 athina-1.3.1/athina/errors/__init__.py
+-rw-r--r--   0        0        0      801 2024-03-19 22:27:57.178079 athina-1.3.1/athina/errors/exceptions.py
+-rw-r--r--   0        0        0     4069 2024-05-03 15:41:49.409717 athina-1.3.1/athina/evals/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-16 19:27:48.886844 athina-1.3.1/athina/evals/base_evaluator.py
+-rw-r--r--   0        0        0     4259 2024-05-16 19:27:48.887245 athina-1.3.1/athina/evals/conversation/conversation_coherence/evaluator.py
+-rw-r--r--   0        0        0     1198 2024-05-03 15:41:49.410542 athina-1.3.1/athina/evals/conversation/conversation_coherence/prompt.py
+-rw-r--r--   0        0        0     4414 2024-05-16 19:27:48.887449 athina-1.3.1/athina/evals/conversation/conversation_resolution/evaluator.py
+-rw-r--r--   0        0        0     1104 2024-05-03 15:41:49.410767 athina-1.3.1/athina/evals/conversation/conversation_resolution/prompt.py
+-rw-r--r--   0        0        0     2579 2024-05-03 15:41:49.411157 athina-1.3.1/athina/evals/eval_type.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179006 athina-1.3.1/athina/evals/function/__init__.py
+-rw-r--r--   0        0        0     3780 2024-05-16 19:27:48.888106 athina-1.3.1/athina/evals/function/function_evaluator.py
+-rw-r--r--   0        0        0    18806 2024-05-03 15:41:49.412956 athina-1.3.1/athina/evals/function/functions.py
+-rw-r--r--   0        0        0    10216 2024-05-03 15:41:49.414039 athina-1.3.1/athina/evals/function/wrapper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.179629 athina-1.3.1/athina/evals/grounded/__init__.py
+-rw-r--r--   0        0        0     4298 2024-05-16 19:27:48.888364 athina-1.3.1/athina/evals/grounded/grounded_evaluator.py
+-rw-r--r--   0        0        0     4178 2024-03-19 22:27:57.179870 athina-1.3.1/athina/evals/grounded/similarity.py
+-rw-r--r--   0        0        0     1708 2024-03-19 22:27:57.179950 athina-1.3.1/athina/evals/grounded/wrapper.py
+-rw-r--r--   0        0        0     3041 2024-05-16 19:27:48.889059 athina-1.3.1/athina/evals/guardrails/gibberish_text/evaluator.py
+-rw-r--r--   0        0        0     3797 2024-05-16 19:27:48.889242 athina-1.3.1/athina/evals/guardrails/sensitive_topics/evaluator.py
+-rw-r--r--   0        0        0     2965 2024-05-16 19:27:48.889409 athina-1.3.1/athina/evals/guardrails/sfw/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180226 athina-1.3.1/athina/evals/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180328 athina-1.3.1/athina/evals/llm/context_contains_enough_information/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-16 19:27:48.889580 athina-1.3.1/athina/evals/llm/context_contains_enough_information/evaluator.py
+-rw-r--r--   0        0        0     1867 2024-03-19 22:27:57.180505 athina-1.3.1/athina/evals/llm/context_contains_enough_information/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180583 athina-1.3.1/athina/evals/llm/custom_prompt/__init__.py
+-rw-r--r--   0        0        0     2856 2024-05-25 05:42:57.983327 athina-1.3.1/athina/evals/llm/custom_prompt/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.180792 athina-1.3.1/athina/evals/llm/does_response_answer_query/__init__.py
+-rw-r--r--   0        0        0     2632 2024-05-03 15:41:49.417364 athina-1.3.1/athina/evals/llm/does_response_answer_query/evaluator.py
+-rw-r--r--   0        0        0     1186 2024-03-19 22:27:57.180970 athina-1.3.1/athina/evals/llm/does_response_answer_query/examples.py
+-rw-r--r--   0        0        0     1238 2024-03-19 22:27:57.181044 athina-1.3.1/athina/evals/llm/example.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181120 athina-1.3.1/athina/evals/llm/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2599 2024-05-03 15:41:49.417490 athina-1.3.1/athina/evals/llm/faithfulness/evaluator.py
+-rw-r--r--   0        0        0     1335 2024-03-19 22:27:57.181288 athina-1.3.1/athina/evals/llm/faithfulness/examples.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.181361 athina-1.3.1/athina/evals/llm/grading_criteria/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-16 19:27:48.889913 athina-1.3.1/athina/evals/llm/grading_criteria/evaluator.py
+-rw-r--r--   0        0        0     5821 2024-05-03 15:41:49.418273 athina-1.3.1/athina/evals/llm/groundedness/evaluator.py
+-rw-r--r--   0        0        0     1601 2024-03-19 22:27:57.181666 athina-1.3.1/athina/evals/llm/groundedness/prompt.py
+-rw-r--r--   0        0        0     4982 2024-05-05 09:24:29.466550 athina-1.3.1/athina/evals/llm/llm_evaluator.py
+-rw-r--r--   0        0        0    10915 2024-05-03 15:41:49.418745 athina-1.3.1/athina/evals/llm/summary_accuracy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182165 athina-1.3.1/athina/evals/ragas/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182276 athina-1.3.1/athina/evals/ragas/answer_correctness/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-03 15:41:49.419035 athina-1.3.1/athina/evals/ragas/answer_correctness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182502 athina-1.3.1/athina/evals/ragas/answer_relevancy/__init__.py
+-rw-r--r--   0        0        0     2441 2024-05-03 15:41:49.419202 athina-1.3.1/athina/evals/ragas/answer_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182699 athina-1.3.1/athina/evals/ragas/answer_semantic_similarity/__init__.py
+-rw-r--r--   0        0        0     2440 2024-05-03 15:41:49.419340 athina-1.3.1/athina/evals/ragas/answer_semantic_similarity/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.182961 athina-1.3.1/athina/evals/ragas/coherence/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-03 15:41:49.419789 athina-1.3.1/athina/evals/ragas/coherence/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183170 athina-1.3.1/athina/evals/ragas/conciseness/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-03 15:41:49.420084 athina-1.3.1/athina/evals/ragas/conciseness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183377 athina-1.3.1/athina/evals/ragas/context_precision/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-03 15:41:49.420494 athina-1.3.1/athina/evals/ragas/context_precision/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183558 athina-1.3.1/athina/evals/ragas/context_recall/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-03 15:41:49.420634 athina-1.3.1/athina/evals/ragas/context_recall/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183719 athina-1.3.1/athina/evals/ragas/context_relevancy/__init__.py
+-rw-r--r--   0        0        0     2159 2024-05-03 15:41:49.420776 athina-1.3.1/athina/evals/ragas/context_relevancy/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.183882 athina-1.3.1/athina/evals/ragas/faithfulness/__init__.py
+-rw-r--r--   0        0        0     2370 2024-05-03 15:41:49.420918 athina-1.3.1/athina/evals/ragas/faithfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184050 athina-1.3.1/athina/evals/ragas/harmfulness/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-03 15:41:49.421222 athina-1.3.1/athina/evals/ragas/harmfulness/evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184253 athina-1.3.1/athina/evals/ragas/maliciousness/__init__.py
+-rw-r--r--   0        0        0     2127 2024-05-03 15:41:49.421640 athina-1.3.1/athina/evals/ragas/maliciousness/evaluator.py
+-rw-r--r--   0        0        0     3298 2024-05-03 15:41:49.421803 athina-1.3.1/athina/evals/ragas/ragas_evaluator.py
+-rw-r--r--   0        0        0     5154 2024-05-03 15:41:49.422152 athina-1.3.1/athina/evals/safety/content_moderation/evaluator.py
+-rw-r--r--   0        0        0     3387 2024-05-03 15:41:49.422800 athina-1.3.1/athina/evals/safety/pii_detection/evaluator.py
+-rw-r--r--   0        0        0     4370 2024-05-03 15:41:49.424028 athina-1.3.1/athina/evals/safety/prompt_injection/evaluator.py
+-rw-r--r--   0        0        0      106 2024-05-03 15:41:49.424321 athina-1.3.1/athina/guard/exception.py
+-rw-r--r--   0        0        0     1404 2024-05-03 15:41:49.424686 athina-1.3.1/athina/guard/guard.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.184508 athina-1.3.1/athina/helpers/__init__.py
+-rw-r--r--   0        0        0     5739 2024-05-16 19:27:48.890218 athina-1.3.1/athina/helpers/athina_logging_helper.py
+-rw-r--r--   0        0        0     1351 2024-03-19 22:27:57.184662 athina-1.3.1/athina/helpers/config.py
+-rw-r--r--   0        0        0      122 2024-03-19 22:27:57.184730 athina-1.3.1/athina/helpers/constants.py
+-rw-r--r--   0        0        0      790 2024-05-16 19:27:48.890420 athina-1.3.1/athina/helpers/dataset_helper.py
+-rw-r--r--   0        0        0      172 2024-03-19 22:27:57.184807 athina-1.3.1/athina/helpers/eval_helper.py
+-rw-r--r--   0        0        0      642 2024-03-19 22:27:57.184880 athina-1.3.1/athina/helpers/function_eval_util.py
+-rw-r--r--   0        0        0     4591 2024-05-03 15:41:49.425070 athina-1.3.1/athina/helpers/get_evaluator.py
+-rw-r--r--   0        0        0      135 2024-05-25 05:42:57.983530 athina-1.3.1/athina/helpers/jinja_helper.py
+-rw-r--r--   0        0        0     2469 2024-05-22 07:52:50.227484 athina-1.3.1/athina/helpers/json.py
+-rw-r--r--   0        0        0      403 2024-03-19 22:27:57.185114 athina-1.3.1/athina/helpers/kwparser.py
+-rw-r--r--   0        0        0      894 2024-05-03 15:41:49.425348 athina-1.3.1/athina/helpers/loader_helper.py
+-rw-r--r--   0        0        0     3051 2024-03-19 22:27:57.185252 athina-1.3.1/athina/helpers/logger.py
+-rw-r--r--   0        0        0      265 2024-03-19 22:27:57.185337 athina-1.3.1/athina/helpers/package_helper.py
+-rw-r--r--   0        0        0     5296 2024-03-19 22:27:57.185429 athina-1.3.1/athina/helpers/run_helper.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.185498 athina-1.3.1/athina/interfaces/__init__.py
+-rw-r--r--   0        0        0     3905 2024-05-03 15:41:49.425463 athina-1.3.1/athina/interfaces/athina.py
+-rw-r--r--   0        0        0      132 2024-03-19 22:27:57.185654 athina-1.3.1/athina/interfaces/data.py
+-rw-r--r--   0        0        0     2065 2024-05-14 15:59:10.451321 athina-1.3.1/athina/interfaces/model.py
+-rw-r--r--   0        0        0      100 2024-03-19 22:27:57.185783 athina-1.3.1/athina/interfaces/openai.py
+-rw-r--r--   0        0        0     2944 2024-05-05 12:12:32.954417 athina-1.3.1/athina/interfaces/result.py
+-rw-r--r--   0        0        0      126 2024-03-19 22:27:57.185951 athina-1.3.1/athina/keys/__init__.py
+-rw-r--r--   0        0        0      322 2024-03-19 22:27:57.186019 athina-1.3.1/athina/keys/athina_api_key.py
+-rw-r--r--   0        0        0      236 2024-03-19 22:27:57.186085 athina-1.3.1/athina/keys/openai_api_key.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.186149 athina-1.3.1/athina/llms/__init__.py
+-rw-r--r--   0        0        0     1368 2024-05-22 07:52:50.227988 athina-1.3.1/athina/llms/abstract_llm_service.py
+-rw-r--r--   0        0        0     1524 2024-05-22 07:52:50.228405 athina-1.3.1/athina/llms/litellm_service.py
+-rw-r--r--   0        0        0     3461 2024-05-22 07:52:50.228694 athina-1.3.1/athina/llms/openai_service.py
+-rw-r--r--   0        0        0      337 2024-03-19 22:27:57.186378 athina-1.3.1/athina/llms/question_answerer.py
+-rw-r--r--   0        0        0     2874 2024-05-21 13:33:12.522927 athina-1.3.1/athina/llms/question_answerer_bulk.py
+-rw-r--r--   0        0        0     3675 2024-03-19 22:27:57.186521 athina-1.3.1/athina/llms/question_answerer_cot.py
+-rw-r--r--   0        0        0     6674 2024-05-03 15:41:49.426272 athina-1.3.1/athina/llms/question_answerer_with_retrieval.py
+-rw-r--r--   0        0        0     2402 2024-03-19 22:27:57.186684 athina-1.3.1/athina/llms/question_generator.py
+-rw-r--r--   0        0        0      323 2024-05-03 15:41:49.426530 athina-1.3.1/athina/loaders/__init__.py
+-rw-r--r--   0        0        0     2326 2024-05-16 23:56:49.987467 athina-1.3.1/athina/loaders/base_loader.py
+-rw-r--r--   0        0        0     2179 2024-05-16 19:27:48.890989 athina-1.3.1/athina/loaders/conversation_loader.py
+-rw-r--r--   0        0        0     6507 2024-05-17 01:08:19.006440 athina-1.3.1/athina/loaders/loader.py
+-rw-r--r--   0        0        0     3597 2024-05-16 19:27:48.892946 athina-1.3.1/athina/loaders/response_loader.py
+-rw-r--r--   0        0        0     2970 2024-05-03 17:07:59.624449 athina-1.3.1/athina/loaders/summary_loader.py
+-rw-r--r--   0        0        0     2380 2024-05-03 15:41:49.427400 athina-1.3.1/athina/loaders/text_loader.py
+-rw-r--r--   0        0        0     1854 2024-03-19 22:27:57.187257 athina-1.3.1/athina/metrics/agreement_score.py
+-rw-r--r--   0        0        0     2448 2024-03-19 22:27:57.187346 athina-1.3.1/athina/metrics/contradiction_score.py
+-rw-r--r--   0        0        0     1342 2024-03-19 22:27:57.187416 athina-1.3.1/athina/metrics/groundedness.py
+-rw-r--r--   0        0        0     2209 2024-03-19 22:27:57.187494 athina-1.3.1/athina/metrics/hallucination_score.py
+-rw-r--r--   0        0        0      246 2024-03-19 22:27:57.187555 athina-1.3.1/athina/metrics/metric.py
+-rw-r--r--   0        0        0     3000 2024-05-03 15:41:49.427514 athina-1.3.1/athina/metrics/metric_type.py
+-rw-r--r--   0        0        0      393 2024-03-19 22:27:57.187682 athina-1.3.1/athina/metrics/passed.py
+-rw-r--r--   0        0        0      275 2024-03-19 22:27:57.187758 athina-1.3.1/athina/metrics/ragas_metric.py
+-rw-r--r--   0        0        0      509 2024-03-19 22:27:57.187846 athina-1.3.1/athina/metrics/similarity_score.py
+-rw-r--r--   0        0        0        0 2024-03-19 22:27:57.187933 athina-1.3.1/athina/runner/__init__.py
+-rw-r--r--   0        0        0     6940 2024-05-16 19:27:48.893298 athina-1.3.1/athina/runner/run.py
+-rw-r--r--   0        0        0      341 2024-05-03 15:41:49.427983 athina-1.3.1/athina/runner/run_wrapper.py
+-rw-r--r--   0        0        0     1781 2024-05-03 15:41:49.428243 athina-1.3.1/athina/scripts/guardrails.py
+-rw-r--r--   0        0        0    13810 2024-05-25 05:42:57.984522 athina-1.3.1/athina/services/athina_api_service.py
+-rw-r--r--   0        0        0      472 2024-05-22 07:52:50.229087 athina-1.3.1/athina/steps/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-25 05:42:57.985041 athina-1.3.1/athina/steps/api.py
+-rw-r--r--   0        0        0     4456 2024-05-22 07:52:50.229580 athina-1.3.1/athina/steps/base.py
+-rw-r--r--   0        0        0     1729 2024-05-22 07:52:50.229864 athina-1.3.1/athina/steps/chain.py
+-rw-r--r--   0        0        0     1501 2024-05-22 07:52:50.230002 athina-1.3.1/athina/steps/conditional.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:52:50.230033 athina-1.3.1/athina/steps/debug.py
+-rw-r--r--   0        0        0      646 2024-05-22 07:52:50.230202 athina-1.3.1/athina/steps/iterator.py
+-rw-r--r--   0        0        0     3696 2024-05-25 05:42:57.985352 athina-1.3.1/athina/steps/llm.py
+-rw-r--r--   0        0        0      787 2024-05-22 07:52:50.230543 athina-1.3.1/athina/steps/transform.py
+-rw-r--r--   0        0        0      996 2024-05-25 05:42:57.985948 athina-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9744 1970-01-01 00:00:00.000000 athina-1.3.1/PKG-INFO
```

### Comparing `athina-1.3.0/README.md` & `athina-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/cli/cli.py` & `athina-1.3.1/athina/cli/cli.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/constants/messages.py` & `athina-1.3.1/athina/constants/messages.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/datasets/conversations.json` & `athina-1.3.1/athina/datasets/conversations.json`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/datasets/dataset.py` & `athina-1.3.1/athina/datasets/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     response: Optional[str] = None
     expected_response: Optional[str] = None
 
 @dataclass
 class Dataset:
     id: str
     source: str
+    data_source: str
     name: str
     description: Optional[str] = None
     language_model_id: Optional[str] = None
     prompt_template: Optional[Any] = None
     rows: List[DatasetRow] = field(default_factory=list)
 
     @staticmethod
@@ -35,29 +36,30 @@
         The newly created dataset object
 
         Raises:
         - Exception: If the dataset could not be created due to an error like invalid parameters, database errors, etc.
         """
         dataset_data = {
                 "source": "dev_sdk",
+                "data_source": "dev_sdk",
                 "name": name,
                 "description": description,
                 "language_model_id": language_model_id,
                 "prompt_template": prompt_template,
                 "dataset_rows": rows or []
             }
         
         # Remove keys where the value is None
         dataset_data = {k: v for k, v in dataset_data.items() if v is not None}
         
         try:
             created_dataset_data = AthinaApiService.create_dataset(dataset_data)
         except Exception as e:
             raise
-        dataset = Dataset(id=created_dataset_data['id'], source=created_dataset_data['source'], name=created_dataset_data['name'], description=created_dataset_data['description'], language_model_id=created_dataset_data['language_model_id'], prompt_template=created_dataset_data['prompt_template'])
+        dataset = Dataset(id=created_dataset_data['id'], source=created_dataset_data['source'], data_source=created_dataset_data['data_source'], name=created_dataset_data['name'], description=created_dataset_data['description'], language_model_id=created_dataset_data['language_model_id'], prompt_template=created_dataset_data['prompt_template'])
         return dataset
 
     @staticmethod
     def add_rows(dataset_id: str, rows: List[DatasetRow]):
         """
         Adds rows to a dataset in batches of 100.
```

### Comparing `athina-1.3.0/athina/datasets/summarization_sample.py` & `athina-1.3.1/athina/datasets/summarization_sample.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/datasets/yc_query_mini.py` & `athina-1.3.1/athina/datasets/yc_query_mini.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/errors/exceptions.py` & `athina-1.3.1/athina/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/__init__.py` & `athina-1.3.1/athina/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/base_evaluator.py` & `athina-1.3.1/athina/evals/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/conversation/conversation_coherence/evaluator.py` & `athina-1.3.1/athina/evals/conversation/conversation_coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/conversation/conversation_coherence/prompt.py` & `athina-1.3.1/athina/evals/conversation/conversation_coherence/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/conversation/conversation_resolution/evaluator.py` & `athina-1.3.1/athina/evals/conversation/conversation_resolution/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/conversation/conversation_resolution/prompt.py` & `athina-1.3.1/athina/evals/conversation/conversation_resolution/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/eval_type.py` & `athina-1.3.1/athina/evals/eval_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/function/function_evaluator.py` & `athina-1.3.1/athina/evals/function/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/function/functions.py` & `athina-1.3.1/athina/evals/function/functions.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/function/wrapper.py` & `athina-1.3.1/athina/evals/function/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/grounded/grounded_evaluator.py` & `athina-1.3.1/athina/evals/grounded/grounded_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/grounded/similarity.py` & `athina-1.3.1/athina/evals/grounded/similarity.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/grounded/wrapper.py` & `athina-1.3.1/athina/evals/grounded/wrapper.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/guardrails/gibberish_text/evaluator.py` & `athina-1.3.1/athina/evals/guardrails/gibberish_text/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/guardrails/sensitive_topics/evaluator.py` & `athina-1.3.1/athina/evals/guardrails/sensitive_topics/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/guardrails/sfw/evaluator.py` & `athina-1.3.1/athina/evals/guardrails/sfw/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/context_contains_enough_information/evaluator.py` & `athina-1.3.1/athina/evals/llm/context_contains_enough_information/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/context_contains_enough_information/examples.py` & `athina-1.3.1/athina/evals/llm/context_contains_enough_information/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/custom_prompt/evaluator.py` & `athina-1.3.1/athina/evals/llm/custom_prompt/evaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Dict
+from jinja2 import Environment
+from athina.helpers.jinja_helper import PreserveUndefined
 
 from athina.llms.abstract_llm_service import AbstractLlmService
 from ..llm_evaluator import LlmEvaluator
 from athina.evals.eval_type import LlmEvalTypeId
 from ..example import FewShotExample
 
 
@@ -47,14 +49,20 @@
         super().__init__(
             model=self._model,
             system_message_template=self._system_message_template,
             user_message_template=self._eval_prompt,
             llm_service=llm_service,
             **kwargs,
         )
+         # Create a custom Jinja2 environment with single curly brace delimiters and PreserveUndefined
+        self.env = Environment(
+            variable_start_string='{', 
+            variable_end_string='}',
+            undefined=PreserveUndefined
+        )
 
     @property
     def name(self):
         return LlmEvalTypeId.CUSTOM_PROMPT.value
 
     @property
     def metric_ids(self) -> List[str]:
@@ -81,10 +89,9 @@
             "eval_prompt": self._eval_prompt,
         }
 
     def is_failure(self, result) -> Optional[bool]:
         return bool(result == "Fail")
 
     def _user_message(self, **kwargs) -> str:
-        return self._user_message_template.format(
-            **kwargs,
-        )
+        template = self.env.from_string(self._user_message_template)
+        return template.render(**kwargs)
```

### Comparing `athina-1.3.0/athina/evals/llm/does_response_answer_query/evaluator.py` & `athina-1.3.1/athina/evals/llm/does_response_answer_query/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/does_response_answer_query/examples.py` & `athina-1.3.1/athina/evals/llm/does_response_answer_query/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/example.py` & `athina-1.3.1/athina/evals/llm/example.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/faithfulness/evaluator.py` & `athina-1.3.1/athina/evals/llm/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/faithfulness/examples.py` & `athina-1.3.1/athina/evals/llm/faithfulness/examples.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/grading_criteria/evaluator.py` & `athina-1.3.1/athina/evals/llm/grading_criteria/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/groundedness/evaluator.py` & `athina-1.3.1/athina/evals/llm/groundedness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/groundedness/prompt.py` & `athina-1.3.1/athina/evals/llm/groundedness/prompt.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/llm_evaluator.py` & `athina-1.3.1/athina/evals/llm/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/llm/summary_accuracy/evaluator.py` & `athina-1.3.1/athina/evals/llm/summary_accuracy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/answer_correctness/evaluator.py` & `athina-1.3.1/athina/evals/ragas/answer_correctness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/answer_relevancy/evaluator.py` & `athina-1.3.1/athina/evals/ragas/answer_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/answer_semantic_similarity/evaluator.py` & `athina-1.3.1/athina/evals/ragas/answer_semantic_similarity/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/coherence/evaluator.py` & `athina-1.3.1/athina/evals/ragas/coherence/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/conciseness/evaluator.py` & `athina-1.3.1/athina/evals/ragas/conciseness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/context_precision/evaluator.py` & `athina-1.3.1/athina/evals/ragas/context_precision/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/context_recall/evaluator.py` & `athina-1.3.1/athina/evals/ragas/context_recall/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/context_relevancy/evaluator.py` & `athina-1.3.1/athina/evals/ragas/context_relevancy/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/faithfulness/evaluator.py` & `athina-1.3.1/athina/evals/ragas/faithfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/harmfulness/evaluator.py` & `athina-1.3.1/athina/evals/ragas/harmfulness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/maliciousness/evaluator.py` & `athina-1.3.1/athina/evals/ragas/maliciousness/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/ragas/ragas_evaluator.py` & `athina-1.3.1/athina/evals/ragas/ragas_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/safety/content_moderation/evaluator.py` & `athina-1.3.1/athina/evals/safety/content_moderation/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/safety/pii_detection/evaluator.py` & `athina-1.3.1/athina/evals/safety/pii_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/evals/safety/prompt_injection/evaluator.py` & `athina-1.3.1/athina/evals/safety/prompt_injection/evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/guard/guard.py` & `athina-1.3.1/athina/guard/guard.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/athina_logging_helper.py` & `athina-1.3.1/athina/helpers/athina_logging_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/config.py` & `athina-1.3.1/athina/helpers/config.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/dataset_helper.py` & `athina-1.3.1/athina/helpers/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/function_eval_util.py` & `athina-1.3.1/athina/helpers/function_eval_util.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/get_evaluator.py` & `athina-1.3.1/athina/helpers/get_evaluator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/json.py` & `athina-1.3.1/athina/helpers/json.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/loader_helper.py` & `athina-1.3.1/athina/helpers/loader_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/logger.py` & `athina-1.3.1/athina/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/helpers/run_helper.py` & `athina-1.3.1/athina/helpers/run_helper.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/interfaces/athina.py` & `athina-1.3.1/athina/interfaces/athina.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/interfaces/model.py` & `athina-1.3.1/athina/interfaces/model.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/interfaces/result.py` & `athina-1.3.1/athina/interfaces/result.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/abstract_llm_service.py` & `athina-1.3.1/athina/llms/abstract_llm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/litellm_service.py` & `athina-1.3.1/athina/llms/litellm_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/openai_service.py` & `athina-1.3.1/athina/llms/openai_service.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/question_answerer_bulk.py` & `athina-1.3.1/athina/llms/question_answerer_bulk.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/question_answerer_cot.py` & `athina-1.3.1/athina/llms/question_answerer_cot.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/question_answerer_with_retrieval.py` & `athina-1.3.1/athina/llms/question_answerer_with_retrieval.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/llms/question_generator.py` & `athina-1.3.1/athina/llms/question_generator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/loaders/base_loader.py` & `athina-1.3.1/athina/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/loaders/conversation_loader.py` & `athina-1.3.1/athina/loaders/conversation_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/loaders/loader.py` & `athina-1.3.1/athina/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/loaders/response_loader.py` & `athina-1.3.1/athina/loaders/response_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/loaders/summary_loader.py` & `athina-1.3.1/athina/loaders/summary_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/loaders/text_loader.py` & `athina-1.3.1/athina/loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/metrics/agreement_score.py` & `athina-1.3.1/athina/metrics/agreement_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/metrics/contradiction_score.py` & `athina-1.3.1/athina/metrics/contradiction_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/metrics/groundedness.py` & `athina-1.3.1/athina/metrics/groundedness.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/metrics/hallucination_score.py` & `athina-1.3.1/athina/metrics/hallucination_score.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/metrics/metric_type.py` & `athina-1.3.1/athina/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/runner/run.py` & `athina-1.3.1/athina/runner/run.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/scripts/guardrails.py` & `athina-1.3.1/athina/scripts/guardrails.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/services/athina_api_service.py` & `athina-1.3.1/athina/services/athina_api_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     def create_dataset(
         dataset: Dict
     ):
         """
         Creates a dataset by calling the Athina API
         """
         try:
-            endpoint = f"{API_BASE_URL}/api/v1/dataset"
+            endpoint = f"{API_BASE_URL}/api/v1/dataset_v2"
             response = requests.post(
                 endpoint,
                 headers=AthinaApiService._headers(),
                 json=dataset,
             )
             if response.status_code == 401:
                 response_json = response.json()
@@ -162,15 +162,15 @@
         Returns:
         The API response data for the dataset after adding the rows.
 
         Raises:
         - CustomException: If the API call fails or returns an error.
         """
         try:
-            endpoint = f"{API_BASE_URL}/api/v1/dataset/{dataset_id}/add-rows"
+            endpoint = f"{API_BASE_URL}/api/v1/dataset_v2/{dataset_id}/add-rows"
             response = requests.post(
                 endpoint,
                 headers=AthinaApiService._headers(),
                 json={"dataset_rows": rows},
             )
             if response.status_code == 401:
                 response_json = response.json()
```

### Comparing `athina-1.3.0/athina/steps/api.py` & `athina-1.3.1/athina/steps/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Step to make an external api call
+import json
 from typing import Union, Dict, Any, Iterable, Optional
-
 import requests
-
 from athina.steps import Step
+from jinja2 import Environment
+from athina.helpers.jinja_helper import PreserveUndefined
 
 
 class ApiCall(Step):
     """
     Step that makes an external API call.
 
     Attributes:
@@ -21,32 +22,44 @@
 
     url: str
     method: str
     headers: Optional[Dict[str, str]] = None
     params: Optional[Dict[str, Any]] = None
     body: Optional[str] = None
     expected_status_codes: Iterable[int] = (200,)
+    env: Environment = None
+
+    class Config:
+        arbitrary_types_allowed = True
 
     def execute(self, input_data: Any) -> Union[Dict[str, Any], None]:
         """Make an API call and return the response."""
 
         if input_data is None:
             input_data = {}
 
         if not isinstance(input_data, dict):
             raise TypeError("Input data must be a dictionary.")
 
+        # Create a custom Jinja2 environment with double curly brace delimiters and PreserveUndefined
+        self.env = Environment(
+            variable_start_string='{{', 
+            variable_end_string='}}',
+            undefined=PreserveUndefined
+        )
+
         if self.body is not None:
-            self.body = self.body.format(**input_data)
+            body_template = self.env.from_string(self.body)
+            self.body = body_template.render(**input_data)
 
         response = requests.request(
             method=self.method,
             url=self.url,
             headers=self.headers,
             params=self.params,
-            json=self.body,
+            json=json.loads(self.body),
         )
 
         if response.status_code in self.expected_status_codes:
             return response.json()
         else:
             return None
```

### Comparing `athina-1.3.0/athina/steps/base.py` & `athina-1.3.1/athina/steps/base.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/steps/chain.py` & `athina-1.3.1/athina/steps/chain.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/steps/conditional.py` & `athina-1.3.1/athina/steps/conditional.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/steps/iterator.py` & `athina-1.3.1/athina/steps/iterator.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/athina/steps/llm.py` & `athina-1.3.1/athina/steps/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import List, Dict, Any, Optional
 from athina.helpers.json import JsonExtractor
 from athina.interfaces.model import Model
 from athina.steps.base import Step
 from athina.llms.abstract_llm_service import AbstractLlmService
 from athina.keys import OpenAiApiKey
 from athina.llms.openai_service import OpenAiService
+from jinja2 import Environment
+from athina.helpers.jinja_helper import PreserveUndefined
 
 
 class PromptMessage(BaseModel):
     role: str
     content: str
 
 class ModelOptions(BaseModel):
@@ -19,28 +21,40 @@
     top_p: Optional[float] = None
     frequency_penalty: Optional[float] = None
     presence_penalty: Optional[float] = None
 
 
 class PromptTemplate(BaseModel):
     messages: List[PromptMessage]
+    env: Environment = None
 
+    class Config:
+        arbitrary_types_allowed = True
     @staticmethod
     def simple(message: str) -> "PromptTemplate":
         """Create a PromptTemplate from a string representation."""
         messages = [PromptMessage(role="user", content=message)]
         return PromptTemplate(messages=messages)
 
     def resolve(self, **kwargs) -> List[PromptMessage]:
         """Render the template with given variables."""
+
+        # Create a custom Jinja2 environment with double curly brace delimiters and PreserveUndefined
+        self.env = Environment(
+            variable_start_string='{{', 
+            variable_end_string='}}',
+            undefined=PreserveUndefined
+        )
         resolved_messages = []
         for message in self.messages:
-            content = message.content.format(**kwargs)
+            content_template = self.env.from_string(message.content)
+            content = content_template.render(**kwargs)
             resolved_message = PromptMessage(role=message.role, content=content)
             resolved_messages.append(resolved_message)
+
         return resolved_messages
 
 
 class PromptExecution(Step):
     """
     Step that executes a prompt using an LLM service.
```

### Comparing `athina-1.3.0/athina/steps/transform.py` & `athina-1.3.1/athina/steps/transform.py`

 * *Files identical despite different names*

### Comparing `athina-1.3.0/pyproject.toml` & `athina-1.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athina"
-version = "1.3.0"
+version = "1.3.1"
 description = "Python SDK to configure and run evaluations for your LLM-based application"
 authors = ["Shiv Sakhuja <shiv@athina.ai>", "Akshat Gupta <akshat@athina.ai>", "Vivek Aditya <vivek@athina.ai>", "Akhil Bisht <akhil@athina.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 retrying = "^1.3.4"
@@ -18,14 +18,15 @@
 datasets = "^2.16.0"
 python-dotenv = "^1.0.0"
 requests = "^2.31.0"
 langchain-openai = "^0.0.3"
 llama-index = "^0.9.40"
 pydantic = ">=2.0,<3.0"
 litellm = "1.35.6"
+jinja2 = "^3.1.4"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `athina-1.3.0/PKG-INFO` & `athina-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: athina
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK to configure and run evaluations for your LLM-based application
 Author: Shiv Sakhuja
 Author-email: shiv@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: datasets (>=2.16.0,<3.0.0)
+Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: langchain (>=0.0.350)
 Requires-Dist: langchain-openai (>=0.0.3,<0.0.4)
 Requires-Dist: litellm (==1.35.6)
 Requires-Dist: llama-index (>=0.9.40,<0.10.0)
 Requires-Dist: openai (>=1.3.4,<2.0.0)
 Requires-Dist: pandas
 Requires-Dist: pydantic (>=2.0,<3.0)
```


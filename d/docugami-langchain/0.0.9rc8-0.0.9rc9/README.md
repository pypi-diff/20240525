# Comparing `tmp/docugami_langchain-0.0.9rc8.tar.gz` & `tmp/docugami_langchain-0.0.9rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.9rc8.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.9rc9.tar", max compression
```

## Comparing `docugami_langchain-0.0.9rc8.tar` & `docugami_langchain-0.0.9rc9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1072 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/LICENSE
--rw-r--r--   0        0        0      361 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/README.md
--rw-r--r--   0        0        0      747 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      487 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     8818 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0     1805 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/agents/models.py
--rw-r--r--   0        0        0    11237 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     9152 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/agents/tool_router_agent.py
--rw-r--r--   0        0        0    16628 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0     1506 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     1415 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3390 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3980 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3838 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3983 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0      647 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     3398 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0      262 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/models.py
--rw-r--r--   0        0        0     4112 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8571 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0      722 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0      124 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/models.py
--rw-r--r--   0        0        0     4409 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0     4006 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/standalone_question_chain.py
--rw-r--r--   0        0        0     4592 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/suggested_questions_chain.py
--rw-r--r--   0        0        0     4193 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/suggested_report_chain.py
--rw-r--r--   0        0        0     3600 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/tool_final_answer_chain.py
--rw-r--r--   0        0        0     4091 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/tool_output_grader_chain.py
--rw-r--r--   0        0        0      567 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/__init__.py
--rw-r--r--   0        0        0      999 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/common.py
--rw-r--r--   0        0        0     3147 2024-05-15 02:52:06.906777 docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/data_type_detection_chain.py
--rw-r--r--   0        0        0     3243 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/date_add_chain.py
--rw-r--r--   0        0        0     3102 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/date_parse_chain.py
--rw-r--r--   0        0        0     2464 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/timespan_parse_chain.py
--rw-r--r--   0        0        0     1604 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     2798 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/history.py
--rw-r--r--   0        0        0      797 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     4206 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/custom_react_json_single_input.py
--rw-r--r--   0        0        0     2091 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1075 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1242 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     2816 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0      735 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/text_cleaning.py
--rw-r--r--   0        0        0     4502 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      847 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/params.py
--rw-r--r--   0        0        0      122 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     7894 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5890 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0      194 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/tools/__init__.py
--rw-r--r--   0        0        0     3958 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/tools/common.py
--rw-r--r--   0        0        0     8697 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     6830 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0      708 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/utils/documents.py
--rw-r--r--   0        0        0     8975 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/utils/sql.py
--rw-r--r--   0        0        0     3389 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/docugami_langchain/utils/string_cleanup.py
--rw-r--r--   0        0        0     2823 2024-05-15 02:52:06.910776 docugami_langchain-0.0.9rc8/pyproject.toml
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/LICENSE
+-rw-r--r--   0        0        0      361 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/README.md
+-rw-r--r--   0        0        0      747 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     8818 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0     1805 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/agents/models.py
+-rw-r--r--   0        0        0    11237 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     9152 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/agents/tool_router_agent.py
+-rw-r--r--   0        0        0    16628 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0     1506 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     1415 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3980 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3838 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3983 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0      647 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     3398 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0      262 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/models.py
+-rw-r--r--   0        0        0     4164 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     8780 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0      722 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/models.py
+-rw-r--r--   0        0        0     4409 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0     4006 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/standalone_question_chain.py
+-rw-r--r--   0        0        0     4592 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/suggested_questions_chain.py
+-rw-r--r--   0        0        0     4193 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/suggested_report_chain.py
+-rw-r--r--   0        0        0     3600 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/tool_final_answer_chain.py
+-rw-r--r--   0        0        0     4091 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/tool_output_grader_chain.py
+-rw-r--r--   0        0        0      567 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/common.py
+-rw-r--r--   0        0        0     3147 2024-05-19 06:50:53.175294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/data_type_detection_chain.py
+-rw-r--r--   0        0        0     3243 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/date_add_chain.py
+-rw-r--r--   0        0        0     3102 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/date_parse_chain.py
+-rw-r--r--   0        0        0     2464 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/timespan_parse_chain.py
+-rw-r--r--   0        0        0     1604 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     2798 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/history.py
+-rw-r--r--   0        0        0      797 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     4206 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/custom_react_json_single_input.py
+-rw-r--r--   0        0        0     2091 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1075 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1242 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     2816 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0      735 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/text_cleaning.py
+-rw-r--r--   0        0        0     4502 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      847 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/params.py
+-rw-r--r--   0        0        0      122 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     7894 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5890 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0      194 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/tools/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/tools/common.py
+-rw-r--r--   0        0        0     8697 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     6830 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0      708 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/utils/documents.py
+-rw-r--r--   0        0        0     8975 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/utils/sql.py
+-rw-r--r--   0        0        0     3389 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/docugami_langchain/utils/string_cleanup.py
+-rw-r--r--   0        0        0     2821 2024-05-19 06:50:53.179294 docugami_langchain-0.0.9rc9/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc9/PKG-INFO
```

### Comparing `docugami_langchain-0.0.9rc8/LICENSE` & `docugami_langchain-0.0.9rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/__init__.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/agents/base.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/agents/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/agents/models.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/agents/models.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/agents/re_act_agent.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/agents/re_act_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/agents/tool_router_agent.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/agents/tool_router_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/base_runnable.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/base_runnable.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/base.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/__init__.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 "- Make sure all column names in SELECT statements actually exist in the table (update column names if you find a near match)",
                 "- Don't select more than 10 columns to avoid making the query so long that it gets truncated",
                 "",
                 "If you see any of the above mistakes, or any other mistakes, rewrite the query to fix them. If there are no mistakes, just reproduce the original query.",
             ],
             stop_sequences=["\n", ";", "<|eot_id|>"],
             additional_runnables=[TextCleaningOutputParser(), SQLFindingOutputParser()],
+            include_output_instruction_suffix=True,
         )
 
     def run(  # type: ignore[override]
         self,
         table_info: str,
         sql_query: str,
         exception: str = "",
```

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,32 +79,35 @@
                 return {
                     "question": question,
                     "sql_query": sql_query,
                     "sql_result": str(self.db.run(sql_query)).strip(),
                 }
 
             except Exception as exc:
-                # If any exception with Raw SQL, try to fix up the SQL
-                # giving the LLM context on the exception to aid fixup
-                fixed_sql_response = self.sql_fixup_chain.run(
-                    table_info=table_info,
-                    sql_query=sql_query,
-                    exception=str(exc),
-                    config=config,  # Pass the config down to link traces in langsmith
-                )
-
-                # Run Fixed-up SQL
-                fixed_sql = fixed_sql_response.value
-                fixed_sql = check_and_format_query(self.db, fixed_sql)
-
-                return {
-                    "question": question,
-                    "sql_query": fixed_sql,
-                    "sql_result": str(self.db.run(fixed_sql)).strip(),
-                }
+                if not self.sql_fixup_chain:
+                    raise
+                else:
+                    # If any exception with Raw SQL, try to fix up the SQL
+                    # giving the LLM context on the exception to aid fixup
+                    fixed_sql_response = self.sql_fixup_chain.run(
+                        table_info=table_info,
+                        sql_query=sql_query,
+                        exception=str(exc),
+                        config=config,  # Pass the config down to link traces in langsmith
+                    )
+
+                    # Run Fixed-up SQL
+                    fixed_sql = fixed_sql_response.value
+                    fixed_sql = check_and_format_query(self.db, fixed_sql)
+
+                    return {
+                        "question": question,
+                        "sql_query": fixed_sql,
+                        "sql_result": str(self.db.run(fixed_sql)).strip(),
+                    }
 
         return {
             "question": itemgetter("question"),
             "sql_query": {
                 "question": itemgetter("question"),
                 "table_info": RunnableLambda(table_info_func),
             }
@@ -145,14 +148,15 @@
                 """- When matching strings in WHERE clauses, always use LIKE with LOWER rather than exact string match with "=" since users may not fully specify complete input with the right """
                 + """casing, for example generate SELECT * from "athletes" WHERE LOWER("last name") LIKE '%jones%' instead of SELECT * from "athletes" WHERE "last name" = 'Jones'""",
                 "- Never provide any additional explanation or discussion, only output the SQLite query requested, which answers the question against the given table description.",
                 "- If example rows are given, pay special attention to them to improve your query e.g. to account for abbreviations or formatting of values.",
             ],
             stop_sequences=["\n", ";", "<|eot_id|>"],
             additional_runnables=[TextCleaningOutputParser(), SQLFindingOutputParser()],
+            include_output_instruction_suffix=True,
         )
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
     ) -> TracedResponse[ExplainedSQLResult]:
```

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/__init__.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/standalone_question_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/standalone_question_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/suggested_questions_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/suggested_questions_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/suggested_report_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/suggested_report_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/tool_final_answer_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/tool_final_answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/rag/tool_output_grader_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/rag/tool_output_grader_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/__init__.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/common.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/data_type_detection_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/data_type_detection_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/date_add_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/date_add_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/date_parse_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/date_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/chains/types/timespan_parse_chain.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/chains/types/timespan_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/config.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/config.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/history.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/history.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/custom_react_json_single_input.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/custom_react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/datetime.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/text_cleaning.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/params.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/params.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/retrievers/fused_summary.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/retrievers/fused_summary.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/retrievers/mappings.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/tools/common.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/tools/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/tools/reports.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/tools/retrieval.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/utils/documents.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/utils/documents.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/utils/sql.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/utils/sql.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/docugami_langchain/utils/string_cleanup.py` & `docugami_langchain-0.0.9rc9/docugami_langchain/utils/string_cleanup.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.9rc8/pyproject.toml` & `docugami_langchain-0.0.9rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.9rc8"
+version = "0.0.9rc9"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/docugami/docugami-langchain/tree/master"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = ">=0.1.52"
-langchain-community = ">=0.0.38"
-langgraph = ">=0.0.48"
+langchain-core = ">=0.2.0"
+langchain-community = ">=0.2.0"
+langgraph = ">=0.0.50"
 dgml-utils = ">=0.3.3"
 wordtodigits = ">=1.0.2"
 python-dateutil = ">=2.9.0"
 pandas = "*"
 pyyaml = ">=6.0.1"
 openpyxl = ">=3.1.2"
-sqlglot = ">=23.15.8"
+sqlglot = ">=23.16.0"
 tabulate = ">=0.9.0"
-rerankers = { extras = ["all"], version = ">=0.2.0" }
+rerankers = { extras = ["all"], version = ">=0.3.0" }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 flaky = "^3.8.1"
 pytest = ">=8.1.1"
```

### Comparing `docugami_langchain-0.0.9rc8/PKG-INFO` & `docugami_langchain-0.0.9rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.9rc8
+Version: 0.0.9rc9
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dgml-utils (>=0.3.3)
-Requires-Dist: langchain-community (>=0.0.38)
-Requires-Dist: langchain-core (>=0.1.52)
-Requires-Dist: langgraph (>=0.0.48)
+Requires-Dist: langchain-community (>=0.2.0)
+Requires-Dist: langchain-core (>=0.2.0)
+Requires-Dist: langgraph (>=0.0.50)
 Requires-Dist: openpyxl (>=3.1.2)
 Requires-Dist: pandas
 Requires-Dist: python-dateutil (>=2.9.0)
 Requires-Dist: pyyaml (>=6.0.1)
-Requires-Dist: rerankers[all] (>=0.2.0)
-Requires-Dist: sqlglot (>=23.15.8)
+Requires-Dist: rerankers[all] (>=0.3.0)
+Requires-Dist: sqlglot (>=23.16.0)
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: wordtodigits (>=1.0.2)
 Project-URL: Repository, https://github.com/docugami/docugami-langchain
 Project-URL: Source Code, https://github.com/docugami/docugami-langchain/tree/master
 Description-Content-Type: text/markdown
 
 # docugami-langchain
```


# Comparing `tmp/blackboxai-2.7.tar.gz` & `tmp/blackboxai-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxai-2.7.tar", last modified: Tue May  7 12:14:57 2024, max compression
+gzip compressed data, was "blackboxai-2.8.tar", last modified: Sun May 19 20:28:48 2024, max compression
```

## Comparing `blackboxai-2.7.tar` & `blackboxai-2.8.tar`

### file list

```diff
@@ -1,160 +1,302 @@
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.909585 blackboxai-2.7/
--rw-r--r--   0 rizkrichard   (501) staff       (20)    33813 2024-05-06 17:45:40.000000 blackboxai-2.7/LICENSE
--rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-05-07 12:14:57.909433 blackboxai-2.7/PKG-INFO
--rw-r--r--   0 rizkrichard   (501) staff       (20)      635 2024-05-07 02:15:32.000000 blackboxai-2.7/README.md
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.859877 blackboxai-2.7/blackboxai/
--rw-r--r--   0 rizkrichard   (501) staff       (20)       25 2024-05-06 17:45:40.000000 blackboxai-2.7/blackboxai/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2698 2024-05-07 05:35:21.000000 blackboxai-2.7/blackboxai/chat.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.860093 blackboxai-2.7/blackboxai/interpreter/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      652 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.862075 blackboxai-2.7/blackboxai/interpreter/core/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2820 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.862848 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1293 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3138 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3046 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/browser.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.863040 blackboxai-2.7/blackboxai/interpreter/core/computer/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.863445 blackboxai-2.7/blackboxai/interpreter/core/computer/ai/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/ai/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     5688 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/ai/ai.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.863959 blackboxai-2.7/blackboxai/interpreter/core/computer/browser/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/browser/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      416 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/browser/browser.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.864343 blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    12950 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/calendar.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.864722 blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      879 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/clipboard.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2831 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/computer.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.866070 blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3293 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/contacts.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.866640 blackboxai-2.7/blackboxai/interpreter/core/computer/display/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/display/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    10556 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/display/display.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.867047 blackboxai-2.7/blackboxai/interpreter/core/computer/docs/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/docs/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      749 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/docs/docs.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.867370 blackboxai-2.7/blackboxai/interpreter/core/computer/files/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/files/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1698 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/files/files.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.867731 blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3553 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/keyboard.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.868058 blackboxai-2.7/blackboxai/interpreter/core/computer/mail/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mail/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     6350 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mail/mail.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.869945 blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    12423 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/mouse.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.871286 blackboxai-2.7/blackboxai/interpreter/core/computer/os/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/os/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2961 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/os/os.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.871717 blackboxai-2.7/blackboxai/interpreter/core/computer/skills/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:30:00.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/skills/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     4535 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/skills/skills.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.873998 blackboxai-2.7/blackboxai/interpreter/core/computer/sms/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/sms/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1399 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/sms/sms.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.874875 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1090 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/base_language.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.881783 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     5164 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1812 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      858 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/html.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1924 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    15293 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2193 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      293 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/python.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2360 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/r.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2503 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/react.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2727 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/shell.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     6715 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     4946 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/terminal.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.883353 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:29:48.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     7097 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/computer_vision.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1479 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/get_active_window.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      929 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      396 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/recipient_utils.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      586 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/computer/utils/run_applescript.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    14529 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/core.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3288 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/core/default_system_message.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.886727 blackboxai-2.7/blackboxai/interpreter/core/llm/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     7323 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/agent_llm.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     9084 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/llm.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     5052 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/run_function_calling_llm.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3899 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/run_text_llm.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.891542 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:30:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    11769 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      711 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/merge_deltas.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1800 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      538 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/llm/vision_for_text_llms.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1688 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/render_message.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    14523 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/respond.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      690 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/search.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     6162 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/server.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.899712 blackboxai-2.7/blackboxai/interpreter/core/utils/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      630 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      360 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1096 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      920 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/lazy_import.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2118 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/scan_code.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     4404 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/system_debug_info.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1736 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/telemetry.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1098 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/temporary_file.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      510 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/core/utils/truncate_output.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.902435 blackboxai-2.7/blackboxai/interpreter/terminal_interface/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2433 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)        0 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.903230 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:28:24.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      611 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/base_block.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2664 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/code_block.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1386 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/message_block.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2905 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/conversation_navigator.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    10586 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/magic_commands.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.903773 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:28:36.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)       25 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    40533 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/profiles.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2304 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/render_past_conversation.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    14917 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    27491 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/terminal_interface.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.908099 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/
--rw-rw-r--   0 rizkrichard   (501) staff       (20)    25835 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3099 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-05-07 05:27:08.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/__init__.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     4954 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/agent_utils.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      512 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      481 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      419 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/cli_input.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     1939 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      884 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     3069 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_output.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      459 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      250 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      184 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)      316 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)       79 2024-05-06 16:51:30.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
--rw-rw-r--   0 rizkrichard   (501) staff       (20)     2887 2024-05-07 12:13:42.000000 blackboxai-2.7/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.908825 blackboxai-2.7/blackboxai.egg-info/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/PKG-INFO
--rw-r--r--   0 rizkrichard   (501) staff       (20)     7239 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/SOURCES.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)        1 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/dependency_links.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)       50 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/entry_points.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)       11 2024-05-07 12:14:57.000000 blackboxai-2.7/blackboxai.egg-info/top_level.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1959 2024-05-07 02:17:56.000000 blackboxai-2.7/pyproject.toml
--rw-r--r--   0 rizkrichard   (501) staff       (20)       38 2024-05-07 12:14:57.909631 blackboxai-2.7/setup.cfg
--rw-r--r--   0 rizkrichard   (501) staff       (20)      523 2024-05-07 03:00:25.000000 blackboxai-2.7/setup.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-05-07 12:14:57.908937 blackboxai-2.7/tests/
--rw-r--r--   0 rizkrichard   (501) staff       (20)    21812 2024-05-07 02:17:56.000000 blackboxai-2.7/tests/test_interpreter.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.878174 blackboxai-2.8/
+-rw-rw-r--   0 em         (501) staff       (20)    33813 2024-05-10 07:30:29.000000 blackboxai-2.8/LICENSE
+-rw-r--r--   0 em         (501) staff       (20)      750 2024-05-19 20:28:48.877962 blackboxai-2.8/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)      635 2024-05-19 15:41:33.000000 blackboxai-2.8/README.md
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.838542 blackboxai-2.8/blackboxai/
+-rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     2718 2024-05-19 20:10:15.000000 blackboxai-2.8/blackboxai/chat.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.838677 blackboxai-2.8/blackboxai/interpreter/
+-rw-r--r--   0 em         (501) staff       (20)      652 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.841246 blackboxai-2.8/blackboxai/interpreter/core/
+-rw-r--r--   0 em         (501) staff       (20)     2820 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.841815 blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_rag/
+-rw-r--r--   0 em         (501) staff       (20)     1293 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-r--r--   0 em         (501) staff       (20)     3138 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     3046 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.842061 blackboxai-2.8/blackboxai/interpreter/core/computer/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.842356 blackboxai-2.8/blackboxai/interpreter/core/computer/ai/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/ai/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     5688 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.842674 blackboxai-2.8/blackboxai/interpreter/core/computer/browser/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/browser/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      416 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.842972 blackboxai-2.8/blackboxai/interpreter/core/computer/calendar/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/calendar/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    12950 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/calendar/calendar.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.843265 blackboxai-2.8/blackboxai/interpreter/core/computer/clipboard/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/clipboard/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      879 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/clipboard/clipboard.py
+-rw-r--r--   0 em         (501) staff       (20)     2831 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/computer.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.843516 blackboxai-2.8/blackboxai/interpreter/core/computer/contacts/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/contacts/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     3293 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/contacts/contacts.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.843807 blackboxai-2.8/blackboxai/interpreter/core/computer/display/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/display/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    10556 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.844058 blackboxai-2.8/blackboxai/interpreter/core/computer/docs/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/docs/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      749 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.844305 blackboxai-2.8/blackboxai/interpreter/core/computer/files/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/files/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1698 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.844599 blackboxai-2.8/blackboxai/interpreter/core/computer/keyboard/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/keyboard/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     3553 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.844899 blackboxai-2.8/blackboxai/interpreter/core/computer/mail/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/mail/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     6350 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/mail/mail.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.845210 blackboxai-2.8/blackboxai/interpreter/core/computer/mouse/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/mouse/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    12423 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.845509 blackboxai-2.8/blackboxai/interpreter/core/computer/os/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/os/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     2961 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.845776 blackboxai-2.8/blackboxai/interpreter/core/computer/skills/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/skills/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     4535 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.846068 blackboxai-2.8/blackboxai/interpreter/core/computer/sms/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/sms/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1399 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/sms/sms.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.846639 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1090 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.848482 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/
+-rw-r--r--   0 em         (501) staff       (20)     5164 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1812 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
+-rw-r--r--   0 em         (501) staff       (20)      858 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/html.py
+-rw-r--r--   0 em         (501) staff       (20)     1924 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
+-rw-r--r--   0 em         (501) staff       (20)    15293 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-r--r--   0 em         (501) staff       (20)     2193 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
+-rw-r--r--   0 em         (501) staff       (20)      293 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/python.py
+-rw-r--r--   0 em         (501) staff       (20)     2360 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/r.py
+-rw-r--r--   0 em         (501) staff       (20)     2503 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/react.py
+-rw-r--r--   0 em         (501) staff       (20)     2727 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/shell.py
+-rw-r--r--   0 em         (501) staff       (20)     6715 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-r--r--   0 em         (501) staff       (20)     4946 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.849461 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     7097 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/computer_vision.py
+-rw-r--r--   0 em         (501) staff       (20)     1479 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/get_active_window.py
+-rw-r--r--   0 em         (501) staff       (20)      929 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-r--r--   0 em         (501) staff       (20)      396 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/recipient_utils.py
+-rw-r--r--   0 em         (501) staff       (20)      586 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/computer/utils/run_applescript.py
+-rw-r--r--   0 em         (501) staff       (20)    14532 2024-05-19 20:28:04.000000 blackboxai-2.8/blackboxai/interpreter/core/core.py
+-rw-r--r--   0 em         (501) staff       (20)     3288 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/default_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.850287 blackboxai-2.8/blackboxai/interpreter/core/llm/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     7323 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/agent_llm.py
+-rw-r--r--   0 em         (501) staff       (20)     9084 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/llm.py
+-rw-r--r--   0 em         (501) staff       (20)     5052 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/run_function_calling_llm.py
+-rw-r--r--   0 em         (501) staff       (20)     3899 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.850833 blackboxai-2.8/blackboxai/interpreter/core/llm/utils/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    11769 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-r--r--   0 em         (501) staff       (20)      711 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/utils/merge_deltas.py
+-rw-r--r--   0 em         (501) staff       (20)     1800 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
+-rw-r--r--   0 em         (501) staff       (20)      538 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/llm/vision_for_text_llms.py
+-rw-r--r--   0 em         (501) staff       (20)     1688 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/render_message.py
+-rw-r--r--   0 em         (501) staff       (20)    14523 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/respond.py
+-rw-r--r--   0 em         (501) staff       (20)      696 2024-05-19 20:28:05.000000 blackboxai-2.8/blackboxai/interpreter/core/search.py
+-rw-r--r--   0 em         (501) staff       (20)     6162 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/server.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.852198 blackboxai-2.8/blackboxai/interpreter/core/utils/
+-rw-r--r--   0 em         (501) staff       (20)      630 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
+-rw-r--r--   0 em         (501) staff       (20)      360 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-r--r--   0 em         (501) staff       (20)     1096 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      920 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/lazy_import.py
+-rw-r--r--   0 em         (501) staff       (20)     2118 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/scan_code.py
+-rw-r--r--   0 em         (501) staff       (20)     4404 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/system_debug_info.py
+-rw-r--r--   0 em         (501) staff       (20)     1736 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/telemetry.py
+-rw-r--r--   0 em         (501) staff       (20)     1098 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/temporary_file.py
+-rw-r--r--   0 em         (501) staff       (20)      510 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.854086 blackboxai-2.8/blackboxai/interpreter/terminal_interface/
+-rw-r--r--   0 em         (501) staff       (20)     2433 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.854640 blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      611 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/base_block.py
+-rw-r--r--   0 em         (501) staff       (20)     2664 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/code_block.py
+-rw-r--r--   0 em         (501) staff       (20)     1386 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/message_block.py
+-rw-r--r--   0 em         (501) staff       (20)     2905 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/conversation_navigator.py
+-rw-r--r--   0 em         (501) staff       (20)    10586 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/magic_commands.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.855053 blackboxai-2.8/blackboxai/interpreter/terminal_interface/profiles/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/profiles/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-r--r--   0 em         (501) staff       (20)    40533 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/profiles/profiles.py
+-rw-r--r--   0 em         (501) staff       (20)     2304 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/render_past_conversation.py
+-rw-r--r--   0 em         (501) staff       (20)    14917 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
+-rw-r--r--   0 em         (501) staff       (20)    27494 2024-05-19 20:28:04.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.857465 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/
+-rw-r--r--   0 em         (501) staff       (20)    25835 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-r--r--   0 em         (501) staff       (20)     3099 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     4954 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/agent_utils.py
+-rw-r--r--   0 em         (501) staff       (20)      512 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
+-rw-r--r--   0 em         (501) staff       (20)      481 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
+-rw-r--r--   0 em         (501) staff       (20)      419 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/cli_input.py
+-rw-r--r--   0 em         (501) staff       (20)     1939 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
+-rw-r--r--   0 em         (501) staff       (20)      884 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-r--r--   0 em         (501) staff       (20)     3069 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/display_output.py
+-rw-r--r--   0 em         (501) staff       (20)      459 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
+-rw-r--r--   0 em         (501) staff       (20)      250 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
+-rw-r--r--   0 em         (501) staff       (20)      184 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-r--r--   0 em         (501) staff       (20)      316 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-r--r--   0 em         (501) staff       (20)       79 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
+-rw-r--r--   0 em         (501) staff       (20)     2887 2024-05-18 20:28:33.000000 blackboxai-2.8/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.877689 blackboxai-2.8/blackboxai.egg-info/
+-rw-r--r--   0 em         (501) staff       (20)      750 2024-05-19 20:28:48.000000 blackboxai-2.8/blackboxai.egg-info/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)    12938 2024-05-19 20:28:48.000000 blackboxai-2.8/blackboxai.egg-info/SOURCES.txt
+-rw-r--r--   0 em         (501) staff       (20)        1 2024-05-19 20:28:48.000000 blackboxai-2.8/blackboxai.egg-info/dependency_links.txt
+-rw-r--r--   0 em         (501) staff       (20)       50 2024-05-19 20:28:48.000000 blackboxai-2.8/blackboxai.egg-info/entry_points.txt
+-rw-r--r--   0 em         (501) staff       (20)       23 2024-05-19 20:28:48.000000 blackboxai-2.8/blackboxai.egg-info/top_level.txt
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.857633 blackboxai-2.8/interpreter/
+-rw-rw-r--   0 em         (501) staff       (20)      652 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.859847 blackboxai-2.8/interpreter/core/
+-rw-rw-r--   0 em         (501) staff       (20)     2820 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.860431 blackboxai-2.8/interpreter/core/ARCHIVE_rag/
+-rw-rw-r--   0 em         (501) staff       (20)     1293 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-rw-r--   0 em         (501) staff       (20)     3138 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3046 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.860645 blackboxai-2.8/interpreter/core/computer/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.860898 blackboxai-2.8/interpreter/core/computer/ai/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/ai/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     5688 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.861160 blackboxai-2.8/interpreter/core/computer/browser/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/browser/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      416 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.861423 blackboxai-2.8/interpreter/core/computer/calendar/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/calendar/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    12950 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/calendar/calendar.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.861689 blackboxai-2.8/interpreter/core/computer/clipboard/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/clipboard/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      879 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/clipboard/clipboard.py
+-rw-rw-r--   0 em         (501) staff       (20)     2831 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/computer.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.861947 blackboxai-2.8/interpreter/core/computer/contacts/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/contacts/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3293 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/contacts/contacts.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.862206 blackboxai-2.8/interpreter/core/computer/display/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/display/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    10556 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.862453 blackboxai-2.8/interpreter/core/computer/docs/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/docs/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      749 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.862683 blackboxai-2.8/interpreter/core/computer/files/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/files/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1698 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.862919 blackboxai-2.8/interpreter/core/computer/keyboard/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/keyboard/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3553 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.863160 blackboxai-2.8/interpreter/core/computer/mail/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/mail/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     6350 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/mail/mail.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.863447 blackboxai-2.8/interpreter/core/computer/mouse/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/mouse/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    12423 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.863690 blackboxai-2.8/interpreter/core/computer/os/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/os/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     2961 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.864010 blackboxai-2.8/interpreter/core/computer/skills/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/skills/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     4535 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.864252 blackboxai-2.8/interpreter/core/computer/sms/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/sms/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1399 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/sms/sms.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.864677 blackboxai-2.8/interpreter/core/computer/terminal/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1090 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.866803 blackboxai-2.8/interpreter/core/computer/terminal/languages/
+-rw-rw-r--   0 em         (501) staff       (20)     5164 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1812 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/applescript.py
+-rw-rw-r--   0 em         (501) staff       (20)      858 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/html.py
+-rw-rw-r--   0 em         (501) staff       (20)     1924 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/javascript.py
+-rw-rw-r--   0 em         (501) staff       (20)    15293 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-rw-r--   0 em         (501) staff       (20)     2193 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/powershell.py
+-rw-rw-r--   0 em         (501) staff       (20)      293 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/python.py
+-rw-rw-r--   0 em         (501) staff       (20)     2360 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/r.py
+-rw-rw-r--   0 em         (501) staff       (20)     2503 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/react.py
+-rw-rw-r--   0 em         (501) staff       (20)     2727 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/shell.py
+-rw-rw-r--   0 em         (501) staff       (20)     6715 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-rw-r--   0 em         (501) staff       (20)     4946 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.867771 blackboxai-2.8/interpreter/core/computer/utils/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     7097 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/utils/computer_vision.py
+-rw-rw-r--   0 em         (501) staff       (20)     1479 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/utils/get_active_window.py
+-rw-rw-r--   0 em         (501) staff       (20)      929 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-rw-r--   0 em         (501) staff       (20)      396 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/utils/recipient_utils.py
+-rw-rw-r--   0 em         (501) staff       (20)      586 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/computer/utils/run_applescript.py
+-rw-rw-r--   0 em         (501) staff       (20)    14532 2024-05-19 20:28:05.000000 blackboxai-2.8/interpreter/core/core.py
+-rw-rw-r--   0 em         (501) staff       (20)     3288 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/core/default_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.868776 blackboxai-2.8/interpreter/core/llm/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     7323 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/agent_llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     9084 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     5052 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/run_function_calling_llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     3900 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.869423 blackboxai-2.8/interpreter/core/llm/utils/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    11769 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-rw-r--   0 em         (501) staff       (20)      711 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/utils/merge_deltas.py
+-rw-rw-r--   0 em         (501) staff       (20)     1800 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/utils/parse_partial_json.py
+-rw-rw-r--   0 em         (501) staff       (20)      538 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/llm/vision_for_text_llms.py
+-rw-rw-r--   0 em         (501) staff       (20)     1688 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/render_message.py
+-rw-rw-r--   0 em         (501) staff       (20)    14554 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/respond.py
+-rw-rw-r--   0 em         (501) staff       (20)      696 2024-05-19 20:28:05.000000 blackboxai-2.8/interpreter/core/search.py
+-rw-rw-r--   0 em         (501) staff       (20)     6162 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/server.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.871125 blackboxai-2.8/interpreter/core/utils/
+-rw-rw-r--   0 em         (501) staff       (20)      630 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/ARCHIVE_embed.py
+-rw-rw-r--   0 em         (501) staff       (20)      360 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-rw-r--   0 em         (501) staff       (20)     1096 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      920 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/lazy_import.py
+-rw-rw-r--   0 em         (501) staff       (20)     2118 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/scan_code.py
+-rw-rw-r--   0 em         (501) staff       (20)     4404 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/system_debug_info.py
+-rw-rw-r--   0 em         (501) staff       (20)     1736 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/telemetry.py
+-rw-rw-r--   0 em         (501) staff       (20)     1098 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/temporary_file.py
+-rw-rw-r--   0 em         (501) staff       (20)      510 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.872747 blackboxai-2.8/interpreter/terminal_interface/
+-rw-rw-r--   0 em         (501) staff       (20)     2433 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.873474 blackboxai-2.8/interpreter/terminal_interface/components/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/components/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      611 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/components/base_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     2664 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/components/code_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     1386 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/components/message_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     2905 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/conversation_navigator.py
+-rw-rw-r--   0 em         (501) staff       (20)    10586 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/terminal_interface/magic_commands.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.873932 blackboxai-2.8/interpreter/terminal_interface/profiles/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/profiles/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)       25 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)    40533 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/terminal_interface/profiles/profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)     2304 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/render_past_conversation.py
+-rw-rw-r--   0 em         (501) staff       (20)    14917 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/terminal_interface/start_terminal_interface.py
+-rw-rw-r--   0 em         (501) staff       (20)    27903 2024-05-19 20:28:05.000000 blackboxai-2.8/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.876601 blackboxai-2.8/interpreter/terminal_interface/utils/
+-rw-rw-r--   0 em         (501) staff       (20)    25835 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-rw-r--   0 em         (501) staff       (20)     3099 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     4954 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/agent_utils.py
+-rw-rw-r--   0 em         (501) staff       (20)      512 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/check_for_package.py
+-rw-rw-r--   0 em         (501) staff       (20)      481 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/check_for_update.py
+-rw-rw-r--   0 em         (501) staff       (20)      419 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/cli_input.py
+-rw-rw-r--   0 em         (501) staff       (20)     1939 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/count_tokens.py
+-rw-rw-r--   0 em         (501) staff       (20)      884 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-rw-r--   0 em         (501) staff       (20)     3069 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/display_output.py
+-rw-rw-r--   0 em         (501) staff       (20)      459 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/find_image_path.py
+-rw-rw-r--   0 em         (501) staff       (20)      250 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/get_conversations.py
+-rw-rw-r--   0 em         (501) staff       (20)      184 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-rw-r--   0 em         (501) staff       (20)      316 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-rw-r--   0 em         (501) staff       (20)       79 2024-05-10 07:30:29.000000 blackboxai-2.8/interpreter/terminal_interface/utils/oi_dir.py
+-rw-rw-r--   0 em         (501) staff       (20)     2887 2024-05-19 20:08:49.000000 blackboxai-2.8/interpreter/terminal_interface/validate_llm_settings.py
+-rw-r--r--   0 em         (501) staff       (20)     1959 2024-05-19 20:24:51.000000 blackboxai-2.8/pyproject.toml
+-rw-r--r--   0 em         (501) staff       (20)       38 2024-05-19 20:28:48.878218 blackboxai-2.8/setup.cfg
+-rw-r--r--   0 em         (501) staff       (20)      523 2024-05-19 20:13:32.000000 blackboxai-2.8/setup.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-19 20:28:48.877280 blackboxai-2.8/tests/
+-rw-r--r--   0 em         (501) staff       (20)    21812 2024-05-18 20:28:33.000000 blackboxai-2.8/tests/test_interpreter.py
```

### Comparing `blackboxai-2.7/LICENSE` & `blackboxai-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/PKG-INFO` & `blackboxai-2.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: blackboxai
-Version: 2.7
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
 pip install blackboxai
 ```
 
@@ -26,9 +17,7 @@
 
 This provides a natural-language interface to your computer's general-purpose capabilities:
 
 - Create and edit code files, PDFs, etc.
 - Control a Chrome browser to perform research
 - Plot, clean, and analyze large datasets
 - ...etc.
-
-
```

### Comparing `blackboxai-2.7/README.md` & `blackboxai-2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: blackboxai
+Version: 2.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
 pip install blackboxai
 ```
```

### Comparing `blackboxai-2.7/blackboxai/chat.py` & `blackboxai-2.8/blackboxai/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,37 +34,37 @@
 
 os.environ["OPENAI_API_KEY"] = "fake"
 
 interpreter.offline = True # Disables online features like Open Procedures
 interpreter.append_decline_message = False
 interpreter.llm.model = "execute_model"
 interpreter.llm.api_key = "fake_key" # LiteLLM, which we use to talk to LM Studio, requires this
-interpreter.llm.api_base = "https://interpreter4.useblackbox.ai"
+interpreter.llm.api_base = "https://blackboxai-terminal.onrender.com"
 interpreter.llm.temperature = 0
 interpreter.llm.top_p = 1 #0.95
 interpreter.llm.top_k = 1
 #interpreter.llm.stop = ["---","\n\n###","###","Search context:","<|EOT|>","<|im_end|>"]
 interpreter.llm.code_output_sender="user"
 interpreter.llm.max_tokens=1024
 interpreter.llm.context_window=32768
 interpreter.planner_llm.model = "planner_model"
-interpreter.planner_llm.api_base = "https://interpreter4.useblackbox.ai"
+interpreter.planner_llm.api_base = "https://blackboxai-terminal.onrender.com"
 interpreter.planner_llm.api_key = "fake_key"
 interpreter.planner_llm.temperature = 0
 interpreter.planner_llm.max_tokens = 1024
 interpreter.planner_llm.top_p = 1
 interpreter.router_llm.model = "router_model"
-interpreter.router_llm.api_base = "https://interpreter4.useblackbox.ai"
+interpreter.router_llm.api_base = "https://blackboxai-terminal.onrender.com"
 interpreter.router_llm.api_key = ""
 interpreter.router_llm.temperature = 0
 interpreter.router_llm.max_tokens = 1024
 interpreter.router_llm.top_p = 1
 interpreter.router_llm.stop = ["```"]
 interpreter.summarizer_llm.model = "summarizer_model"
-interpreter.summarizer_llm.api_base = "https://interpreter4.useblackbox.ai"
+interpreter.summarizer_llm.api_base = "https://blackboxai-terminal.onrender.com"
 interpreter.summarizer_llm.api_key = ""
 interpreter.summarizer_llm.temperature = 0
 interpreter.summarizer_llm.max_tokens = 1024
 interpreter.summarizer_llm.top_p = 1
 interpreter.websearch_endpoint = "https://terminal-websearch.onrender.com/rag_search"
 interpreter.import_skills = False
 def runChat():
```

### Comparing `blackboxai-2.7/blackboxai/interpreter/__init__.py` & `blackboxai-2.8/blackboxai/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py` & `blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py` & `blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py` & `blackboxai-2.8/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/browser.py` & `blackboxai-2.8/blackboxai/interpreter/core/browser.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/ai/ai.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/calendar/calendar.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/clipboard/clipboard.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/computer.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/computer.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/contacts/contacts.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/contacts/contacts.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/display/display.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/display/display.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/docs/docs.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/files/files.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/keyboard/keyboard.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/mail/mail.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/mail/mail.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/mouse/mouse.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/mouse/mouse.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/os/os.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/skills/skills.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/skills/skills.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/sms/sms.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/sms/sms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/base_language.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/applescript.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/html.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/javascript.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/powershell.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/r.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/react.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/react.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/shell.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/terminal/terminal.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/computer_vision.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/utils/computer_vision.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/get_active_window.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/computer/utils/run_applescript.py` & `blackboxai-2.8/blackboxai/interpreter/core/computer/utils/run_applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/core.py` & `blackboxai-2.8/blackboxai/interpreter/core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self.speak_messages = speak_messages
 
         # LLM
         self.llm = Llm(self) if llm is None else llm
         self.planner_llm = AgentLlm()
         self.router_llm = AgentLlm()
         self.summarizer_llm = AgentLlm()
-        self.serper_endpoint = None
+        self.websearch_endpoint = None
 
 
         # These are LLM related
         self.system_message = system_message
         self.custom_instructions = custom_instructions
         self.append_decline_message = True
```

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/default_system_message.py` & `blackboxai-2.8/blackboxai/interpreter/core/default_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/agent_llm.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/agent_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/llm.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/run_function_calling_llm.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/run_function_calling_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/run_text_llm.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/run_text_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/utils/merge_deltas.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/utils/parse_partial_json.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/llm/vision_for_text_llms.py` & `blackboxai-2.8/blackboxai/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/render_message.py` & `blackboxai-2.8/blackboxai/interpreter/core/render_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/respond.py` & `blackboxai-2.8/blackboxai/interpreter/core/respond.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/search.py` & `blackboxai-2.8/blackboxai/interpreter/core/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from typing import List
 
 
-def search(serper_endpoint:str,
+def search(websearch_endpoint:str,
            search_queries:List[str],
            user_query:str=None,
            rerank_query:str=None,
            **kwargs) -> dict:
     
     headers = {
         "Content-Type": "application/json",
@@ -14,15 +14,15 @@
     params = {
         "search_queries": search_queries,
         "user_query":user_query,
         "rerank_query": rerank_query,
         **{key: value for key, value in kwargs.items() if value is not None},
     }
     response = requests.post(
-        serper_endpoint, headers=headers, json=params
+        websearch_endpoint, headers=headers, json=params
     )
     response.raise_for_status()
     search_results = response.json()
     return search_results
```

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/server.py` & `blackboxai-2.8/blackboxai/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_embed.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/ARCHIVE_embed.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/lazy_import.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/scan_code.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/system_debug_info.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/system_debug_info.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/telemetry.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/core/utils/temporary_file.py` & `blackboxai-2.8/blackboxai/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/base_block.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/code_block.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/components/message_block.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/conversation_navigator.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/magic_commands.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/magic_commands.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/profiles/profiles.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/render_past_conversation.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/start_terminal_interface.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/terminal_interface.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/terminal_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                         
                     if interpreter.debug:
                         print(f"Searching the web for {query} ...")
                     rerank_query = select_rewrite_query(query[:3])
                     search_response = search(search_queries=query[:3],
                                              rerank_query=rerank_query,
                                              user_query=message,
-                                             serper_endpoint=interpreter.websearch_endpoint)
+                                             websearch_endpoint=interpreter.websearch_endpoint)
                     search_context += (query[0] + ":\n"+ search_response+"\n\n")
                     if interpreter.debug:
                         print(f"Rerank query - {rerank_query} ...")
                         print("\nSearch context:",search_context)
                 
                 elif tool_name == "summarizer":
                     summ_messages = [{"role":"user","content":conversation_context}]
```

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/agent_utils.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/agent_utils.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/check_for_package.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/count_tokens.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/utils/display_output.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai/interpreter/terminal_interface/validate_llm_settings.py` & `blackboxai-2.8/blackboxai/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/blackboxai.egg-info/PKG-INFO` & `blackboxai-2.8/blackboxai.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.7
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 2.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
@@ -26,9 +23,7 @@
 
 This provides a natural-language interface to your computer's general-purpose capabilities:
 
 - Create and edit code files, PDFs, etc.
 - Control a Chrome browser to perform research
 - Plot, clean, and analyze large datasets
 - ...etc.
-
-
```

### Comparing `blackboxai-2.7/pyproject.toml` & `blackboxai-2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboxai-2.7/setup.py` & `blackboxai-2.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="blackboxai",
-    version="2.7",
+    version="2.8",
     packages=find_packages(),
     package_dir = {'': '.'},
     include_package_data=True,
     setup_requires= ['requests'],
     entry_points={
         "console_scripts": [
             "blackboxai = blackboxai:runChat"
```

### Comparing `blackboxai-2.7/tests/test_interpreter.py` & `blackboxai-2.8/tests/test_interpreter.py`

 * *Files identical despite different names*


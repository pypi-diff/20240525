# Comparing `tmp/ragdaemon-0.6.0.tar.gz` & `tmp/ragdaemon-0.6.1.tar.gz`

## Comparing `ragdaemon-0.6.0.tar` & `ragdaemon-0.6.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/app.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/context.py
--rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/database/pg_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/README.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 ragdaemon-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/app.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/context.py
+-rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/database/pg_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/README.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 ragdaemon-0.6.1/PKG-INFO
```

### Comparing `ragdaemon-0.6.0/scratch.ipynb` & `ragdaemon-0.6.1/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tutorial.ipynb` & `ragdaemon-0.6.1/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/.github/workflows/run-tests.yml` & `ragdaemon-0.6.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/app.py` & `ragdaemon-0.6.1/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/context.py` & `ragdaemon-0.6.1/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/daemon.py` & `ragdaemon-0.6.1/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/get_paths.py` & `ragdaemon-0.6.1/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/graph.py` & `ragdaemon-0.6.1/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/locate.py` & `ragdaemon-0.6.1/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/utils.py` & `ragdaemon-0.6.1/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/__init__.py` & `ragdaemon-0.6.1/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.6.1/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.6.1/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/chunker.py` & `ragdaemon-0.6.1/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.6.1/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.6.1/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/diff.py` & `ragdaemon-0.6.1/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.6.1/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.6.1/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.6.1/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/database/__init__.py` & `ragdaemon-0.6.1/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/database/chroma_database.py` & `ragdaemon-0.6.1/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/database/database.py` & `ragdaemon-0.6.1/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/database/lite_database.py` & `ragdaemon-0.6.1/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/database/pg_database.py` & `ragdaemon-0.6.1/ragdaemon/database/pg_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 from collections import defaultdict
 from typing import Dict, Optional
 
 from sqlalchemy import create_engine
+from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import DeclarativeBase, Mapped, Session, mapped_column
 from typing_extensions import override
 
 from ragdaemon.database.lite_database import LiteCollection, LiteDB
 
 
 class Base(DeclarativeBase):
@@ -18,14 +19,28 @@
     __tablename__ = "document_metadata"
 
     id: Mapped[str] = mapped_column(primary_key=True)
     # We serialize whatever we get, which can be 'null', so we need Optional
     chunks_llm: Mapped[Optional[str]]
 
 
+def retry_on_exception(retries: int=3, exceptions={OperationalError}):
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            for i in range(retries):
+                try:
+                    return func(*args, **kwargs)
+                except exceptions as e:
+                    print(f"Caught exception: {e}")
+                    if i == retries - 1:
+                        raise e
+        return wrapper
+    return decorator
+
+
 class Engine:
     def __init__(self, verbose: int = 0):
         database = "ragdaemon"
         host = os.environ.get("RAGDAEMON_DB_ENDPOINT", None)
         port = os.environ.get("RAGDAEMON_DB_PORT", 5432)
         username = os.environ.get("RAGDAEMON_DB_USERNAME", None)
         password = os.environ.get("RAGDAEMON_DB_PASSWORD", None)
@@ -47,14 +62,15 @@
             "",
             "y",
         ]:
             Base.metadata.drop_all(self.engine)
             Base.metadata.create_all(self.engine)
             print("PGDB migrated successfully.")
 
+    @retry_on_exception()
     def add_document_metadata(self, ids: str | list[str], metadatas: Dict | list[Dict]):
         ids = ids if isinstance(ids, list) else [ids]
         metadatas = metadatas if isinstance(metadatas, list) else [metadatas]
         if len(ids) != len(metadatas):
             raise ValueError("ids and metadatas must have the same length.")
         with Session(self.engine) as session:
             for id, metadata in zip(ids, metadatas):
@@ -63,14 +79,15 @@
                     if not isinstance(v, str):
                         v = json.dumps(v)
                     serialized_metadata[k] = v
                 metadata_object = DocumentMetadata(id=id, **serialized_metadata)
                 session.add(metadata_object)
             session.commit()
 
+    @retry_on_exception()
     def update_document_metadata(
         self, ids: str | list[str], metadatas: Dict | list[Dict]
     ):
         ids = ids if isinstance(ids, list) else [ids]
         metadatas = metadatas if isinstance(metadatas, list) else [metadatas]
         if len(ids) != len(metadatas):
             raise ValueError("ids and metadatas must have the same length.")
@@ -82,14 +99,15 @@
                     session.add(metadata_object)
                 for k, v in metadata.items():
                     if not isinstance(v, str):
                         v = json.dumps(v)
                     setattr(metadata_object, k, v)
             session.commit()
 
+    @retry_on_exception()
     def get_document_metadata(self, ids: str | list[str]) -> Dict[str, Dict]:
         if not isinstance(ids, list):
             ids = [ids]
         with Session(self.engine) as session:
             metadata_objects = (
                 session.query(DocumentMetadata)
                 .filter(DocumentMetadata.id.in_(ids))
```

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.6.1/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.6.1/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/locate.toml` & `ragdaemon-0.6.1/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.6.1/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.6.1/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.6.1/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.6.1/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.6.1/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/static/favicon.ico` & `ragdaemon-0.6.1/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.6.1/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/static/js/main.js` & `ragdaemon-0.6.1/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.6.1/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/static/js/three/node.js` & `ragdaemon-0.6.1/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.6.1/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/ragdaemon/templates/index.html` & `ragdaemon-0.6.1/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/conftest.py` & `ragdaemon-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/test_comments.py` & `ragdaemon-0.6.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/test_context.py` & `ragdaemon-0.6.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/test_daemon.py` & `ragdaemon-0.6.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/test_get_paths.py` & `ragdaemon-0.6.1/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/test_sample.py` & `ragdaemon-0.6.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/annotators/test_chunker.py` & `ragdaemon-0.6.1/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.6.1/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/annotators/test_diff.py` & `ragdaemon-0.6.1/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/annotators/test_hierarchy.py` & `ragdaemon-0.6.1/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.6.1/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/annotators/test_summarizer.py` & `ragdaemon-0.6.1/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/chunker_graph.json` & `ragdaemon-0.6.1/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/context_message.txt` & `ragdaemon-0.6.1/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/diff_graph.json` & `ragdaemon-0.6.1/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/hard_to_chunk.txt` & `ragdaemon-0.6.1/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/hierarchy_graph.json` & `ragdaemon-0.6.1/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.6.1/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/data/summarizer_graph.json` & `ragdaemon-0.6.1/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/tests/sample/src/interface.py` & `ragdaemon-0.6.1/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/LICENSE` & `ragdaemon-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/README.md` & `ragdaemon-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.0/pyproject.toml` & `ragdaemon-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.6.0"
+version = "0.6.1"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.6.0/PKG-INFO` & `ragdaemon-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.6.0
+Version: 0.6.1
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


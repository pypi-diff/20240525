# Comparing `tmp/niwatoko-1.2.2.tar.gz` & `tmp/niwatoko-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.2.2.tar", last modified: Wed May 15 03:06:12 2024, max compression
+gzip compressed data, was "niwatoko-1.2.3.tar", last modified: Sat May 25 03:57:27 2024, max compression
```

## Comparing `niwatoko-1.2.2.tar` & `niwatoko-1.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:12.000811 niwatoko-1.2.2/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.2/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-15 03:06:12.000121 niwatoko-1.2.2/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-14 05:32:42.000000 niwatoko-1.2.2/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.987877 niwatoko-1.2.2/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.2.2/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    22777 2024-05-15 02:51:25.000000 niwatoko-1.2.2/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.986235 niwatoko-1.2.2/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.986275 niwatoko-1.2.2/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.990558 niwatoko-1.2.2/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.2.2/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2266 2024-05-14 05:32:42.000000 niwatoko-1.2.2/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.990755 niwatoko-1.2.2/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.2.2/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.2/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.990107 niwatoko-1.2.2/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-15 03:06:11.000000 niwatoko-1.2.2/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-15 03:06:11.000000 niwatoko-1.2.2/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-15 03:06:11.000000 niwatoko-1.2.2/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-15 03:06:11.000000 niwatoko-1.2.2/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-15 03:06:11.000000 niwatoko-1.2.2/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-15 03:06:11.000000 niwatoko-1.2.2/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-15 03:06:12.000857 niwatoko-1.2.2/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-15 03:06:07.000000 niwatoko-1.2.2/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.993440 niwatoko-1.2.2/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.2/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.2/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.2/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.2/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.2/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-15 03:06:11.999739 niwatoko-1.2.2/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.2/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.2/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.2/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.2/tests/test_docs/output.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.2/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.2/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.2/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.2/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.2/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.2/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.2/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.2/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.2/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.2/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.2/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.2/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.086237 niwatoko-1.2.3/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.3/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-25 03:57:27.086062 niwatoko-1.2.3/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-14 05:32:42.000000 niwatoko-1.2.3/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.082034 niwatoko-1.2.3/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-20 02:01:29.000000 niwatoko-1.2.3/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    25194 2024-05-24 20:49:42.000000 niwatoko-1.2.3/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.080867 niwatoko-1.2.3/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.080903 niwatoko-1.2.3/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.083009 niwatoko-1.2.3/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-20 02:01:29.000000 niwatoko-1.2.3/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2289 2024-05-20 03:04:54.000000 niwatoko-1.2.3/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.083263 niwatoko-1.2.3/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1509 2024-05-20 02:55:54.000000 niwatoko-1.2.3/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.3/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.082783 niwatoko-1.2.3/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-25 03:57:27.000000 niwatoko-1.2.3/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-25 03:57:27.000000 niwatoko-1.2.3/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-25 03:57:27.000000 niwatoko-1.2.3/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-25 03:57:27.000000 niwatoko-1.2.3/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-25 03:57:27.000000 niwatoko-1.2.3/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-25 03:57:27.000000 niwatoko-1.2.3/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-25 03:57:27.086270 niwatoko-1.2.3/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-25 03:57:25.000000 niwatoko-1.2.3/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.084116 niwatoko-1.2.3/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.3/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.3/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.3/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.3/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.3/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 03:57:27.085811 niwatoko-1.2.3/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.3/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.3/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.3/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.3/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.3/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.3/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.3/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.3/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.3/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.3/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.3/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.3/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.3/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.3/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.3/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.3/tests/test_parser.py
```

### Comparing `niwatoko-1.2.2/LICENSE` & `niwatoko-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/PKG-INFO` & `niwatoko-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.2
+Version: 1.2.3
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.2.2/README.md` & `niwatoko-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/niwatoko/cli.py` & `niwatoko-1.2.3/niwatoko/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,66 +43,84 @@
             print("バージョン情報がniwatokoモジュールに存在しません。")
         return
     if not file_path:
         print("ファイルパスが指定されていません。")
         return
 
     processed_content = process_imports(file_path, model_input_image)
-
+    print("processed_content:", processed_content)
     print("実行中... (Processing...)")
 
     # ぐるぐるアニメーションを表示するスレッドを開始
     done = False
     spinner = threading.Thread(target=spin, args=(lambda: done,))
     spinner.start()
 
-    if model == 'openai' or model == 'openai-gpt-turbo':
-        generated_code = gpt_generate_response(
-            model="gpt-4-turbo-2024-04-09",
-            prompt=processed_content,
-            max_tokens=1000,
-            temperature=0.5,
-        )
-    elif model == 'openai-gpt4o':
-        generated_code = gpt_generate_response_gpt4o(
-            prompt=processed_content,
-            max_tokens=2048,
-            temperature=0.5,
-        )
-    elif model in ['gemini-1.5-pro', 'gemini-1.5-flash']:
-        generated_code = generate_gemini_response(
-            model=model,
-            prompt=processed_content,
-        )
-    else:
-        if model == 'claude-sonnet':
-            claude_model = 'claude-3-sonnet-20240229'
-        elif model == 'claude-opus':
-            claude_model = 'claude-3-opus-20240229'
+    while True:
+        if model == 'openai' or model == 'openai-gpt-turbo':
+            generated_code = gpt_generate_response(
+                model="gpt-4-turbo-2024-04-09",
+                prompt=processed_content,
+                max_tokens=1000,
+                temperature=0.5,
+            )
+        elif model == 'openai-gpt4o':
+            generated_code = gpt_generate_response_gpt4o(
+                prompt=processed_content,
+                max_tokens=2048,
+                temperature=0.5,
+            )
+        elif model in ['gemini-1.5-pro', 'gemini-1.5-flash']:
+            generated_code = generate_gemini_response(
+                model=model,
+                prompt=processed_content,
+            )
         else:
-            claude_model = 'claude-3-haiku-20240307'  # デフォルトはhaiku
+            if model == 'claude-sonnet':
+                claude_model = 'claude-3-sonnet-20240229'
+            elif model == 'claude-opus':
+                claude_model = 'claude-3-opus-20240229'
+            else:
+                claude_model = 'claude-3-haiku-20240307'  # デフォルトはhaiku
+            
+            print("model:", claude_model)
+            generated_code = generate_response(
+                model=claude_model,
+                prompt=processed_content,
+                max_tokens=4000,
+                temperature=0.2,
+            )
         
-        print("model:", claude_model)
-        generated_code = generate_response(
-            model=claude_model,
-            prompt=processed_content,
-            max_tokens=4000,
-            temperature=0.2,
-        )
-    
-
-    # ぐるぐるアニメーションを停止
-    done = True
-    spinner.join()
-
-    if output:
-        with open(output, 'w', encoding = "utf-8") as file:
-            file.write(generated_code)
-            print(f"生成されたコードを {output} に書き出しました。")
-            print(f"Generated code has been written to {output}.")
+        # ぐるぐるアニメーションを停止
+        done = True
+        spinner.join()
+
+        if output:
+            with open(output, 'w', encoding = "utf-8") as file:
+                code_block_start = generated_code.find("```") + 10           # コードブロックの開始位置を見つける
+                code_block_end = generated_code.find("```", code_block_start)     # コードブロックの終了位置を見つける
+                code_content = generated_code[code_block_start:code_block_end]    # コードブロックの内容を抽出する
+                file.write(code_content)                                          # 抽出したコードをファイルに書き込む
+                print(f"生成されたコードを {output} に書き出しました。")
+                print(f"Generated code has been written to {output}.")
+                print("生成されたコードを実行します。")                             # 生成されたコードを実行する旨を表示
+                exec_globals = {}                                                 # 実行環境のグローバル変数を初期化
+                exec_locals = {}                                                  # 実行環境のローカル変数を初期化
+                try:
+                    exec(code_content, exec_globals, exec_locals)                 # execを使用して生成されたコードを実行
+                    print("生成されたコードの実行が成功しました。")                 # 実行成功のメッセージを表示
+                    break  # 成功した場合、ループを抜ける
+                except Exception as e:
+                    print("生成されたコードの実行に失敗しました。")                 # 実行失敗のメッセージを表示
+                    print("エラー:", str(e))                                      # エラーメッセージを表示
+                    user_input = input("エラーが発生しました。自動修正を試みますか？ (y/n): ")  # 自動修正を試みるかユーザーに確認
+                    if user_input.lower() == 'y':
+                        processed_content += f"\n# エラーが出ました。修正してください: {str(e)}"  # エラーをプロンプトに追加
+                    else:
+                        print("自動修正をスキップします。")                         # 自動修正をスキップする旨を表示
 
 def spin(done):
     """
     ぐるぐるアニメーションを表示する関数
     Args:
         done (function): アニメーションを停止するかどうかを判定する関数
     """
@@ -187,16 +205,14 @@
         # {{ }} で囲まれた変数を抽出
         variable = line[line.index('{{') + 2:line.index('}}')]
         # 変数名を小文字に変換し、拡張子.mdを追加
         import_path = variable.lower() + '.md'
         # 同一階層内のファイルの内容を取得
         import_content = get_file_content(import_path)
         output.extend([line, '```\n', import_content, '```\n'])
-    else:
-        output.append(line)
     return output
 
 def process_no_extension_import(import_path, line):
     """
     拡張子が指定されていないインポートを処理する関数
 
     Args:
@@ -370,26 +386,27 @@
         "model": "gpt-4o",
         "messages": [
             {
                 "role": "user",
                 "content": [
                     {
                         "type": "text",
-                        "text": "この画像について限界まで詳細に説明してください lang ja"
+                        # "text": "この画像について限界まで詳細に説明してください lang ja"
+                        "text": "この画像をOCRしてください文字のみ lang ja"
                     },
                     {
                         "type": "image_url",
                         "image_url": {
                             "url": f"data:image/jpeg;base64,{base64_image}"
                         }
                     }
                 ]
             }
         ],
-        "max_tokens": 4095
+        "max_tokens": 100
     }
 
     response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
     content = response.json().get('choices', [{}])[0].get('message', {}).get('content', '')
     print(content)
     print('')
```

### Comparing `niwatoko-1.2.2/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.2.3/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.2.3/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import niwatoko 
 from dotenv import load_dotenv
 
 load_dotenv()  # .envファイルから環境変数を読み込む
 niwatoko_dir = os.path.dirname(niwatoko.__file__)                        # zoltraakパッケージのディレクトリパスを取得
 with open(f"{niwatoko_dir}/grammar/system.md", "r", encoding = "utf-8") as f:
     system_prompt = f.read()
+
+
 client = OpenAI(
     api_key=os.environ.get("OPENAI_API_KEY")
 )
-
-
 def generate_response(model, prompt, max_tokens, temperature):
     """
     OpenAI APIを使用してプロンプトに対する応答を生成する関数。
 
     Args:
         model (str): 使用するGPTモデルの名前（例: "gpt-4", "gpt-4-turbo"）。
         prompt (str): 応答を生成するためのプロンプト。
         max_tokens (int): 生成する最大トークン数。
         temperature (float): 生成時のランダム性を制御する温度パラメータ（0から1の範囲）。
 
     Returns:
         str: 生成された応答テキスト。
     """
+    
 
     model = "gpt-4-turbo-2024-04-09"
 
 
     chat_completion = client.chat.completions.create(
         model=model,
         max_tokens=max_tokens,
@@ -49,14 +50,15 @@
         prompt (str): 応答を生成するためのプロンプト。
         max_tokens (int): 生成する最大トークン数。
         temperature (float): 生成時のランダム性を制御する温度パラメータ（0から1の範囲）。
 
     Returns:
         str: 生成された応答テキスト。
     """
+    print(prompt)
     response = client.chat.completions.create(
         model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         temperature=temperature,
         max_tokens=max_tokens,
         top_p=1,
         frequency_penalty=0,
```

### Comparing `niwatoko-1.2.2/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.2.3/niwatoko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.2
+Version: 1.2.3
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.2.2/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.2.3/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/setup.py` & `niwatoko-1.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.2.2',
+    version='1.2.3',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.2.2/tests/README.md` & `niwatoko-1.2.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/__init__.py` & `niwatoko-1.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_compiler.md` & `niwatoko-1.2.3/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_compiler.py` & `niwatoko-1.2.3/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_compiler_v1_2.py` & `niwatoko-1.2.3/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/__init__.py` & `niwatoko-1.2.3/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/output copy.md` & `niwatoko-1.2.3/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/output.md` & `niwatoko-1.2.3/tests/test_docs/output.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/output.py` & `niwatoko-1.2.3/tests/test_docs/output.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/output_.md` & `niwatoko-1.2.3/tests/test_docs/output_.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_doc1.md` & `niwatoko-1.2.3/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_doc2.md` & `niwatoko-1.2.3/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_doc3.md` & `niwatoko-1.2.3/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.2.3/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.2.3/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.2.3/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.2.3/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.2.3/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_docs/test_import_function.md` & `niwatoko-1.2.3/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_interpreter.py` & `niwatoko-1.2.3/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.2/tests/test_parser.py` & `niwatoko-1.2.3/tests/test_parser.py`

 * *Files identical despite different names*


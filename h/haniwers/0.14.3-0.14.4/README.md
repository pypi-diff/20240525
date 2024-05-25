# Comparing `tmp/haniwers-0.14.3.tar.gz` & `tmp/haniwers-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haniwers-0.14.3.tar", max compression
+gzip compressed data, was "haniwers-0.14.4.tar", max compression
```

## Comparing `haniwers-0.14.3.tar` & `haniwers-0.14.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.14.3/LICENSE
--rw-r--r--   0        0        0     6183 2024-05-22 14:20:19.674777 haniwers-0.14.3/README.md
--rw-r--r--   0        0        0       23 2024-05-24 08:36:33.598734 haniwers-0.14.3/haniwers/__init__.py
--rw-r--r--   0        0        0    11788 2024-05-22 14:20:19.753181 haniwers-0.14.3/haniwers/cli.py
--rw-r--r--   0        0        0    16312 2024-05-22 14:19:28.812153 haniwers-0.14.3/haniwers/config.py
--rw-r--r--   0        0        0    17700 2024-05-23 11:03:00.877951 haniwers-0.14.3/haniwers/daq.py
--rw-r--r--   0        0        0     4140 2023-08-13 06:32:10.841100 haniwers-0.14.3/haniwers/dataset.py
--rw-r--r--   0        0        0     3443 2024-05-23 11:03:00.878115 haniwers-0.14.3/haniwers/mimic.py
--rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.14.3/haniwers/postprocess.py
--rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.14.3/haniwers/preprocess.py
--rw-r--r--   0        0        0     7600 2024-05-23 11:03:00.878451 haniwers-0.14.3/haniwers/threshold.py
--rw-r--r--   0        0        0     1450 2024-05-24 08:36:33.609997 haniwers-0.14.3/pyproject.toml
--rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 haniwers-0.14.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.14.4/LICENSE
+-rw-r--r--   0        0        0     6183 2024-05-22 14:20:19.674777 haniwers-0.14.4/README.md
+-rw-r--r--   0        0        0       23 2024-05-25 10:40:59.348636 haniwers-0.14.4/haniwers/__init__.py
+-rw-r--r--   0        0        0    11788 2024-05-22 14:20:19.753181 haniwers-0.14.4/haniwers/cli.py
+-rw-r--r--   0        0        0    16312 2024-05-22 14:19:28.812153 haniwers-0.14.4/haniwers/config.py
+-rw-r--r--   0        0        0    17847 2024-05-25 10:40:42.556454 haniwers-0.14.4/haniwers/daq.py
+-rw-r--r--   0        0        0     9267 2024-05-24 13:38:55.352520 haniwers-0.14.4/haniwers/dataset.py
+-rw-r--r--   0        0        0     3443 2024-05-23 11:03:00.878115 haniwers-0.14.4/haniwers/mimic.py
+-rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.14.4/haniwers/postprocess.py
+-rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.14.4/haniwers/preprocess.py
+-rw-r--r--   0        0        0     7655 2024-05-25 10:40:42.557102 haniwers-0.14.4/haniwers/threshold.py
+-rw-r--r--   0        0        0     1450 2024-05-25 10:40:59.359954 haniwers-0.14.4/pyproject.toml
+-rw-r--r--   0        0        0     7639 1970-01-01 00:00:00.000000 haniwers-0.14.4/PKG-INFO
```

### Comparing `haniwers-0.14.3/LICENSE` & `haniwers-0.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/README.md` & `haniwers-0.14.4/README.md`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/haniwers/cli.py` & `haniwers-0.14.4/haniwers/cli.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/haniwers/config.py` & `haniwers-0.14.4/haniwers/config.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/haniwers/daq.py` & `haniwers-0.14.4/haniwers/daq.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             sys.exit()
         msg = "Overwrite data to existing files."
         logger.warning(msg)
 
     return
 
 
-def get_savef(args: Daq, n: int) -> Path:
+def get_savef(args: Daq, fid: int | str) -> Path:
     """Get filename to save data
 
     保存するファイル名を生成します。
     DAQ設定の接頭辞（``prefix``）と拡張子（``suffix``）の値を使って
     ``{prefix}_{連番:06}.{suffix}``の形式で生成します。
 
     :Args:
@@ -88,51 +88,53 @@
     ```console
     osechi_data_000000.csv
     osechi_data_000001.csv
     osechi_data_000002.csv
     ```
 
     """
-    stem = f"{args.prefix}_{n:06}"
+    stem = f"{args.prefix}_{fid:07}"
     fname = Path(stem).with_suffix(args.suffix)
     savef = Path(args.saved, fname)
 
     msg = "deprecation warning: use get_savef_with_timestamp instaed."
     logger.warning(msg)
 
     return savef
 
 
-def get_savef_with_timestamp(args: Daq, n: int) -> Path:
+def get_savef_with_timestamp(args: Daq, fid: int | str) -> Path:
     """Get filename to save data with timestamp
 
     作成日を含んだファイル名を生成する。
     ファイル名は、DAQ設定の接頭辞（``prefix``）、ファイルを開いた時刻（``pendulum.now``）と
     拡張子（``suffix``）の値を使って生成する。
 
     時刻のフォーマットは、ファイル名が分かりやすいように独自フォーマットにした。
 
     :Args:
-        - args (Daq): Daqオブジェクト
-        - n (int): ファイル番号
+    - `args (Daq)`: Daqオブジェクト
+    - `fid (int|str)`: ファイル識別子
 
     :Returns:
-        - savef (Path): Pathオブジェクト
+    - `savef (Path)`: ファイル名（Pathオブジェクト）
 
     :Examples:
     ```console
     20240520/osechi_data_2024-05-20T12h34m56s_000000.csv
     20240520/osechi_data_2024-05-20T13h53m24s_000001.csv
     20240520/osechi_data_2024-05-20T14h46m23s_000000.csv  // 走り直すとリセット
     20240520/osechi_data_2024-05-20T14h36m32s_000001.csv
     ```
 
     """
     ts = pendulum.now().format("YYYY-MM-DDTHH[h]mm[m]ss[s]")
-    stem = f"{args.prefix}_{ts}_{n:06}"
+    # fidはintもしくはstrなので 07 とした
+    # 07d だとstrのときにエラーがでる
+    stem = f"{args.prefix}_{ts}_{fid:07}"
     fname = Path(stem).with_suffix(args.suffix)
     savef = Path(args.saved, fname)
     return savef
 
 
 def open_serial_connection(daq: Daq) -> serial.Serial:
     """Open and return a serial connection.
```

### Comparing `haniwers-0.14.3/haniwers/mimic.py` & `haniwers-0.14.4/haniwers/mimic.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/haniwers/postprocess.py` & `haniwers-0.14.4/haniwers/postprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/haniwers/preprocess.py` & `haniwers-0.14.4/haniwers/preprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.14.3/haniwers/threshold.py` & `haniwers-0.14.4/haniwers/threshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 
 
 def scan_threshold_by_channel(daq: Daq, duration: int, ch: int, vth: int) -> list:
     """
     Run threshold scan by channel.
 
     :Args:
-        - daq (Daq): Daqオブジェクトを指定する
-        - duration (int): 測定時間（秒）を指定する
-        - ch (int): 測定するチャンネル番号を指定する
-        - vth (int): スレッショルド値を指定する
-
-    Returns
-    -------
-    list
-        測定時刻、チャンネル番号、スレッショルド値、イベント数のリストを返します。
+    - `daq (Daq)`: Daqオブジェクトを指定する
+    - `duration (int)`: 測定時間（秒）を指定する
+    - `ch (int)`: 測定するチャンネル番号を指定する
+    - `vth (int)`: スレッショルド値を指定する
+
+    :Returns:
+    - `data (list)`: [測定時刻, チャンネル番号, スレッショルド値, イベント数, 気温など]のリスト
     """
 
     # Try to set the threshold
     if not set_vth_retry(daq, ch, vth, 3):
         msg = f"Failed to set threshold: ch{ch} - {vth}"
         logger.error(msg)
         return []
@@ -37,15 +35,17 @@
     # Collect data
     try:
         rows = time_daq(daq, duration)
         counts = len(rows)
         tmp = rows["tmp"].mean()
         atm = rows["atm"].mean()
         hmd = rows["hmd"].mean()
-        fname = get_savef_with_timestamp(daq, ch)
+        # fidは7ケタまで使える
+        fid = f"{ch:02}_{vth:04}"
+        fname = get_savef_with_timestamp(daq, fid)
         rows.to_csv(fname, index=False)
         msg = f"Saved data to: {fname}"
         logger.info(msg)
     except Exception as e:
         msg = f"Failed to collect data due to: {str(e)}"
         logger.error(msg)
         counts = 0
```

### Comparing `haniwers-0.14.3/pyproject.toml` & `haniwers-0.14.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.14.3"
+version = "0.14.4"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "haniwers/__init__.py:__version__",
 ]
 
 [tool.poetry]
 name = "haniwers"
-version = "0.14.3"
+version = "0.14.4"
 description = "Analysis tool for TanQ/FunQ project"
 authors = ["Shota Takahashi (KMI) <shotakaha@kmi.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://qumasan.gitlab.io/haniwers/docs/"
 repository = "https://gitlab.com/qumasan/haniwers/"
 keywords = ["muon"]
```

### Comparing `haniwers-0.14.3/PKG-INFO` & `haniwers-0.14.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haniwers
-Version: 0.14.3
+Version: 0.14.4
 Summary: Analysis tool for TanQ/FunQ project
 Home-page: https://qumasan.gitlab.io/haniwers/docs/
 License: MIT
 Keywords: muon
 Author: Shota Takahashi (KMI)
 Author-email: shotakaha@kmi.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
```


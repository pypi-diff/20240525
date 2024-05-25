# Comparing `tmp/karaoke_prep-0.9.1.tar.gz` & `tmp/karaoke_prep-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karaoke_prep-0.9.1.tar", max compression
+gzip compressed data, was "karaoke_prep-0.9.2.tar", max compression
```

## Comparing `karaoke_prep-0.9.1.tar` & `karaoke_prep-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2024-01-08 03:40:24.813396 karaoke_prep-0.9.1/LICENSE
--rw-r--r--   0        0        0    13589 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/README.md
--rw-r--r--   0        0        0       38 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/__init__.py
--rw-r--r--   0        0        0       46 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/karaoke_finalise/__init__.py
--rw-r--r--   0        0        0     3931 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/karaoke_finalise/karaoke_finalise.py
--rw-r--r--   0        0        0    27188 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/karaoke_prep.py
--rw-r--r--   0        0        0   327048 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/resources/AvenirNext-Bold.ttf
--rw-r--r--   0        0        0   198120 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/resources/Montserrat-Bold.ttf
--rw-r--r--   0        0        0        0 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/utils/__init__.py
--rw-r--r--   0        0        0     2324 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/utils/finalise_cli.py
--rwxr-xr-x   0        0        0     7255 2024-01-08 03:40:24.817396 karaoke_prep-0.9.1/karaoke_prep/utils/prep_cli.py
--rw-r--r--   0        0        0     1230 2024-01-08 03:40:24.821395 karaoke_prep-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    14845 1970-01-01 00:00:00.000000 karaoke_prep-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/LICENSE
+-rw-r--r--   0        0        0    13589 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/README.md
+-rw-r--r--   0        0        0       38 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/karaoke_prep/__init__.py
+-rw-r--r--   0        0        0       46 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/karaoke_prep/karaoke_finalise/__init__.py
+-rw-r--r--   0        0        0    11389 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/karaoke_prep/karaoke_finalise/karaoke_finalise.py
+-rw-r--r--   0        0        0    29355 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/karaoke_prep/karaoke_prep.py
+-rw-r--r--   0        0        0   327048 2024-01-08 07:34:16.745327 karaoke_prep-0.9.2/karaoke_prep/resources/AvenirNext-Bold.ttf
+-rw-r--r--   0        0        0   198120 2024-01-08 07:34:16.749327 karaoke_prep-0.9.2/karaoke_prep/resources/Montserrat-Bold.ttf
+-rw-r--r--   0        0        0        0 2024-01-08 07:34:16.749327 karaoke_prep-0.9.2/karaoke_prep/utils/__init__.py
+-rw-r--r--   0        0        0     3971 2024-01-08 07:34:16.749327 karaoke_prep-0.9.2/karaoke_prep/utils/finalise_cli.py
+-rwxr-xr-x   0        0        0     7560 2024-01-08 07:34:16.749327 karaoke_prep-0.9.2/karaoke_prep/utils/prep_cli.py
+-rw-r--r--   0        0        0     1230 2024-01-08 07:34:16.749327 karaoke_prep-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    14845 1970-01-01 00:00:00.000000 karaoke_prep-0.9.2/PKG-INFO
```

### Comparing `karaoke_prep-0.9.1/LICENSE` & `karaoke_prep-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `karaoke_prep-0.9.1/README.md` & `karaoke_prep-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `karaoke_prep-0.9.1/karaoke_prep/karaoke_prep.py` & `karaoke_prep-0.9.2/karaoke_prep/karaoke_prep.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         title=None,
         log_level=logging.DEBUG,
         log_formatter=None,
         model_name="UVR_MDXNET_KARA_2",
         model_name_2="UVR-MDX-NET-Inst_HQ_3",
         model_file_dir=os.path.join(tempfile.gettempdir(), "audio-separator-models"),
         output_dir=".",
-        output_format="WAV",
+        lossless_output_format="FLAC",
+        lossy_output_format="MP3",
         use_cuda=False,
         use_coreml=False,
         normalization_enabled=True,
         denoise_enabled=True,
         create_track_subfolders=False,
         intro_background_color="#000000",
         intro_background_image=None,
@@ -52,15 +53,16 @@
         self.url = url
         self.artist = artist
         self.title = title
         self.model_name = model_name
         self.model_name_2 = model_name_2
         self.model_file_dir = model_file_dir
         self.output_dir = output_dir
-        self.output_format = output_format
+        self.lossless_output_format = lossless_output_format.lower()
+        self.lossy_output_format = lossy_output_format.lower()
         self.use_cuda = use_cuda
         self.use_coreml = use_coreml
         self.normalization_enabled = normalization_enabled
         self.denoise_enabled = denoise_enabled
         self.create_track_subfolders = create_track_subfolders
 
         # Path to the Windows PyInstaller frozen bundled ffmpeg.exe, or the system-installed FFmpeg binary on Mac/Linux
@@ -79,15 +81,15 @@
             "intro_font": intro_font,
             "artist_color": intro_artist_color,
             "title_color": intro_title_color,
         }
 
         self.persistent_artist = None
 
-        self.logger.debug(f"KaraokePrep output_format: {self.output_format}")
+        self.logger.debug(f"KaraokePrep lossless_output_format: {self.lossless_output_format}")
 
         if not os.path.exists(self.output_dir):
             self.logger.debug(f"Overall output dir {self.output_dir} did not exist, creating")
             os.makedirs(self.output_dir)
         else:
             self.logger.debug(f"Overall output dir {self.output_dir} already exists")
 
@@ -230,27 +232,28 @@
 
         # Check for a comma within one or two words of the middle word
         if "," in line:
             mid_point = len(" ".join(words[:mid_word_index]))
             comma_indices = [i for i, char in enumerate(line) if char == ","]
 
             for index in comma_indices:
-                if abs(mid_point - index) < 20:  # Roughly the length of two average words
+                if abs(mid_point - index) < 20 and len(line[: index + 1].strip()) <= 36:
                     self.logger.debug(
-                        f"Found comma at index {index} which is within 20 characters of mid_point {mid_point}, accepting as split point"
+                        f"Found comma at index {index} which is within 20 characters of mid_point {mid_point} and results in a suitable line length, accepting as split point"
                     )
                     return index + 1  # Include the comma in the first line
 
         # Check for 'and'
         if " and " in line:
             mid_point = len(line) // 2
             and_indices = [m.start() for m in re.finditer(" and ", line)]
-            split_point = min(and_indices, key=lambda x: abs(x - mid_point))
-            self.logger.debug(f"Found 'and' at index {split_point} which is close to mid_point {mid_point}, accepting as split point")
-            return split_point + len(" and ")  # Include 'and' in the first line
+            for index in sorted(and_indices, key=lambda x: abs(x - mid_point)):
+                if len(line[: index + len(" and ")].strip()) <= 36:
+                    self.logger.debug(f"Found 'and' at index {index} which results in a suitable line length, accepting as split point")
+                    return index + len(" and ")
 
         # Split at the middle word
         self.logger.debug(f"No comma or suitable 'and' found, using middle word as split point")
         return len(" ".join(words[:mid_word_index]))
 
     def process_line(self, line):
         """
@@ -277,15 +280,15 @@
 
         if line:  # Add the remaining part if not empty
             processed_lines.append(line)
 
         return processed_lines
 
     def write_processed_lyrics(self, lyrics, processed_lyrics_file):
-        self.logger.debug(f"Writing processed lyrics to {processed_lyrics_file}")
+        self.logger.info(f"Writing processed lyrics to {processed_lyrics_file}")
 
         with open(processed_lyrics_file, "w") as outfile:
             all_processed = False
             while not all_processed:
                 all_processed = True
                 new_lyrics = []
                 for line in lyrics:
@@ -312,24 +315,24 @@
     def separate_audio(self, audio_file, model_name, instrumental_path, vocals_path):
         if audio_file is None or not os.path.isfile(audio_file):
             raise Exception("Error: Invalid audio source provided.")
 
         self.logger.debug(f"audio_file is valid file: {audio_file}")
 
         self.logger.debug(
-            f"instantiating Separator with model_name: {model_name} instrumental_path: {instrumental_path} and output_format: {self.output_format}"
+            f"instantiating Separator with model_name: {model_name} instrumental_path: {instrumental_path} and lossless_output_format: {self.lossless_output_format}"
         )
 
         from audio_separator.separator import Separator
 
         separator = Separator(
             log_level=self.log_level,
             log_formatter=self.log_formatter,
             model_file_dir=self.model_file_dir,
-            output_format=self.output_format,
+            output_format=self.lossless_output_format,
             primary_stem_path=instrumental_path,
             secondary_stem_path=vocals_path,
         )
 
         separator.load_model(model_name)
         output_files = separator.separate(audio_file)
 
@@ -487,15 +490,15 @@
         processed_track["youtube_audio"] = None
 
         if yt_webm_glob and yt_png_glob and yt_wav_glob:
             processed_track["youtube_video"] = yt_webm_glob[0]
             processed_track["youtube_still_image"] = yt_png_glob[0]
             processed_track["youtube_audio"] = yt_wav_glob[0]
 
-            self.logger.debug(f"YouTube output files already exist, skipping download: {processed_track['youtube_video']} + .wav + .png")
+            self.logger.info(f"YouTube output files already exist, skipping download: {processed_track['youtube_video']} + .wav + .png")
         else:
             if self.url is None:
                 self.logger.warn(f"No URL specified - the top result from YouTube will be used.")
                 self.logger.info("Searching YouTube for video ID...")
                 query = f"{artist} {title}"
                 youtube_id = self.get_youtube_id_for_top_search_result(query)
             else:
@@ -515,40 +518,74 @@
                 self.logger.info("Converting downloaded video to WAV for audio processing...")
                 processed_track["youtube_audio"] = self.convert_to_wav(processed_track["youtube_video"], output_filename_no_extension)
             else:
                 self.logger.warning(f"Skipping {title} by {artist} due to missing YouTube ID.")
 
         self.logger.info(f"Separating audio twice for track: {title} by {artist}")
 
-        instrumental_path = os.path.join(track_output_dir, f"{artist_title} (Instrumental {self.model_name}).{self.output_format}")
-        vocals_path = os.path.join(track_output_dir, f"{artist_title} (Vocals {self.model_name}).{self.output_format}")
+        instrumental_path = os.path.join(track_output_dir, f"{artist_title} (Instrumental {self.model_name}).{self.lossless_output_format}")
+        vocals_path = os.path.join(track_output_dir, f"{artist_title} (Vocals {self.model_name}).{self.lossless_output_format}")
+
+        instrumental_path_lossy = os.path.join(
+            track_output_dir, f"{artist_title} (Instrumental {self.model_name}).{self.lossy_output_format}"
+        )
+        vocals_path_lossy = os.path.join(track_output_dir, f"{artist_title} (Vocals {self.model_name}).{self.lossy_output_format}")
 
         if os.path.isfile(instrumental_path) and os.path.isfile(vocals_path):
             self.logger.debug(f"Separated audio files already exist in output paths, skipping separation: {instrumental_path}")
         else:
             self.separate_audio(processed_track["youtube_audio"], self.model_name, instrumental_path, vocals_path)
+            self.convert_to_lossy(instrumental_path, instrumental_path_lossy)
+            self.convert_to_lossy(vocals_path, vocals_path_lossy)
 
         processed_track["instrumental_audio"] = instrumental_path
         processed_track["vocals_audio"] = vocals_path
 
-        instrumental_path_2 = os.path.join(track_output_dir, f"{artist_title} (Instrumental {self.model_name_2}).{self.output_format}")
-        vocals_path_2 = os.path.join(track_output_dir, f"{artist_title} (Vocals {self.model_name_2}).{self.output_format}")
+        processed_track["instrumental_audio_lossy"] = instrumental_path_lossy
+        processed_track["vocals_audio_lossy"] = vocals_path_lossy
+
+        instrumental_path_2 = os.path.join(
+            track_output_dir, f"{artist_title} (Instrumental {self.model_name_2}).{self.lossless_output_format}"
+        )
+        vocals_path_2 = os.path.join(track_output_dir, f"{artist_title} (Vocals {self.model_name_2}).{self.lossless_output_format}")
+
+        instrumental_path_2_lossy = os.path.join(
+            track_output_dir, f"{artist_title} (Instrumental {self.model_name_2}).{self.lossy_output_format}"
+        )
+        vocals_path_2_lossy = os.path.join(track_output_dir, f"{artist_title} (Vocals {self.model_name_2}).{self.lossy_output_format}")
 
         if os.path.isfile(instrumental_path_2) and os.path.isfile(vocals_path_2):
             self.logger.debug(f"Separated audio files already exist in output paths, skipping separation: {instrumental_path_2}")
         else:
             self.separate_audio(processed_track["youtube_audio"], self.model_name_2, instrumental_path_2, vocals_path_2)
+            self.convert_to_lossy(instrumental_path_2, instrumental_path_2_lossy)
+            self.convert_to_lossy(vocals_path_2, vocals_path_2_lossy)
 
         processed_track["instrumental_audio_2"] = instrumental_path_2
         processed_track["vocals_audio_2"] = vocals_path_2
 
+        processed_track["instrumental_audio_2_lossy"] = instrumental_path_2_lossy
+        processed_track["vocals_audio_2_lossy"] = vocals_path_2_lossy
+
         self.logger.info("Script finished, audio downloaded, lyrics fetched and audio separated!")
 
         return processed_track
 
+    def convert_to_lossy(self, input_filename, output_filename):
+        if input_filename is None or not os.path.isfile(input_filename):
+            raise Exception(f"Error: Invalid input file provided for convert_to_lossy: {input_filename}")
+
+        self.logger.info(f"Converting {self.lossless_output_format} audio to lossy {self.lossy_output_format} format")
+
+        ffmpeg_extras = "-q:a 0" if self.lossy_output_format == "mp3" else ""
+
+        ffmpeg_command = f'{self.ffmpeg_base_command} -i "{input_filename}" {ffmpeg_extras} "{output_filename}"'
+        self.logger.debug(f"Running command: {ffmpeg_command}")
+        os.system(ffmpeg_command)
+
     def is_playlist_url(self):
         """
         Checks if the provided URL is a YouTube playlist URL.
         """
         if self.url and "playlist?list=" in self.url:
             return True
         return False
```

### Comparing `karaoke_prep-0.9.1/karaoke_prep/resources/AvenirNext-Bold.ttf` & `karaoke_prep-0.9.2/karaoke_prep/resources/AvenirNext-Bold.ttf`

 * *Files identical despite different names*

### Comparing `karaoke_prep-0.9.1/karaoke_prep/resources/Montserrat-Bold.ttf` & `karaoke_prep-0.9.2/karaoke_prep/resources/Montserrat-Bold.ttf`

 * *Files identical despite different names*

### Comparing `karaoke_prep-0.9.1/karaoke_prep/utils/prep_cli.py` & `karaoke_prep-0.9.2/karaoke_prep/utils/prep_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,23 @@
     parser.add_argument(
         "--output_dir",
         default=".",
         help="Optional: directory to write output files (default: <current dir>). Example: --output_dir=/app/karaoke",
     )
 
     parser.add_argument(
-        "--output_format",
-        default="mp3",
-        help="Optional: output format for separated audio (default: mp3). Example: --output_format=flac",
+        "--lossless_output_format",
+        default="FLAC",
+        help="Optional: lossless output format for separated audio (default: FLAC). Example: --lossless_output_format=WAV",
+    )
+
+    parser.add_argument(
+        "--lossy_output_format",
+        default="MP3",
+        help="Optional: lossy output format for separated audio (default: MP3). Example: --lossy_output_format=OGG",
     )
 
     parser.add_argument(
         "--use_cuda",
         action="store_true",
         help="Optional: use Nvidia GPU with CUDA for separation (default: %(default)s). Example: --use_cuda=true",
     )
@@ -162,15 +168,16 @@
         title=title,
         url=url,
         log_formatter=log_formatter,
         log_level=log_level,
         model_name=args.model_name,
         model_file_dir=args.model_file_dir,
         output_dir=args.output_dir,
-        output_format=args.output_format,
+        lossless_output_format=args.lossless_output_format,
+        lossy_output_format=args.lossy_output_format,
         use_cuda=args.use_cuda,
         use_coreml=args.use_coreml,
         normalization_enabled=args.normalize,
         denoise_enabled=args.denoise,
         create_track_subfolders=args.no_track_subfolders,
         intro_background_color=args.intro_background_color,
         intro_background_image=args.intro_background_image,
```

### Comparing `karaoke_prep-0.9.1/pyproject.toml` & `karaoke_prep-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "karaoke-prep"
-version = "0.9.1"
+version = "0.9.2"
 description = "Prepare for karaoke video creation, by downloading audio and lyrics for a specified song or playlist from youtube and separating audio stems. After syncing, finalise the video with a title screen!"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "karaoke_prep"}]
 homepage = "https://github.com/karaokenerds/karaoke-prep"
 repository = "https://github.com/karaokenerds/karaoke-prep"
```

### Comparing `karaoke_prep-0.9.1/PKG-INFO` & `karaoke_prep-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karaoke-prep
-Version: 0.9.1
+Version: 0.9.2
 Summary: Prepare for karaoke video creation, by downloading audio and lyrics for a specified song or playlist from youtube and separating audio stems. After syncing, finalise the video with a title screen!
 Home-page: https://github.com/karaokenerds/karaoke-prep
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: karaoke-prep Version: 0.9.1 Summary: Prepare for
+Metadata-Version: 2.1 Name: karaoke-prep Version: 0.9.2 Summary: Prepare for
 karaoke video creation, by downloading audio and lyrics for a specified song or
 playlist from youtube and separating audio stems. After syncing, finalise the
 video with a title screen! Home-page: https://github.com/karaokenerds/karaoke-
 prep License: MIT Author: Andrew Beveridge Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```


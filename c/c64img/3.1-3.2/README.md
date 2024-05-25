# Comparing `tmp/c64img-3.1.tar.gz` & `tmp/c64img-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/c64img-3.1.tar", last modified: Sun Jun 17 13:00:34 2018, max compression
+gzip compressed data, was "c64img-3.2.tar", last modified: Sat May 25 14:41:25 2024, max compression
```

## Comparing `c64img-3.1.tar` & `c64img-3.2.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2018-06-17 13:00:34.000000 c64img-3.1/
--rw-r--r--   0 gryf      (1000) gryf      (1000)       19 2018-06-17 13:00:22.000000 c64img-3.1/MANIFEST.in
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2018-06-17 13:00:34.000000 c64img-3.1/c64img/
--rw-r--r--   0 gryf      (1000) gryf      (1000)     5044 2018-06-17 13:00:22.000000 c64img-3.1/c64img/cmd_convert.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)       20 2018-06-17 13:00:22.000000 c64img-3.1/c64img/__init__.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)      503 2018-06-17 13:00:22.000000 c64img-3.1/c64img/path.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     5615 2018-06-17 13:00:22.000000 c64img-3.1/c64img/hires.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)    11452 2018-06-17 13:00:22.000000 c64img-3.1/c64img/multi.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     1545 2018-06-17 13:00:22.000000 c64img-3.1/c64img/logger.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)    17770 2018-06-17 13:00:22.000000 c64img-3.1/c64img/base.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     9432 2018-06-17 13:00:34.000000 c64img-3.1/PKG-INFO
--rw-r--r--   0 gryf      (1000) gryf      (1000)     6976 2018-06-17 13:00:22.000000 c64img-3.1/README.rst
--rwxr-xr-x   0 gryf      (1000) gryf      (1000)     1337 2018-06-17 13:00:22.000000 c64img-3.1/setup.py
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2018-06-17 13:00:34.000000 c64img-3.1/scripts/
--rwxr-xr-x   0 gryf      (1000) gryf      (1000)      123 2018-06-17 13:00:22.000000 c64img-3.1/scripts/image2c64
--rw-r--r--   0 gryf      (1000) gryf      (1000)       38 2018-06-17 13:00:34.000000 c64img-3.1/setup.cfg
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2018-06-17 13:00:34.000000 c64img-3.1/c64img.egg-info/
--rw-r--r--   0 gryf      (1000) gryf      (1000)     9432 2018-06-17 13:00:34.000000 c64img-3.1/c64img.egg-info/PKG-INFO
--rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2018-06-17 13:00:34.000000 c64img-3.1/c64img.egg-info/requires.txt
--rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2018-06-17 13:00:34.000000 c64img-3.1/c64img.egg-info/top_level.txt
--rw-r--r--   0 gryf      (1000) gryf      (1000)        1 2018-06-17 13:00:34.000000 c64img-3.1/c64img.egg-info/dependency_links.txt
--rw-r--r--   0 gryf      (1000) gryf      (1000)      318 2018-06-17 13:00:34.000000 c64img-3.1/c64img.egg-info/SOURCES.txt
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     1528 2024-05-25 14:40:46.000000 c64img-3.2/LICENSE
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       19 2024-05-25 14:40:46.000000 c64img-3.2/MANIFEST.in
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     7974 2024-05-25 14:41:25.814042 c64img-3.2/PKG-INFO
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     7014 2024-05-25 14:40:46.000000 c64img-3.2/README.rst
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/c64img/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       20 2024-05-25 14:40:46.000000 c64img-3.2/c64img/__init__.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    18012 2024-05-25 14:40:46.000000 c64img-3.2/c64img/base.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     5044 2024-05-25 14:40:46.000000 c64img-3.2/c64img/cmd_convert.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     5542 2024-05-25 14:40:46.000000 c64img-3.2/c64img/hires.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     1545 2024-05-25 14:40:46.000000 c64img-3.2/c64img/logger.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    11505 2024-05-25 14:40:46.000000 c64img-3.2/c64img/multi.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)      503 2024-05-25 14:40:46.000000 c64img-3.2/c64img/path.py
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/c64img.egg-info/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     7974 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/PKG-INFO
+-rw-r--r--   0 gryf      (1000) gryf      (1000)      447 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/SOURCES.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)        1 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/dependency_links.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/requires.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/top_level.txt
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/scripts/
+-rwxr-xr-x   0 gryf      (1000) gryf      (1000)      123 2024-05-25 14:40:46.000000 c64img-3.2/scripts/image2c64
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       38 2024-05-25 14:41:25.814042 c64img-3.2/setup.cfg
+-rwxr-xr-x   0 gryf      (1000) gryf      (1000)     1449 2024-05-25 14:40:46.000000 c64img-3.2/setup.py
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/tests/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    18171 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_base.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     7578 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_convert.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    11119 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_hires.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     2508 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_logger.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    16490 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_multi.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)      871 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_path.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `c64img-3.1/c64img/cmd_convert.py` & `c64img-3.2/c64img/cmd_convert.py`

 * *Files identical despite different names*

### Comparing `c64img-3.1/c64img/hires.py` & `c64img-3.2/c64img/hires.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 
     def get_binary_data(self):
         """
         Return binary data for the char
         """
         result = {"bitmap": [], "screen-ram": 0}
 
-        for row in zip(*[iter(sorted(self.pixels))] * 8):
+        pixel_keys = sorted(self.pixels.keys())
+
+        for key_row in [pixel_keys[index:index+8]
+                        for index in range(0, len(pixel_keys), 8)]:
             char_line = 0
-            for idx, pixel in enumerate(row):
-                bit_ = self.colors.get(self.pixels[pixel], 0)
-                char_line += bit_ * 2 ** (7 - idx)
+            for key in key_row:
+                bit_ = self.colors.get(self.pixels[key], 0)
+                char_line += bit_ * 2 ** (7 - key[1])
             result['bitmap'].append(char_line)
 
         colors = dict([(y, x) for x, y in self.colors.items()])
         if 0 in colors:
             result['screen-ram'] = colors[0]
 
         if 1 in colors:
@@ -53,20 +56,20 @@
                           "hires": self._save_ash,  # make sane default
                           "art-studio-hires": self._save_ash}
 
     def _get_displayer(self):
         """
         Get displayer for hires picture
         """
-        border = "%c" % self._get_border()
-        displayer = ["\x01\x08\x0b\x08\x0a\x00\x9e\x32\x30\x36\x34\x00"
-                     "\x00\x00\x00\x00\x00\x78\xa9", border, "\x8d\x20\xd0\xa9"
-                     "\x00\x8d\x21\xd0\xa9\xbb\x8d\x11\xd0\xa9\x3c\x8d"
-                     "\x18\xd0\x4c\x25\x08"]
-        return "".join(displayer)
+        return bytearray([0x01, 0x08, 0x0b, 0x08, 0x0a, 0x00, 0x9e, 0x32,
+                          0x30, 0x36, 0x34, 0x00, 0x00, 0x00, 0x00, 0x00,
+                          0x00, 0x78, 0xa9, self._get_border(), 0x8d, 0x20,
+                          0xd0, 0xa9, 0x00, 0x8d, 0x21, 0xd0, 0xa9, 0xbb,
+                          0x8d, 0x11, 0xd0, 0xa9, 0x3c, 0x8d, 0x18, 0xd0,
+                          0x4c, 0x25, 0x08])
 
     def _fill_memory(self):
         """
         Create bitmap/screen and error map as a picture if needed.
         """
         self.data["bitmap"] = []
         self.data["screen-ram"] = []
@@ -107,54 +110,46 @@
 
     def _save_prg(self, filename):
         """
         Save executable version of the picture
         """
         file_obj = open(filename, "wb")
         file_obj.write(self._get_displayer())
-        file_obj.write(984 * chr(0))
-        file_obj.write("".join([chr(col) for col in self.data["screen-ram"]]))
-        file_obj.write(4120 * chr(0))
-        file_obj.write("".join([chr(byte) for byte in self.data["bitmap"]]))
+        file_obj.write(984 * b'\x00')
+        file_obj.write(bytearray(self.data["screen-ram"]))
+        file_obj.write(4120 * b'\x00')
+        file_obj.write(bytearray(self.data["bitmap"]))
         file_obj.close()
         self.log.info("Saved executable under `%s' file", filename)
         return True
 
     def _save_ash(self, filename):
         """
         Save as Art Studio hires
         """
         file_obj = open(filename, "wb")
-        file_obj.write("%c%c" % (0x00, 0x20))
-
-        for char in self.data['bitmap']:
-            file_obj.write("%c" % char)
-
-        for char in self.data["screen-ram"]:
-            file_obj.write("%c" % char)
-
-        border = self._get_border()
-        file_obj.write("%c" % border)
-        file_obj.write("\x00\x00\x00\x00\x00\x00")
+        file_obj.write(bytearray([0x00, 0x20]))
+        file_obj.write(bytearray(self.data['bitmap']))
+        file_obj.write(bytearray(self.data["screen-ram"]))
+        file_obj.write(bytearray([self._get_border()]))
+        file_obj.write(6 * b'\x00')
         file_obj.close()
         self.log.info("Saved in Art Studio Hires format under `%s' file",
                       filename)
         return True
 
     def _save_raw(self, filename):
         """
         Save raw data
         """
         with open(filename + "_screen.raw", "wb") as file_obj:
-            file_obj.write("".join([chr(col)
-                                    for col in self.data["screen-ram"]]))
+            file_obj.write(bytearray(self.data["screen-ram"]))
 
         with open(filename + "_bitmap.raw", "wb") as file_obj:
-            file_obj.write("".join([chr(byte)
-                                    for byte in self.data["bitmap"]]))
+            file_obj.write(bytearray(self.data["bitmap"]))
 
         self.log.info("Saved raw data under `%s_*' files", filename)
         return True
 
     def _check_dimensions(self):
         """
         Check for image dimensions. Same as in superclass, needed for feedback
```

### Comparing `c64img-3.1/c64img/multi.py` & `c64img-3.2/c64img/multi.py`

 * *Files 23% similar despite different names*

```diff
@@ -154,24 +154,28 @@
             self.log.error("Wrong picture dimensions: %dx%d", width, height)
         return result
 
     def _get_displayer(self):
         """
         Get displayer for multicolor picture (based on kickassembler example)
         """
-        border = chr(self._get_border())
-        background = chr(self._get_background())
-        displayer = ["\x01\x08\x0b\x08\n\x00\x9e2064\x00\x00\x00\x00\x00\x00"
-                     "\xa98\x8d\x18\xd0\xa9\xd8\x8d\x16\xd0\xa9;\x8d\x11\xd0"
-                     "\xa9", border, "\x8d \xd0\xa9", background, "\x8d!\xd0"
-                     "\xa2\x00\xbd\x00\x1c\x9d\x00\xd8\xbd\x00\x1d\x9d\x00"
-                     "\xd9\xbd\x00\x1e\x9d\x00\xda\xbd\x00\x1f\x9d\x00\xdb"
-                     "\xe8\xd0\xe5LF\x08"]
+        border = self._get_border()
+        background = self._get_background()
 
-        return "".join(displayer)
+        return bytearray([0x01, 0x08, 0x0b, 0x08, 0x0a, 0x00, 0x9e,
+                          0x32, 0x30, 0x36, 0x34,
+                          0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xa9,
+                          0x38, 0x8d, 0x18, 0xd0, 0xa9, 0xd8, 0x8d, 0x16,
+                          0xd0, 0xa9, 0x3b, 0x8d, 0x11, 0xd0, 0xa9, border,
+                          0x8d, 0x20, 0xd0, 0xa9, background, 0x8d, 0x21,
+                          0xd0, 0xa2, 0x00, 0xbd, 0x00, 0x1c, 0x9d, 0x00,
+                          0xd8, 0xbd, 0x00, 0x1d, 0x9d, 0x00, 0xd9, 0xbd,
+                          0x00, 0x1e, 0x9d, 0x00, 0xda, 0xbd, 0x00, 0x1f,
+                          0x9d, 0x00, 0xdb, 0xe8, 0xd0, 0xe5, 0x4c, 0x46,
+                          0x08])
 
     def _fill_memory(self):
         """
         Create bitmap, screen-ram, color-ram and error map as a picture if
         needed.
         """
         self.data["bitmap"] = []
@@ -252,61 +256,51 @@
 
     def _save_prg(self, filename):
         """
         Save executable version of the picture
         """
         file_obj = open(filename, "wb")
         file_obj.write(self._get_displayer())
-        file_obj.write(951 * chr(0))
-        file_obj.write("".join([chr(col) for col in self.data["color-ram"]]))
-        file_obj.write(3096 * chr(0))
-        file_obj.write("".join([chr(col) for col in self.data["screen-ram"]]))
-        file_obj.write(24 * chr(0))
-        file_obj.write("".join([chr(byte) for byte in self.data["bitmap"]]))
+        file_obj.write(951 * b'\x00')
+        file_obj.write(bytearray(self.data["color-ram"]))
+        file_obj.write(3096 * b'\x00')
+        file_obj.write(bytearray(self.data["screen-ram"]))
+        file_obj.write(24 * b'\x00')
+        file_obj.write(bytearray(self.data["bitmap"]))
         file_obj.close()
         self.log.info("Saved executable under `%s' file", filename)
         return True
 
     def _save_koala(self, filename):
         """
         Save as Koala format
         """
         file_obj = open(filename, "wb")
-        file_obj.write("%c%c" % (0x00, 0x60))
-
-        for char in self.data['bitmap']:
-            file_obj.write("%c" % char)
-
-        for char in self.data["color-ram"]:
-            file_obj.write("%c" % char)
-
-        for char in self.data["screen-ram"]:
-            file_obj.write("%c" % char)
-
-        file_obj.write(chr(self.data["background"]))
+        file_obj.write(bytearray([0x00, 0x60]))
+        file_obj.write(bytearray(self.data['bitmap']))
+        file_obj.write(bytearray(self.data["color-ram"]))
+        file_obj.write(bytearray(self.data["screen-ram"]))
+        file_obj.write(bytearray([self.data["background"]]))
 
         file_obj.close()
         self.log.info("Saved in Koala format under `%s' file", filename)
         return True
 
     def _save_raw(self, filename):
         """
         Save as raw data
         """
 
         with open(filename + "_bitmap.raw", "wb") as file_obj:
-            for char in self.data['bitmap']:
-                file_obj.write("%c" % char)
+            file_obj.write(bytearray(self.data['bitmap']))
 
         with open(filename + "_screen.raw", "wb") as file_obj:
-            for char in self.data["screen-ram"]:
-                file_obj.write("%c" % char)
+            file_obj.write(bytearray(self.data["screen-ram"]))
 
         with open(filename + "_color-ram.raw", "wb") as file_obj:
-            for char in self.data["color-ram"]:
-                file_obj.write("%c" % char)
+            file_obj.write(bytearray(self.data["color-ram"]))
 
         with open(filename + "_bg.raw", "wb") as file_obj:
-            file_obj.write(chr(self.data["background"]))
+            file_obj.write(bytearray([self.data["background"]]))
 
         self.log.info("Saved in raw format under `%s_*' files", filename)
         return True
```

### Comparing `c64img-3.1/c64img/logger.py` & `c64img-3.2/c64img/logger.py`

 * *Files identical despite different names*

### Comparing `c64img-3.1/c64img/base.py` & `c64img-3.2/c64img/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         return self.clash
 
     def _compare_colors_with_prev_char(self, colors, repeat=False):
         """
         Make a color map to the pixels comparing to the previous data
         """
         needs_repeat = False
-        for color in colors:
+        for color in sorted(colors):
             if color == self.background:
                 continue
             if repeat:
                 if color in self.colors:
                     continue
 
                 for pair, taken in self.pixel_state.items():
@@ -317,22 +317,25 @@
         """
         Check for the most frequent color on the picture. Can be used to
         auto detect background/border colors.
         Value remembered in attribute data['most_freq_color'] is an
         index in the C64 palette (NOT the source image palette!).
         """
         pal = self._src_image.getpalette()
-        pal = [tuple(pal[index:index + 3]) for index in xrange(0, len(pal),
-                                                               3)]
+        pal = [tuple(pal[index:index + 3]) for index in range(0, len(pal), 3)]
         sorted_hist = sorted([(count, index)
                               for index, count in enumerate(histogram[:16])],
                              reverse=True)
         self.data['most_freq_colors'] = []
         for _, index in sorted_hist:
-            color = self._palette_map[pal[index]]
+            try:
+                color = self._palette_map[pal[index]]
+            except IndexError:
+                # image palette have incomplete amount of colors - ignore
+                continue
             self.data['most_freq_colors'].append(color)
 
         self.data['most_freq_color'] = self.data['most_freq_colors'][0]
 
     def _colors_check(self, histogram):
         """
         Find out how many same colors do we have. Just an information to the
@@ -348,14 +351,17 @@
         return no_of_colors
 
     def _get_palette(self):
         """
         Return source image palette as RGB tuples
         """
         pal = self._src_image.getpalette()
+        if len(pal) < 48:
+            # image does not have full palette - fill gap with 0
+            pal.extend([0 for _ in range(48-len(pal))])
         return [(pal[i], pal[i + 1], pal[i + 2]) for i in range(0, 16 * 3, 3)]
 
     def _fill_memory(self):
         """
         Create bitmap/screen-ram/color-ram colors if needed. Should be
         implemented in concrete implementation.
         """
```

### Comparing `c64img-3.1/README.rst` & `c64img-3.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 expected. Mutlicolor pictures will be scaled down to 160x200. Picture will be
 converted to 16 colors. During that process some information can be lost, if
 used more than 16 colors.
 
 Requirements:
 -------------
 
-+ `Python 2.7`_
++ `Python`_ 2.7, >3.5
 + `Pillow`_ module
 
 
 Installation
 ------------
 
 Like other standard Python pro programs, ``c64img`` provide a convenient way to
@@ -54,15 +54,15 @@
 
    $ pip install c64img
 
 finally, if you prefer to use virtualenv:
 
 .. code:: shell-session
 
-   $ virtualenv -p python2 venvname
+   $ virtualenv venvname
    $ source venvname/bin/activate
    (venvname) $ pip install c64img
 
 After that, you should be able to access ``image2c64`` script or import
 ``c64img`` module in Python interpreter.
 
 Usage:
@@ -72,25 +72,25 @@
 
 .. code:: shell-session
 
    $ image2c64 --help
 
 Besides fine-tuning options like ``-b``/``--border`` for selecting border
 color, ``-g``/``--background`` for selecting background color, it allows to
-select aprorpiate output format:
+select appropriate output format:
 
 - *multi* - for pure data located at ``$6000``
 - *hires* - same, but for hires bitmap and colors (``$2000``)
 - *koala* - multicolor bitmap in Koala format
 - *art-studio-hires* - high resolution bitmap in Art Studio format (hires
   version)
 
 Those formats should be passed using ``-f``/``--format`` parameter.
 
-Furthemore two more switches can be used for output format:
+Furthermore two more switches can be used for output format:
 
 - *raw* (``-r``, ``--raw``) - this will produce four files (*prefix* is
   obtained from the input image file name, or by using ``-o`` switch for
   output):
 
   - ``prefix_bg.raw`` 1-byte file with background color,
   - ``prefix_screen.raw`` - screen colors (usually placed at $0400),
@@ -165,14 +165,15 @@
    $ ./image2c64 -f multi -x -e fix test_images/clash.multi.png
    WARNING: Cannot remap color; using background - 'Light green'
    $
 
 Changes
 -------
 
++ 2021-08-14 Forgot to push python3 support!
 + 2018-06-12 Added information about possibility to convert picture to chars
   (no conversion! Just an info in log!)
 + 2015-09-10 Rearranged repository into separate modules for maintainability
 + 2014-11-16 Added mechanism for automatic clashes fix
 + 2014-11-11 Fixed issue with color clash check in multicolor
 + 2014-11-11 Added ``grafx2`` option into error param. In such case image will
   be opened in `grafx2`_ program alongside with the error pic on spare screen.
@@ -188,11 +189,11 @@
 This software is licensed under 3-clause BSD license. See LICENSE file for
 details.
 
 
 .. _PNG2HIRES_ v0.2 gfx format converter: http://www.atlantis-prophecy.org/onslaught/legal.html
 .. _pillow: https://github.com/python-imaging/Pillow
 .. _grafx2: http://grafx2.chez.com
-.. _python 2.7: https://www.python.org
+.. _python: https://www.python.org
 .. _setuptools: https://pypi.python.org/pypi/setuptools
 .. _pip: https://github.com/pypa/pip
 .. _pypi: https://pypi.org
```

### Comparing `c64img-3.1/setup.py` & `c64img-3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
       url='https://bitbucket.org/gryf/image2c64',
       download_url='https://bitbucket.org/gryf/image2c64.git',
       keywords=['c64', 'image', 'converter', 'koala', 'Art Studio', 'raw'],
       install_requires=['Pillow'],
       scripts=['scripts/image2c64'],
       classifiers=['Programming Language :: Python :: 2',
                    'Programming Language :: Python :: 2.7',
-                   'Programming Language :: Python :: 2 :: Only',
+                   'Programming Language :: Python :: 3',
+                   'Programming Language :: Python :: 3.5',
+                   'Programming Language :: Python :: 3.6',
                    'Development Status :: 5 - Production/Stable',
                    'Environment :: Console',
                    'Intended Audience :: End Users/Desktop',
                    'License :: OSI Approved :: BSD License',
                    'Operating System :: OS Independent',
                    'Topic :: Multimedia :: Graphics',
                    'Topic :: Multimedia :: Graphics :: Graphics Conversion'],
```


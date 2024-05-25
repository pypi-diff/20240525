# Comparing `tmp/terminaltexteffects-0.9.2.tar.gz` & `tmp/terminaltexteffects-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminaltexteffects-0.9.2.tar", max compression
+gzip compressed data, was "terminaltexteffects-0.9.3.tar", max compression
```

## Comparing `terminaltexteffects-0.9.2.tar` & `terminaltexteffects-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.9.2/LICENSE
--rwxr-xr-x   0        0        0    12812 2024-05-11 11:39:58.361920 terminaltexteffects-0.9.2/README.md
--rwxr-xr-x   0        0        0      474 2024-05-11 12:14:52.710254 terminaltexteffects-0.9.2/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.9.2/terminaltexteffects/__init__.py
--rwxr-xr-x   0        0        0     2054 2024-05-11 11:36:03.464604 terminaltexteffects-0.9.2/terminaltexteffects/__main__.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.9.2/terminaltexteffects/effects/__init__.py
--rwxr-xr-x   0        0        0    17753 2024-05-11 02:30:33.705429 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_beams.py
--rwxr-xr-x   0        0        0    15747 2024-05-11 02:30:33.705887 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_binarypath.py
--rwxr-xr-x   0        0        0    18978 2024-05-11 02:30:33.706344 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_blackhole.py
--rwxr-xr-x   0        0        0    10743 2024-05-11 02:30:33.706729 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_bouncyballs.py
--rwxr-xr-x   0        0        0    17536 2024-05-11 02:30:33.707172 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_bubbles.py
--rwxr-xr-x   0        0        0     7978 2024-05-11 02:30:33.707521 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_burn.py
--rwxr-xr-x   0        0        0    11370 2024-05-11 02:30:33.707917 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_crumble.py
--rwxr-xr-x   0        0        0    11098 2024-05-11 02:30:33.708254 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_decrypt.py
--rwxr-xr-x   0        0        0    13625 2024-05-11 02:30:33.708606 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_errorcorrect.py
--rwxr-xr-x   0        0        0     7643 2024-05-11 02:30:33.709011 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_expand.py
--rwxr-xr-x   0        0        0    14006 2024-05-11 02:30:33.709598 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_fireworks.py
--rwxr-xr-x   0        0        0    10352 2024-05-11 02:30:33.709967 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_middleout.py
--rwxr-xr-x   0        0        0    17071 2024-05-11 02:30:33.710369 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_orbittingvolley.py
--rwxr-xr-x   0        0        0    10990 2024-05-11 02:30:33.722626 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_overflow.py
--rwxr-xr-x   0        0        0    12173 2024-05-11 02:30:33.722985 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_pour.py
--rwxr-xr-x   0        0        0    11913 2024-05-11 02:30:33.723338 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_print.py
--rwxr-xr-x   0        0        0     9893 2024-05-11 02:30:33.723681 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_rain.py
--rwxr-xr-x   0        0        0     7648 2024-05-11 02:30:33.724000 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_random_sequence.py
--rwxr-xr-x   0        0        0    19574 2024-05-11 02:30:33.724409 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_rings.py
--rwxr-xr-x   0        0        0     8099 2024-05-11 02:30:33.736965 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_scattered.py
--rwxr-xr-x   0        0        0    13682 2024-05-11 02:30:33.739745 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_slide.py
--rwxr-xr-x   0        0        0    14154 2024-05-11 02:30:33.741774 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_spotlights.py
--rwxr-xr-x   0        0        0    11045 2024-05-11 02:30:33.744093 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_spray.py
--rwxr-xr-x   0        0        0    15062 2024-05-11 02:30:33.746289 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_swarm.py
--rwxr-xr-x   0        0        0    20266 2024-05-11 02:30:33.748715 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_synthgrid.py
--rwxr-xr-x   0        0        0    13906 2024-05-11 02:30:33.750929 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_unstable.py
--rwxr-xr-x   0        0        0     8383 2024-05-11 02:30:33.752675 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_verticalslice.py
--rwxr-xr-x   0        0        0    22571 2024-05-11 02:30:33.754914 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_vhstape.py
--rwxr-xr-x   0        0        0    10335 2024-05-11 02:30:33.756690 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_waves.py
--rwxr-xr-x   0        0        0     9519 2024-05-11 02:30:33.758437 terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_wipe.py
--rwxr-xr-x   0        0        0        0 2024-05-05 17:33:51.724578 terminaltexteffects-0.9.2/terminaltexteffects/engine/__init__.py
--rwxr-xr-x   0        0        0    22748 2024-05-05 17:33:51.741057 terminaltexteffects-0.9.2/terminaltexteffects/engine/animation.py
--rwxr-xr-x   0        0        0    11162 2024-05-05 17:33:51.752448 terminaltexteffects-0.9.2/terminaltexteffects/engine/base_character.py
--rwxr-xr-x   0        0        0     4837 2024-05-11 02:30:33.760461 terminaltexteffects-0.9.2/terminaltexteffects/engine/base_effect.py
--rwxr-xr-x   0        0        0    22354 2024-05-05 17:33:51.800192 terminaltexteffects-0.9.2/terminaltexteffects/engine/motion.py
--rwxr-xr-x   0        0        0    30508 2024-05-11 12:11:48.558883 terminaltexteffects-0.9.2/terminaltexteffects/engine/terminal.py
--rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.9.2/terminaltexteffects/py.typed
--rwxr-xr-x   0        0        0     4780 2024-05-11 02:30:33.763094 terminaltexteffects-0.9.2/terminaltexteffects/template/effect_template.py
--rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.9.2/terminaltexteffects/utils/__init__.py
--rwxr-xr-x   0        0        0     2432 2024-05-05 17:33:51.818449 terminaltexteffects-0.9.2/terminaltexteffects/utils/ansitools.py
--rwxr-xr-x   0        0        0    12883 2024-05-05 17:33:51.829129 terminaltexteffects-0.9.2/terminaltexteffects/utils/argsdataclass.py
--rwxr-xr-x   0        0        0    15541 2024-05-09 10:47:29.473915 terminaltexteffects-0.9.2/terminaltexteffects/utils/argvalidators.py
--rwxr-xr-x   0        0        0     2399 2024-05-05 17:33:51.832912 terminaltexteffects-0.9.2/terminaltexteffects/utils/colorterm.py
--rwxr-xr-x   0        0        0    13639 2024-05-05 17:33:51.833389 terminaltexteffects-0.9.2/terminaltexteffects/utils/easing.py
--rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.9.2/terminaltexteffects/utils/exceptions.py
--rwxr-xr-x   0        0        0     9843 2024-05-05 17:33:51.833880 terminaltexteffects-0.9.2/terminaltexteffects/utils/geometry.py
--rwxr-xr-x   0        0        0    10349 2024-05-11 02:41:27.527818 terminaltexteffects-0.9.2/terminaltexteffects/utils/graphics.py
--rwxr-xr-x   0        0        0     7140 2024-05-05 17:33:51.847877 terminaltexteffects-0.9.2/terminaltexteffects/utils/hexterm.py
--rw-r--r--   0        0        0    13342 1970-01-01 00:00:00.000000 terminaltexteffects-0.9.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-08-13 20:34:07.346818 terminaltexteffects-0.9.3/LICENSE
+-rwxr-xr-x   0        0        0    12477 2024-05-13 11:25:33.953166 terminaltexteffects-0.9.3/README.md
+-rwxr-xr-x   0        0        0      474 2024-05-13 11:57:07.312834 terminaltexteffects-0.9.3/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-08-12 13:15:55.921216 terminaltexteffects-0.9.3/terminaltexteffects/__init__.py
+-rwxr-xr-x   0        0        0     2054 2024-05-11 11:36:03.464604 terminaltexteffects-0.9.3/terminaltexteffects/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:37.688921 terminaltexteffects-0.9.3/terminaltexteffects/effects/__init__.py
+-rwxr-xr-x   0        0        0    17753 2024-05-11 02:30:33.705429 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_beams.py
+-rwxr-xr-x   0        0        0    15747 2024-05-11 02:30:33.705887 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_binarypath.py
+-rwxr-xr-x   0        0        0    18978 2024-05-11 02:30:33.706344 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_blackhole.py
+-rwxr-xr-x   0        0        0    10743 2024-05-11 02:30:33.706729 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_bouncyballs.py
+-rwxr-xr-x   0        0        0    17536 2024-05-11 02:30:33.707172 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_bubbles.py
+-rwxr-xr-x   0        0        0     7978 2024-05-11 02:30:33.707521 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_burn.py
+-rwxr-xr-x   0        0        0    11370 2024-05-11 02:30:33.707917 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_crumble.py
+-rwxr-xr-x   0        0        0    11098 2024-05-11 02:30:33.708254 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_decrypt.py
+-rwxr-xr-x   0        0        0    13625 2024-05-11 02:30:33.708606 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_errorcorrect.py
+-rwxr-xr-x   0        0        0     7643 2024-05-11 02:30:33.709011 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_expand.py
+-rwxr-xr-x   0        0        0    14006 2024-05-11 02:30:33.709598 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_fireworks.py
+-rwxr-xr-x   0        0        0    10352 2024-05-11 02:30:33.709967 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_middleout.py
+-rwxr-xr-x   0        0        0    17071 2024-05-11 02:30:33.710369 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_orbittingvolley.py
+-rwxr-xr-x   0        0        0    10990 2024-05-11 02:30:33.722626 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_overflow.py
+-rwxr-xr-x   0        0        0    12173 2024-05-11 02:30:33.722985 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_pour.py
+-rwxr-xr-x   0        0        0    11913 2024-05-11 02:30:33.723338 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_print.py
+-rwxr-xr-x   0        0        0     9893 2024-05-11 02:30:33.723681 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_rain.py
+-rwxr-xr-x   0        0        0     7648 2024-05-11 02:30:33.724000 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_random_sequence.py
+-rwxr-xr-x   0        0        0    19574 2024-05-11 02:30:33.724409 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_rings.py
+-rwxr-xr-x   0        0        0     8099 2024-05-11 02:30:33.736965 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_scattered.py
+-rwxr-xr-x   0        0        0    13682 2024-05-11 02:30:33.739745 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_slide.py
+-rwxr-xr-x   0        0        0    14154 2024-05-11 02:30:33.741774 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_spotlights.py
+-rwxr-xr-x   0        0        0    11045 2024-05-11 02:30:33.744093 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_spray.py
+-rwxr-xr-x   0        0        0    15062 2024-05-11 02:30:33.746289 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_swarm.py
+-rwxr-xr-x   0        0        0    20266 2024-05-11 02:30:33.748715 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_synthgrid.py
+-rwxr-xr-x   0        0        0    13906 2024-05-11 02:30:33.750929 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_unstable.py
+-rwxr-xr-x   0        0        0     8383 2024-05-11 02:30:33.752675 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_verticalslice.py
+-rwxr-xr-x   0        0        0    22571 2024-05-11 02:30:33.754914 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_vhstape.py
+-rwxr-xr-x   0        0        0    10335 2024-05-11 02:30:33.756690 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_waves.py
+-rwxr-xr-x   0        0        0     9519 2024-05-11 02:30:33.758437 terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_wipe.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 17:33:51.724578 terminaltexteffects-0.9.3/terminaltexteffects/engine/__init__.py
+-rwxr-xr-x   0        0        0    22748 2024-05-05 17:33:51.741057 terminaltexteffects-0.9.3/terminaltexteffects/engine/animation.py
+-rwxr-xr-x   0        0        0    11162 2024-05-05 17:33:51.752448 terminaltexteffects-0.9.3/terminaltexteffects/engine/base_character.py
+-rwxr-xr-x   0        0        0     5102 2024-05-13 11:54:58.988925 terminaltexteffects-0.9.3/terminaltexteffects/engine/base_effect.py
+-rwxr-xr-x   0        0        0    22354 2024-05-05 17:33:51.800192 terminaltexteffects-0.9.3/terminaltexteffects/engine/motion.py
+-rwxr-xr-x   0        0        0    31042 2024-05-13 11:53:59.988319 terminaltexteffects-0.9.3/terminaltexteffects/engine/terminal.py
+-rwxr-xr-x   0        0        0        0 2024-04-12 11:52:35.092907 terminaltexteffects-0.9.3/terminaltexteffects/py.typed
+-rwxr-xr-x   0        0        0     4780 2024-05-11 02:30:33.763094 terminaltexteffects-0.9.3/terminaltexteffects/template/effect_template.py
+-rwxr-xr-x   0        0        0        0 2023-07-22 17:59:26.632934 terminaltexteffects-0.9.3/terminaltexteffects/utils/__init__.py
+-rwxr-xr-x   0        0        0     2432 2024-05-05 17:33:51.818449 terminaltexteffects-0.9.3/terminaltexteffects/utils/ansitools.py
+-rwxr-xr-x   0        0        0    12883 2024-05-05 17:33:51.829129 terminaltexteffects-0.9.3/terminaltexteffects/utils/argsdataclass.py
+-rwxr-xr-x   0        0        0    15541 2024-05-09 10:47:29.473915 terminaltexteffects-0.9.3/terminaltexteffects/utils/argvalidators.py
+-rwxr-xr-x   0        0        0     2399 2024-05-05 17:33:51.832912 terminaltexteffects-0.9.3/terminaltexteffects/utils/colorterm.py
+-rwxr-xr-x   0        0        0    13639 2024-05-05 17:33:51.833389 terminaltexteffects-0.9.3/terminaltexteffects/utils/easing.py
+-rwxr-xr-x   0        0        0        0 2024-04-26 11:00:38.378584 terminaltexteffects-0.9.3/terminaltexteffects/utils/exceptions.py
+-rwxr-xr-x   0        0        0     9843 2024-05-05 17:33:51.833880 terminaltexteffects-0.9.3/terminaltexteffects/utils/geometry.py
+-rwxr-xr-x   0        0        0    10349 2024-05-11 02:41:27.527818 terminaltexteffects-0.9.3/terminaltexteffects/utils/graphics.py
+-rwxr-xr-x   0        0        0     7140 2024-05-05 17:33:51.847877 terminaltexteffects-0.9.3/terminaltexteffects/utils/hexterm.py
+-rw-r--r--   0        0        0    13007 1970-01-01 00:00:00.000000 terminaltexteffects-0.9.3/PKG-INFO
```

### Comparing `terminaltexteffects-0.9.2/LICENSE` & `terminaltexteffects-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/README.md` & `terminaltexteffects-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -241,53 +241,44 @@
 
 ## In-Development Preview
 
 Any effects shown below are in development and will be available in the next release.
 
 ## Latest Release Notes
 
-## 0.9.1
+## 0.9.3
 
 ---
 
-### New Features (0.9.1)
+### New Features (0.9.3)
 
 ---
 
-#### New Engine Features (0.9.1)
+#### New Engine Features (0.9.3)
 
-* Terminal dimension auto-detection supports automatically detecting a single dimensions.
+* Added argument to the `BaseEffect.terminal_output()` context manager. `end_symbol` (default `\n`) is used to specify
+the symbol that will be printed after the effect completes. Set to `''` or `' '` to enable animated prompts.
 
-### Changes (0.9.1)
+### Changes (0.9.3)
 
 ---
 
-#### Effects Changes (0.9.1)
+#### Engine Changes (0.9.3)
 
-* All effects have been updated to use the new `update()` method and `frame` property of
-  `base_effect.BaseEffectIterator`. See Engine Changes for more info.
+* Removed unnecessary write calls for cursor positioning on every frame.
+* Separated functionality related to cursor positioning and frame timing out of `Terminal.print()` and into
+`Terminal.enforce_framerate()`, `Terminal.prep_outputarea()` and `Terminal.move_cursor_to_top()`.
 
-#### Engine Changes (0.9.1)
+### Bug Fixes (0.9.3)
 
-* `base_effect.BaseEffectIterator` now has an `update()` method which calls the `tick()` method of all active characters
-  and manages the `active_characters` list.
-* `base_effect.BaseEffectIterator` has a `frame` property which calls `Terminal.get_formatted_output_string()` and
-  returns the string.
-* `TerminalConfig.terminal_dimensions` has been split into `TerminalConfig.terminal_width` and
-  `TerminalConfig.terminal_height` to simply the command line argument for dimensions and make it more obvious which
-  dimensions is being specified when interacting with `effect.terminal_config`.
-
-#### Other Changes (0.9.1)
+---
 
-* Updated help output for `--terminal-dimensions` argument.
+#### Engine Fixes (0.9.3)
 
-### Bug Fixes (0.9.1)
+* Fixed the output area of an effect being 1 row less than specified via the `Terminal.terminal_height` attribute. This
+  was caused by mixing use of `print()` and `sys.stdout.write()`.
 
 ---
 
-#### Engine Fixes (0.9.1)
-
-* Fixed division by zero error when the terminal height was set to 1.
-
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for more information.
```

#### html2text {}

```diff
@@ -133,25 +133,21 @@
 057338f4e007) #### Swarm ![swarm_demo](https://github.com/ChrisBuilds/
 terminaltexteffects/assets/57874186/305e8390-a0fb-4edb-a541-7b52cef77c09) ####
 VHSTape ![vhstape_demo](https://github.com/ChrisBuilds/terminaltexteffects/
 assets/57874186/720abbf4-f97d-4ce9-96ee-15ef973488d2) #### Waves ![waves_demo]
 (https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/ea9b04ca-
 e526-4c7e-b98d-a98a42f7137f) ## In-Development Preview Any effects shown below
 are in development and will be available in the next release. ## Latest Release
-Notes ## 0.9.1 --- ### New Features (0.9.1) --- #### New Engine Features
-(0.9.1) * Terminal dimension auto-detection supports automatically detecting a
-single dimensions. ### Changes (0.9.1) --- #### Effects Changes (0.9.1) * All
-effects have been updated to use the new `update()` method and `frame` property
-of `base_effect.BaseEffectIterator`. See Engine Changes for more info. ####
-Engine Changes (0.9.1) * `base_effect.BaseEffectIterator` now has an `update()`
-method which calls the `tick()` method of all active characters and manages the
-`active_characters` list. * `base_effect.BaseEffectIterator` has a `frame`
-property which calls `Terminal.get_formatted_output_string()` and returns the
-string. * `TerminalConfig.terminal_dimensions` has been split into
-`TerminalConfig.terminal_width` and `TerminalConfig.terminal_height` to simply
-the command line argument for dimensions and make it more obvious which
-dimensions is being specified when interacting with `effect.terminal_config`.
-#### Other Changes (0.9.1) * Updated help output for `--terminal-dimensions`
-argument. ### Bug Fixes (0.9.1) --- #### Engine Fixes (0.9.1) * Fixed division
-by zero error when the terminal height was set to 1. ## License Distributed
-under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/
-terminaltexteffects/blob/main/LICENSE.md) for more information.
+Notes ## 0.9.3 --- ### New Features (0.9.3) --- #### New Engine Features
+(0.9.3) * Added argument to the `BaseEffect.terminal_output()` context manager.
+`end_symbol` (default `\n`) is used to specify the symbol that will be printed
+after the effect completes. Set to `''` or `' '` to enable animated prompts.
+### Changes (0.9.3) --- #### Engine Changes (0.9.3) * Removed unnecessary write
+calls for cursor positioning on every frame. * Separated functionality related
+to cursor positioning and frame timing out of `Terminal.print()` and into
+`Terminal.enforce_framerate()`, `Terminal.prep_outputarea()` and
+`Terminal.move_cursor_to_top()`. ### Bug Fixes (0.9.3) --- #### Engine Fixes
+(0.9.3) * Fixed the output area of an effect being 1 row less than specified
+via the `Terminal.terminal_height` attribute. This was caused by mixing use of
+`print()` and `sys.stdout.write()`. --- ## License Distributed under the MIT
+License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/
+main/LICENSE.md) for more information.
```

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/__main__.py` & `terminaltexteffects-0.9.3/terminaltexteffects/__main__.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_beams.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_beams.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_binarypath.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_binarypath.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_blackhole.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_blackhole.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_bouncyballs.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_bouncyballs.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_bubbles.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_bubbles.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_burn.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_burn.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_crumble.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_crumble.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_decrypt.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_decrypt.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_errorcorrect.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_errorcorrect.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_expand.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_expand.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_fireworks.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_fireworks.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_middleout.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_middleout.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_orbittingvolley.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_orbittingvolley.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_overflow.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_overflow.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_pour.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_pour.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_print.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_print.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_rain.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_rain.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_random_sequence.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_random_sequence.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_rings.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_rings.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_scattered.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_scattered.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_slide.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_slide.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_spotlights.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_spotlights.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_spray.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_spray.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_swarm.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_swarm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_synthgrid.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_synthgrid.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_unstable.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_unstable.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_verticalslice.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_verticalslice.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_vhstape.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_vhstape.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_waves.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_waves.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/effects/effect_wipe.py` & `terminaltexteffects-0.9.3/terminaltexteffects/effects/effect_wipe.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/engine/animation.py` & `terminaltexteffects-0.9.3/terminaltexteffects/engine/animation.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/engine/base_character.py` & `terminaltexteffects-0.9.3/terminaltexteffects/engine/base_character.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/engine/base_effect.py` & `terminaltexteffects-0.9.3/terminaltexteffects/engine/base_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     BaseEffect(Generic[T]): An abstract base class that defines the basic structure for an effect. Provides the `__iter__`
         method and a context manager for terminal output.
 """
 
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from copy import deepcopy
-from typing import Generic, TypeVar
+from typing import Generator, Generic, TypeVar
 
 from terminaltexteffects.engine.base_character import EffectCharacter
 from terminaltexteffects.engine.terminal import Terminal, TerminalConfig
 from terminaltexteffects.utils.argsdataclass import ArgsDataClass
 
 T = TypeVar("T", bound=ArgsDataClass)
 
@@ -113,24 +113,28 @@
         self.effect_config = self._config_cls()
         self.terminal_config = TerminalConfig()
 
     def __iter__(self) -> BaseEffectIterator:
         return self._iterator_cls(self)
 
     @contextmanager
-    def terminal_output(self):
+    def terminal_output(self, end_symbol: str = "\n") -> Generator[Terminal, None, None]:
         """Context manager for terminal output. Prepares the terminal for output and restores it after.
 
+        Args:
+            end_symbol (str, optional): Symbol to print after the effect has completed. Defaults to newline.
+
         Yields:
-            terminal (Terminal): Terminal object for output.
+            Terminal: Terminal object for handling output.
 
         Raises:
-            Exception: Any exception that occurs within the context manager.
+            Exception: Any exception that occurs within the context manager will be raised before restoring the terminal
+            state.
         """
         terminal = Terminal(self.input_data, self.terminal_config)
         try:
             terminal.prep_outputarea()
             yield terminal
         except:  # noqa: E722
             raise
         finally:
-            terminal.restore_cursor()
+            terminal.restore_cursor(end_symbol)
```

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/engine/motion.py` & `terminaltexteffects-0.9.3/terminaltexteffects/engine/motion.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/engine/terminal.py` & `terminaltexteffects-0.9.3/terminaltexteffects/engine/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,15 @@
                 self._height = self.detected_terminal_dimensions[1]
 
         self._next_character_id = 0
         self._input_characters = self._decompose_input(self.config.xterm_colors, self.config.no_color)
         self._added_characters: list[EffectCharacter] = []
         self._input_width = max([character.input_coord.column for character in self._input_characters])
         self._input_height = max([character.input_coord.row for character in self._input_characters])
-        self.output_area = OutputArea(min(max(self._height - 1, 1), self._input_height), self._input_width)
+        self.output_area = OutputArea(min(max(self._height, 1), self._input_height), self._input_width)
         self._input_characters = [
             character
             for character in self._input_characters
             if character.input_coord.row <= self.output_area.top
             and character.input_coord.column <= self.output_area.right
         ]
         self.character_by_input_coord: dict[Coord, EffectCharacter] = {
@@ -421,23 +421,14 @@
             row = character.motion.current_coord.row - 1
             column = character.motion.current_coord.column - 1
             if 0 <= row < self.output_area.top and 0 <= column < self.output_area.right:
                 rows[row][column] = character.symbol
         terminal_state = ["".join(row) for row in rows]
         self.terminal_state = terminal_state
 
-    def prep_outputarea(self) -> None:
-        """Prepares the terminal for the effect by adding empty lines and hiding the cursor."""
-        sys.stdout.write(ansitools.HIDE_CURSOR())
-        print("\n" * (self.output_area.top - 1))
-
-    def restore_cursor(self) -> None:
-        """Restores the cursor visibility."""
-        sys.stdout.write(ansitools.SHOW_CURSOR())
-
     def get_characters(
         self,
         *,
         input_characters: bool = True,
         fill_chars: bool = False,
         added_chars: bool = False,
         sort: CharacterSort = CharacterSort.TOP_TO_BOTTOM_LEFT_TO_RIGHT,
@@ -627,32 +618,54 @@
         Returns:
             str: The formatted output string.
         """
         self._update_terminal_state()
         output_string = "\n".join(self.terminal_state[::-1])
         return output_string
 
-    def print(self, output_string: str, *, enforce_frame_rate: bool = True):
+    def prep_outputarea(self) -> None:
+        """Prepares the terminal for the effect by adding empty lines and hiding the cursor."""
+        sys.stdout.write(ansitools.HIDE_CURSOR())
+        sys.stdout.write(("\n" * (self.output_area.top)))
+        sys.stdout.write(ansitools.DEC_SAVE_CURSOR_POSITION())
+
+    def restore_cursor(self, end_symbol: str = "\n") -> None:
+        """Restores the cursor visibility and prints the end_symbol.
+
+        Args:
+            end_symbol (str, optional): The symbol to print after the effect has completed. Defaults to newline.
+        """
+        sys.stdout.write(ansitools.SHOW_CURSOR())
+        sys.stdout.write(end_symbol)
+
+    def print(self, output_string: str, *, enforce_frame_rate: bool = True) -> None:
         """Prints the current terminal state to stdout while preserving the cursor position.
 
         Args:
             output_string (str): The string to be printed.
             enforce_frame_rate (bool, optional): Whether to enforce the frame rate set in the terminal config. Defaults to True.
 
         Notes:
             This method includes animation timing to control the frame rate.
             If the time since the last print is less than required to limit the frame rate, the method will sleep for the remaining time
             to ensure a consistent animation speed.
 
         """
         if enforce_frame_rate:
-            frame_delay = 1 / self._frame_rate
-            time_since_last_print = time.time() - self._last_time_printed
-            if time_since_last_print < frame_delay:
-                time.sleep(frame_delay - time_since_last_print)
-        sys.stdout.write(ansitools.DEC_SAVE_CURSOR_POSITION())
-        sys.stdout.write(ansitools.MOVE_CURSOR_UP(self.output_area.top))
-        sys.stdout.write(ansitools.MOVE_CURSOR_TO_COLUMN(1))
+            self.enforce_framerate()
+        self.move_cursor_to_top()
         sys.stdout.write(output_string)
-        sys.stdout.write(ansitools.DEC_RESTORE_CURSOR_POSITION())
         sys.stdout.flush()
+
+    def enforce_framerate(self):
+        """Enforces the frame rate set in the terminal config by sleeping if the time since
+        the last frame is shorter than the expected frame delay."""
+        frame_delay = 1 / self._frame_rate
+        time_since_last_print = time.time() - self._last_time_printed
+        if time_since_last_print < frame_delay:
+            time.sleep(frame_delay - time_since_last_print)
         self._last_time_printed = time.time()
+
+    def move_cursor_to_top(self):
+        """Restores the cursor position to the top of the output area."""
+        sys.stdout.write(ansitools.DEC_RESTORE_CURSOR_POSITION())
+        sys.stdout.write(ansitools.MOVE_CURSOR_UP(self.output_area.top))
```

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/template/effect_template.py` & `terminaltexteffects-0.9.3/terminaltexteffects/template/effect_template.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/ansitools.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/ansitools.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/argsdataclass.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/argsdataclass.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/argvalidators.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/argvalidators.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/colorterm.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/colorterm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/easing.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/easing.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/geometry.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/graphics.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/graphics.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/terminaltexteffects/utils/hexterm.py` & `terminaltexteffects-0.9.3/terminaltexteffects/utils/hexterm.py`

 * *Files identical despite different names*

### Comparing `terminaltexteffects-0.9.2/PKG-INFO` & `terminaltexteffects-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminaltexteffects
-Version: 0.9.2
+Version: 0.9.3
 Summary: A collection of visual effects that can be applied to terminal piped stdin text.
 License: MIT
 Author: Chris
 Author-email: 741258@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -256,54 +256,45 @@
 
 ## In-Development Preview
 
 Any effects shown below are in development and will be available in the next release.
 
 ## Latest Release Notes
 
-## 0.9.1
+## 0.9.3
 
 ---
 
-### New Features (0.9.1)
+### New Features (0.9.3)
 
 ---
 
-#### New Engine Features (0.9.1)
+#### New Engine Features (0.9.3)
 
-* Terminal dimension auto-detection supports automatically detecting a single dimensions.
+* Added argument to the `BaseEffect.terminal_output()` context manager. `end_symbol` (default `\n`) is used to specify
+the symbol that will be printed after the effect completes. Set to `''` or `' '` to enable animated prompts.
 
-### Changes (0.9.1)
+### Changes (0.9.3)
 
 ---
 
-#### Effects Changes (0.9.1)
+#### Engine Changes (0.9.3)
 
-* All effects have been updated to use the new `update()` method and `frame` property of
-  `base_effect.BaseEffectIterator`. See Engine Changes for more info.
+* Removed unnecessary write calls for cursor positioning on every frame.
+* Separated functionality related to cursor positioning and frame timing out of `Terminal.print()` and into
+`Terminal.enforce_framerate()`, `Terminal.prep_outputarea()` and `Terminal.move_cursor_to_top()`.
 
-#### Engine Changes (0.9.1)
+### Bug Fixes (0.9.3)
 
-* `base_effect.BaseEffectIterator` now has an `update()` method which calls the `tick()` method of all active characters
-  and manages the `active_characters` list.
-* `base_effect.BaseEffectIterator` has a `frame` property which calls `Terminal.get_formatted_output_string()` and
-  returns the string.
-* `TerminalConfig.terminal_dimensions` has been split into `TerminalConfig.terminal_width` and
-  `TerminalConfig.terminal_height` to simply the command line argument for dimensions and make it more obvious which
-  dimensions is being specified when interacting with `effect.terminal_config`.
-
-#### Other Changes (0.9.1)
+---
 
-* Updated help output for `--terminal-dimensions` argument.
+#### Engine Fixes (0.9.3)
 
-### Bug Fixes (0.9.1)
+* Fixed the output area of an effect being 1 row less than specified via the `Terminal.terminal_height` attribute. This
+  was caused by mixing use of `print()` and `sys.stdout.write()`.
 
 ---
 
-#### Engine Fixes (0.9.1)
-
-* Fixed division by zero error when the terminal height was set to 1.
-
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/main/LICENSE.md) for more information.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: terminaltexteffects Version: 0.9.2 Summary: A
+Metadata-Version: 2.1 Name: terminaltexteffects Version: 0.9.3 Summary: A
 collection of visual effects that can be applied to terminal piped stdin text.
 License: MIT Author: Chris Author-email: 741258@pm.me Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Description-Content-Type: text/markdown
                                      _[_T_T_E_]
@@ -139,25 +139,21 @@
 057338f4e007) #### Swarm ![swarm_demo](https://github.com/ChrisBuilds/
 terminaltexteffects/assets/57874186/305e8390-a0fb-4edb-a541-7b52cef77c09) ####
 VHSTape ![vhstape_demo](https://github.com/ChrisBuilds/terminaltexteffects/
 assets/57874186/720abbf4-f97d-4ce9-96ee-15ef973488d2) #### Waves ![waves_demo]
 (https://github.com/ChrisBuilds/terminaltexteffects/assets/57874186/ea9b04ca-
 e526-4c7e-b98d-a98a42f7137f) ## In-Development Preview Any effects shown below
 are in development and will be available in the next release. ## Latest Release
-Notes ## 0.9.1 --- ### New Features (0.9.1) --- #### New Engine Features
-(0.9.1) * Terminal dimension auto-detection supports automatically detecting a
-single dimensions. ### Changes (0.9.1) --- #### Effects Changes (0.9.1) * All
-effects have been updated to use the new `update()` method and `frame` property
-of `base_effect.BaseEffectIterator`. See Engine Changes for more info. ####
-Engine Changes (0.9.1) * `base_effect.BaseEffectIterator` now has an `update()`
-method which calls the `tick()` method of all active characters and manages the
-`active_characters` list. * `base_effect.BaseEffectIterator` has a `frame`
-property which calls `Terminal.get_formatted_output_string()` and returns the
-string. * `TerminalConfig.terminal_dimensions` has been split into
-`TerminalConfig.terminal_width` and `TerminalConfig.terminal_height` to simply
-the command line argument for dimensions and make it more obvious which
-dimensions is being specified when interacting with `effect.terminal_config`.
-#### Other Changes (0.9.1) * Updated help output for `--terminal-dimensions`
-argument. ### Bug Fixes (0.9.1) --- #### Engine Fixes (0.9.1) * Fixed division
-by zero error when the terminal height was set to 1. ## License Distributed
-under the MIT License. See [LICENSE](https://github.com/ChrisBuilds/
-terminaltexteffects/blob/main/LICENSE.md) for more information.
+Notes ## 0.9.3 --- ### New Features (0.9.3) --- #### New Engine Features
+(0.9.3) * Added argument to the `BaseEffect.terminal_output()` context manager.
+`end_symbol` (default `\n`) is used to specify the symbol that will be printed
+after the effect completes. Set to `''` or `' '` to enable animated prompts.
+### Changes (0.9.3) --- #### Engine Changes (0.9.3) * Removed unnecessary write
+calls for cursor positioning on every frame. * Separated functionality related
+to cursor positioning and frame timing out of `Terminal.print()` and into
+`Terminal.enforce_framerate()`, `Terminal.prep_outputarea()` and
+`Terminal.move_cursor_to_top()`. ### Bug Fixes (0.9.3) --- #### Engine Fixes
+(0.9.3) * Fixed the output area of an effect being 1 row less than specified
+via the `Terminal.terminal_height` attribute. This was caused by mixing use of
+`print()` and `sys.stdout.write()`. --- ## License Distributed under the MIT
+License. See [LICENSE](https://github.com/ChrisBuilds/terminaltexteffects/blob/
+main/LICENSE.md) for more information.
```


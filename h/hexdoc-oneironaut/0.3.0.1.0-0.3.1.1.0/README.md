# Comparing `tmp/hexdoc_oneironaut-0.3.0.1.0.tar.gz` & `tmp/hexdoc_oneironaut-0.3.1.1.0.tar.gz`

## Comparing `hexdoc_oneironaut-0.3.0.1.0.tar` & `hexdoc_oneironaut-0.3.1.1.0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/gradle.properties
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__version__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/__init__.py
--rw-r--r--   0        0        0    15700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.hexdoc.json
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0    43280 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json
--rw-r--r--   0        0        0    64897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/cell.json
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/hex_resistant_block.json
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_gel.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_ice.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/noosphere_basalt.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/pseudoamethyst_block.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker_glass.json
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_sensor.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_powered.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/super_budding.json
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/beacon_staff.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/cell.json
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/circle.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/echo_staff.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/endless_phial.json
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/hex_resistant_block.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/media_gel.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/media_ice.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/memory_fragment.json
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/noosphere_basalt.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_echo.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_flame.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_noosphere.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_block.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_shard.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker_glass.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_casting.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_filled.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_sensor.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_trap.json
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/super_budding.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/thought_slurry_bucket.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern_tinted.json
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/hex_resistant_block.png
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel.png
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel_energized.png
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_ice.png
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png
--rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png
--rw-r--r--   0        0        0   117562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/beacon_staff.png
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/memory_fragment.png
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/not_missing.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/book.json
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/basics/slipway_hint.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_main.json
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/mindrender.json
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/wisp_lantern.json
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science1.json
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science2.json
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science3.json
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise1.json
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise2.json
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise3.json
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise4.json
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/misc_patterns.json
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/soulprints.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/glow_ambit.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infusemedia.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/echo_staff.json
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/endless_phial.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/hex_resistant_block.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker.json
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker_glass.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/reverberation_rod.json
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_sensor.json
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_trap.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/super_budding.json
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern_tinted.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_templates/__init__.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/LICENSE
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/gradle.properties
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/__version__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/__init__.py
+-rw-r--r--   0        0        0    15700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.hexdoc.json
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0    43280 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json
+-rw-r--r--   0        0        0    64897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/cell.json
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/hex_resistant_block.json
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_gel.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_ice.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/noosphere_basalt.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/pseudoamethyst_block.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker_glass.json
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_sensor.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_powered.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/super_budding.json
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/beacon_staff.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/cell.json
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/circle.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/echo_staff.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/endless_phial.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/hex_resistant_block.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/media_gel.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/media_ice.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/memory_fragment.json
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/noosphere_basalt.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_echo.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_flame.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_noosphere.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_block.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_shard.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker_glass.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_casting.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_filled.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_sensor.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_trap.json
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/super_budding.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/thought_slurry_bucket.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern_tinted.json
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/hex_resistant_block.png
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel.png
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel_energized.png
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_ice.png
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png
+-rw-r--r--   0        0        0   117562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/beacon_staff.png
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/memory_fragment.png
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png
+-rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/not_missing.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/book.json
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/basics/slipway_hint.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_main.json
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/mindrender.json
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/wisp_lantern.json
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science1.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science2.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science3.json
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise1.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise2.json
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise3.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise4.json
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/misc_patterns.json
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/soulprints.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/glow_ambit.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infusemedia.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/echo_staff.json
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/endless_phial.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/hex_resistant_block.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker_glass.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/reverberation_rod.json
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_sensor.json
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_trap.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/super_budding.json
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern_tinted.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_templates/__init__.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/LICENSE
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/doc/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.1.1.0/PKG-INFO
```

### Comparing `hexdoc_oneironaut-0.3.0.1.0/gradle.properties` & `hexdoc_oneironaut-0.3.1.1.0/gradle.properties`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 kotlin.stdlib.default.dependency=false
 
 # needed for mixins to work for forge
 asmVersion=9.4
 
 # mod info
 modID=oneironaut
-modVersion=0.3.0
+modVersion=0.3.1
 mavenGroup=net.oneironaut
 
 # publishing
 curseforgeId=
 modrinthId=
 
 # core
 minecraftVersion=1.19.2
 yarnMappingsVersion=1.19.2+build.28:v2
 enabledPlatforms=fabric,forge
-fabricLoaderVersion=0.15.0
+fabricLoaderVersion=0.15.11
 fabricApiVersion=0.77.0+1.19.2
 fabricKotlinVersion=1.9.0+kotlin.1.8.0
 forgeVersion=1.19.2-43.2.11
 forgeKotlinVersion=3.12.0
 architecturyVersion=6.5.85
 mixinExtrasVersion=0.2.0-beta.9
```

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # This file is auto-generated by hatch-gradle-version. Do not edit.
 
-GRADLE_VERSION = "0.3.0"
-FULL_VERSION = "0.3.0.1.0"
+GRADLE_VERSION = "0.3.1"
+FULL_VERSION = "0.3.1.1.0"
 
 ARCHITECTURY_VERSION = "6.5.85"
 ASM_VERSION = "9.4"
 CARDINAL_COMPONENTS_VERSION = "5.0.2"
 CCA_VERSION = "5.0.2"
 CURSEFORGE_ID = ""
 ENABLED_PLATFORMS = "fabric,forge"
 ENTITY_REACH_VERSION = "2.3.0"
 FABRIC_API_VERSION = "0.77.0+1.19.2"
 FABRIC_KOTLIN_VERSION = "1.9.0+kotlin.1.8.0"
-FABRIC_LOADER_VERSION = "0.15.0"
+FABRIC_LOADER_VERSION = "0.15.11"
 FORGE_KOTLIN_VERSION = "3.12.0"
 FORGE_VERSION = "1.19.2-43.2.11"
 GECKOLIB_VERSION = "3.1.40"
 GLOOP_VERSION = "0.2.0"
 HEXAL_VERSION = "0.2.18"
 HEXCASTING_VERSION = "0.10.3"
 JETBRAINS_ANNOTATIONS_VERSION = "23.0.0"
 KOTLIN_STDLIB_DEFAULT_DEPENDENCY = "false"
 MAVEN_GROUP = "net.oneironaut"
 MINECRAFT_VERSION = "1.19.2"
 MIXIN_EXTRAS_VERSION = "0.2.0-beta.9"
 MOD_I_D = "oneironaut"
-MOD_VERSION = "0.3.0"
+MOD_VERSION = "0.3.1"
 MODRINTH_ID = ""
 ORG_GRADLE_JVMARGS = "-Xmx2048M"
 PATCHOULI_VERSION = "77"
 PAUCAL_VERSION = "0.5.0"
 SERIALIZATION_HOOKS_VERSION = "0.3.24"
 TRINKETS_VERSION = "3.4.1"
 WNBOI_VERSION = "0.0.4"
```

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_hooks.py` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/cell.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/cell.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_gel.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_gel.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_sensor.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_sensor.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_powered.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_powered.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/hex_resistant_block.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/hex_resistant_block.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel_energized.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel_energized.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_ice.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_ice.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/beacon_staff.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/beacon_staff.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/memory_fragment.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/memory_fragment.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/not_missing.png` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/not_missing.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise1.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise1.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise3.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise3.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/misc_patterns.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/misc_patterns.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/soulprints.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/soulprints.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/glow_ambit.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/glow_ambit.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infusemedia.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infusemedia.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json` & `hexdoc_oneironaut-0.3.1.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/.gitignore` & `hexdoc_oneironaut-0.3.1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/LICENSE` & `hexdoc_oneironaut-0.3.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/pyproject.toml` & `hexdoc_oneironaut-0.3.1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/doc/README.md` & `hexdoc_oneironaut-0.3.1.1.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.3.0.1.0/PKG-INFO` & `hexdoc_oneironaut-0.3.1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hexdoc-oneironaut
-Version: 0.3.0.1.0
+Version: 0.3.1.1.0
 Summary: Python web book docgen and hexdoc plugin for Oneironaut.
 Project-URL: Homepage, https://beholderface.github.io/oneironaut
 Project-URL: Source, https://github.com/beholderface/oneironaut
 Author: beholderface
 License-File: LICENSE
 Keywords: hexdoc
 Requires-Python: >=3.11
```


# Comparing `tmp/open_samus_returns_rando-1.3.2.tar.gz` & `tmp/open_samus_returns_rando-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_samus_returns_rando-1.3.2.tar", last modified: Wed May 22 17:06:56 2024, max compression
+gzip compressed data, was "open_samus_returns_rando-1.3.3.tar", last modified: Sat May 25 14:14:37 2024, max compression
```

## Comparing `open_samus_returns_rando-1.3.2.tar` & `open_samus_returns_rando-1.3.3.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.877788 open_samus_returns_rando-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.849788 open_samus_returns_rando-1.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.849788 open_samus_returns_rando-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 17:06:56.873788 open_samus_returns_rando-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:06:56.877788 open_samus_returns_rando-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.849788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.853788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.853788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.853788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/doors.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/heatzone.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/savestation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/scenario.lua
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/ship.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/sprites_texturehud.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.857787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s000_surface.lua
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s010_area1.lua
--rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s020_area2.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s025_area2b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s028_area2c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s030_area3.lua
--rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s033_area3b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s036_area3c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s040_area4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s050_area5.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s060_area6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s065_area6b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s067_area6c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    42108 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s070_area7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s090_area9.lua
--rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s100_area10.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/
--rw-r--r--   0 runner    (1001) docker     (127)    23772 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/item_offworld.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/missile_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.841787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/doorshieldbeamburst.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/doorshieldbeamburst_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.861788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/doorshieldbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/doorshieldbomb_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/doorshieldgrapplebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/doorgrapple_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/
--rw-r--r--   0 runner    (1001) docker     (127)    50240 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/doorshieldicebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/doorcreature_i.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/spiderweb_i.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/
--rw-r--r--   0 runner    (1001) docker     (127)    47188 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/doorshieldlocked.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/doorshieldlocked_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.865788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/gui/textures/
--rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
--rw-r--r--   0 runner    (1001) docker     (127)   524555 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/gui/textures/texturehud.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.845787 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.869788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/maps/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/maps/textures/chozoartifactor_o.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.869788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/cosmetics.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/elevators.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/metroid_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/lua_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.869788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/elevators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/spawn_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.869788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/custom_pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/samus_returns_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.873788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    27356 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/door_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/hint_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/metroid_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    12343 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/static_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/tunable_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.873788 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 17:06:56.000000 open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.873788 open_samus_returns_rando-1.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:06:56.873788 open_samus_returns_rando-1.3.2/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    51547 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/tests/test_files/item_models_test.json
--rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-22 17:06:44.000000 open_samus_returns_rando-1.3.2/tests/test_lua_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.459619 open_samus_returns_rando-1.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-25 14:14:37.459619 open_samus_returns_rando-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:14:37.459619 open_samus_returns_rando-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.423619 open_samus_returns_rando-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.435619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.435619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.435619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.439619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/doors.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/heatzone.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/savestation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/scenario.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/ship.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/sprites_texturehud.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.443619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s000_surface.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s010_area1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s020_area2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s025_area2b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s028_area2c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s030_area3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s033_area3b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s036_area3c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s040_area4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s050_area5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s060_area6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s065_area6b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s067_area6c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    42108 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s070_area7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s090_area9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s100_area10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    23772 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/item_offworld.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/missile_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/doorshieldbeamburst.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/doorshieldbeamburst_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/doorshieldbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/doorshieldbomb_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/doorshieldgrapplebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/doorgrapple_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.427619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    50240 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/doorshieldicebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/doorcreature_i.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/spiderweb_i.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.447620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    47188 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/doorshieldlocked.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.451619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/doorshieldlocked_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.451619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/gui/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)   524555 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/gui/textures/texturehud.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.431620 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.451619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/maps/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/maps/textures/chozoartifactor_o.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.455619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/cosmetics.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/elevators.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/metroid_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/lua_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.455619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/elevators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/spawn_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.455619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/custom_pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14546 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/samus_returns_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.455619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27356 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/door_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/hint_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/metroid_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/static_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/tunable_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.459619 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 14:14:37.000000 open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.455619 open_samus_returns_rando-1.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:14:37.459619 open_samus_returns_rando-1.3.3/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    51547 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/tests/test_files/item_models_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-25 14:14:29.000000 open_samus_returns_rando-1.3.3/tests/test_lua_util.py
```

### Comparing `open_samus_returns_rando-1.3.2/.github/dependabot.yml` & `open_samus_returns_rando-1.3.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/.github/workflows/python.yml` & `open_samus_returns_rando-1.3.3/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/.gitignore` & `open_samus_returns_rando-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/LICENSE` & `open_samus_returns_rando-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/PKG-INFO` & `open_samus_returns_rando-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.3.2
+Version: 1.3.3
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `open_samus_returns_rando-1.3.2/README.md` & `open_samus_returns_rando-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/pyproject.toml` & `open_samus_returns_rando-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/cli.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/constants.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/constants.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/debug.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/debug.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/doors.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/doors.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/guilib.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/guilib.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/heatzone.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/heatzone.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/room_names.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/room_names.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/savestation.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/savestation.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/scenario.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/scenario.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/ship.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/ship.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/sprites_splashes.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/sprites_splashes.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/custom/sprites_texturehud.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/custom/sprites_texturehud.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s000_surface.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s000_surface.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s010_area1.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s010_area1.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s020_area2.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s020_area2.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s025_area2b.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s025_area2b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s028_area2c.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s028_area2c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s030_area3.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s030_area3.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s033_area3b.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s033_area3b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s036_area3c.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s036_area3c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s040_area4.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s040_area4.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s050_area5.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s050_area5.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s060_area6.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s060_area6.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s065_area6b.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s065_area6b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s067_area6c.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s067_area6c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s070_area7.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s070_area7.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s090_area9.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s090_area9.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s100_area10.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s100_area10.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizersuit.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizersuit.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/item_offworld.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/item_offworld/models/item_offworld.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/powerup_icemissile.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/missile_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_icemissile/models/textures/missile_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/doorshieldbeamburst.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/doorshieldbeamburst.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/doorshieldbeamburst_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbeamburst/models/textures/doorshieldbeamburst_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/doorshieldbomb.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/doorshieldbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/doorshieldbomb_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldbomb/models/textures/doorshieldbomb_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/doorshieldgrapplebeam.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/doorshieldgrapplebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/doorgrapple_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldgrapplebeam/models/textures/doorgrapple_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/doorshieldicebeam.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/doorshieldicebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/doorcreature_i.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/doorcreature_i.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/spiderweb_i.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldicebeam/models/textures/spiderweb_i.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/doorshieldlocked.bcmdl` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/doorshieldlocked.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/doorshieldlocked_d.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/actors/props/doorshieldlocked/models/textures/doorshieldlocked_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/gui/textures/texturehud.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/gui/textures/texturehud.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/romfs/maps/textures/chozoartifactor_o.bctex` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/romfs/maps/textures/chozoartifactor_o.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/schema.json` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/schema.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/chozoseal_template.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/chozoseal_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/cosmetics.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/cosmetics.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/custom_init.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/metroid_template.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/metroid_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/lua_editor.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/lua_editor.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/collision_camera_table.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/collision_camera_table.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/credits.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/credits.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/elevators.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/elevators.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/lua_util.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/lua_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/spawn_points.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/spawn_points.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/misc_patches/text_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/misc_patches/text_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/patch_util.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/patcher_editor.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/custom_pickups.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/custom_pickups.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/model_data.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/model_data.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/pickups/pickup.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/pickups/pickup.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/samus_returns_patcher.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/samus_returns_patcher.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/door_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/door_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/game_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/game_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/heat_room_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/heat_room_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/map_icons.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/map_icons.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/metroid_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/metroid_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/static_fixes.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/static_fixes.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,18 +278,22 @@
             new_block["name1"] = sg_casca
             types: ListContainer = typing.cast(ListContainer, new_group["types"])
             types[0]["blocks"].append(new_block)
             bmsbk.raw.block_groups.append(new_group)
             bmsbk_cc_obj = next(cc_obj for cc_obj in bmsbk.raw.collision_cameras if cc_name in cc_obj.name)
             bmsbk_cc_obj.entries.append(len(bmsbk.raw.block_groups) - 1)
 
+def patch_area7_item(editor: PatcherEditor) -> None:
+    area7 = editor.get_scenario("s090_area9")
+    area7.add_actor_to_entity_groups("PostOmega_003", "LE_Item_009")
 
 def apply_static_fixes(editor: PatcherEditor) -> None:
     patch_multi_room_gammas(editor)
     patch_pickup_rotation(editor)
     patch_pickup_position(editor)
     remove_area7_grapple_block(editor)
     patch_a7_save_screw_blocks(editor)
     shoot_supers_without_missiles(editor)
     nerf_ridley_fight(editor)
     increase_pb_drop_chance(editor)
     fix_wrong_cc_actor_deletions(editor)
+    patch_area7_item(editor)
```

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/specific_patches/tunable_patches.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/specific_patches/tunable_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando/validator_with_default.py` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/PKG-INFO` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.3.2
+Version: 1.3.3
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `open_samus_returns_rando-1.3.2/src/open_samus_returns_rando.egg-info/SOURCES.txt` & `open_samus_returns_rando-1.3.3/src/open_samus_returns_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/tests/test_files/item_models_test.json` & `open_samus_returns_rando-1.3.3/tests/test_files/item_models_test.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.3.2/tests/test_files/starter_preset_patcher.json` & `open_samus_returns_rando-1.3.3/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*


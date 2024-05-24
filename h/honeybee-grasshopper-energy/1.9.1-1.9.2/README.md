# Comparing `tmp/honeybee-grasshopper-energy-1.9.1.tar.gz` & `tmp/honeybee-grasshopper-energy-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-grasshopper-energy-1.9.1.tar", last modified: Sat Jul 18 04:48:08 2020, max compression
+gzip compressed data, was "dist/honeybee-grasshopper-energy-1.9.2.tar", last modified: Sat Jul 18 17:44:42 2020, max compression
```

## Comparing `honeybee-grasshopper-energy-1.9.1.tar` & `honeybee-grasshopper-energy-1.9.2.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2695 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1838 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/deploy.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      332 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/dev-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4653 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Adiabatic by Type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply ConstructionSet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Load Values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4558 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Opaque Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply ProgramType.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9727 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Room Schedules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4893 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Setpoint Values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4526 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Shade Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4594 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Shade Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5405 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Window Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2476 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Blend ProgramTypes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4915 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Blind Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5735 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Color Faces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5730 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Color Rooms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3986 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Constant Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6469 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB ConstructionSet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2917 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Custom Simulation Output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Custom Window Gap Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4748 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2677 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet Interior.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3814 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2749 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Equipment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2195 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Infiltration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2366 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Lighting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2121 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct People.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2900 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct ProgramType.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4295 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2550 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Setpoint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3287 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Ventilation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3748 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Equipment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2503 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Exterior Construction Subset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4607 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Fixed Interval Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3521 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Gene Pool to Day Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Glass Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Ground Construction Subset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5274 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB IdealAir.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2964 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Infiltration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5533 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Interior Construction Subset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3460 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Lighting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8130 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Load Measure.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7820 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Model to IDF.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10663 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Model to OSM.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Opaque Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Opaque Material No Mass.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3132 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Opaque Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3028 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB People.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4589 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB ProgramType.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2539 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Custom Result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5133 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Face Result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5581 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read HVAC Sizing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1848 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Result Dictionary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3637 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Room Comfort Result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11289 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Room Energy Result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1672 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Zone Sizing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3676 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Run IDF.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5153 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Run OSM.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5072 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Run OSW.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4681 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Schedule to Data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3658 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Construction Sets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Constructions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2487 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Materials.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Programs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2334 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Schedules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5519 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Seasonal Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3454 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Setpoint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2560 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Shade Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4309 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Shade Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6699 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Shadow Calculation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2314 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Simulation Control.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3918 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Simulation Output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5984 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Simulation Parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2685 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Sizing Parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4503 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Subface Subset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5915 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Thermal Load Balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Type Limit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4514 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Ventilation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7517 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Weekly Schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6485 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Construction Shade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2675 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Construction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3026 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Gap Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2622 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3929 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Adiabatic by Type.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4289 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply ConstructionSet.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5890 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Load Values.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5043 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Opaque Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply ProgramType.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6825 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Room Schedules.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4655 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Setpoint Values.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4603 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Shade Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5643 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Shade Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5231 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Window Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4543 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Blend ProgramTypes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4206 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Blind Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2858 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Building Programs.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2540 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Building Vintages.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2551 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Climate Zones.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6979 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Color Faces.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6408 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Color Rooms.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5383 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Constant Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2563 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Construction Types.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5923 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB ConstructionSet.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4744 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Custom Simulation Output.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Custom Window Gap Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4975 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4207 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet Interior.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5268 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5000 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Equipment.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4455 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Infiltration.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4069 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Lighting.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4212 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct People.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct ProgramType.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5170 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4078 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Setpoint.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Ventilation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Equipment.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5228 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Exterior Construction Subset.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Face Energy Attributes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5867 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Fixed Interval Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4597 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Gene Pool to Day Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4042 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Glass Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4840 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Ground Construction Subset.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5666 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB IdealAir.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4951 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Infiltration.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4817 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Interior Construction Subset.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4220 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Lighting.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Load Measure.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Model to IDF.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     9160 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Model to OSM.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4454 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Opaque Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3693 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Opaque Material No Mass.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3881 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Opaque Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4355 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB People.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5411 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB ProgramType.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4394 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Custom Result.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5587 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Face Result.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6498 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read HVAC Sizing.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5283 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Result Dictionary.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5039 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Room Comfort Result.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     7583 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Room Energy Result.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4175 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Zone Sizing.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Room Energy Attributes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5027 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Run IDF.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6106 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Run OSM.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5872 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Run OSW.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5611 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Schedule to Data.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5157 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Construction Sets.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4775 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Constructions.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4473 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Materials.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5287 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Programs.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4006 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Schedules.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5886 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Seasonal Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4201 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Setpoint.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3649 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Shade Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3881 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Shade Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5933 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Shadow Calculation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4382 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Simulation Control.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5691 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Simulation Output.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6214 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Simulation Parameter.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5006 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Sizing Parameter.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4709 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Subface Subset.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6295 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Thermal Load Balance.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4354 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Type Limit.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5840 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Ventilation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6626 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Weekly Schedule.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Construction Shade.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4278 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Construction.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3522 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Gap Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3386 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Material.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2695 2020-07-18 04:48:07.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11527 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-18 04:48:07.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-07-18 04:48:07.000000 honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/pass_tests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/samples/
--rw-rw-r--   0 travis    (2000) travis    (2000)    71405 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/samples/creating_constructions.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)    60573 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/samples/creating_programs.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)    49060 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/samples/creating_schedules.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)   426010 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/samples/full_building_energy_model.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)    58457 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/samples/shoe_box_energy_model.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)   142466 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/samples/single_family_energy_model.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-07-18 04:48:08.000000 honeybee-grasshopper-energy-1.9.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      886 2020-07-18 04:47:24.000000 honeybee-grasshopper-energy-1.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2695 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1838 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/deploy.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      332 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/dev-requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4701 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Adiabatic by Type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply ConstructionSet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Load Values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4558 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Opaque Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply ProgramType.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9727 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Room Schedules.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4893 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Setpoint Values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4526 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Shade Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4594 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Shade Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5405 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Window Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2476 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Blend ProgramTypes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4915 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Blind Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5735 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Color Faces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5730 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Color Rooms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3986 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Constant Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6469 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB ConstructionSet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2917 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Custom Simulation Output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Custom Window Gap Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4748 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2677 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet Interior.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3814 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2749 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Equipment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2195 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Infiltration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2366 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Lighting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2121 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct People.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2900 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct ProgramType.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4295 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2550 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Setpoint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3287 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Ventilation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3748 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Equipment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2503 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Exterior Construction Subset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4607 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Fixed Interval Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3521 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Gene Pool to Day Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Glass Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2474 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Ground Construction Subset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5274 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB IdealAir.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2964 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Infiltration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5533 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Interior Construction Subset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3460 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Lighting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8130 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Load Measure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7820 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Model to IDF.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10663 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Model to OSM.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Opaque Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Opaque Material No Mass.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3132 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Opaque Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3028 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB People.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4589 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB ProgramType.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2539 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Custom Result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5133 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Face Result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5581 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read HVAC Sizing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1848 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Result Dictionary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3637 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Room Comfort Result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11289 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Room Energy Result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1672 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Zone Sizing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3676 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Run IDF.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5153 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Run OSM.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5072 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Run OSW.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4681 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Schedule to Data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3658 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Construction Sets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Constructions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2487 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Materials.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Programs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2334 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Schedules.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5519 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Seasonal Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3454 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Setpoint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2560 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Shade Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4309 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Shade Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6699 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Shadow Calculation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2314 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Simulation Control.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3918 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Simulation Output.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5984 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Simulation Parameter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2685 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Sizing Parameter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4503 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Subface Subset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5915 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Thermal Load Balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Type Limit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4514 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Ventilation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7517 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Weekly Schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6485 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Construction Shade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2675 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Construction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3026 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Gap Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2622 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4017 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Adiabatic by Type.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4289 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply ConstructionSet.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5890 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Load Values.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5043 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Opaque Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply ProgramType.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6825 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Room Schedules.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4655 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Setpoint Values.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4603 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Shade Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5643 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Shade Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5231 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Window Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4543 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Blend ProgramTypes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4206 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Blind Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2858 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Building Programs.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2540 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Building Vintages.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2551 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Climate Zones.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6979 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Color Faces.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6408 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Color Rooms.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5383 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Constant Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2563 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Construction Types.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5923 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB ConstructionSet.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4744 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Custom Simulation Output.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Custom Window Gap Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4975 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4207 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet Interior.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5268 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5000 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Equipment.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4455 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Infiltration.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4069 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Lighting.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4212 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct People.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct ProgramType.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5170 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4078 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Setpoint.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Ventilation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Equipment.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5228 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Exterior Construction Subset.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Face Energy Attributes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5867 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Fixed Interval Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4597 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Gene Pool to Day Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4042 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Glass Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4840 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Ground Construction Subset.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5666 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB IdealAir.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4951 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Infiltration.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4817 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Interior Construction Subset.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4220 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Lighting.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Load Measure.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6654 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Model to IDF.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9160 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Model to OSM.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4454 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Opaque Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3693 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Opaque Material No Mass.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3881 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Opaque Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4355 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB People.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5411 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB ProgramType.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4394 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Custom Result.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5587 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Face Result.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6498 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read HVAC Sizing.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5283 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Result Dictionary.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5039 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Room Comfort Result.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7583 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Room Energy Result.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4175 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Zone Sizing.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Room Energy Attributes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5027 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Run IDF.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6106 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Run OSM.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5872 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Run OSW.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5611 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Schedule to Data.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5157 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Construction Sets.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4775 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Constructions.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4473 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Materials.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5287 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Programs.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4006 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Schedules.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5886 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Seasonal Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4201 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Setpoint.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3649 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Shade Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3881 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Shade Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5933 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Shadow Calculation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4382 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Simulation Control.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5691 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Simulation Output.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6214 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Simulation Parameter.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5006 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Sizing Parameter.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4709 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Subface Subset.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6295 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Thermal Load Balance.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4354 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Type Limit.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5840 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Ventilation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6626 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Weekly Schedule.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5449 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Construction Shade.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4278 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Construction.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3522 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Gap Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3386 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Material.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2695 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11527 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/pass_tests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/samples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71405 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/samples/creating_constructions.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60573 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/samples/creating_programs.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49060 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/samples/creating_schedules.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)   426010 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/samples/full_building_energy_model.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58457 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/samples/shoe_box_energy_model.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)   142466 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/samples/single_family_energy_model.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-07-18 17:44:42.000000 honeybee-grasshopper-energy-1.9.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      886 2020-07-18 17:44:00.000000 honeybee-grasshopper-energy-1.9.2/setup.py
```

### Comparing `honeybee-grasshopper-energy-1.9.1/.travis.yml` & `honeybee-grasshopper-energy-1.9.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/LICENSE` & `honeybee-grasshopper-energy-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/PKG-INFO` & `honeybee-grasshopper-energy-1.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-grasshopper-energy
-Version: 1.9.1
+Version: 1.9.2
 Summary: Honeybee Energy plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/honeybee-grasshopper-energy
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-energy.svg?branch=master)](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-energy)
```

### Comparing `honeybee-grasshopper-energy-1.9.1/README.md` & `honeybee-grasshopper-energy-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Adiabatic by Type.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Adiabatic by Type.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     
     Returns:
         hb_objs: The input honeybee objects with their boundary conditions edited.
 """
 
 ghenv.Component.Name = "HB Adiabatic by Type"
 ghenv.Component.NickName = 'AdiabaticByType'
-ghenv.Component.Message = '0.1.0'
+ghenv.Component.Message = '0.1.1'
 ghenv.Component.Category = 'HB-Energy'
 ghenv.Component.SubCategory = '0 :: Basic Properties'
 ghenv.Component.AdditionalHelpFromDocStrings = "5"
 
 
 try:  # import the core honeybee dependencies
-    from honeybee.boundarycondition import Outdoors, Surface, boundary_conditions
+    from honeybee.boundarycondition import Outdoors, Ground, Surface, boundary_conditions
     from honeybee.facetype import Wall, RoofCeiling, Floor
     from honeybee.room import Room
     from honeybee.face import Face
     from honeybee.orientation import angles_from_num_orient, face_orient_index
 except ImportError as e:
     raise ImportError('\nFailed to import honeybee:\n\t{}'.format(e))
 
@@ -61,19 +61,19 @@
         isinstance(face.type, face_type)
 
 
 def check_and_assign_adiabatic_to_face(face):
     """Check if a face if of a relevant type and assign Adiabatic if so."""
     
     # assign the adiabatic property to roofs
-    if roofs_ and check_type(face, Outdoors, RoofCeiling):
+    if roofs_ and check_type(face, (Outdoors, Ground), RoofCeiling):
         face.boundary_condition = boundary_conditions.adiabatic
     
     # assign the adiabatic property to exposed floors
-    if exposed_floors_ and check_type(face, Outdoors, Floor):
+    if exposed_floors_ and check_type(face, (Outdoors, Ground), Floor):
         face.boundary_condition = boundary_conditions.adiabatic
     
     # assign the adiabatic property to exposed floors
     if interior_walls_ and check_type(face, Surface, Wall):
         face.boundary_condition = boundary_conditions.adiabatic
     
     # assign the adiabatic property to exposed floors
@@ -87,20 +87,20 @@
     
     # assign the adiabatic property to the walls
     if len(exterior_walls_) > 0:
         angles = angles_from_num_orient(len(exterior_walls_))
         for obj in hb_objs:
             if isinstance(obj, Room):
                 for face in obj.faces:
-                    if check_type(face, Outdoors, Wall):
+                    if check_type(face, (Outdoors, Ground), Wall):
                         orient_i = face_orient_index(face, angles)
                         if orient_i is not None and exterior_walls_[orient_i]:
                             face.boundary_condition = boundary_conditions.adiabatic
             else:  # assume it is a Face
-                if check_type(obj, Outdoors, Wall):
+                if check_type(obj, (Outdoors, Ground), Wall):
                     orient_i = face_orient_index(obj, angles)
                     if orient_i is not None and exterior_walls_[orient_i]:
                         obj.boundary_condition = boundary_conditions.adiabatic
     
     # assign the adiabatic property to all of the other face types
     for obj in hb_objs:
         if isinstance(obj, Room):
```

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply ConstructionSet.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply ConstructionSet.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Load Values.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Load Values.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Opaque Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Opaque Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply ProgramType.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply ProgramType.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Room Schedules.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Room Schedules.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Setpoint Values.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Setpoint Values.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Shade Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Shade Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Shade Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Shade Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Apply Window Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Apply Window Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Blend ProgramTypes.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Blend ProgramTypes.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Blind Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Blind Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Color Faces.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Color Faces.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Color Rooms.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Color Rooms.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Constant Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Constant Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB ConstructionSet.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB ConstructionSet.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Custom Simulation Output.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Custom Simulation Output.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Custom Window Gap Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Custom Window Gap Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet Interior.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet Interior.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct ConstructionSet.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Equipment.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Equipment.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Infiltration.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Infiltration.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Lighting.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Lighting.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct People.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct People.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct ProgramType.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct ProgramType.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Setpoint.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Setpoint.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Deconstruct Ventilation.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Deconstruct Ventilation.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Equipment.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Equipment.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Exterior Construction Subset.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Exterior Construction Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Fixed Interval Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Fixed Interval Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Gene Pool to Day Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Gene Pool to Day Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Glass Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Glass Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Ground Construction Subset.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Ground Construction Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB IdealAir.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB IdealAir.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Infiltration.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Infiltration.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Interior Construction Subset.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Interior Construction Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Lighting.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Lighting.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Load Measure.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Load Measure.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Model to IDF.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Model to IDF.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Model to OSM.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Model to OSM.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Opaque Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Opaque Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Opaque Material No Mass.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Opaque Material No Mass.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Opaque Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Opaque Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB People.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB People.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB ProgramType.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB ProgramType.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Custom Result.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Custom Result.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Face Result.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Face Result.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read HVAC Sizing.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read HVAC Sizing.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Result Dictionary.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Result Dictionary.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Room Comfort Result.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Room Comfort Result.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Room Energy Result.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Room Energy Result.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Read Zone Sizing.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Read Zone Sizing.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Run IDF.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Run IDF.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Run OSM.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Run OSM.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Run OSW.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Run OSW.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Schedule to Data.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Schedule to Data.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Construction Sets.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Construction Sets.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Constructions.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Materials.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Programs.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Programs.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Search Schedules.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Search Schedules.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Seasonal Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Seasonal Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Setpoint.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Setpoint.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Shade Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Shade Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Shade Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Shade Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Shadow Calculation.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Shadow Calculation.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Simulation Control.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Simulation Control.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Simulation Output.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Simulation Output.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Simulation Parameter.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Simulation Parameter.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Sizing Parameter.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Sizing Parameter.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Subface Subset.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Subface Subset.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Thermal Load Balance.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Thermal Load Balance.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Type Limit.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Type Limit.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Ventilation.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Ventilation.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Weekly Schedule.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Weekly Schedule.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Construction Shade.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Construction Shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Construction.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Construction.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Gap Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Gap Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/src/HB Window Material.py` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/src/HB Window Material.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply ConstructionSet.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply ConstructionSet.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Load Values.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Load Values.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Opaque Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Opaque Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply ProgramType.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply ProgramType.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Room Schedules.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Room Schedules.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Setpoint Values.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Setpoint Values.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Shade Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Shade Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Shade Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Shade Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Apply Window Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Apply Window Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Blend ProgramTypes.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Blend ProgramTypes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Blind Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Blind Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Building Programs.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Building Programs.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Building Vintages.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Building Vintages.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Climate Zones.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Climate Zones.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Color Faces.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Color Faces.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Color Rooms.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Color Rooms.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Constant Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Constant Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Construction Types.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Construction Types.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB ConstructionSet.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB ConstructionSet.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Custom Simulation Output.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Custom Simulation Output.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Custom Window Gap Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Custom Window Gap Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet Interior.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet Interior.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct ConstructionSet.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Equipment.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Equipment.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Infiltration.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Infiltration.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Lighting.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Lighting.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct People.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct People.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct ProgramType.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct ProgramType.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Setpoint.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Setpoint.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Deconstruct Ventilation.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Deconstruct Ventilation.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Equipment.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Equipment.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Exterior Construction Subset.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Exterior Construction Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Face Energy Attributes.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Face Energy Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Fixed Interval Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Fixed Interval Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Gene Pool to Day Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Gene Pool to Day Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Glass Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Glass Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Ground Construction Subset.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Ground Construction Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB IdealAir.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB IdealAir.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Infiltration.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Infiltration.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Interior Construction Subset.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Interior Construction Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Lighting.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Lighting.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Load Measure.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Load Measure.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Model to IDF.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Model to IDF.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Model to OSM.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Model to OSM.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Opaque Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Opaque Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Opaque Material No Mass.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Opaque Material No Mass.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Opaque Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Opaque Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB People.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB People.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB ProgramType.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB ProgramType.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Custom Result.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Custom Result.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Face Result.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Face Result.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read HVAC Sizing.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read HVAC Sizing.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Result Dictionary.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Result Dictionary.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Room Comfort Result.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Room Comfort Result.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Room Energy Result.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Room Energy Result.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Read Zone Sizing.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Read Zone Sizing.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Room Energy Attributes.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Room Energy Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Run IDF.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Run IDF.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Run OSM.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Run OSM.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Run OSW.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Run OSW.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Schedule to Data.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Schedule to Data.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Construction Sets.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Construction Sets.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Constructions.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Constructions.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Materials.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Materials.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Programs.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Programs.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Search Schedules.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Search Schedules.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Seasonal Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Seasonal Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Setpoint.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Setpoint.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Shade Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Shade Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Shade Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Shade Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Shadow Calculation.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Shadow Calculation.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Simulation Control.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Simulation Control.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Simulation Output.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Simulation Output.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Simulation Parameter.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Simulation Parameter.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Sizing Parameter.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Sizing Parameter.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Subface Subset.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Subface Subset.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Thermal Load Balance.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Thermal Load Balance.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Type Limit.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Type Limit.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Ventilation.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Ventilation.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Weekly Schedule.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Weekly Schedule.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Construction Shade.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Construction Shade.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Construction.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Construction.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Gap Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Gap Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy/user_objects/HB Window Material.ghuser` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy/user_objects/HB Window Material.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/PKG-INFO` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-grasshopper-energy
-Version: 1.9.1
+Version: 1.9.2
 Summary: Honeybee Energy plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/honeybee-grasshopper-energy
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-energy.svg?branch=master)](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-energy)
```

### Comparing `honeybee-grasshopper-energy-1.9.1/honeybee_grasshopper_energy.egg-info/SOURCES.txt` & `honeybee-grasshopper-energy-1.9.2/honeybee_grasshopper_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/samples/creating_constructions.gh` & `honeybee-grasshopper-energy-1.9.2/samples/creating_constructions.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/samples/creating_programs.gh` & `honeybee-grasshopper-energy-1.9.2/samples/creating_programs.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/samples/creating_schedules.gh` & `honeybee-grasshopper-energy-1.9.2/samples/creating_schedules.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/samples/full_building_energy_model.gh` & `honeybee-grasshopper-energy-1.9.2/samples/full_building_energy_model.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/samples/shoe_box_energy_model.gh` & `honeybee-grasshopper-energy-1.9.2/samples/shoe_box_energy_model.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/samples/single_family_energy_model.gh` & `honeybee-grasshopper-energy-1.9.2/samples/single_family_energy_model.gh`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-energy-1.9.1/setup.py` & `honeybee-grasshopper-energy-1.9.2/setup.py`

 * *Files identical despite different names*


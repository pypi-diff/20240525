# Comparing `tmp/tt_damage_calculator-4.2.0.tar.gz` & `tmp/tt_damage_calculator-4.3.0.tar.gz`

## Comparing `tt_damage_calculator-4.2.0.tar` & `tt_damage_calculator-4.3.0.tar`

### file list

```diff
@@ -1,73 +1,85 @@
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 tt_damage_calculator-4.2.0/Cargo.toml
--rw-r--r--   0        0        0       66 2021-10-16 03:58:34.000000 tt_damage_calculator-4.2.0/.gitattributes
--rw-r--r--   0        0        0      631 2023-03-05 05:41:55.000000 tt_damage_calculator-4.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      752 2022-05-06 16:25:32.000000 tt_damage_calculator-4.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2022-05-06 20:53:50.000000 tt_damage_calculator-4.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0       62 2023-03-31 00:36:24.000000 tt_damage_calculator-4.2.0/.gitignore
--rw-r--r--   0        0        0    35823 2022-05-13 02:13:43.000000 tt_damage_calculator-4.2.0/LICENSE
--rw-r--r--   0        0        0      252 2023-03-31 01:22:44.000000 tt_damage_calculator-4.2.0/Makefile
--rw-r--r--   0        0        0     3863 2023-03-10 19:57:09.000000 tt_damage_calculator-4.2.0/README.md
--rw-r--r--   0        0        0      999 2023-03-31 00:28:47.000000 tt_damage_calculator-4.2.0/Toontown Damage Calculator.spec
--rw-r--r--   0        0        0     3221 2023-03-09 05:25:34.000000 tt_damage_calculator-4.2.0/change.log
--rw-r--r--   0        0        0   327692 2023-03-05 05:41:55.000000 tt_damage_calculator-4.2.0/preview.png
--rw-r--r--   0        0        0      873 2023-03-10 04:24:34.000000 tt_damage_calculator-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     6940 2023-03-10 04:03:38.000000 tt_damage_calculator-4.2.0/src/calc.rs
--rw-r--r--   0        0        0     1701 2023-03-10 04:03:38.000000 tt_damage_calculator-4.2.0/src/gags.rs
--rw-r--r--   0        0        0     1138 2023-03-10 04:03:38.000000 tt_damage_calculator-4.2.0/src/lib.rs
--rw-r--r--   0        0        0     2658 2023-03-10 04:03:38.000000 tt_damage_calculator-4.2.0/src/settings.rs
--rw-r--r--   0        0        0      233 2023-03-10 04:28:38.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/Toontown Damage Calculator.py
--rw-r--r--   0        0        0      175 2023-03-10 18:39:36.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/__init__.py
--rw-r--r--   0        0        0      115 2023-03-10 04:03:38.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/__main__.py
--rw-r--r--   0        0        0    18030 2023-03-10 20:31:06.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/app.py
--rw-r--r--   0        0        0     4719 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/anvil.png
--rw-r--r--   0        0        0     4382 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/aoogah.png
--rw-r--r--   0        0        0     3236 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/banana-peel.png
--rw-r--r--   0        0        0     3599 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/barbaraseville.png
--rw-r--r--   0        0        0     2657 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/barnaclebessie.png
--rw-r--r--   0        0        0     4581 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/big-weight.png
--rw-r--r--   0        0        0     4646 2022-10-06 18:42:43.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/bike-horn.png
--rw-r--r--   0        0        0     7073 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/birthday-cake.png
--rw-r--r--   0        0        0     4713 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/bugle.png
--rw-r--r--   0        0        0     2838 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clerkclara.png
--rw-r--r--   0        0        0     2651 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clerkpenny.png
--rw-r--r--   0        0        0     3252 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clerkwill.png
--rw-r--r--   0        0        0     3377 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clumsyned.png
--rw-r--r--   0        0        0    21597 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/coghp.png
--rw-r--r--   0        0        0     6298 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/cream-pie-slice.png
--rw-r--r--   0        0        0     5200 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/cupcake.png
--rw-r--r--   0        0        0     4771 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/elephant-trunk.png
--rw-r--r--   0        0        0     6840 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/fire-hose.png
--rw-r--r--   0        0        0     5395 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/flower-pot.png
--rw-r--r--   0        0        0     4583 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/fog-horn.png
--rw-r--r--   0        0        0     2990 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/franzneckvein.png
--rw-r--r--   0        0        0     5353 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/fruit-pie-slice.png
--rw-r--r--   0        0        0     6572 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/geyser.png
--rw-r--r--   0        0        0     4756 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/glass-of-water.png
--rw-r--r--   0        0        0     4816 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/grand-piano.png
--rw-r--r--   0        0        0     5704 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/marbles.png
--rw-r--r--   0        0        0     3897 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/moezart.png
--rw-r--r--   0        0        0     6409 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/opera-singer.png
--rw-r--r--   0        0        0     4435 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/quicksand.png
--rw-r--r--   0        0        0     3426 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/railroad.png
--rw-r--r--   0        0        0     3334 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/rake.png
--rw-r--r--   0        0        0     5926 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/safe.png
--rw-r--r--   0        0        0     5548 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/sandbag.png
--rw-r--r--   0        0        0     4245 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/seltzer-bottle.png
--rw-r--r--   0        0        0     4041 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/sidsonata.png
--rw-r--r--   0        0        0     4905 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/squirt-gun.png
--rw-r--r--   0        0        0     3883 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/squirting-flower.png
--rw-r--r--   0        0        0     5035 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/storm-cloud.png
--rw-r--r--   0        0        0     4161 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/tnt.png
--rw-r--r--   0        0        0     5882 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/toontanic.png
--rw-r--r--   0        0        0     6241 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/trapdoor.png
--rw-r--r--   0        0        0     4180 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/wedding-cake.png
--rw-r--r--   0        0        0     4353 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whistle.png
--rw-r--r--   0        0        0    10462 2022-05-03 02:38:18.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whole-cream-pie.ico
--rw-r--r--   0        0        0     4796 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whole-cream-pie.png
--rw-r--r--   0        0        0     5210 2022-10-06 18:42:44.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whole-fruit-pie.png
--rw-r--r--   0        0        0      135 2023-03-05 05:41:55.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/settings.toml
--rw-r--r--   0        0        0        5 2023-03-09 01:38:45.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/version.txt
--rw-r--r--   0        0        0     1569 2023-03-10 04:03:38.000000 tt_damage_calculator-4.2.0/src/tt_damage_calculator/update_checker.py
--rw-r--r--   0        0        0    31430 2023-03-09 05:05:59.000000 tt_damage_calculator-4.2.0/Cargo.lock
--rw-r--r--   0        0        0     3863 2023-03-10 19:57:09.000000 tt_damage_calculator-4.2.0/readme.md
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 tt_damage_calculator-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 tt_damage_calculator-4.3.0/Cargo.toml
+-rw-r--r--   0     1001      127       66 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.gitattributes
+-rw-r--r--   0     1001      127      619 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      722 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      127      624 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      127     6125 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127       73 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.gitignore
+-rw-r--r--   0     1001      127      108 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/.kateproject
+-rw-r--r--   0     1001      127     1193 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      127    35149 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/LICENSE
+-rw-r--r--   0     1001      127      662 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/Makefile
+-rw-r--r--   0     1001      127     7295 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/README.md
+-rw-r--r--   0     1001      127      948 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/Toontown Damage Calculator.spec
+-rw-r--r--   0     1001      127     4301 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/change.log
+-rw-r--r--   0     1001      127       34 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/requirements-dev.txt
+-rw-r--r--   0     1001      127     5845 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/calc.rs
+-rw-r--r--   0     1001      127     1846 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/gags.rs
+-rw-r--r--   0     1001      127      935 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/lib.rs
+-rw-r--r--   0     1001      127     2839 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/settings.rs
+-rw-r--r--   0     1001      127      214 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/Toontown Damage Calculator.py
+-rw-r--r--   0     1001      127      238 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/__init__.py
+-rw-r--r--   0     1001      127      334 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/__main__.py
+-rw-r--r--   0     1001      127     4719 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/anvil.png
+-rw-r--r--   0     1001      127     4382 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/aoogah.png
+-rw-r--r--   0     1001      127     3236 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/banana-peel.png
+-rw-r--r--   0     1001      127     3599 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/barbaraseville.png
+-rw-r--r--   0     1001      127     2657 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/barnaclebessie.png
+-rw-r--r--   0     1001      127     4581 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/big-weight.png
+-rw-r--r--   0     1001      127     4646 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/bike-horn.png
+-rw-r--r--   0     1001      127     7073 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/birthday-cake.png
+-rw-r--r--   0     1001      127     4713 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/bugle.png
+-rw-r--r--   0     1001      127     2838 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clerkclara.png
+-rw-r--r--   0     1001      127     2651 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clerkpenny.png
+-rw-r--r--   0     1001      127     3252 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clerkwill.png
+-rw-r--r--   0     1001      127     3377 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clumsyned.png
+-rw-r--r--   0     1001      127    21597 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/coghp.png
+-rw-r--r--   0     1001      127     6298 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/cream-pie-slice.png
+-rw-r--r--   0     1001      127     5200 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/cupcake.png
+-rw-r--r--   0     1001      127     4771 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/elephant-trunk.png
+-rw-r--r--   0     1001      127     6840 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/fire-hose.png
+-rw-r--r--   0     1001      127     5395 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/flower-pot.png
+-rw-r--r--   0     1001      127     4583 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/fog-horn.png
+-rw-r--r--   0     1001      127     2990 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/franzneckvein.png
+-rw-r--r--   0     1001      127     5353 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/fruit-pie-slice.png
+-rw-r--r--   0     1001      127     6572 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/geyser.png
+-rw-r--r--   0     1001      127     4756 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/glass-of-water.png
+-rw-r--r--   0     1001      127     4816 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/grand-piano.png
+-rw-r--r--   0     1001      127     5704 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/marbles.png
+-rw-r--r--   0     1001      127     3897 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/moezart.png
+-rw-r--r--   0     1001      127     6409 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/opera-singer.png
+-rw-r--r--   0     1001      127     4435 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/quicksand.png
+-rw-r--r--   0     1001      127     3426 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/railroad.png
+-rw-r--r--   0     1001      127     3334 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/rake.png
+-rw-r--r--   0     1001      127     5926 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/safe.png
+-rw-r--r--   0     1001      127     5548 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/sandbag.png
+-rw-r--r--   0     1001      127     4245 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/seltzer-bottle.png
+-rw-r--r--   0     1001      127     4041 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/sidsonata.png
+-rw-r--r--   0     1001      127     4905 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/squirt-gun.png
+-rw-r--r--   0     1001      127     3883 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/squirting-flower.png
+-rw-r--r--   0     1001      127     5035 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/storm-cloud.png
+-rw-r--r--   0     1001      127     4161 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/tnt.png
+-rw-r--r--   0     1001      127     5882 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/toontanic.png
+-rw-r--r--   0     1001      127     6241 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/trapdoor.png
+-rw-r--r--   0     1001      127     4180 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/wedding-cake.png
+-rw-r--r--   0     1001      127     4353 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whistle.png
+-rw-r--r--   0     1001      127    10462 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whole-cream-pie.ico
+-rw-r--r--   0     1001      127     4796 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whole-cream-pie.png
+-rw-r--r--   0     1001      127     5210 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whole-fruit-pie.png
+-rw-r--r--   0     1001      127      138 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/settings.toml
+-rw-r--r--   0     1001      127        5 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/version.txt
+-rw-r--r--   0     1001      127    30051 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/src/tt_damage_calculator/widgets.py
+-rw-r--r--   0     1001      127   171296 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/arch.png
+-rw-r--r--   0     1001      127   242259 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/gags-organic.png
+-rw-r--r--   0     1001      127   247217 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/gags-press.png
+-rw-r--r--   0     1001      127   242449 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/gags.png
+-rw-r--r--   0     1001      127    18268 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/headerfooter.png
+-rw-r--r--   0     1001      127   217464 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/history.png
+-rw-r--r--   0     1001      127   242430 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/lure.png
+-rw-r--r--   0     1001      127   164246 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/preview.png
+-rw-r--r--   0     1001      127   219591 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/settings.png
+-rw-r--r--   0     1001      127     8936 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/settingstoml.png
+-rw-r--r--   0     1001      127   240892 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/wiki/status.png
+-rw-r--r--   0     1001      127    37243 2024-05-24 23:55:36.000000 tt_damage_calculator-4.3.0/Cargo.lock
+-rw-r--r--   0     1001      127     1023 2024-05-24 23:55:31.000000 tt_damage_calculator-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8049 1970-01-01 00:00:00.000000 tt_damage_calculator-4.3.0/PKG-INFO
```

### Comparing `tt_damage_calculator-4.2.0/Cargo.toml` & `tt_damage_calculator-4.3.0/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [package]
 name = "rustygag"
 description = "Rust library providing the backend of the Toontown Damage Calculator."
 authors = ["Vhou-Atroph"]
 license = "GPLv3"
-version = "4.2.0"
+version = "4.3.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
-name = "rustygag"
+name = "tt_damage_calculator"
 crate-type = ["cdylib"]
 
 [dependencies.pyo3]
-version = "0.18.1"
+version = "0.21.2"
 features = ["extension-module"]
 
-[package.metadata.maturin]
-name = "tt_damage_calculator.rustygag"
+[dependencies.serde]
+version = "1.0.201"
+features = ["derive"]
+
+[dependencies.tokio]
+version = "1.37.0"
+features = ["full"]
 
 [dependencies]
-serde = { version = "1.0.154", features = ["derive"] }
-toml = "0.7.2"
-reqwest = "0.11.14"
-tokio = { version = "1.26.0", features = ["full"] }
+toml = "0.8.12"
+reqwest = "0.12.4"
```

### Comparing `tt_damage_calculator-4.2.0/.github/FUNDING.yml` & `tt_damage_calculator-4.3.0/.github/FUNDING.yml`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# These are supported funding model platforms
-
-github: [Vhou-Atroph]
-patreon: # Replace with a single Patreon username
-open_collective: # Replace with a single Open Collective username
-ko_fi: vhouatroph
-tidelift: # Replace with a single Tidelift platform-name/package-name e.g., npm/babel
-community_bridge: # Replace with a single Community Bridge project-name e.g., cloud-foundry
-liberapay: # Replace with a single Liberapay username
-issuehunt: # Replace with a single IssueHunt username
-otechie: # Replace with a single Otechie username
-custom: # Replace with up to 4 custom sponsorship URLs e.g., ['link1', 'link2']
+# These are supported funding model platforms
+
+github: [Vhou-Atroph]
+patreon: # Replace with a single Patreon username
+open_collective: # Replace with a single Open Collective username
+ko_fi: vhouatroph
+tidelift: # Replace with a single Tidelift platform-name/package-name e.g., npm/babel
+community_bridge: # Replace with a single Community Bridge project-name e.g., cloud-foundry
+liberapay: # Replace with a single Liberapay username
+issuehunt: # Replace with a single IssueHunt username
+otechie: # Replace with a single Otechie username
+custom: # Replace with up to 4 custom sponsorship URLs e.g., ['link1', 'link2']
```

### Comparing `tt_damage_calculator-4.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `tt_damage_calculator-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
----
-name: Feature Request
-about: Suggest an idea for the project
-title: "[Enhancement]"
-labels: enhancement
-assignees: ''
-
----
-
-**Is your feature request related to a problem? Please describe.**  
-A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
-
-**Describe the solution you'd like**  
-A clear and concise description of what you want to happen.
-
-**Describe alternatives you've considered**  
-A clear and concise description of any alternative solutions or features you've considered.
-
-**Additional context**  
-Add any other context or screenshots about the feature request here.
+---
+name: Feature Request
+about: Suggest an idea for the project
+title: "[Enhancement]"
+labels: enhancement
+assignees: ''
+
+---
+
+**Is your feature request related to a problem? Please describe.**  
+A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
+
+**Describe the solution you'd like**  
+A clear and concise description of what you want to happen.
+
+**Describe alternatives you've considered**  
+A clear and concise description of any alternative solutions or features you've considered.
+
+**Additional context**  
+Add any other context or screenshots about the feature request here.
```

### Comparing `tt_damage_calculator-4.2.0/LICENSE` & `tt_damage_calculator-4.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `tt_damage_calculator-4.2.0/Toontown Damage Calculator.spec` & `tt_damage_calculator-4.3.0/Toontown Damage Calculator.spec`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# -*- mode: python ; coding: utf-8 -*-
-
-
-block_cipher = None
-
-
-a = Analysis(
-    ['src\\tt_damage_calculator\\Toontown Damage Calculator.py'],
-    pathex=[],
-    binaries=[],
-    datas=[],
-    hiddenimports=[],
-    hookspath=[],
-    hooksconfig={},
-    runtime_hooks=[],
-    excludes=[],
-    win_no_prefer_redirects=False,
-    win_private_assemblies=False,
-    cipher=block_cipher,
-    noarchive=False,
-)
-pyz = PYZ(a.pure, a.zipped_data, cipher=block_cipher)
-
-exe = EXE(
-    pyz,
-    a.scripts,
-    a.binaries,
-    a.zipfiles,
-    a.datas,
-    [],
-    name='Toontown Damage Calculator',
-    debug=False,
-    bootloader_ignore_signals=False,
-    strip=False,
-    upx=True,
-    upx_exclude=[],
-    runtime_tmpdir=None,
-    console=False,
-    disable_windowed_traceback=False,
-    argv_emulation=False,
-    target_arch=None,
-    codesign_identity=None,
-    entitlements_file=None,
-    icon=['src\\tt_damage_calculator\\assets\\img\\whole-cream-pie.ico'],
-)
+# -*- mode: python ; coding: utf-8 -*-
+
+
+block_cipher = None
+
+
+a = Analysis(
+    ['src/tt_damage_calculator/Toontown Damage Calculator.py'],
+    pathex=[],
+    binaries=[],
+    datas=[],
+    hiddenimports=[],
+    hookspath=[],
+    hooksconfig={},
+    runtime_hooks=[],
+    excludes=[],
+    win_no_prefer_redirects=False,
+    win_private_assemblies=False,
+    cipher=block_cipher,
+    noarchive=False,
+)
+pyz = PYZ(a.pure, a.zipped_data, cipher=block_cipher)
+
+exe = EXE(
+    pyz,
+    a.scripts,
+    a.binaries,
+    a.zipfiles,
+    a.datas,
+    [],
+    name='Toontown Damage Calculator',
+    debug=False,
+    bootloader_ignore_signals=False,
+    strip=False,
+    upx=True,
+    upx_exclude=[],
+    runtime_tmpdir=None,
+    console=False,
+    disable_windowed_traceback=False,
+    argv_emulation=False,
+    target_arch=None,
+    codesign_identity=None,
+    entitlements_file=None,
+    icon=['src/tt_damage_calculator/assets/img/whole-cream-pie.ico'],
+)
```

### Comparing `tt_damage_calculator-4.2.0/change.log` & `tt_damage_calculator-4.3.0/change.log`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,93 @@
---Toontown Gag Damage Calculator V2.0.0--
-
-- Live calculation is now here! The calculate button is a thing of the past.
-- Several incorrect gag damage values have been fixed both visually and mathematically.
- - Bugle
- - Marbles
- - Quicksand
-- The dropdowns are the same size as everything else! How cool is that?!
-- Updating lure damage bonus to be accurate to the latest versions of Toontown Rewritten.
-
---V2.0.0a--
-- More incorrect gag damage values have been fixed.
- - Squirting Flower
- - Cream Pie Slice
-
---V2.1--
-- Added number indicators for how many of each gag is used in a given turn.
-
---V2.2--
-- SOS Cards are real
-- Fixed Bugle (again)
-
---V2.2.1--
-- Keybind for organic toggle
-- Keybind for def toggle
-- Keybind for calculation reset
-- Keybind for lure toggle
-
---V2.3--
-- V2 Calculation - might not work as intended, please test it out in cog golf courses and let me know if there's any issues.
-- Reworked how the level indicator works to make it easier to add higher level cogs in the future.
-
---V3--
-- Moved math funcitons to mod/calculators.py
-- Added version.txt for future update checking, maybe?
-
---V3.1.0--
-- Added the update checker. It is accessed through the new menu bar under "Program."
-
---V3.1.1--
-- Changed the naming system of variables and functions to snake_case for more readability
-- Added "Exit" menu option under Program menu bar.
-
---V3.2.0--
-- Created gags.py, which stores gag objects. Gag objects have type, name, track, and dmg. They also have method .makeorg(), which will evaluate the organic damage of the gag object.
-- Made gag buttons more efficient by removing individual functions and making a single that applies to every button.
-- With these changes, there's probably some kind of new (or old, unnoticed) issue out there. Please submit any such issue you find.
-
---V3.2.1--
-- Bugfix: Fixed gag history displaying incorrectly if a gag was organic or not after using it as organic once.
-- Moved "Pin Window" button to the Program menu. More things will probably be moved into the menu bar at some point.
-- Pin window has also been given a keybind- alt+up
-
---V3.3.0--
-- settings.toml! This will store personal settings for the gag calculator!
-- Keybinds are stored here- it's now possible to edit keybinds by changing this file instead of having to use the ones I created. Note that keybinds are currently only editable through settings.toml and are configured at launch. If a keybind is not possible, the program will crash immediately with an error that looks like: '_tkinter.TclError: bad event type or keysym "Shfit_L".'
-- The program now requires an external library: tomli.
-
---V3.3.2--
-- Added a new level of defense.
-
---V4.0.0--
-- Converted several modules to Rust.
-- Removed tomli dependency
-- Moved V2, Defense, and Status Locking to the new Calculations menu
-
---V4.1.0--
-- Upgraded to Python 3.11
-- Fixed a bug with V2.0 cog calculation
-
---V4.2.0--
-- See the programming of this update partially streamed live!
-  - https://www.youtube.com/watch?v=-RaI5TbVKCA
-- Fixed a minor bug that resulted in versions being mismatched on the update checker.
-- Changed project format to be publishable on Pypi.
+--Toontown Gag Damage Calculator V2.0.0--
+
+- Live calculation is now here! The calculate button is a thing of the past.
+- Several incorrect gag damage values have been fixed both visually and mathematically.
+ - Bugle
+ - Marbles
+ - Quicksand
+- The dropdowns are the same size as everything else! How cool is that?!
+- Updating lure damage bonus to be accurate to the latest versions of Toontown Rewritten.
+
+--V2.0.0a--
+- More incorrect gag damage values have been fixed.
+ - Squirting Flower
+ - Cream Pie Slice
+
+--V2.1--
+- Added number indicators for how many of each gag is used in a given turn.
+
+--V2.2--
+- SOS Cards are real
+- Fixed Bugle (again)
+
+--V2.2.1--
+- Keybind for organic toggle
+- Keybind for def toggle
+- Keybind for calculation reset
+- Keybind for lure toggle
+
+--V2.3--
+- V2 Calculation - might not work as intended, please test it out in cog golf courses and let me know if there's any issues.
+- Reworked how the level indicator works to make it easier to add higher level cogs in the future.
+
+--V3--
+- Moved math funcitons to mod/calculators.py
+- Added version.txt for future update checking, maybe?
+
+--V3.1.0--
+- Added the update checker. It is accessed through the new menu bar under "Program."
+
+--V3.1.1--
+- Changed the naming system of variables and functions to snake_case for more readability
+- Added "Exit" menu option under Program menu bar.
+
+--V3.2.0--
+- Created gags.py, which stores gag objects. Gag objects have type, name, track, and dmg. They also have method .makeorg(), which will evaluate the organic damage of the gag object.
+- Made gag buttons more efficient by removing individual functions and making a single that applies to every button.
+- With these changes, there's probably some kind of new (or old, unnoticed) issue out there. Please submit any such issue you find.
+
+--V3.2.1--
+- Bugfix: Fixed gag history displaying incorrectly if a gag was organic or not after using it as organic once.
+- Moved "Pin Window" button to the Program menu. More things will probably be moved into the menu bar at some point.
+- Pin window has also been given a keybind- alt+up
+
+--V3.3.0--
+- settings.toml! This will store personal settings for the gag calculator!
+- Keybinds are stored here- it's now possible to edit keybinds by changing this file instead of having to use the ones I created. Note that keybinds are currently only editable through settings.toml and are configured at launch. If a keybind is not possible, the program will crash immediately with an error that looks like: '_tkinter.TclError: bad event type or keysym "Shfit_L".'
+- The program now requires an external library: tomli.
+
+--V3.3.2--
+- Added a new level of defense.
+
+--V4.0.0--
+- Converted several modules to Rust.
+- Removed tomli dependency
+- Moved V2, Defense, and Status Locking to the new Calculations menu
+
+--V4.1.0--
+- Upgraded to Python 3.11
+- Fixed a bug with V2.0 cog calculation
+
+--V4.2.0--
+- See the programming of this update partially streamed live!
+  - https://www.youtube.com/watch?v=-RaI5TbVKCA
+- Fixed a minor bug that resulted in versions being mismatched on the update checker.
+- Changed project format to be publishable on Pypi.
+
+--V4.2.1--
+- Fixed a bug that caused a 404 error when using the update checker.
+
+--V4.3.0--
+- Updated the calculator for Under New Management!
+- Organic squirt and drop now have a 15% bonus
+- Organic gag damage ceils in general
+- Reinforced Plating is no longer a mechanic
+- Added negative defense
+- Added snowballs
+- Added the ability to add custom gags to a calculation
+- Organic toggle is now affected by status lock. This is an experimental change and may be reverted at some point in the future.
+- Massive backend rewrite
+- Compiling of executable versions the gag calculator now uses Github Actions rather than my own hardware. This means releases for MacOS are now possible alongside Windows and Linux!
+- Executable files for Linux are now also supplied in releases. These should work for any Linux distribution that uses glibc, but Ubuntu is the distribution that is specifcally targeted.
+- Keybinds now have a hardcoded default, if an error happens when setting a keybind it will fall back on this default.
+- Removed the menu bar's update checker, this change is tentative and there may be a new iteration of the update checker in the future.
```

### Comparing `tt_damage_calculator-4.2.0/src/gags.rs` & `tt_damage_calculator-4.3.0/src/gags.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-//! TT-Damage-Calculator
-//! Copyright (C) 2022-2023 Vhou-Atroph
-
-use pyo3::prelude::*;
-
-/// This struct is for a basic Gag, which is a thing that toons use against cogs in the wild and wacky game Toontown Rewritten (or any of the other private servers I guess.)
-/// | Field | Description                                     |
-/// |-------|-------------------------------------------------|
-/// | gtype | Whether the gag is a regular gag or an SOS Card |
-/// | name  | The name of the gag.                            |
-/// | track | The gag track a gag belongs to as a String      |
-/// | level | The level that the gag is                       |
-/// | dmg   | The amount of damage a gag may do to a  cog.    |
-#[pyclass]
-pub struct Gag {
-    #[pyo3(get, set)]
-    gtype: String,
-    #[pyo3(get, set)]
-    name: String,
-    #[pyo3(get, set)]
-    track: String,
-    #[pyo3(get, set)]
-    level: u8,
-    #[pyo3(get, set)]
-    dmg: i64,
-}
-
-#[pymethods]
-impl Gag {
-
-    /// Creates a new Gag struct.
-    #[new]
-    pub fn new(gtype:String,name:String,track:String,level:u8,dmg:i64) -> Self {
-        Self { gtype, name, track, level, dmg }
-    }
-
-    /// Returns the damage an organic gag of a certain type does.
-    pub fn button_press(&self,org_val:bool) -> PyResult<(i64,String)> { // (damage,name)
-        if self.gtype == "Gag" && org_val {return Ok((org(self.dmg),format!("Organic {}",self.name)))}
-        Ok((self.dmg,self.name.clone()))
-    }
-}
-
-/// Evaluates the amount of damage a gag will do when organic.
-fn org(n:i64) -> i64 {
-    let org_boost_f = n as f64 * 0.1;
-    if org_boost_f < 1.0 {return n+1_i64}
-    n + org_boost_f.floor() as i64
+//! TT-Damage-Calculator
+//! Copyright (C) 2022-2024 Vhou-Atroph
+
+use pyo3::prelude::*;
+
+/// This struct is for a basic Gag, which is a thing that toons use against cogs in the wild and wacky game Toontown Rewritten (or any of the other private servers I guess.)
+/// | Field | Description                                     |
+/// |-------|-------------------------------------------------|
+/// | gtype | Whether the gag is a regular gag or an SOS Card |
+/// | name  | The name of the gag.                            |
+/// | track | The gag track a gag belongs to as a String      |
+/// | level | The level that the gag is                       |
+/// | dmg   | The amount of damage a gag may do to a  cog.    |
+#[pyclass]
+pub struct Gag {
+    #[pyo3(get, set)]
+    gtype: String,
+    #[pyo3(get, set)]
+    name: String,
+    #[pyo3(get, set)]
+    track: String,
+    #[pyo3(get, set)]
+    level: u8,
+    #[pyo3(get, set)]
+    dmg: i64,
+}
+
+#[pymethods]
+impl Gag {
+
+    /// Creates a new Gag struct.
+    #[new]
+    pub fn new(gtype:String,name:String,track:String,level:u8,dmg:i64) -> Self {
+        Self { gtype, name, track, level, dmg }
+    }
+
+    /// Returns the damage an organic gag of a certain type does.
+    pub fn button_press(&self,org_val:bool) -> (i64,String) { // (damage,name)
+        if self.gtype == "Gag" && org_val {return (self.org(),format!("Organic {}",self.name))}
+        (self.dmg,self.name.clone())
+    }
+
+    /// Returns the amount of damage a gag will do when organic.
+    fn org(&self) -> i64 {
+        let boost;
+        match self.track.as_str() {
+            "Squirt" => boost = 0.15,
+            "Drop" => boost = 0.15,
+            _ => boost = 0.1
+        }
+        let org_boost_f = self.dmg as f64 * boost;
+        if org_boost_f < 1.0 {return self.dmg + 1_i64}
+        self.dmg + org_boost_f.ceil() as i64
+    }
 }
```

### Comparing `tt_damage_calculator-4.2.0/src/settings.rs` & `tt_damage_calculator-4.3.0/src/settings.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-//! TT-Damage-Calculator
-//! Copyright (C) 2022-2023 Vhou-Atroph
-
-use std::fs;
-
-use pyo3::prelude::*;
-use serde::{Serialize, Deserialize};
-
-/// Struct for the Settings file
-#[pyclass]
-#[derive(Serialize,Deserialize)]
-pub struct Settings {
-    #[pyo3(get, set)]
-    keybinds: Keybinds
-}
-
-/// Struct for the Keybinds portion of the Settings file
-#[pyclass]
-#[derive(Serialize,Deserialize,Clone)]
-/// | Field   | Description                         |
-/// |---------|-------------------------------------|
-/// | organic | Keybind for the organic toggle      |
-/// | lure    | Keybind for the lure toggle         |
-/// | reset   | Keybind to reset calculations       |
-/// | lock    | Keybind to toggle status lock       |
-/// | defense | Keybind to set cog defense          |
-/// | v2      | Keybind to set v2 cog level         |
-/// | pin     | Keybind to toggle window pin status |
-pub struct Keybinds {
-    #[pyo3(get, set)]
-    organic: String,
-    #[pyo3(get, set)]
-    lure: String,
-    #[pyo3(get, set)]
-    reset: String,
-    #[pyo3(get, set)]
-    lock: String,
-    #[pyo3(get, set)]
-    defense: String,
-    #[pyo3(get, set)]
-    v2: String,
-    #[pyo3(get, set)]
-    pin: String,
-}
-
-#[pymethods]
-impl Settings {
-
-    /// Opens the Settings file.
-    #[new]
-    fn new(file:&str) -> Self {
-        let data =  fs::read_to_string(file).unwrap();
-        let settings: Settings = toml::from_str(data.as_str()).unwrap();
-        settings
-    }
-}
-
-/// Swap a toggle
-#[pyfunction]
-pub fn toggleswap(toggle:bool) -> bool {
-    return !toggle
-}
-
-/// Specifically swap the organic gags toggle, which is significantly more painful than the checkbox ones!
-#[pyfunction]
-pub fn orgswap(toggle:bool) -> (bool,String,String,String) { // (state,indicator,bg,activebg)
-    if toggle {return (false,String::from("OFF"),String::from("#1888D3"),String::from("#186AD3"));} 
-    (true,String::from("ON"),String::from("darkorange"),String::from("orange"))
-}
-
-/// Get GitHub version.txt file
-#[tokio::main]
-async fn git_version(gitfile:&str) -> Result<String,Box<dyn std::error::Error>> {
-    let data = reqwest::get(gitfile).await?.text().await?;
-    Ok(data)
-}
-
-/// Compare local and git repo versions.txt file
-#[pyfunction]
-pub fn comp_data(localfile:String) -> (bool,String,String) { // (diff,repo,loc)
-    let repo_ver = git_version("https://raw.githubusercontent.com/Vhou-Atroph/TT-Damage-Calculator/main/mod/version.txt").unwrap();
-    let local_ver = fs::read_to_string(localfile).unwrap();
-    if repo_ver == local_ver {return (true,repo_ver,local_ver);} (false,repo_ver,local_ver)
-}
+//! TT-Damage-Calculator
+//! Copyright (C) 2022-2024 Vhou-Atroph
+
+use std::fs;
+
+use pyo3::prelude::*;
+use serde::{Serialize, Deserialize};
+
+/// Struct for the Settings file
+#[pyclass]
+#[derive(Serialize,Deserialize)]
+pub struct Settings {
+    #[pyo3(get, set)]
+    keybinds: Keybinds
+}
+
+#[pymethods]
+impl Settings {
+
+    /// Opens the Settings file.
+    #[new]
+    fn new(file:&str) -> Self {
+        let data =  fs::read_to_string(file).unwrap();
+        let settings: Settings = toml::from_str(data.as_str()).unwrap();
+        settings
+    }
+}
+
+/// Struct for the Keybinds portion of the Settings file
+/// | Field            | Description                         |
+/// |------------------|-------------------------------------|
+/// | organic          | Keybind for the organic toggle      |
+/// | lure             | Keybind for the lure toggle         |
+/// | reset            | Keybind to reset calculations       |
+/// | lock             | Keybind to toggle status lock       |
+/// | defense          | Keybind to set cog defense          |
+/// | negative_defense | Keybind to set negative cog defense |
+/// | pin              | Keybind to toggle window pin status |
+#[pyclass]
+#[derive(Serialize,Deserialize,Clone)]
+pub struct Keybinds {
+    #[pyo3(get, set)]
+    organic: String,
+    #[pyo3(get, set)]
+    lure: String,
+    #[pyo3(get, set)]
+    reset: String,
+    #[pyo3(get, set)]
+    lock: String,
+    #[pyo3(get, set)]
+    defense: String,
+    #[pyo3(get, set)]
+    negative_defense: String,
+    #[pyo3(get, set)]
+    pin: String,
+}
+
+#[pymethods]
+impl Keybinds {
+
+    /// Get default keybinds in case settings.toml keybinds are unusable for whatever reason
+    #[staticmethod]
+    pub fn default() -> Keybinds {
+        Keybinds {
+            organic: String::from("Shift_L"),
+            lure: String::from("Control-l"),
+            reset: String::from("Control-r"),
+            lock: String::from("Control-x"),
+            defense: String::from("Control-d"),
+            negative_defense: String::from("Alt-d"),
+            pin: String::from("Alt-Up")
+        }
+    }
+}
+
+/// Swap a toggle
+#[pyfunction]
+pub fn toggleswap(toggle:bool) -> bool {
+    return !toggle
+}
+
+/// Get GitHub version.txt file
+#[tokio::main]
+async fn git_version(gitfile:&str) -> Result<String,Box<dyn std::error::Error>> {
+    let data = reqwest::get(gitfile).await?.text().await?;
+    Ok(data)
+}
+
+/// Compare local and git repo versions.txt file
+#[pyfunction]
+pub fn comp_data(localfile:String) -> (bool,String,String) { // (diff,repo,loc)
+    let repo_ver = git_version("https://raw.githubusercontent.com/Vhou-Atroph/TT-Damage-Calculator/main/src/tt_damage_calculator/assets/version.txt").unwrap();
+    let local_ver = fs::read_to_string(localfile).unwrap();
+    if repo_ver == local_ver {return (true,repo_ver,local_ver);} (false,repo_ver,local_ver)
+}
```

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/anvil.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/anvil.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/aoogah.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/aoogah.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/banana-peel.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/banana-peel.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/barbaraseville.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/barbaraseville.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/barnaclebessie.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/barnaclebessie.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/big-weight.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/big-weight.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/bike-horn.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/bike-horn.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/birthday-cake.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/birthday-cake.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/bugle.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/bugle.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clerkclara.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clerkclara.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clerkpenny.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clerkpenny.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clerkwill.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clerkwill.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/clumsyned.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/clumsyned.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/coghp.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/coghp.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/cream-pie-slice.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/cream-pie-slice.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/cupcake.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/cupcake.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/elephant-trunk.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/elephant-trunk.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/fire-hose.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/fire-hose.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/flower-pot.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/flower-pot.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/fog-horn.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/fog-horn.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/franzneckvein.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/franzneckvein.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/fruit-pie-slice.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/fruit-pie-slice.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/geyser.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/geyser.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/glass-of-water.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/glass-of-water.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/grand-piano.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/grand-piano.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/marbles.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/marbles.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/moezart.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/moezart.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/opera-singer.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/opera-singer.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/quicksand.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/quicksand.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/railroad.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/railroad.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/rake.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/rake.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/safe.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/safe.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/sandbag.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/sandbag.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/seltzer-bottle.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/seltzer-bottle.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/sidsonata.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/sidsonata.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/squirt-gun.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/squirt-gun.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/squirting-flower.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/squirting-flower.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/storm-cloud.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/storm-cloud.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/tnt.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/tnt.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/toontanic.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/toontanic.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/trapdoor.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/trapdoor.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/wedding-cake.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/wedding-cake.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whistle.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whistle.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whole-cream-pie.ico` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whole-cream-pie.ico`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whole-cream-pie.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whole-cream-pie.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/src/tt_damage_calculator/assets/img/whole-fruit-pie.png` & `tt_damage_calculator-4.3.0/src/tt_damage_calculator/assets/img/whole-fruit-pie.png`

 * *Files identical despite different names*

### Comparing `tt_damage_calculator-4.2.0/Cargo.lock` & `tt_damage_calculator-4.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,107 +1,141 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
+name = "atomic-waker"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
+
+[[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
+
+[[package]]
+name = "backtrace"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
-version = "1.4.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.79"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.32"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "errno"
-version = "0.2.8"
+name = "equivalent"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
+name = "errno"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "1.9.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
-dependencies = [
- "instant",
-]
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
@@ -118,299 +152,319 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.26"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e5317663a9089767a1ec00a487df42e0ca174b61b4483213ac24448e4664df5"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.26"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec90ff4d0fe1f57d600049061dc6bb68ed03c7d2fbd697274c41805dcb3f8608"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-sink"
-version = "0.3.26"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f310820bb3e8cfd46c80db4d7fb8353e15dfff853a127158425f31e0be6c8364"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.26"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf79a1bf610b10f42aea489289c5a2c478a786509693b80cd39c44ccd936366"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.26"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c1d6de3acfef38d2be4b1f543f553131788603495be83da675e180c8d6b7bd1"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-core",
  "futures-task",
  "pin-project-lite",
  "pin-utils",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.28.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+
+[[package]]
 name = "h2"
-version = "0.3.16"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be7b54589b581f624f566bf5d8eb2bab1db736c51528720b6bd36b96b55924d"
+checksum = "fa82e28a107a8cc405f0839610bdc9b15f1e25ec7d696aa5cf173edbcb1486ab"
 dependencies = [
+ "atomic-waker",
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
- "futures-util",
  "http",
  "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "http"
-version = "0.2.9"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
 dependencies = [
  "bytes",
+ "futures-core",
  "http",
+ "http-body",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
-name = "httpdate"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
-
-[[package]]
 name = "hyper"
-version = "0.14.24"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e011372fa0b68db8350aa7a248930ecc7839bf46d8485577d69f117a75f164c"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
- "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
- "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "smallvec",
  "tokio",
- "tower-service",
- "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-tls"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
+checksum = "70206fc6890eaca9fde8a0bf71caa2ddfc9fe045ac9e5c70df101a7dbde866e0"
 dependencies = [
  "bytes",
+ "http-body-util",
  "hyper",
+ "hyper-util",
  "native-tls",
  "tokio",
  "tokio-native-tls",
+ "tower-service",
+]
+
+[[package]]
+name = "hyper-util"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d8d52be92d09acc2e01dddb7fde3ad983fc6489c7db4837e605bc3fca4cb63e"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http",
+ "http-body",
+ "hyper",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower",
+ "tower-service",
+ "tracing",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
- "autocfg",
+ "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "instant"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "io-lifetimes"
-version = "1.0.6"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfa919a82ea574332e2de6e74b4c36e74d41982b335080fa59d4ef31be20fdf3"
-dependencies = [
- "libc",
- "windows-sys 0.45.0",
-]
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "ipnet"
-version = "2.7.1"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e22bd8629359895450b59ea7a776c850561b96a3b1d31321c1949d9e6c9146"
+checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a60c7ce501c71e03a9c9c0d35b861413ae925bd979cc7a4e30d060069aaac8d"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
+
+[[package]]
+name = "miniz_oxide"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
+dependencies = [
+ "adler",
+]
 
 [[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
- "log",
  "wasi",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -425,349 +479,412 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "object"
+version = "0.32.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "openssl"
-version = "0.10.45"
+version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b102428fd03bc5edf97f62620f7298614c45cedf287c271e7ed450bbaf83f2e1"
+checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.80"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23bbbf7854cd45b83958ebe919f0e8e516793727652e27fda10a8384cfc790b7"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
+
+[[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.14"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21eed90ec8570952d53b772ecf8f206aa1ec9a3d76b2521c56c42973f2d91ee9"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
+ "http-body-util",
  "hyper",
  "hyper-tls",
+ "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
+ "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
+ "sync_wrapper",
+ "system-configuration",
  "tokio",
  "tokio-native-tls",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.24"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
+
+[[package]]
 name = "rustix"
-version = "0.36.9"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd5c6ff11fecd55b40746d1995a02f2eb375bf8c00d192d521ee09f42bef37bc"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
  "errno",
- "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "rustls-pemfile"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
+dependencies = [
+ "base64",
+ "rustls-pki-types",
+]
+
+[[package]]
+name = "rustls-pki-types"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
+
+[[package]]
 name = "rustygag"
-version = "4.2.0"
+version = "4.3.0"
 dependencies = [
  "pyo3",
  "reqwest",
  "serde",
  "tokio",
  "toml",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
-version = "2.8.2"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.8.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c9bb296072e961fcbd8853511dd39c2d8be2deb1e17c6860b1d30732b323b4"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.154"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cdd151213925e7f1ab45a9bbfb129316bd00799784b174b7cc7bcd16961c49e"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.154"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fc80d722935453bcafdc2c9a73cd6fac4dc1938f0346035d84bf99fa9e33217"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.1"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+checksum = "79e674e01f999af37c49f70a6ede167a8a60b2503e56c5599532a65baa5969a0"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -778,74 +895,100 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
+checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.4.9"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.109"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "sync_wrapper"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
+
+[[package]]
+name = "system-configuration"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
+dependencies = [
+ "bitflags 1.3.2",
+ "core-foundation",
+ "system-configuration-sys",
+]
+
+[[package]]
+name = "system-configuration-sys"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -857,37 +1000,36 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
- "autocfg",
+ "backtrace",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -898,341 +1040,396 @@
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml"
-version = "0.7.2"
+version = "0.8.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7afcae9e3f0fe2c370fd4657108972cbb2fa9db1b9f84849cefd80741b01cb6"
+checksum = "a4e43f8cc456c9704c851ae29c67e17ef65d2c30017c17a9765b89c382dc8bba"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.4"
+version = "0.22.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a1eb0622d28f4b9c90adc4ea4b2b46b47663fde9ac5fafcb14a1369d5508825"
+checksum = "c127785850e8c20836d49732ae6abfa47616e60bf9d9f57c43c250361a9db96c"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.11"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524b68aca1d05e03fdf03fcdce2c6c94b6daf6d16861ddaa7e4f2b6638a9052c"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
+name = "windows-sys"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
+name = "windows-targets"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows-targets",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.3.5"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee7b2c67f962bf5042bfd8b6a916178df33a26eec343ae064cb8e069f638fa6f"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
-version = "0.10.1"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
- "winapi",
+ "cfg-if",
+ "windows-sys 0.48.0",
 ]
```


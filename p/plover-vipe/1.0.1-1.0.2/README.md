# Comparing `tmp/plover_vipe-1.0.1.tar.gz` & `tmp/plover_vipe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_vipe-1.0.1.tar", last modified: Thu May 23 22:28:56 2024, max compression
+gzip compressed data, was "plover_vipe-1.0.2.tar", last modified: Sat May 25 11:59:12 2024, max compression
```

## Comparing `plover_vipe-1.0.1.tar` & `plover_vipe-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 22:28:56.354637 plover_vipe-1.0.1/
--rw-rw-rw-   0        0        0    35147 2024-05-20 19:03:30.000000 plover_vipe-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       58 2024-05-22 16:43:10.000000 plover_vipe-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1698 2024-05-23 22:28:56.353639 plover_vipe-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      978 2024-05-22 16:43:10.000000 plover_vipe-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-23 22:28:56.319729 plover_vipe-1.0.1/plover_vipe/
--rw-rw-rw-   0        0        0        0 2024-05-20 19:03:31.000000 plover_vipe-1.0.1/plover_vipe/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 22:28:56.346677 plover_vipe-1.0.1/plover_vipe/dictionaries/
--rw-rw-rw-   0        0        0     1033 2024-04-15 18:48:45.000000 plover_vipe-1.0.1/plover_vipe/dictionaries/vipe_commands.json
--rw-rw-rw-   0        0        0   277903 2024-05-23 20:48:51.000000 plover_vipe-1.0.1/plover_vipe/dictionaries/vipe_main.json
--rw-rw-rw-   0        0        0     5076 2024-05-21 20:48:23.000000 plover_vipe-1.0.1/plover_vipe/system.py
-drwxrwxrwx   0        0        0        0 2024-05-23 22:28:56.350647 plover_vipe-1.0.1/plover_vipe.egg-info/
--rw-rw-rw-   0        0        0     1698 2024-05-23 22:28:56.000000 plover_vipe-1.0.1/plover_vipe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-23 22:28:56.000000 plover_vipe-1.0.1/plover_vipe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 22:28:56.000000 plover_vipe-1.0.1/plover_vipe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-23 22:28:56.000000 plover_vipe-1.0.1/plover_vipe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 22:28:56.000000 plover_vipe-1.0.1/plover_vipe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 22:28:56.000000 plover_vipe-1.0.1/plover_vipe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-23 21:44:32.000000 plover_vipe-1.0.1/plover_vipe.egg-info/zip-safe
--rw-rw-rw-   0        0        0      932 2024-05-23 22:28:56.357653 plover_vipe-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       63 2024-05-20 19:03:31.000000 plover_vipe-1.0.1/setup.py
--rw-rw-rw-   0        0        0      146 2024-05-20 19:03:31.000000 plover_vipe-1.0.1/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-25 11:59:12.092819 plover_vipe-1.0.2/
+-rw-rw-rw-   0        0        0    35147 2024-05-20 19:03:30.000000 plover_vipe-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       58 2024-05-22 16:43:10.000000 plover_vipe-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2081 2024-05-25 11:59:12.091823 plover_vipe-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2024-05-24 21:49:51.000000 plover_vipe-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 11:59:12.049937 plover_vipe-1.0.2/plover_vipe/
+-rw-rw-rw-   0        0        0        0 2024-05-20 19:03:31.000000 plover_vipe-1.0.2/plover_vipe/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 11:59:12.086836 plover_vipe-1.0.2/plover_vipe/dictionaries/
+-rw-rw-rw-   0        0        0     1033 2024-04-15 18:48:45.000000 plover_vipe-1.0.2/plover_vipe/dictionaries/vipe_commands.json
+-rw-rw-rw-   0        0        0   279680 2024-05-25 09:47:47.000000 plover_vipe-1.0.2/plover_vipe/dictionaries/vipe_main.json
+-rw-rw-rw-   0        0        0     5076 2024-05-21 20:48:23.000000 plover_vipe-1.0.2/plover_vipe/system.py
+drwxrwxrwx   0        0        0        0 2024-05-25 11:59:12.089859 plover_vipe-1.0.2/plover_vipe.egg-info/
+-rw-rw-rw-   0        0        0     2081 2024-05-25 11:59:11.000000 plover_vipe-1.0.2/plover_vipe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-05-25 11:59:11.000000 plover_vipe-1.0.2/plover_vipe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 11:59:11.000000 plover_vipe-1.0.2/plover_vipe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-25 11:59:11.000000 plover_vipe-1.0.2/plover_vipe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-25 11:59:11.000000 plover_vipe-1.0.2/plover_vipe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-25 11:59:11.000000 plover_vipe-1.0.2/plover_vipe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-23 21:44:32.000000 plover_vipe-1.0.2/plover_vipe.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      932 2024-05-25 11:59:12.101825 plover_vipe-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       63 2024-05-20 19:03:31.000000 plover_vipe-1.0.2/setup.py
+-rw-rw-rw-   0        0        0      146 2024-05-20 19:03:31.000000 plover_vipe-1.0.2/tox.ini
```

### Comparing `plover_vipe-1.0.1/LICENSE` & `plover_vipe-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_vipe-1.0.1/PKG-INFO` & `plover_vipe-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover_vipe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Norwegian realtime system for Plover
 Home-page: https://github.com/nikolasnjerve/Plover__Vipe
 Author-email: nikolasnjerve@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: plover plover_plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
@@ -21,14 +21,25 @@
 ==========================
 
 Vipe (Norwegian stenography system) support for Plover.
 
 It remaps W to V and Z to N. I have also added some simple ortography rules.
 
 
+The steno keyboard chart. 
+--------------------------
+
+This chart contains the letters for norwegian steno
+https://docs.google.com/drawings/d/1m3cIkRPlEk2SmmVI_mmRBNIiuxUh-wDy2_A_Pn_ZUZQ/edit?usp=sharing
+
+
+this chart contains most of the letter combinations
+https://docs.google.com/drawings/d/1TlvdrWSf1BHJG6P3KkEr4j49XLYwzMm85dw4BtpkfPo/edit?usp=sharing
+
+
 
 Recommended Usage
 -----------------
 
 Since the Vipe dictionary will change in the future, it it highly recommended to create a separate dictionary with your own mappings.
 
 
@@ -43,15 +54,15 @@
 
 	.\plover_console.exe -s plover_plugins install git+https://github.com/nikolasnjerve/Plover__Vipe
 
 Mac
 
 .. code:: bash
 
-	/Applications/Plover.app/Contents/MacOS/Plover -s plover_plugins install <path-to-plover-vipe-git-repo>
+	/Applications/Plover.app/Contents/MacOS/Plover -s plover_plugins install https://github.com/nikolasnjerve/Plover__Vipe
 
 
 Special Thanks
 --------------
 
 Special thanks to Martin Koerner for letting me use Regenpfeifer as a template for Vipe.
```

### Comparing `plover_vipe-1.0.1/plover_vipe/dictionaries/vipe_commands.json` & `plover_vipe-1.0.2/plover_vipe/dictionaries/vipe_commands.json`

 * *Files identical despite different names*

### Comparing `plover_vipe-1.0.1/plover_vipe/dictionaries/vipe_main.json` & `plover_vipe-1.0.2/plover_vipe/dictionaries/vipe_main.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942658479320932%*

 * *Differences: {"'AF/SKVREU'": "'avgi'",*

 * * "'AN/ON/SE'": "'annonse'",*

 * * "'EN/-R/SHEU'": "'energi'",*

 * * "'EN/ER/SHEU/PVOEU/RAU'": "'energibyrå'",*

 * * "'ERN/SHEU'": "'energi'",*

 * * "'ERN/SHEU/PABG/-R'": "'energipakker'",*

 * * "'ERN/SHEU/POL/TEUBG'": "'energipolitikk'",*

 * * "'ERN/SHEU/POL/TEUBGN'": "'energipolitikken'",*

 * * "'ERN/SHEU/PVOEU/RAU'": "'energibyrå'",*

 * * "'EUL/PROUF'": "'ildprøve'",*

 * * "'EUL/PROUFN'": "'ildprøven'",*

 * * "'EUN/PVOEUG/TKE'": "'innebygde'",*

 * * "'EUN/STEN/TKEU'": "'innstendig'",*

 * * "'EUN/TPOURT/E'": "'innførte'",*

 * * "'HOEUR/SEU/A'": […]*

```diff
@@ -564,14 +564,15 @@
     "AF/SHRUT/-R": "avslutter",
     "AF/SHRUT/-S": "avsluttes",
     "AF/SHRUT/E": "avslutte",
     "AF/SHRUT/ET": "avsluttet",
     "AF/SHRUT/TPH-G": "avslutning",
     "AF/SHRUT/TPH-GN": "avslutningen",
     "AF/SHRUTS": "avsluttes",
+    "AF/SKVREU": "avgi",
     "AF/SKVREUF/TER": "avgifter",
     "AF/SKVREUFT": "avgift",
     "AF/SKVROR/E": "avgjorde",
     "AF/SKVRORT": "avgjort",
     "AF/SKVROU/RE": "avgj\u00f8re",
     "AF/SKVROUR": "avgj\u00f8r",
     "AF/SKVROUR/EL/SEN": "avgj\u00f8relsen",
@@ -867,14 +868,15 @@
     "AN/KOEPL": "ankomme",
     "AN/KON/TKA": "anakonda",
     "AN/KOPL": "ankom",
     "AN/KOPL/E": "ankomme",
     "AN/KOPL/TPHE": "ankommende",
     "AN/KOPLTS": "ankomst",
     "AN/OEU/A": "And\u00f8ya",
+    "AN/ON/SE": "annonse",
     "AN/ON/SER/TE": "annonserte",
     "AN/OPB": "andunge",
     "AN/OPB/E": "andunge",
     "AN/PHA/SHON": "animasjon",
     "AN/PHA/SHON/TPEUPL": "animasjonsfilm",
     "AN/PHA/TOUR": "animat\u00f8r",
     "AN/PHAFBG": "animalsk",
@@ -1585,18 +1587,20 @@
     "EL/TKRE/OPL/SORG/-N": "eldreomsorgen",
     "EL/TREUS/TET": "elektrisitet",
     "EL/VA": "elva",
     "EL/VE": "elleve",
     "EL/VEUS": "Elvis",
     "ELGS/TPHE": "elskende",
     "EN": "enn",
+    "EN/-R/SHEU": "energi",
     "EN/-R/TKPVEU/VERBG": "energiverk",
     "EN/A": "enda",
     "EN/E": "ende",
     "EN/EN": "enden",
+    "EN/ER/SHEU/PVOEU/RAU": "energibyr\u00e5",
     "EN/ER/TKPVEU": "energi",
     "EN/HET": "enhet",
     "EN/HET/-R": "enheter",
     "EN/KHRED/TPH-G": "innledning",
     "EN/PVUD/SKVREUFR": "anbudsgiver",
     "EN/S/TE": "eneste",
     "EN/SEU/TKEU": "ensidig",
@@ -1684,14 +1688,19 @@
     "ER/TPARG": "erfaring",
     "ERB": "enger",
     "ERB/EUBG": "aerobic",
     "ERBG": "{erke^}",
     "ERDN": "ender",
     "ERG/SUN": "Egersund",
     "ERG/TPHO/PHEU": "ergonomi",
+    "ERN/SHEU": "energi",
+    "ERN/SHEU/PABG/-R": "energipakker",
+    "ERN/SHEU/POL/TEUBG": "energipolitikk",
+    "ERN/SHEU/POL/TEUBGN": "energipolitikken",
+    "ERN/SHEU/PVOEU/RAU": "energibyr\u00e5",
     "ERN/SOUBG/E": "unders\u00f8ke",
     "ERT": "etter",
     "ERT/HROEUS/-R": "etterlyser",
     "ERT/PAU": "etterp\u00e5",
     "ERT/PHEUD": "ettermiddag",
     "ERT/PHEUD/-N": "ettermiddagen",
     "ERT/SEN/E": "ettersende",
@@ -1780,14 +1789,16 @@
     "EUF/ER/SEN": "Iversen",
     "EUF/REU": "ivrig",
     "EUFN/STER/-G": "investering",
     "EUFPL": "i forbindelse med",
     "EUFR": "iver",
     "EUL/E": "ile",
     "EUL/HRE": "ille",
+    "EUL/PROUF": "ildpr\u00f8ve",
+    "EUL/PROUFN": "ildpr\u00f8ven",
     "EUL/VARS/HREN": "illevarslende",
     "EUN": "inn",
     "EUN/-N/TPOR": "innenfor",
     "EUN/E": "inne",
     "EUN/EN": "innen",
     "EUN/EU": "inni",
     "EUN/HOL": "innhold",
@@ -1812,14 +1823,15 @@
     "EUN/PHELG/-R": "innmeldinger",
     "EUN/PVAE/RER": "inneb\u00e6rer",
     "EUN/PVAER/E": "inneb\u00e6re",
     "EUN/PVHRATN": "innblandet",
     "EUN/PVHREUBG": "innblikk",
     "EUN/PVOEUG/-R/TPHE": "innbyggerne",
     "EUN/PVOEUG/RE": "innbyggere",
+    "EUN/PVOEUG/TKE": "innebygde",
     "EUN/PVRUD": "innbrudd",
     "EUN/ROUPL/E": "innr\u00f8mme",
     "EUN/ROUPL/ER": "innr\u00f8mmer",
     "EUN/ROUPL/ET": "innr\u00f8mmet",
     "EUN/SAT/SEN": "innsatsen",
     "EUN/SE": "innse",
     "EUN/SER": "innser",
@@ -1832,14 +1844,15 @@
     "EUN/SKVREN/OUR": "ingeni\u00f8r",
     "EUN/SKVREUBG": "inngikk",
     "EUN/SKVROU": "innsj\u00f8",
     "EUN/SOEUN": "innsyn",
     "EUN/SPEUL": "innspill",
     "EUN/SPRA/SHOSN/KHEULD": "inspirasjonskilde",
     "EUN/STA/HRA/SHON": "installasjon",
+    "EUN/STEN/TKEU": "innstendig",
     "EUN/STEU/TUT": "institutt",
     "EUN/STEUL/-G": "innstilling",
     "EUN/STEULG": "innstilling",
     "EUN/STEULG/-N": "innstillingen",
     "EUN/STEULT": "innstilt",
     "EUN/STRU/ER/E": "instruere",
     "EUN/STRU/PHETN": "instrument",
@@ -1895,14 +1908,15 @@
     "EUN/TPOR/PHE/RER": "informerer",
     "EUN/TPOR/PHER/E": "informere",
     "EUN/TPOR/PHERT": "informert",
     "EUN/TPOR/TPHA/SKVRON": "informasjon",
     "EUN/TPOU/RES": "innf\u00f8res",
     "EUN/TPOURG": "innf\u00f8ring",
     "EUN/TPOURT": "innf\u00f8rt",
+    "EUN/TPOURT/E": "innf\u00f8rte",
     "EUN/TR/SKVRU/TPHE": "intervjuene",
     "EUN/TR/SKVRUR": "intervjuer",
     "EUN/TRE": "inntre",
     "EUN/TRE/SATN": "interessant",
     "EUN/TRE/SATN/E": "interessante",
     "EUN/TRE/SE": "interesse",
     "EUN/TRE/SER/-R": "interesserer",
@@ -2293,14 +2307,15 @@
     "HOEUG/HREU/E": "hyggelige",
     "HOEUG/HREU/RE": "hyggeligere",
     "HOEUG/HREU/STE": "hyggeligeste",
     "HOEUL/-R": "hyler",
     "HOEUL/E": "hylle",
     "HOEUL/S-T": "hyllest",
     "HOEUR/RAD/KALT": "h\u00f8yreradikalt",
+    "HOEUR/SEU/A": "h\u00f8yresida",
     "HOEURD": "h\u00f8yder",
     "HOEURL": "hyler",
     "HOEUT": "h\u00f8yt",
     "HOEUT/A": "hytta",
     "HOEUT/E": "hytte",
     "HOEUTS": "h\u00f8yst",
     "HOF": "hoff",
@@ -2432,14 +2447,15 @@
     "HRAEUD": "leid",
     "HRAEUF": "Leif",
     "HRAF": "lav",
     "HRAF/-R": "laver",
     "HRAF/E": "lave",
     "HRAF/STE": "laveste",
     "HRAFT": "lavt",
+    "HRAFT/E": "lafte",
     "HRAFT/PVEUL": "lastebil",
     "HRAG": "lag",
     "HRAG/ETS": "lagets",
     "HRAG/PHAN/RET": "lagmannsrett",
     "HRAG/R-G": "lagring",
     "HRAG/RET": "lagret",
     "HRAG/T": "laget",
@@ -2448,14 +2464,15 @@
     "HRAGT": "laget",
     "HRAN": "land",
     "HRAN/E": "landet",
     "HRAN/EN/E": "landene",
     "HRAN/ETS": "landets",
     "HRAN/HRAG": "landslag",
     "HRAN/PHOU/TE": "landsm\u00f8te",
+    "HRAN/PHOUT/VE/TABG": "landsm\u00f8tevedtak",
     "HRAN/PVRUBG": "landbruk",
     "HRAN/PVRUBG/E": "landbruket",
     "HRAN/PVRUBG/TKEP/E": "landbruksdepartementet",
     "HRAN/SERT": "lansert",
     "HRAN/SERT/E": "lanserte",
     "HRAN/SKAP": "landskap",
     "HRAN/SKAP/E": "landskapet",
@@ -2557,14 +2574,15 @@
     "HRE/VERT/E": "leverte",
     "HREBG": "lek",
     "HREBG/-R": "leker",
     "HREBG/E": "leke",
     "HREBG/TPHES": "Leknes",
     "HREBGS/AN/TKER": "Alexander",
     "HRED": "led",
+    "HRED/-L/SEN": "ledelsen",
     "HRED/-R/TPHE": "lederne",
     "HRED/TPH-G/-R": "ledninger",
     "HRED/TPHE": "ledende",
     "HREF": "lev",
     "HREF/RAN/TKOUR": "leverand\u00f8r",
     "HREF/RAN/TKOUR/-R": "leverand\u00f8rer",
     "HREF/TKE": "levde",
@@ -2782,14 +2800,15 @@
     "HROUTS": "l\u00f8st",
     "HRU": "lue",
     "HRU/EU/SE": "Louise",
     "HRU/HREU": "lille",
     "HRU/RE": "lure",
     "HRU/RER": "lurer",
     "HRUBG/-N/PVURG": "Luxembourg",
+    "HRUBG/-R": "lukker",
     "HRUBG/E/TKE": "lukkede",
     "HRUBG/KET": "lukket",
     "HRUBG/TE": "lukte",
     "HRUBG/TER": "lukter",
     "HRUBG/TKE": "lukkede",
     "HRUD/VEUBG/SEN": "Ludvigsen",
     "HRUDN": "lund",
@@ -2945,14 +2964,15 @@
     "KARPL/OEU": "Karm\u00f8y",
     "KART": "kart",
     "KART/E": "carte",
     "KART/E/TPHE/PHU": "carte-meny",
     "KART/HREG/E": "kartlegge",
     "KAS/-R": "kasser",
     "KAS/E/RER": "kasserer",
+    "KAS/PVEUL": "kassebil",
     "KAS/ROL": "kaserolle",
     "KAS/TE": "kaste",
     "KASN": "kassen",
     "KAT": "katt",
     "KAT/REU/TPHE": "Kathrine",
     "KAT/TKPVO/REUN": "kategorien",
     "KATN/-R": "kanter",
@@ -3107,14 +3127,15 @@
     "KHREU/TPABGS": "klimaks",
     "KHREUBG/E": "klikke",
     "KHREUP": "klipp",
     "KHRO*PL": "klump",
     "KHRO/KA": "klokka",
     "KHRO/KEN": "klokken",
     "KHRO/REUD": "klorid",
+    "KHRO/TPHE": "klone",
     "KHROBG/A": "klokken",
     "KHROEU/PA": "klypa",
     "KHROEU/PE": "klype",
     "KHRORG": "klogger",
     "KHROS": "kloss",
     "KHROS/TER": "kloster",
     "KHROU/VER": "kl\u00f8ver",
@@ -3365,27 +3386,30 @@
     "KRA/PHEUL/A": "Camilla",
     "KRAF": "krav",
     "KRAF/E": "kravet",
     "KRAF/TEU": "kraftig",
     "KRAF/TEU/E": "kraftige",
     "KRAF/TPHE": "kravene",
     "KRAFT": "kraft",
+    "KRAFT/PHAR/KED/E": "kraftmarkedet",
+    "KRAFT/POL/TEUBGN": "kraftpolitikken",
     "KRAFT/VERBG": "kraftverk",
     "KRAG/ROU": "Krager\u00f8",
     "KRAL/REUN/E": "Cathrine",
     "KRAN": "kran",
     "KRAN/TKA": "Canada",
     "KRAN/TO/TPHA": "Cantona",
     "KRAP/HREN": "Cappelen",
     "KRAPB/-L": "krangel",
     "KRAPB/HRE": "krangle",
     "KRAPBL": "krangel",
     "KRAPL/PUS": "campus",
     "KRARL": "Carl",
     "KRARL/SEN": "Carlsen",
+    "KRAS": "krass",
     "KRE/KREUL/SKVRE": "Cecilie",
     "KRE/TEUF": "kreativ",
     "KRE/VE": "kreve",
     "KRE/VER": "krever",
     "KRE/VET": "krevet",
     "KRED/KAFN": "kreditkassen",
     "KREF/-S": "kreves",
@@ -3619,14 +3643,15 @@
     "OEU/A": "\u00f8ya",
     "OEU/E": "\u00f8ye",
     "OEU/PVHREUBG": "\u00f8yeblikk",
     "OEU/PVHREUBG/E": "\u00f8yeblikket",
     "OEU/STAEUN": "\u00d8ystein",
     "OEU/TKPVARN": "\u00d8ygarden",
     "OEU/TPHE": "\u00f8yne",
+    "OEU/TPHE/TPHE": "\u00f8ynene",
     "OEU/VEUN": "\u00d8yvind",
     "OEUBG/TPHO/PHEUN": "\u00f8konomien",
     "OEUBGSN": "\u00f8ksen",
     "OEUN": "\u00f8yen",
     "OEURBG/SHAU/TPHOUR/T": "yrkessj\u00e5f\u00f8r",
     "OEUT": "\u00f8yet",
     "OEUT/E": "yte",
@@ -4045,14 +4070,15 @@
     "PA/REUS": "Paris",
     "PA/RO/TKEUN": "parodien",
     "PA/SE": "passe",
     "PA/SER": "passer",
     "PA/TPHEL": "panel",
     "PA/TPHEUBG": "panikk",
     "PABG/-R": "pakker",
+    "PABG/A": "pakka",
     "PABG/E": "pakke",
     "PABG/KER": "pakker",
     "PABG/STAN": "Pakistan",
     "PABGT": "pakket",
     "PADN/PHEUN": "pandemien",
     "PAEU/HR-G": "peiling",
     "PAEU/HREUPB": "peiling",
@@ -4065,14 +4091,17 @@
     "PAN/-R": "panner",
     "PAN/E": "panne",
     "PAN/EN": "pannen",
     "PAN/TKE/PHEUN": "pandemien",
     "PAN/TPHE": "pannene",
     "PAN/TPHEN": "pannen",
     "PAOR/TKEUN": "parodien",
+    "PAOU/KE": "pauke",
+    "PAOU/SE": "pause",
+    "PAOUBG/TPHE": "paukene",
     "PAR": "par",
     "PAR/A/SOEUBG/HRO/TKPVEUN": "parapsykologien",
     "PAR/A/SOEUBG/HROG/SKE": "parapsykologiske",
     "PAR/E": "paret",
     "PAR/HRA/PHETN/E": "parlamentet",
     "PAR/HRELT": "parallelt",
     "PAR/KEN": "parken",
@@ -4115,15 +4144,15 @@
     "PAU/PEBGT": "p\u00e5pekt",
     "PAU/PERBG": "p\u00e5peker",
     "PAU/PHEUN/HR/SE": "p\u00e5minnelse",
     "PAU/PHEUN/HR/SER": "p\u00e5minnelser",
     "PAU/PVUD": "p\u00e5bud",
     "PAU/RAEUN": "p\u00e5regne",
     "PAU/ROUR/TPHE": "p\u00e5r\u00f8rende",
-    "PAU/SE": "pause",
+    "PAU/SE": "p\u00e5se",
     "PAU/STAN": "p\u00e5stand",
     "PAU/STAN/-N": "p\u00e5standen",
     "PAU/STAN/-R": "p\u00e5stander",
     "PAU/STAN/TPHE": "p\u00e5standene",
     "PAU/THRE/PHOEUDN/HET": "p\u00e5talemyndigheten",
     "PAU/TKPVAU": "p\u00e5g\u00e5",
     "PAU/TKPVAU/TPHE": "p\u00e5g\u00e5ende",
@@ -4656,14 +4685,15 @@
     "PHORD/-R/TPHE": "morderne",
     "PHORN/TKAG/TPH-S": "morgendagens",
     "PHORTN": "Morten",
     "PHOS/KVA": "Moskva",
     "PHOS/TER": "moster",
     "PHOSN": "Mons",
     "PHOT": "mot",
+    "PHOT/KREFT/TPHE": "motkreftene",
     "PHOT/SAT/E": "motsatte",
     "PHOT/SET": "motsette",
     "PHOT/SET/TPH-G": "motsetning",
     "PHOT/STAN": "motstand",
     "PHOT/STAN/TKER": "motstander",
     "PHOT/STAN/TKRE": "motstandere",
     "PHOT/TA": "motta",
@@ -4974,14 +5004,15 @@
     "PROD/SER/-S": "produseres",
     "PROD/SERT": "produsert",
     "PROD/SETN/-R": "produsenter",
     "PROD/SHON": "produksjon",
     "PROD/UBG/TEUF": "produktiv",
     "PROEUF/TKE": "pr\u00f8vde",
     "PROF": "profesjonell",
+    "PROF/HRERT": "profilert",
     "PROF/KA/SHON": "provokasjon",
     "PROF/SHO/TPHEL": "profesjonell",
     "PROF/SHO/TPHEL/E": "profesjonelle",
     "PROG/HRE/TKER": "programleder",
     "PROG/HRED/-R": "programleder",
     "PROG/RA/PHERG/-N": "programmeringen",
     "PROT/KOL/-N": "protokollen",
@@ -5394,14 +5425,15 @@
     "PVEUL/PARBG/-N": "bilparken",
     "PVEUL/SKVRE": "billige",
     "PVEUL/SKVRE/RE": "billigere",
     "PVEUL/TK-T": "bildet",
     "PVEUL/TKE": "bilde",
     "PVEUL/TKE/TEBGS": "billedtekst",
     "PVEUL/TKE/TPHE": "bildene",
+    "PVEUL/TKER": "bilder",
     "PVEUL/TPHE": "bilene",
     "PVEUN": "bind",
     "PVEUN/-G": "binding",
     "PVEUN/E": "binde",
     "PVEUN/E/TPHE": "bindene",
     "PVEUR/TKPVER": "Birger",
     "PVEUR/TKPVEUT/E": "Birgitte",
@@ -5449,14 +5481,15 @@
     "PVHRO/TKEU/E": "blodige",
     "PVHRO/TOURBT/SKVRE": "blodt\u00f8rstige",
     "PVHROPL/STER": "blomster",
     "PVHROPL/STREUPB": "blomstring",
     "PVHROPLS": "blomst",
     "PVHROUD/-G": "bl\u00f8dning",
     "PVHROUD/TPHE": "bl\u00f8dende",
+    "PVHROUF": "bl\u00f8ff",
     "PVHRUN/TKER": "blunder",
     "PVHRUS": "blues",
     "PVO": "bo",
     "PVO*D": "bodd",
     "PVO*EU": "Bye",
     "PVO*R": "bord",
     "PVO*R/SKVREUBG": "bordslkikk",
@@ -6096,14 +6129,15 @@
     "ROS/-R": "roser",
     "ROSN/PVORG": "rosenborg",
     "ROT": "rot",
     "ROU": "r\u00f8d",
     "ROU/HRARSN": "R\u00f8d-larsen",
     "ROU/KET": "r\u00f8ket",
     "ROU/ROS": "R\u00f8ros",
+    "ROU/TKPVROUN": "r\u00f8dgr\u00f8nn",
     "ROU/TROEU/E": "r\u00f8dtr\u00f8ye",
     "ROU/VEUN": "r\u00f8dvin",
     "ROU/VEUN/SAUS": "r\u00f8dvinssaus",
     "ROUBG": "r\u00f8k",
     "ROUFR": "r\u00f8ver",
     "ROUPLT": "r\u00f8mt",
     "ROUR": "r\u00f8r",
@@ -6604,36 +6638,39 @@
     "SHO*UN": "skj\u00f8nn",
     "SHOBG": "sjokk",
     "SHOBG/ER/TPHE": "sjokkerende",
     "SHOBG/ERT": "sjokkert",
     "SHOBG/HRA/TKE": "sjokolade",
     "SHOEU": "sky",
     "SHOEU/T-R": "skyter",
+    "SHOEU/TE": "skyte",
     "SHOEU/TER": "sk\u00f8yter",
     "SHOEUF": "skyv",
     "SHOEUG/-N": "skyggen",
     "SHOEUGN": "skyggen",
     "SHOEUL": "skyld",
     "SHOEUL/-N": "skylden",
     "SHOEUL/TE": "skyldte",
     "SHOEUL/TKEU": "skyldig",
     "SHOEULS": "skyldtes",
     "SHOEUN/E": "skyndte",
     "SHOEURT": "skyter",
+    "SHOEUT": "skyt",
     "SHOEUT/-G": "skyting",
     "SHOEUT/E": "skyte",
     "SHOR/TPHA/HREUFT": "journalist",
     "SHOR/TPHA/HREUFT/TPHE": "journalistene",
     "SHOR/TPHA/HREUS/TER": "journalister",
     "SHOR/TPHA/HREUTS/-N": "journalisten",
     "SHOU": "sj\u00f8",
     "SHOU/RER": "kj\u00f8rer",
     "SHOU/TPHE": "skj\u00f8nne",
     "SHOU/TPOLG": "sj\u00f8folk",
     "SHOUL": "sj\u00f8l",
+    "SHOUL/RAUD/RET": "sj\u00f8lr\u00e5derett",
     "SHOUN": "sj\u00f8en",
     "SHOUN/-R": "skj\u00f8nner",
     "SHOUN/ER": "skj\u00f8nner",
     "SHOUR": "skj\u00f8r",
     "SHOUR/TKAL": "Stj\u00f8rdal",
     "SHOUT": "skj\u00f8t",
     "SHOUTN": "skj\u00f8nt",
@@ -6718,14 +6755,15 @@
     "SKAF/ET": "skaffet",
     "SKAL": "skal",
     "SKAL/ET": "skallet",
     "SKAN/SKVRA": "Scania",
     "SKAN/TKAL": "skandale",
     "SKAN/TKEU/TPHAF/SKVRA": "skandinavia",
     "SKAP": "skap",
+    "SKAP/-R": "skaper",
     "SKAP/TE": "skapte",
     "SKAP/TPHE": "skapende",
     "SKAPL": "skam",
     "SKAPS": "skapes",
     "SKAPT": "skapt",
     "SKAR": "skar",
     "SKARD": "skader",
@@ -7505,14 +7543,15 @@
     "STEPL/R": "stemmer",
     "STEPL/TE": "stemte",
     "STEPL/TPH-G": "stemning",
     "STEPL/TPH-G/-N": "stemningen",
     "STEPL/TPH-G/EN": "stemningen",
     "STEPL/TPHE": "stemmene",
     "STEPL/TPHEUPB/EN": "stemningen",
+    "STER/KE": "sterke",
     "STER/KE/RE": "sterkere",
     "STER/KRE": "sterkere",
     "STERBG": "sterk",
     "STERBG/-T": "sterkt",
     "STERBG/ST": "sterkest",
     "STERBGT": "sterkt",
     "STERPL": "stemmer",
@@ -7692,14 +7731,15 @@
     "STPHEUL": "snill",
     "STPHEUL/HRE": "snille",
     "STPHEUL/RE": "snillere",
     "STPHEUT": "snitt",
     "STPHOU": "sn\u00f8",
     "STPHOUN": "sn\u00f8en",
     "STPHU": "snu",
+    "STPHU/OP/RA/SHON": "snuoperasjon",
     "STPHUD": "snudd",
     "STPHUD/E": "snudde",
     "STPHUN/TPOR/TPHUFT/EU": "snusfornuftig",
     "STPHUR": "snur",
     "STR*EBG": "strekk",
     "STR/PVRAN": "storebrand",
     "STRA/TEG/EUBGS": "strategisk",
@@ -7736,14 +7776,15 @@
     "STREFR": "strever",
     "STREPB": "streng",
     "STREPB/RE": "strengere",
     "STREPBT": "strengt",
     "STRES": "stress",
     "STREUD": "strid",
     "STREUD/-N": "striden",
+    "STREUD/TPH-S": "stridens",
     "STREUL": "tvil",
     "STREUPB/E": "strenge",
     "STREUPL": "stream",
     "STREUPL/E": "streame",
     "STROEUBG": "stryk",
     "STROEUN": "Stryn",
     "STROUBG": "str\u00f8k",
@@ -7773,14 +7814,15 @@
     "STUN": "stund",
     "STVAR/TE": "svarte",
     "SU/PERT": "supert",
     "SU/RE": "sure",
     "SUBG/SES": "suksess",
     "SUBG/SES/-N": "suksessen",
     "SUF/REN": "suveren",
+    "SUF/REN/TET": "suverenitet",
     "SUF/RETN": "suverent",
     "SUL/TET": "sultet",
     "SUL/TPAT": "sulfat",
     "SULT": "sult",
     "SULT/TPHE": "sultne",
     "SUN": "sund",
     "SUN/HORD/HRAN": "Sunnhordland",
@@ -8270,14 +8312,16 @@
     "TKE/PHO/KRA/TEU": "demokrati",
     "TKE/PHON/-R": "demoner",
     "TKE/PHON/SKE": "demoniske",
     "TKE/PHON/STER/ER": "demonstrere",
     "TKE/PHON/STRE/RE": "demonstrere",
     "TKE/PHORN": "demoner",
     "TKE/PVAT": "debatt",
+    "TKE/PVAT/-N": "debatten",
+    "TKE/PVATN": "debatten",
     "TKE/PVOEU": "debut",
     "TKE/PVU/TER/TE": "debuterte",
     "TKE/RE": "dere",
     "TKE/RES": "deres",
     "TKE/SAER": "dessert",
     "TKE/SAOEUN": "design",
     "TKE/SEPL/PVER": "desember",
@@ -8651,14 +8695,18 @@
     "TKPVRAEUD": "greid",
     "TKPVRAEUP": "greip",
     "TKPVRAEUT": "greit",
     "TKPVRAF/PHA/SHEUN": "gravemaskin",
     "TKPVRAFR": "graver",
     "TKPVRAN": "gran",
     "TKPVRAN/AUSN": "Gran\u00e5sen",
+    "TKPVRAN/TEUFT": "garantist",
+    "TKPVRAN/TEUFT/-R": "garantister",
+    "TKPVRAN/TEUN": "garantien",
+    "TKPVRAN/TEUS/TEN": "garantisten",
     "TKPVRAN/TKE": "grande",
     "TKPVRAPL": "gram",
     "TKPVRAT/HRE/RER": "gratulerer",
     "TKPVRAT/HRER/ER": "gratulerer",
     "TKPVRAU": "gr\u00e5",
     "TKPVRAU/TE": "gr\u00e5te",
     "TKPVRAU/TER": "gr\u00e5ter",
@@ -8855,14 +8903,15 @@
     "TOE/REUN": "teorien",
     "TOEF": "Tove",
     "TOEU/PER": "typer",
     "TOEU/TKHREU": "tydelig",
     "TOEUBG": "tykk",
     "TOEUBG/-L/SE": "tykkelse",
     "TOEUD/E": "tyde",
+    "TOEUD/HREU/RE": "tydeligere",
     "TOEUD/HREU/VEUS": "tydeligvis",
     "TOEUF": "tyv",
     "TOEUF/AURG": "tyve\u00e5ring",
     "TOEUF/REU": "tyveri",
     "TOEUF/TPHE": "tyvene",
     "TOEUG/EUS": "tyggis",
     "TOEUN/-N": "tynn",
@@ -9053,14 +9102,15 @@
     "TPAR/SUN": "Farsund",
     "TPAR/TKPVE": "farge",
     "TPAR/TOEU": "fart\u00f8y",
     "TPAR/TOEU/E": "fart\u00f8yet",
     "TPAR/VAN": "farvann",
     "TPAR/VEL": "farvel",
     "TPARBG/TPHES": "Fagernes",
+    "TPARD": "fader",
     "TPARG/-R": "farger",
     "TPARG/ER": "farger",
     "TPARG/REUBG/E": "fargerike",
     "TPARN": "faren",
     "TPART": "fart",
     "TPART/-N": "farten",
     "TPAS/TE": "faste",
@@ -9099,14 +9149,15 @@
     "TPEL/ES/SKAP": "fellesskap",
     "TPEL/HRES": "felles",
     "TPEL/SKAP/E": "fellesskapet",
     "TPEL/TE": "felte",
     "TPEL/TET": "feltet",
     "TPELG": "felg",
     "TPELS": "felles",
+    "TPELS/TPOR/PVUN/E": "Fellesforbundet",
     "TPELT": "felt",
     "TPEN/PHEN": "fenomen",
     "TPEN/PHEN/-R": "fenomener",
     "TPEN/PHEN/-T": "fenomenet",
     "TPEN/PHEN/TPHE": "fenomenene",
     "TPEN/PHERN": "fenomener",
     "TPEN/PHETN": "fenomenet",
@@ -9494,14 +9545,15 @@
     "TPHOUD/VEN/TKEU": "n\u00f8dvendig",
     "TPHOURD/TE": "nerdete",
     "TPHOUT": "n\u00f8dt",
     "TPHR-F/TPH-R": "telefonnummer",
     "TPHR-PBLG": "fly",
     "TPHR/KVR/K-T/TPHEUPB": "flyktning",
     "TPHRABGS": "flaks",
+    "TPHRABGS/TUT": "flasketut",
     "TPHRAET": "flate",
     "TPHRAFBG/-R": "flasker",
     "TPHRAFBG/E": "flaske",
     "TPHRAG": "flagg",
     "TPHRAGT": "flagget",
     "TPHRAOU": "flau",
     "TPHRAOUT": "flaut",
@@ -9515,14 +9567,15 @@
     "TPHREBG": "flekk",
     "TPHREBG/STKPVROR": "Flekkefjord",
     "TPHREBGS/EU/PVELT": "fleksibelt",
     "TPHREBGS/PVEUL/TET": "fleksibilitet",
     "TPHREBGS/PVHRE": "fleksible",
     "TPHREG": "anlegg",
     "TPHRER": "fler",
+    "TPHRER/TAL": "flertall",
     "TPHRER/TAL/E": "flertallet",
     "TPHRES/HRAN": "Flesland",
     "TPHRES/TE": "fleste",
     "TPHRET": "flett",
     "TPHRET/-R": "fletter",
     "TPHREU": "fly",
     "TPHREU/E": "flyet",
@@ -9803,14 +9856,15 @@
     "TPOR/SVA/RE": "forsvare",
     "TPOR/SVA/RET": "forsvaret",
     "TPOR/SVAR": "forsvar",
     "TPOR/SVAR/E": "forsvaret",
     "TPOR/SVAR/ER": "forsvarer",
     "TPOR/SVAR/HREU": "forsvarlig",
     "TPOR/SVAR/PHEUN/STER": "forsvarsminister",
+    "TPOR/SVAR/RE": "forsvarere",
     "TPOR/SVAR/TKEP": "forsvarsdepartementet",
     "TPOR/SVATN": "forsvant",
     "TPOR/SVEUN/-R": "forsvinner",
     "TPOR/T/PVRED/SE": "forberedelse",
     "TPOR/TA": "foreta",
     "TPOR/TAL/TE": "fortalte",
     "TPOR/TALT": "fortalt",
@@ -9851,14 +9905,15 @@
     "TPOR/TPAT/REN": "forfatteren",
     "TPOR/TPAUL/E": "forf\u00f8lge",
     "TPOR/TPER/TKHREU": "forferdelig",
     "TPOR/TPERD/HR/SE": "forferdelse",
     "TPOR/TPHE/PVU": "Fornebu",
     "TPOR/TPHO*EUL/SE": "fornyelse",
     "TPOR/TPHOEU/-T": "fornyet",
+    "TPOR/TPHOEU/PVAR": "fornybar",
     "TPOR/TPHOEUD": "forn\u00f8yd",
     "TPOR/TPHUF/TEU": "fornuftig",
     "TPOR/TPHUFT": "fornuft",
     "TPOR/TRE": "fortere",
     "TPOR/TREBG/-R": "foretrekker",
     "TPOR/TRUBG/TPHE": "foretrukne",
     "TPOR/TVEUL/-T": "fortvilet",
@@ -9939,14 +9994,16 @@
     "TPOULT": "f\u00f8lt",
     "TPOUR": "f\u00f8r",
     "TPOUR/*E": "f\u00f8rre",
     "TPOUR/-R/PROUF/E": "f\u00f8rerpr\u00f8ve",
     "TPOUR/KORT": "f\u00f8rerkort",
     "TPOUR/STE": "f\u00f8rste",
     "TPOUR/TKE": "F\u00f8rde",
+    "TPOURG": "f\u00f8ring",
+    "TPOURG/-R": "f\u00f8ringer",
     "TPOURG/SON": "Ferguson",
     "TPOURL": "f\u00f8ler",
     "TPOURS/TE/SKVREPL": "f\u00f8rsthjelp",
     "TPOURT": "f\u00f8rt",
     "TPOURTS": "f\u00f8rst",
     "TPOURTS/PHA/TPHEN/SEUS": "f\u00f8rsteamanuensis",
     "TPOURTS/VOPL/TPHE": "f\u00f8rstkommende",
@@ -10321,14 +10378,15 @@
     "U/SED/KAN/HREU": "usedvanlig",
     "U/SEUBG/-R": "usikker",
     "U/SEUBG/R-T": "usikkert",
     "U/SEUBG/RE": "usikre",
     "U/SEURBG/HET": "usikkerhet",
     "U/SHOEUL/TKEU": "uskyldig",
     "U/SKOEL": "ungdomsskole",
+    "U/SOS/SKVRAL": "usosial",
     "U/T-N/TKOURS": "utend\u00f8rs",
     "U/TAL/SKVRE": "utallige",
     "U/TEPBG/HREU": "utenkelig",
     "U/TK": "utenriksdepartementet",
     "U/TKEUR": "utenriksdepartementet",
     "U/TPHEUBG": "unik",
     "U/TPHEUBG/E": "unike",
@@ -10424,14 +10482,15 @@
     "UT/AL/E": "uttale",
     "UT/ARB": "utarbeide",
     "UT/ARB/-T": "utarbeidet",
     "UT/E": "ute",
     "UT/EN": "uten",
     "UT/HRAEU/RE": "utleiere",
     "UT/HRAN": "utland",
+    "UT/HRAN/KAB/HREN/E": "utenlandskablene",
     "UT/HRAN/SK": "utenlandsk",
     "UT/HRASN/KE": "utenlandske",
     "UT/HRAUN": "utl\u00e5n",
     "UT/HREFRT": "utlevert",
     "UT/HREN/-G/-R": "utlendinger",
     "UT/HROUFT": "utl\u00f8st",
     "UT/HROUFT/E": "utl\u00f8ste",
@@ -10634,14 +10693,15 @@
     "VAFBGN": "vasken",
     "VAL/KA*PL": "valgkamp",
     "VAL/KA*PL/-N": "valgkampen",
     "VAL/KOPL/TE": "valgkomit\u00e9",
     "VAL/KOPL/TEN": "valgkomiteen",
     "VAL/SKRED": "valgskred",
     "VALG": "valg",
+    "VALG/E": "valget",
     "VALG/TPHE": "valgene",
     "VALGT": "valgt",
     "VALT": "valgt",
     "VAN": "vann",
     "VAN/AF/SKVREUFT": "vannavgift",
     "VAN/E": "vane",
     "VAN/E/TPHE": "vannene",
@@ -10665,14 +10725,15 @@
     "VAPL/POEUR": "vampyr",
     "VAR": "var",
     "VAR/EU": "varig",
     "VAR/OR/TPOUR": "varaordf\u00f8rer",
     "VAR/PHE": "varme",
     "VAR/PHEN": "varmen",
     "VAR/PHERBG": "varemerke",
+    "VAR/PVEUL": "varebil",
     "VAR/SEL": "varsel",
     "VAR/SHRET": "varslet",
     "VAR/SKVRA/SHON": "variasjon",
     "VAR/SKVRAN/TEN": "varianten",
     "VAR/SKVRAN/TER": "varianter",
     "VAR/SKVRER/ER": "varierer",
     "VAR/SKVRER/TE": "varierte",
@@ -10771,14 +10832,15 @@
     "VEN/E/TPHE": "vennene",
     "VEN/ER": "venner",
     "VEN/EUN/-R": "venninner",
     "VEN/EURN": "venninner",
     "VEN/HREU": "vennlig",
     "VEN/SKAP": "vennskap",
     "VEN/STRE": "venstre",
+    "VEN/STRE/SEU/A": "venstresida",
     "VEN/STRES": "venstres",
     "VEN/T-G": "venting",
     "VEN/T-R": "venter",
     "VEN/TE": "vente",
     "VEN/TES": "ventes",
     "VEN/TET": "ventet",
     "VEN/TEUPB": "venting",
@@ -10891,14 +10953,15 @@
     "VEUL/TKE": "vilde",
     "VEULD": "vil du",
     "VEULT": "vilt",
     "VEUN": "vin",
     "VEUN/-N": "vinden",
     "VEUN/-R/TPHE": "vinnerne",
     "VEUN/E": "vinne",
+    "VEUN/KRAFT": "vindkraft",
     "VEUN/PHON/POL/E": "vinmonopolet",
     "VEUN/RE": "vinnere",
     "VEUN/REN": "vinneren",
     "VEUN/STRA": "Vinstra",
     "VEUN/TE/REN": "vinteren",
     "VEUN/TER": "vinter",
     "VEUN/TKU/-R": "vinduer",
```

### Comparing `plover_vipe-1.0.1/plover_vipe/system.py` & `plover_vipe-1.0.2/plover_vipe/system.py`

 * *Files identical despite different names*

### Comparing `plover_vipe-1.0.1/plover_vipe.egg-info/PKG-INFO` & `plover_vipe-1.0.2/plover_vipe.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover_vipe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Norwegian realtime system for Plover
 Home-page: https://github.com/nikolasnjerve/Plover__Vipe
 Author-email: nikolasnjerve@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: plover plover_plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
@@ -21,14 +21,25 @@
 ==========================
 
 Vipe (Norwegian stenography system) support for Plover.
 
 It remaps W to V and Z to N. I have also added some simple ortography rules.
 
 
+The steno keyboard chart. 
+--------------------------
+
+This chart contains the letters for norwegian steno
+https://docs.google.com/drawings/d/1m3cIkRPlEk2SmmVI_mmRBNIiuxUh-wDy2_A_Pn_ZUZQ/edit?usp=sharing
+
+
+this chart contains most of the letter combinations
+https://docs.google.com/drawings/d/1TlvdrWSf1BHJG6P3KkEr4j49XLYwzMm85dw4BtpkfPo/edit?usp=sharing
+
+
 
 Recommended Usage
 -----------------
 
 Since the Vipe dictionary will change in the future, it it highly recommended to create a separate dictionary with your own mappings.
 
 
@@ -43,15 +54,15 @@
 
 	.\plover_console.exe -s plover_plugins install git+https://github.com/nikolasnjerve/Plover__Vipe
 
 Mac
 
 .. code:: bash
 
-	/Applications/Plover.app/Contents/MacOS/Plover -s plover_plugins install <path-to-plover-vipe-git-repo>
+	/Applications/Plover.app/Contents/MacOS/Plover -s plover_plugins install https://github.com/nikolasnjerve/Plover__Vipe
 
 
 Special Thanks
 --------------
 
 Special thanks to Martin Koerner for letting me use Regenpfeifer as a template for Vipe.
```

### Comparing `plover_vipe-1.0.1/setup.cfg` & `plover_vipe-1.0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6c6f 7665 725f 7669 7065 0d0a   = plover_vipe..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 310d  version = 1.0.1.
+00000020: 7665 7273 696f 6e20 3d20 312e 302e 320d  version = 1.0.2.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 204e  .description = N
 00000040: 6f72 7765 6769 616e 2072 6561 6c74 696d  orwegian realtim
 00000050: 6520 7379 7374 656d 2066 6f72 2050 6c6f  e system for Plo
 00000060: 7665 720d 0a6c 6f6e 675f 6465 7363 7269  ver..long_descri
 00000070: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
 00000080: 4144 4d45 2e72 7374 0d0a 6175 7468 6f72  ADME.rst..author
 00000090: 7320 3d20 4d61 7274 696e 204b 6f65 726e  s = Martin Koern
```


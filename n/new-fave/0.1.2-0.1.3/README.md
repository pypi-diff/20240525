# Comparing `tmp/new_fave-0.1.2.tar.gz` & `tmp/new_fave-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_fave-0.1.2.tar", max compression
+gzip compressed data, was "new_fave-0.1.3.tar", max compression
```

## Comparing `new_fave-0.1.2.tar` & `new_fave-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2024-02-21 16:07:06.894339 new_fave-0.1.2/LICENSE
--rw-r--r--   0        0        0     3228 2024-05-22 14:03:09.249328 new_fave-0.1.2/README.md
--rw-r--r--   0        0        0     1595 2024-05-23 15:58:20.109870 new_fave-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      574 2024-05-21 21:01:28.578047 new_fave-0.1.2/src/new_fave/__init__.py
--rw-r--r--   0        0        0    12368 2024-05-21 21:01:28.578205 new_fave-0.1.2/src/new_fave/extract.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578240 new_fave-0.1.2/src/new_fave/measurements/__init__.py
--rw-r--r--   0        0        0    31010 2024-05-23 15:58:20.110092 new_fave-0.1.2/src/new_fave/measurements/vowel_measurement.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578638 new_fave-0.1.2/src/new_fave/optimize/__init__.py
--rw-r--r--   0        0        0     3803 2024-05-23 15:58:20.110310 new_fave-0.1.2/src/new_fave/optimize/optimize.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.579017 new_fave-0.1.2/src/new_fave/patterns/__init__.py
--rw-r--r--   0        0        0     2147 2024-05-21 21:01:28.579186 new_fave-0.1.2/src/new_fave/patterns/common_processing.py
--rw-r--r--   0        0        0     4841 2024-05-21 21:01:28.579358 new_fave-0.1.2/src/new_fave/patterns/fave_audio_textgrid.py
--rw-r--r--   0        0        0     5154 2024-05-21 21:01:28.579511 new_fave-0.1.2/src/new_fave/patterns/fave_corpus.py
--rw-r--r--   0        0        0     5626 2024-05-21 21:01:28.579682 new_fave-0.1.2/src/new_fave/patterns/fave_subcorpora.py
--rw-r--r--   0        0        0     6623 2024-05-21 21:01:28.579857 new_fave-0.1.2/src/new_fave/patterns/writers.py
--rw-r--r--   0        0        0     4801 2024-05-21 21:01:28.580184 new_fave-0.1.2/src/new_fave/resources/cmu2labov.yml
--rw-r--r--   0        0        0    11332 2024-05-21 21:01:28.580389 new_fave-0.1.2/src/new_fave/resources/cmu2phila.yml
--rw-r--r--   0        0        0      891 2024-05-21 21:01:28.580616 new_fave-0.1.2/src/new_fave/resources/cmu_parser.yml
--rw-r--r--   0        0        0      275 2024-05-23 15:58:20.110491 new_fave-0.1.2/src/new_fave/resources/fasttrack_config.yml
--rw-r--r--   0        0        0      427 2024-05-21 21:01:28.581070 new_fave-0.1.2/src/new_fave/resources/fave_measurement.yml
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581108 new_fave-0.1.2/src/new_fave/speaker/__init__.py
--rw-r--r--   0        0        0     4443 2024-05-21 21:01:28.581421 new_fave-0.1.2/src/new_fave/speaker/speaker.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581454 new_fave-0.1.2/src/new_fave/utils/__init__.py
--rw-r--r--   0        0        0       50 2024-05-21 21:01:28.581731 new_fave-0.1.2/src/new_fave/utils/corpus.py
--rw-r--r--   0        0        0      440 2024-05-21 21:01:28.581968 new_fave-0.1.2/src/new_fave/utils/fasttrack_config.py
--rw-r--r--   0        0        0     2516 2024-05-21 21:01:28.582099 new_fave-0.1.2/src/new_fave/utils/local_resources.py
--rw-r--r--   0        0        0     3082 2024-05-21 21:01:28.582378 new_fave-0.1.2/src/new_fave/utils/textgrid.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 new_fave-0.1.2/setup.py
--rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 new_fave-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-21 16:07:06.894339 new_fave-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3228 2024-05-25 14:31:32.569739 new_fave-0.1.3/README.md
+-rw-r--r--   0        0        0     1613 2024-05-25 19:29:40.565577 new_fave-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      574 2024-05-21 21:01:28.578047 new_fave-0.1.3/src/new_fave/__init__.py
+-rw-r--r--   0        0        0    12368 2024-05-21 21:01:28.578205 new_fave-0.1.3/src/new_fave/extract.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578240 new_fave-0.1.3/src/new_fave/measurements/__init__.py
+-rw-r--r--   0        0        0    31010 2024-05-25 19:08:04.140948 new_fave-0.1.3/src/new_fave/measurements/vowel_measurement.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578638 new_fave-0.1.3/src/new_fave/optimize/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-23 15:58:20.110310 new_fave-0.1.3/src/new_fave/optimize/optimize.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.579017 new_fave-0.1.3/src/new_fave/patterns/__init__.py
+-rw-r--r--   0        0        0     2147 2024-05-21 21:01:28.579186 new_fave-0.1.3/src/new_fave/patterns/common_processing.py
+-rw-r--r--   0        0        0     4841 2024-05-21 21:01:28.579358 new_fave-0.1.3/src/new_fave/patterns/fave_audio_textgrid.py
+-rw-r--r--   0        0        0     5154 2024-05-21 21:01:28.579511 new_fave-0.1.3/src/new_fave/patterns/fave_corpus.py
+-rw-r--r--   0        0        0     5626 2024-05-21 21:01:28.579682 new_fave-0.1.3/src/new_fave/patterns/fave_subcorpora.py
+-rw-r--r--   0        0        0     6623 2024-05-21 21:01:28.579857 new_fave-0.1.3/src/new_fave/patterns/writers.py
+-rw-r--r--   0        0        0     4801 2024-05-21 21:01:28.580184 new_fave-0.1.3/src/new_fave/resources/cmu2labov.yml
+-rw-r--r--   0        0        0    11332 2024-05-21 21:01:28.580389 new_fave-0.1.3/src/new_fave/resources/cmu2phila.yml
+-rw-r--r--   0        0        0      891 2024-05-21 21:01:28.580616 new_fave-0.1.3/src/new_fave/resources/cmu_parser.yml
+-rw-r--r--   0        0        0      275 2024-05-23 15:58:20.110491 new_fave-0.1.3/src/new_fave/resources/fasttrack_config.yml
+-rw-r--r--   0        0        0      427 2024-05-21 21:01:28.581070 new_fave-0.1.3/src/new_fave/resources/fave_measurement.yml
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581108 new_fave-0.1.3/src/new_fave/speaker/__init__.py
+-rw-r--r--   0        0        0     4443 2024-05-21 21:01:28.581421 new_fave-0.1.3/src/new_fave/speaker/speaker.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581454 new_fave-0.1.3/src/new_fave/utils/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-21 21:01:28.581731 new_fave-0.1.3/src/new_fave/utils/corpus.py
+-rw-r--r--   0        0        0      440 2024-05-21 21:01:28.581968 new_fave-0.1.3/src/new_fave/utils/fasttrack_config.py
+-rw-r--r--   0        0        0     2516 2024-05-21 21:01:28.582099 new_fave-0.1.3/src/new_fave/utils/local_resources.py
+-rw-r--r--   0        0        0     3082 2024-05-21 21:01:28.582378 new_fave-0.1.3/src/new_fave/utils/textgrid.py
+-rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 new_fave-0.1.3/setup.py
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 new_fave-0.1.3/PKG-INFO
```

### Comparing `new_fave-0.1.2/LICENSE` & `new_fave-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/README.md` & `new_fave-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/pyproject.toml` & `new_fave-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "new-fave"
-version = "0.1.2"
+version = "0.1.3"
 description = "New Vowel Extraction Suite"
 authors = ["JoFrhwld <jofrhwld@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "new_fave", from="src"}]
 homepage = "https://forced-alignment-and-vowel-extraction.github.io/new-fave/"
 repository = "https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave"
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 aligned-textgrid = "^0.6.6"
-fasttrackpy = "^0.4.5"
+fasttrackpy = "^0.4.6"
 numpy = "^1.26.4"
 tqdm = "^4.66.2"
 fave-recode = "^0.3.0"
 click = "^8.1.7"
 cloup = "^3.0.5"
 fave-measurement-point = "0.1.3"
 polars = "^0.20.18"
 xlsx2csv = "^0.8.2"
 python-magic = {version = "^0.4.27", markers = "sys_platform != 'win32'"}
 python-magic-bin = {version = "^0.4.14", markers = "sys_platform == 'win32'"}
+scipy = "^1.13.1"
 
 
 [tool.poetry.group.docs.dependencies]
 quartodoc = "^0.7.2"
 ipython = "^8.21.0"
 nbformat = "^5.9.2"
 jupyter = "^1.0.0"
```

### Comparing `new_fave-0.1.2/src/new_fave/__init__.py` & `new_fave-0.1.3/src/new_fave/__init__.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/extract.py` & `new_fave-0.1.3/src/new_fave/extract.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/measurements/vowel_measurement.py` & `new_fave-0.1.3/src/new_fave/measurements/vowel_measurement.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/optimize/optimize.py` & `new_fave-0.1.3/src/new_fave/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/patterns/common_processing.py` & `new_fave-0.1.3/src/new_fave/patterns/common_processing.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/patterns/fave_audio_textgrid.py` & `new_fave-0.1.3/src/new_fave/patterns/fave_audio_textgrid.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/patterns/fave_corpus.py` & `new_fave-0.1.3/src/new_fave/patterns/fave_corpus.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/patterns/fave_subcorpora.py` & `new_fave-0.1.3/src/new_fave/patterns/fave_subcorpora.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/patterns/writers.py` & `new_fave-0.1.3/src/new_fave/patterns/writers.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/resources/cmu2labov.yml` & `new_fave-0.1.3/src/new_fave/resources/cmu2labov.yml`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/resources/cmu2phila.yml` & `new_fave-0.1.3/src/new_fave/resources/cmu2phila.yml`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/resources/cmu_parser.yml` & `new_fave-0.1.3/src/new_fave/resources/cmu_parser.yml`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/speaker/speaker.py` & `new_fave-0.1.3/src/new_fave/speaker/speaker.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/utils/local_resources.py` & `new_fave-0.1.3/src/new_fave/utils/local_resources.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/src/new_fave/utils/textgrid.py` & `new_fave-0.1.3/src/new_fave/utils/textgrid.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.2/setup.py` & `new_fave-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,32 +15,33 @@
 package_data = \
 {'': ['*'], 'new_fave': ['resources/*']}
 
 install_requires = \
 ['aligned-textgrid>=0.6.6,<0.7.0',
  'click>=8.1.7,<9.0.0',
  'cloup>=3.0.5,<4.0.0',
- 'fasttrackpy>=0.4.5,<0.5.0',
+ 'fasttrackpy>=0.4.6,<0.5.0',
  'fave-measurement-point==0.1.3',
  'fave-recode>=0.3.0,<0.4.0',
  'numpy>=1.26.4,<2.0.0',
  'polars>=0.20.18,<0.21.0',
+ 'scipy>=1.13.1,<2.0.0',
  'tqdm>=4.66.2,<5.0.0',
  'xlsx2csv>=0.8.2,<0.9.0']
 
 extras_require = \
 {':sys_platform != "win32"': ['python-magic>=0.4.27,<0.5.0'],
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fave-extract = new_fave.extract:fave_extract']}
 
 setup_kwargs = {
     'name': 'new-fave',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'New Vowel Extraction Suite',
     'long_description': '# new-fave\n\n![PyPI](https://img.shields.io/pypi/v/new-fave.png) [![Python CI](https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/new-fave/graph/badge.svg?token=8JRGOB9NMN)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/new-fave) [![Maintainability](https://api.codeclimate.com/v1/badges/2f00920067765c0ad77f/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/new-fave/maintainability) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n## What is `new-fave`?\n\n`new-fave` is a tool for automating and optimizing vowel formant extraction. It is philosophically similar (and named after) [the FAVE-suite](https://github.com/JoFrhwld/FAVE). However, `new-fave` has been completely written from scratch, and has some key differences from the FAVE-suite.\n\n1. **`new-fave` does not include a forced-aligner.**\n    It can process alignments produced by fave-align, \n    but we would recommend using the Monteal Forced Aligner instead\n2. **`new-fave` does not require speaker demographics.**\n    You can optionally pass `fave-extract` a speaker\n    demographics file to be merged into your formant data,\n    but this does *not* influence how the data is processed\n    in any way. Besides including file name and speaker\n    number data, you can pass *any* demographic information\n    you would like.\n3. **`new-fave` does not assume North American English vowels**.\n    Your alignments can contain any set of vowels, in\n    any transcription system, as long as you can provide \n    a regular expression to identify them.\n4. **`new-fave` is customizable.**\n    With config files, you can customize vowel recoding,\n    labelset parsing, and point measurement heuristics.\n5. **`new-fave` is focused on formant tracks.**\n    You can still produce single point measurements \n    for vowels, but `new-fave` is built upon \n    the [FastTrack](https://fasttrackiverse.github.io/fasttrackpy/) method. By default, it will write \n    output files including point measurements, full\n    formant tracks, and Discrete Cosine Transform \n    coefficients.\n6. **`new-fave` is maintainable**. As time goes on, and the \n    code base needs updating, the organization and \n    infrastructure of `new-fave` should allow it to be\n    readilly updateable.\n\nYou can read more at [the `new-fave` documentation](https://forced-alignment-and-vowel-extraction.github.io/new-fave/).\n\n## Installation\n\nYou can install `new-fave` with `pip`.\n\n```bash\n# bash\npip install new-fave\n```\n\n## Usage\n\nTo use the default settings (which assume CMU \ndictionary transcriptions), you can use one of these \npatterns.\n\n### A single audio + textgrid pair\n\n```bash\n# bash\nfave-extract audio-textgrid speaker1.wav speaker1.TextGrid\n```\n\n### A directory of audio + textgrid pairs\n\n```bash\n# bash\nfave-extract corpus speakers/\n```\n\n### Multiple subdirectories of audio + textgrid pairs\n\n```bash\n# bash\nfave-extract subcorpora data/*\n```',
     'author': 'JoFrhwld',
     'author_email': 'jofrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://forced-alignment-and-vowel-extraction.github.io/new-fave/',
```

### Comparing `new_fave-0.1.2/PKG-INFO` & `new_fave-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: new-fave
-Version: 0.1.2
+Version: 0.1.3
 Summary: New Vowel Extraction Suite
 Home-page: https://forced-alignment-and-vowel-extraction.github.io/new-fave/
 License: GPLv3
 Author: JoFrhwld
 Author-email: jofrhwld@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.6,<0.7.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloup (>=3.0.5,<4.0.0)
-Requires-Dist: fasttrackpy (>=0.4.5,<0.5.0)
+Requires-Dist: fasttrackpy (>=0.4.6,<0.5.0)
 Requires-Dist: fave-measurement-point (==0.1.3)
 Requires-Dist: fave-recode (>=0.3.0,<0.4.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: polars (>=0.20.18,<0.21.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
+Requires-Dist: scipy (>=1.13.1,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: xlsx2csv (>=0.8.2,<0.9.0)
 Project-URL: Repository, https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave
 Description-Content-Type: text/markdown
 
 # new-fave
```


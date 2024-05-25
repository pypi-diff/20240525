# Comparing `tmp/chrfinder-0.0.1.tar.gz` & `tmp/chrfinder-0.0.2.tar.gz`

## Comparing `chrfinder-0.0.1.tar` & `chrfinder-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,70 @@
--rw-r--r--   0        0        0    22375 2020-02-02 00:00:00.000000 chrfinder-0.0.1/project_report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.1/pytest
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.1/python
--rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 chrfinder-0.0.1/report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.1/sphinx-build
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 chrfinder-0.0.1/tox.ini
--rw-r--r--   0        0        0  3450189 2020-02-02 00:00:00.000000 chrfinder-0.0.1/assets/Caf_Ace_Asp.gif
--rw-r--r--   0        0        0   415096 2020-02-02 00:00:00.000000 chrfinder-0.0.1/assets/Image_Chrfinder.webp
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 chrfinder-0.0.1/data/README.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/.buildinfo
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/genindex.html
--rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/index.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/objects.inv
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/py-modindex.html
--rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/search.html
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/searchindex.js
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_modules/index.html
--rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_modules/chrfinder/example_module.html
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_sources/index.md.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_sources/api/chrfinder.rst.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_sources/api/modules.rst.txt
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/basic.css
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/clipboard.min.js
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/copy-button.svg
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/copybutton.css
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/copybutton.js
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/debug.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/doctools.js
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/plus.png
--rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/searchtools.js
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/skeleton.css
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/sphinx_highlight.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/scripts/furo-extensions.js
--rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/scripts/furo.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0        0        0    28551 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/scripts/furo.js.map
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/styles/furo-extensions.css
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/styles/furo-extensions.css.map
--rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/styles/furo.css
--rw-r--r--   0        0        0    76416 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/_static/styles/furo.css.map
--rw-r--r--   0        0        0    18411 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/api/chrfinder.html
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/docs_out/api/modules.html
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/source/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/source/api/Chrfinder.rst
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chrfinder-0.0.1/docs/source/api/modules.rst
--rw-r--r--   0        0        0    18873 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/Properties.ipynb
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/classify.py
--rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/dsantos.ipynb
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/get_df_infos.py
--rw-r--r--   0        0        0     9350 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/pka_lookup.py
--rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 chrfinder-0.0.1/notebooks/search_pka.py
--rw-r--r--   0        0        0    14806 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/22.05 Anthony.ipynb
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/Chrfinder.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/classify.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/example_module.py
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/pka_lookup.py
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/pubchemprops.py
--rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/search_pka.py
--rw-r--r--   0        0        0    11058 2020-02-02 00:00:00.000000 chrfinder-0.0.1/src/Chrfinder/chroma/codecorrected.ipynb
--rw-r--r--   0        0        0    12476 2020-02-02 00:00:00.000000 chrfinder-0.0.1/tests/test_complete.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chrfinder-0.0.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 chrfinder-0.0.1/LICENSE
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 chrfinder-0.0.1/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 chrfinder-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 chrfinder-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.2/pytest
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.2/python
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.2/sphinx-build
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 chrfinder-0.0.2/tox.ini
+-rw-r--r--   0        0        0  3450189 2020-02-02 00:00:00.000000 chrfinder-0.0.2/assets/Caf_Ace_Asp.gif
+-rw-r--r--   0        0        0   415096 2020-02-02 00:00:00.000000 chrfinder-0.0.2/assets/Image_Chrfinder.webp
+-rw-r--r--   0        0        0   772009 2020-02-02 00:00:00.000000 chrfinder-0.0.2/assets/edited-error-molecule-not-added.gif
+-rw-r--r--   0        0        0   422911 2020-02-02 00:00:00.000000 chrfinder-0.0.2/assets/edited-hydrocarbure.gif
+-rw-r--r--   0        0        0   695205 2020-02-02 00:00:00.000000 chrfinder-0.0.2/assets/edited-limit.gif
+-rw-r--r--   0        0        0   606751 2020-02-02 00:00:00.000000 chrfinder-0.0.2/assets/edited-naphtalene-.gif
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 chrfinder-0.0.2/data/README.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/.buildinfo
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/genindex.html
+-rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/index.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/objects.inv
+-rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/py-modindex.html
+-rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/search.html
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/searchindex.js
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_modules/index.html
+-rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_modules/chrfinder/example_module.html
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_sources/index.md.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_sources/api/chrfinder.rst.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_sources/api/modules.rst.txt
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/basic.css
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/clipboard.min.js
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/copy-button.svg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/copybutton.css
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/copybutton.js
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/debug.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/doctools.js
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/plus.png
+-rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/searchtools.js
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/skeleton.css
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/scripts/furo-extensions.js
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/scripts/furo.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0        0        0    28551 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/scripts/furo.js.map
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/styles/furo-extensions.css
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/styles/furo-extensions.css.map
+-rw-r--r--   0        0        0    51030 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/styles/furo.css
+-rw-r--r--   0        0        0    76416 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/_static/styles/furo.css.map
+-rw-r--r--   0        0        0    18411 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/api/chrfinder.html
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/docs_out/api/modules.html
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/source/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/source/api/Chrfinder.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chrfinder-0.0.2/docs/source/api/modules.rst
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 chrfinder-0.0.2/notebooks/__init__.py
+-rw-r--r--   0        0        0    21339 2020-02-02 00:00:00.000000 chrfinder-0.0.2/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0    14106 2020-02-02 00:00:00.000000 chrfinder-0.0.2/src/Chrfinder/Chrfinder.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 chrfinder-0.0.2/src/Chrfinder/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 chrfinder-0.0.2/src/Chrfinder/classify.py
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 chrfinder-0.0.2/src/Chrfinder/pka_lookup.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 chrfinder-0.0.2/src/Chrfinder/pubchemprops.py
+-rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 chrfinder-0.0.2/src/Chrfinder/search_pka.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 chrfinder-0.0.2/tests/test_complete.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chrfinder-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 chrfinder-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 chrfinder-0.0.2/README.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 chrfinder-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 chrfinder-0.0.2/PKG-INFO
```

### Comparing `chrfinder-0.0.1/project_report.ipynb` & `chrfinder-0.0.2/notebooks/project_report.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659070569968811%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(4, \'<p style="text-align: justify;">Chromatography is a '*

 * *            'crucial analytical method in chemistry used for separating, identifying, and '*

 * *            'quantifying components in a mixture, and selecting the appropriate type of '*

 * *            'chromatography (e.g., gas chromatography, liquid chromatography, thin-layer '*

 * *            'chromatography) is essential for optimal results. This is why we decided to create a '*

 * *            'programming tool that allo […]*

```diff
@@ -7,15 +7,15 @@
                 "tags": []
             },
             "source": [
                 "<center><h1> Determination of the best chromatography type </h1></center>\n",
                 "    \n",
                 "## **Introduction**\n",
                 "\n",
-                "<p style=\"text-align: justify;\">Chromatography is a crucial analytical method in chemistry used for separating, identifying, and quantifying components in a mixture, and selecting the appropriate type of chromatography (e.g., gas chromatography, liquid chromatography, thin-layer chromatography) is essential for optimal results. This is why we decided to create a programming tool that allows to determine easily the chromatpgraphy type as well as the best eluaent needed to carry out the chromatography. \n",
+                "<p style=\"text-align: justify;\">Chromatography is a crucial analytical method in chemistry used for separating, identifying, and quantifying components in a mixture, and selecting the appropriate type of chromatography (e.g., gas chromatography, liquid chromatography, thin-layer chromatography) is essential for optimal results. This is why we decided to create a programming tool that allows to determine easily the chromatpgraphy type as well as the best eluent needed to carry out the chromatography. \n",
                 "This report details the development and execution of a programming project aimed at creating a tool to determine the most suitable chromatography technique for analyzing a given mixture of molecules. The project was conducted using python programming laguage. The different functions created to make this tool are listed in different notebooks in which each of them are commented. Moreover, the full project has been written on the source python file. \n",
                 "To carry out this project, a data base has been used in order to extract all the important information that were needed to establish the best chromatography type, then a function that takes into account all the different information has been created and finaly, a user interface has been created.\n",
                 "\n",
                 "## **Objectives**\n",
                 "\n",
                 "The primary objective of this project was to develop a program that:\n",
                 "\n",
@@ -40,21 +40,54 @@
             },
             "source": [
                 "## **Methodology**"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "b66a1e56-b03d-49c0-8b6c-617a9a99a2d4",
+            "metadata": {},
+            "source": [
+                "### 1. Graphical User Interface ###\n",
+                "\n",
+                "<p style=\"text-align: justify;\">A simple user interface was developed using Tkinter, allowing users to input the name of several molecules and obtain chromatography recommendations. The user can give molecule names that will be added to a listbox to keep in mind the different molecules in the mixture. The user then decides to determine the best chromatography type that will be indicated on the interface using the \"Determine Chromatography\" button. If an error occurs, an error message will be displayed using a message box on the user interface."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ba83b8eb-0577-4442-8682-cd0c5ef6aa9d",
+            "metadata": {},
+            "source": [
+                "<div style=\"display: flex; justify-content: center; align-items: center; padding: 20px;\">\n",
+                "    <div style=\"margin: 10px;\">\n",
+                "        <img src=\"../assets/edited-hydrocarbure.gif\" alt=\"hydrocarbures\" style=\"width: 400px; height: auto;\">\n",
+                "    </div>\n",
+                "    <div style=\"margin: 10px;\">\n",
+                "        <img src=\"../assets/edited-naphtalene-.gif\" alt=\"HPLCexample\" style=\"width: 400px; height: auto;\">\n",
+                "    </div>\n",
+                "</div>\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "bde3e92d-ce16-4a6e-89ff-ad6d621f70b8",
+            "metadata": {},
+            "source": [
+                "These two examples show how the results appear on the user ineterface when molecules are added. Above, two different mixtures are given, hence, two different results appear on the screen."
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "d8118e51-91b4-41d6-a303-a0eae89b3c70",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "\n",
-                "### 1. Data Collection and Preparation ###\n",
+                "### 2. Data Collection and Preparation ###\n",
                 "<p style=\"text-align: justify;\">\n",
                 "A dataset containing various molecular properties (e.g., molecular weight, polarity, solubility) and corresponding successful chromatography types was compiled.\n",
                 "Data preprocessing included handling missing values such as the pKa values. Relevant features such as molecular weight, polarity index, boiling point, pKa and solubility were selected and added to a data frame. \n",
                 "\n",
                 "First we import the function from the Chrfinder.py file."
             ]
         },
@@ -130,15 +163,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b7b676ba-e6c2-48df-8a86-ddccaed0aba3",
             "metadata": {},
             "source": [
-                "### 2. Determination of the chromatography type ###\n",
+                "### 3. Determination of the chromatography type ###\n",
                 "<p style=\"text-align: justify;\">\n",
                 "A function has been created to determine the most suiatble chromatography type based on the physical-chemical properties of the molecules saved on a data frame. To do this the following dependencies has tp be installed:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
@@ -235,41 +268,18 @@
                 "print(f\"Eluent nature: {eluent_nature}\")\n",
                 "if proposed_pH is not None:\n",
                 "    print(f\"Proposed pH for the eluent: {proposed_pH}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b66a1e56-b03d-49c0-8b6c-617a9a99a2d4",
-            "metadata": {},
-            "source": [
-                "### 3. Graphical User Interface ###\n",
-                "\n",
-                "<p style=\"text-align: justify;\">A simple user interface was developed using Tkinter, allowing users to input the name of several molecules and obtain chromatography recommendations. The user can give molecule names that will be added to a listbox to keep in mind the different molecules in the mixture. The user then decides to determine the best chromatography type that will be indicated on the interface using the \"Determine Chromatography\" button. If an error occurs, an error message will be displayed using a message box on the user interface.\n",
-                "\n",
-                "\n",
-                "PHOTOS DE L\"INTERFACE"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "ba83b8eb-0577-4442-8682-cd0c5ef6aa9d",
-            "metadata": {},
-            "source": [
-                "<div style=\"text-align: center;\">\n",
-                "  <img src=\"Caf_Ace_Asp.gif\" alt=\"interface_caf_ace_asp\" style=\"width: 300px; height: auto;\">\n",
-                "</div>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "e699e4ea-0fdf-41a6-8443-96c345fe6cf2",
             "metadata": {},
             "source": [
-                "### 4. Explanation of each part of get_df_properties(mixture) ###\n",
+                "### 4. Explanation of each part of get_df_properties(mixture) (c.f. Methodology.2.) ###\n",
                 "#### Getting 'CID', 'MolecularFormula', 'MolecularWeight', 'InChIKey', 'IUPACName', 'XLogP' using PubChem requests \n",
                 "(only missing Boiling Point and pka)\n",
                 "\n",
                 "This part of the code uses pubchempy and the code of *Maxim Shevelev* (pubchemprops.py) to easily find most of the properties. It takes into arguments a list of compound's names. It will return a dictionnary for each compound with the following properties: 'CID', 'MolecularFormula', 'MolecularWeight', 'InChIKey', 'IUPACName', 'XLogP'.\n",
                 "\n",
                 "The tkinter interface returns a list of compounds as string. The first part of the code iterates through the whole list (compound_list), and encodes every compound name (string) as URL. Then it will search for the properties on pubchem using pubchempy and add them into a dictionnary."
             ]
@@ -277,40 +287,21 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "954d86e1-1d89-477d-9feb-aed0a541dc01",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from Chrfinder.Chrfinder import get_df_properties\n",
+                "\n",
                 "compound_list = [\"caffeine\", \"Aspartame\", \"Acesulfame K\"]\n",
                 "#Delete '#' for a list with a wrong name\n",
                 "#compound_list = [\"Water\", \"Acetone\", \"Wrong name\"]\n",
                 "\n",
-                "\n",
-                "for compound_name in compound_list:\n",
-                "    compound_name_encoded = urllib.parse.quote(compound_name.strip())\n",
-                "    try: \n",
-                "        first_data = get_first_layer_props(compound_name_encoded, ['MolecularFormula', 'MolecularWeight', 'InChIKey', 'IUPACName', 'XLogP'])\n",
-                "        compound_info = {}\n",
-                "        for prop in ['CID', 'MolecularFormula', 'MolecularWeight', 'InChIKey', 'IUPACName', 'XLogP']:\n",
-                "            if prop == 'MolecularWeight':\n",
-                "                MolecularWeight_string = first_data.get(prop)\n",
-                "                if MolecularWeight_string is not None:\n",
-                "                    MolecularWeight_float = float(MolecularWeight_string)\n",
-                "                    compound_info[prop] = MolecularWeight_float\n",
-                "                else:\n",
-                "                    compound_info[prop] = None\n",
-                "            else:\n",
-                "                compound_info[prop] = first_data.get(prop)\n",
-                "    except urllib.error.HTTPError as e:\n",
-                "        if e.code == 404:\n",
-                "            print(f'{compound_name} not found on PubChem')\n",
-                "        else:\n",
-                "            print(f'An error occurred: {e}')\n",
-                "    print(compound_info)"
+                "get_df_properties(compound_list, verbose = True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b6138509-2218-4a73-93b0-72d6ff46dd99",
             "metadata": {},
             "source": [
@@ -324,28 +315,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "56af93f0-23b1-4c1d-87ea-0e14d7ada4fd",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from Chrfinder.Chrfinder import find_pka\n",
+                "\n",
                 "#inchikey of caffeine\n",
                 "inchikey_string = 'RYYVLZVUVIJVGH-UHFFFAOYSA-N'\n",
                 "\n",
-                "def find_pka(inchikey_string, verbose=False):\n",
-                "    text_pka = pka_lookup_pubchem(inchikey_string, \"inchikey\")\n",
-                "    if verbose:\n",
-                "        print(text_pka)\n",
-                "    if text_pka is not None and 'pKa' in text_pka:\n",
-                "            pKa_value = text_pka['pKa']\n",
-                "            return pKa_value\n",
-                "    else:\n",
-                "        return None\n",
-                "\n",
-                "find_pka(inchikey_string)"
+                "find_pka(inchikey_string, verbose=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e85c78ef-6b74-4c76-b52d-2c0ee46eb94b",
             "metadata": {},
             "source": [
@@ -359,46 +342,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e749f89d-f77b-4ed8-b250-1fbf4b7c3718",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def find_boiling_point(name):\n",
-                "    text_dict = get_second_layer_props(str(name), ['Boiling Point', 'Vapor Pressure'])\n",
-                "    Boiling_point_values = []\n",
-                "    pattern_celsius = r'([-+]?\\d*\\.\\d+|\\d+) \u00b0C'\n",
-                "    pattern_F = r'([-+]?\\d*\\.\\d+|\\d+) \u00b0F'\n",
-                "\n",
-                "    print(text_dict)\n",
-                "    \n",
-                "    for item in text_dict['Boiling Point']:\n",
-                "        if 'Value' in item and 'StringWithMarkup' in item['Value']:\n",
-                "            string_value = item['Value']['StringWithMarkup'][0]['String']\n",
-                "\n",
-                "            #Search for Celsius values, if found: adds to the list Boiling_point_values\n",
-                "            match_celsius = re.search(pattern_celsius, string_value)\n",
-                "            if match_celsius:\n",
-                "                celsius = float(match_celsius.group(1))\n",
-                "                Boiling_point_values.append(celsius)\n",
-                "\n",
-                "            #Search for Farenheit values, if found: converts farenheit to celsius before adding to the list Boiling_point_values\n",
-                "            match_F = re.search(pattern_F, string_value)\n",
-                "            if match_F:\n",
-                "                fahrenheit_temp = float(match_F.group(1))\n",
-                "                celsius_from_F = round(((fahrenheit_temp - 32) * (5/9)), 2)\n",
-                "                Boiling_point_values.append(celsius_from_F)\n",
-                "                \n",
-                "    if Boiling_point_values:\n",
-                "        Boiling_temp = round((sum(Boiling_point_values) / len(Boiling_point_values)), 2)\n",
-                "    else:\n",
-                "        Boiling_temp = None\n",
-                "    return Boiling_temp\n",
+                "from Chrfinder.Chrfinder import find_boiling_point\n",
                 "\n",
-                "find_boiling_point(\"Caffeine\")"
+                "mixture = \"Caffeine\"\n",
+                "find_boiling_point(mixture, verbose= True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "37f96a51-0e85-49f9-a2dc-db3f5efcba13",
             "metadata": {},
             "source": [
@@ -409,38 +364,65 @@
                 "**Feature Importance:** \n",
                 "<p style=\"text-align: justify;\">\n",
                 "Polarity index, molecular weight, and solubility were identified as the most influential features in determining the suitable chromatography type.\n",
                 "\n",
                 "**User Feedback:**\n",
                 "<p style=\"text-align: justify;\">\n",
                 "The interactive nature of the user interface allowed for seamless user input and clear presentation of results, enhancing the user experience.\n",
+                "    \n",
+                "When error occurs, messages appear to inform the user of the encountered error. An example of this feature is shown bellow:\n",
+                "\n",
+                "<div style=\"text-align: center; padding: 20px;\">\n",
+                "    <img src=\"../assets/edited-error-molecule-not-added.gif\" alt=\"errornomolecule\" style=\"width: 400px; height: auto;\">\n",
+                "</div>"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "d5e4d262-3ffc-4f86-acfd-b2c31a154928",
+            "metadata": {},
+            "source": [
+                "  \n",
                 "\n",
                 "## **Limits** ##\n",
                 "\n",
+                "The example bellow shows the limit of the program. Indeed, the suitable chromatography given by the interface is not correct, this is due to the fact that the boiling point is not given in pubchem which generates an error in the determination of the chromatography. Hence, a lack of data is limiting our project.\n",
+                "\n",
+                "<div style=\"text-align: center; padding: 20px;\">\n",
+                "    <img src=\"../assets/edited-limit.gif\" alt=\"limit\" style=\"width: 400px; height: auto;\">\n",
+                "</div>\n",
+                "\n",
                 "##### Take into account: \n",
                 "- It takes into account **wrong names** and **compounds with no pages on PubChem**: it returns \"The_compound_name\" not found on PubChem'\n",
                 "- The code works even with missing boiling point or pka in dataframe.\n",
                 "\n",
                 "##### To improve: \n",
                 "- **Build a database**: mostly with thermostability for better choice of chromatography;\n",
                 "- Taking into account **multiple pKa** values for polyacids for exemple;\n",
                 "- Optimize the research: search only one time the **same name**, don't search for **one name**;\n",
                 "- **Easier usage and options** of functionnalities to search physicalchemical properties in a dataframe;\n",
-                "\n",
+                "\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "5945292b-5b88-4879-9eb5-5eeec0413f89",
+            "metadata": {},
+            "source": [
                 "## **Encountered difficulties** ##\n",
                 "\n",
                 "A lot of challenges were faced to make request to pubchem:\n",
                 "- Handling of **errors concerning pubchem**, no page found, wrong compound name, etc\n",
                 "  \n",
                 "- How to **extract string using regex**, used for pka, boiling temperature (\u00b0C) and (\u00b0F).\n",
                 "  \n",
                 "- Handling of **pka errors wrongly written in Pubchem** (either value in value, either input in the key of the dictionnary) <br>\n",
                 "    {\"pka = 20.0\", } instead of {'pKa': '14'}\n",
                 "  \n",
-                "- Tests of pubchem request, ///\n",
+                "- Tests of pubchem request,\n",
                 "   \n",
                 "## **Conclusion** ##\n",
                 "<p style=\"text-align: justify;\">\n",
                 "The project successfully developed a robust program for recommending chromatography techniques based on molecular composition. The use of a user interface facilitated an efficient and interactive development process, enabling easy experimentation and visualization. This tool has significant potential applications in chemical analysis, improving efficiency and accuracy in selecting the appropriate analytical methods.\n",
                 "\n",
                 "## **Future Work** ##\n",
                 "\n",
@@ -450,14 +432,22 @@
                 "- Improve the code to have a more efficient way to take the information on the molecules contained in the mixture to have the results more rapidly.\n",
                 "- Integrating the program with real-time data acquisition systems for automated analysis.\n",
                 "- Enhancing the user interface with more sophisticated visualization tools and user-friendly features.\n",
                 "- By continuing to refine and expand this tool, it can become an invaluable resource for chemists and researchers in analytical laboratories.\n",
                 "\n",
                 "This report provides an overview of the programming project conducted using Python, detailing the development process, results, and future directions for the chromatography recommendation program.\n"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "99622666-191d-489e-9281-6058f7d85a4c",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `chrfinder-0.0.1/tox.ini` & `chrfinder-0.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/assets/Caf_Ace_Asp.gif` & `chrfinder-0.0.2/assets/Caf_Ace_Asp.gif`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/assets/Image_Chrfinder.webp` & `chrfinder-0.0.2/assets/Image_Chrfinder.webp`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/genindex.html` & `chrfinder-0.0.2/docs/docs_out/genindex.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/index.html` & `chrfinder-0.0.2/docs/docs_out/index.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/py-modindex.html` & `chrfinder-0.0.2/docs/docs_out/py-modindex.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/search.html` & `chrfinder-0.0.2/docs/docs_out/search.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/searchindex.js` & `chrfinder-0.0.2/docs/docs_out/searchindex.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_modules/index.html` & `chrfinder-0.0.2/docs/docs_out/_modules/index.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_modules/chrfinder/example_module.html` & `chrfinder-0.0.2/docs/docs_out/_modules/chrfinder/example_module.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/basic.css` & `chrfinder-0.0.2/docs/docs_out/_static/basic.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/clipboard.min.js` & `chrfinder-0.0.2/docs/docs_out/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/copybutton.css` & `chrfinder-0.0.2/docs/docs_out/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/copybutton.js` & `chrfinder-0.0.2/docs/docs_out/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/copybutton_funcs.js` & `chrfinder-0.0.2/docs/docs_out/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/debug.css` & `chrfinder-0.0.2/docs/docs_out/_static/debug.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/doctools.js` & `chrfinder-0.0.2/docs/docs_out/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/language_data.js` & `chrfinder-0.0.2/docs/docs_out/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/pygments.css` & `chrfinder-0.0.2/docs/docs_out/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/searchtools.js` & `chrfinder-0.0.2/docs/docs_out/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/skeleton.css` & `chrfinder-0.0.2/docs/docs_out/_static/skeleton.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/sphinx_highlight.js` & `chrfinder-0.0.2/docs/docs_out/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/scripts/furo.js` & `chrfinder-0.0.2/docs/docs_out/_static/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/scripts/furo.js.map` & `chrfinder-0.0.2/docs/docs_out/_static/scripts/furo.js.map`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/styles/furo-extensions.css` & `chrfinder-0.0.2/docs/docs_out/_static/styles/furo-extensions.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/styles/furo-extensions.css.map` & `chrfinder-0.0.2/docs/docs_out/_static/styles/furo-extensions.css.map`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/styles/furo.css` & `chrfinder-0.0.2/docs/docs_out/_static/styles/furo.css`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/_static/styles/furo.css.map` & `chrfinder-0.0.2/docs/docs_out/_static/styles/furo.css.map`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/api/chrfinder.html` & `chrfinder-0.0.2/docs/docs_out/api/chrfinder.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/docs_out/api/modules.html` & `chrfinder-0.0.2/docs/docs_out/api/modules.html`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/docs/source/conf.py` & `chrfinder-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/notebooks/classify.py` & `chrfinder-0.0.2/src/Chrfinder/classify.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/notebooks/pka_lookup.py` & `chrfinder-0.0.2/src/Chrfinder/pka_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 Author: Khoi Van 2020
 
 This script takes a CAS number and look up its pKa (dissociation constant) 
 from Pubchem and return it if found; return None, otherwise
 
 Change notes:
 - 2020-02-14:
-  - Instead of just returning the result, return the result combo as json dict
+- Instead of just returning the result, return the result combo as json dict
 
 """
 
 import re
 import sys
 import traceback
 import xml.etree.ElementTree as ET
 from typing import Optional
 
 import pandas as pd
 import pubchempy as pcp  # https://pubchempy.readthedocs.io/en/latest/guide/gettingstarted.html
 import requests
 
-from classify import classify
+from .classify import classify
 
 
 debug = False
 
 
 def pka_lookup_pubchem(identifier, namespace=None, domain='compound') -> Optional[str]:
     global debug
```

### Comparing `chrfinder-0.0.1/notebooks/search_pka.py` & `chrfinder-0.0.2/src/Chrfinder/search_pka.py`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/src/Chrfinder/Chrfinder.py` & `chrfinder-0.0.2/src/Chrfinder/Chrfinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Returns:
         None
     """
     element = mixture_entry.get()
     mixture.append(element)
     mixture_listbox.insert(tk.END, element.strip())
 
+
 def add_entry_widget(root):
     """
     Add entry widgets to the root window.
 
     Args:
         root (tk.Tk): The root window of the Tkinter application.
 
@@ -182,15 +183,16 @@
     for prop in compound_properties:
         if isinstance(prop, dict):
             valid_properties.append(prop)
     df = pd.DataFrame(valid_properties)
     # Set the property names from the first dictionary as column headers
     if len(valid_properties) > 0:
         df = df.reindex(columns=valid_properties[0].keys())
-    print(df)
+    if verbose:
+        print(df)
     return(df)
 
 def det_chromato(df):
     """
     Determine the type of chromatography based on compound properties.
 
     Conditions: Boiling temperature, molar mass, pka, LogP. To improve: add Thermal stability.
```

### Comparing `chrfinder-0.0.1/src/Chrfinder/__init__.py` & `chrfinder-0.0.2/src/Chrfinder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#"""The package find the best chromatography based on properties of the mixture."""
-
-#from __future__ import annotations
+"""The package finds the best chromatography based on properties of the mixture."""
 
 __version__ = "0.0.1"
 
 from .pubchemprops import get_cid_by_name, get_first_layer_props, get_second_layer_props
 from .pka_lookup import pka_lookup_pubchem
 from .Chrfinder import add_molecule, find_pka, find_boiling_point, get_df_properties, det_chromato, update_results, main
```

### Comparing `chrfinder-0.0.1/src/Chrfinder/pubchemprops.py` & `chrfinder-0.0.2/src/Chrfinder/pubchemprops.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,53 +9,66 @@
 """
 
 import urllib.request, json
 
 
 def pubchem_parsing(url):
     """
-        Get the link to PubChem API, parse it for JSON and then translate that
-        to Python dictionary;
-        This is just to follow the DRY principle
+    Parses the response from a given URL to PubChem API and returns the result as a Python dictionary.
+
+    Args:
+        url (str): The URL to query the PubChem API.
+
+    Returns:
+        dict: A Python dictionary containing the parsed JSON response from the PubChem API.
     """
     req = urllib.request.Request(url)
     res = urllib.request.urlopen(req).read()
     fin = json.loads(res.decode())
     return fin
 
 
 def get_cid_by_name(compound_name):
     """
-        1. Accepts the compound name
-        2. Searches PubChem by this name
-        3. Returns the compound's PubChem CID
-    """
+    Fetches the PubChem Compound Identifier (CID) for a given compound name.
+
+    Args:
+        compound_name (str): The name of the compound to search for in PubChem.
 
+    Returns:
+        int: The PubChem CID corresponding to the provided compound name.
+
+    Raises:
+        KeyError: If the PubChem API response does not contain the expected structure.
+        Exception: If there is an error while communicating with PubChem or parsing the response.
+    """
+    encoded_name = urllib.parse.quote(compound_name)
+    
     # Construct the link to PubChem's PUG REST API
-    pubchem_record_link = "https://pubchem.ncbi.nlm.nih.gov/rest/pug/compound/"
-    pubchem_record_link += "name/%s/record/JSON" % compound_name
+    pubchem_record_link = f"https://pubchem.ncbi.nlm.nih.gov/rest/pug/compound/name/{encoded_name}/record/JSON"
 
     # Parse the JSON received from PubChem to Python Dictionary
     general_info = pubchem_parsing(pubchem_record_link)
 
     # Get the CID
     compound_cid = general_info['PC_Compounds'][0]['id']['id']['cid']
 
     return compound_cid
 
 
 def get_first_layer_props(compound_name, first_layer_props):
     """
-        1. Accepts the compound name as a String and the required first layer
-           props as a List
-        2. Finds its CID
-        3. Creates a link to PubChem PUG REST API to get the required properties
-        4. Returns a dictionary with the required props
-        NOTE: <First layer props> means that these properties can be directly
-              accessed via the convenient PubChem PUG REST API
+    Retrieves the properties directly accessible via the PubChem PUG REST API for a given compound.
+
+    Args:
+        compound_name (str): The name of the compound to retrieve properties for.
+        first_layer_props (list of str): A list of strings representing the required first layer properties.
+
+    Returns:
+        dict: A dictionary containing the requested first layer properties for the compound.
     """
     compound_cid = get_cid_by_name(compound_name)
 
     # Make a string out of the required first layer props list
     req_props_string = ','.join(first_layer_props)
 
     pubchem_pug_rest_api_link = "https://pubchem.ncbi.nlm.nih.gov/rest/pug/"
@@ -65,22 +78,26 @@
     first_layer_props_data = pubchem_parsing(pubchem_pug_rest_api_link)['PropertyTable']['Properties'][0]
 
     return first_layer_props_data
 
 
 def get_second_layer_props(compound_name, required_properties):
     """
-        1. Accepts the compound name
-        2. Gets the CID for this compound
-        3. Searches PubChem for data for the specified CID
-        4. Cycles through the fetched data to select required fields
-        5. Returns a dictionary with specified properties of specified compound
+    Fetches the compound's CID, searches PubChem for data for the specified CID, cycles through the fetched data to select the required fields, and returns a dictionary with the specified properties for a given compound.
 
-        NOTE: <Second layer properties> means that these properties can not be
-              accessed directly via the PubChem PUG REST API.
+    Args:
+        compound_name (str): The name of the compound to retrieve properties for.
+        required_properties (list of str): A list of strings representing the required properties.
+
+    Returns:
+        dict: A dictionary containing the specified properties of the given compound.
+
+    Raises:
+        KeyError: If the PubChem API response does not contain the expected structure.
+        Exception: If there is an error while communicating with PubChem or parsing the response.
     """
     # Get the compound's PubChem CID
     compound_cid = get_cid_by_name(compound_name)
 
     # Contsruct the link
     pubchem_all_data_link = "https://pubchem.ncbi.nlm.nih.gov/rest/pug_view/"
     pubchem_all_data_link += "data/compound/%s/JSON" % compound_cid
```

### Comparing `chrfinder-0.0.1/.gitignore` & `chrfinder-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/LICENSE` & `chrfinder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chrfinder-0.0.1/README.md` & `chrfinder-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,80 +2,75 @@
   <img src="assets/Image_Chrfinder.webp" alt="Project Logo" width="650"/>
 </p>
 
 # Chrfinder
 
 ## <ins>Project overview</ins>
 
-[![PyPI version](http://img.shields.io/pypi/v/PubChemPy.svg?style=flat)](https://pypi.python.org/pypi/Chrfinder)
-
-[![License](http://img.shields.io/pypi/l/PubChemPy.svg?style=flat)](https://github.com/Averhv/Chrfinder/blob/master/LICENSE)
-
-
-
+<h1 align="center">
+    
+[![PyPI version](https://img.shields.io/pypi/v/Chrfinder?style=plastic&color=blue)](https://pypi.python.org/pypi/Chrfinder) [![License](https://img.shields.io/github/license/Averhv/Chrfinder?style=plastic&color=Orange)](https://github.com/Averhv/Chrfinder/blob/master/LICENSE) <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/Chrfinder?style=plastic" />
+</h1>
 
 Welcome to **Chrfinder**! This project **automates the selection of the most suitable chromatography** technique . By simply providing the **names** of the molecules in the mixture, the code retrieves their physicochemical properties from **PubChem** (web source) and determines the optimal chromatography method based on these properties. It also gives the optimal conditions.
 
 ## ✅ <ins>Benefits</ins>
 
 - **🚀 Efficiency**: Automates the property retrieval and decision-making process, saving time and reducing manual effort.
 - **🎯 Accuracy**: Utilizes precise physicochemical data to ensure the most suitable chromatography technique is chosen.
 - **🌐 Versatility**: Supports a wide range of organic compounds and chromatography methods (PubChem database).
 
 
 ## ⚙ <ins>Installation</ins>
 
 Create a new environment, you may also give the environment a different name. 
 
-```
+```bash
 conda create -n chrfinder python=3.10 
 ```
 
-```
+```bash
 conda activate chrfinder
-pip install .
+pip install Chrfinder
 ```
 
-If you need jupyter lab, install it 
+## 🛠️ <ins>Installation for Development</ins>
 
-```
+To get started with Chrfinder, you can follow these steps:
+```bash
+git clone https://github.com/Averhv/Chrfinder.git
+cd Chrfinder
+pip install .
 pip install jupyterlab
+jupyter lab
 ```
-
-## 🛠️ <ins>Development installation</ins>
-
-Initialize Git (only for the first time). 
-
-Note: You should have create an empty repository on `https://github.com:Averhv/Chrfinder`.
-
-```
-git init
-git add * 
-git add .*
-git commit -m "Initial commit" 
-git branch -M main
-git remote add origin git@github.com:Averhv/Chrfinder.git 
-git push -u origin main
-```
-
-Then add and commit changes as usual. 
-
-To install the package, run
-
-```
+#### Optional: Installing for Development and Testing
+If you want to contribute to Chrfinder or run the tests and get coverage, you can install the package in editable mode along with the necessary dependencies for testing and documentation:
+```bash
+git clone https://github.com/Averhv/Chrfinder.git
+cd Chrfinder
 pip install -e ".[test,doc]"
+pip install jupyterlab
+jupyter lab
 ```
 
-#### Run tests and get coverage
-
-```
+Then you need to run the tests as follow in your terminal:
+```bash
 pip install tox
 tox
 ```
-
+One can also run the following to get better **readability**:
+- runs tests for the Chrfinder.py file
+- measures code coverage
+- generates coverage reports in both XML and terminal formats
+- provides verbose output during test execution.
+```bash
+pytest --cov=src/Chrfinder.py --cov-report xml:.tox/coverage.xml --cov-report term -vv
+```
+Test result: 15 passed in ~20s
 ## 📒 <ins>Features</ins>
 
 ```python
 from chrfinder import main
 
 # Running the whole file ask for molecules through Tkinter and returns the best chromatography
 main()
```

### Comparing `chrfinder-0.0.1/pyproject.toml` & `chrfinder-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [build-system] 
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Chrfinder"
+version = "0.0.2"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 description = "The package find the best chromatography based on properties of the mixture"
 dependencies = [
     "pandas",
     "pubchempy",
@@ -25,15 +26,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dynamic = ["version"]
+
 
 [project.urls]
 source = "https://github.com/Averhv/Chrfinder"
 tracker = "https://github.com/Averhv/Chrfinder/issues"
 
 
 [project.optional-dependencies]
@@ -56,18 +57,44 @@
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.coverage.run]
-omit = [
-    '__init__.py'
-]
+source = ["src/Chrfinder"]
+command_line = "-m pytest tests/test_complete.py"
+branch = true
 
 [tool.coverage.report]
+# Regexes for lines to exclude from consideration
 exclude_also = [
+    # Don't complain about missing debug-only code:
+    "def __repr__",
+    "if self\\.debug",
+
+    # Don't complain if tests don't hit defensive assertion code:
+    "raise AssertionError",
+    "raise NotImplementedError",
+
+    # Don't complain if non-runnable code isn't run:
+    "if 0:",
     "if __name__ == .__main__.:",
-]
+
+    # Don't complain about abstract methods, they aren't run:
+    "@(abc\\.)?abstractmethod",
+    ]
+
+ignore_errors = true
+
+[tool.coverage.html]
+directory = "coverage_html_report"
+
+[tool.coverage.paths]
+source = [
+    "src/",
+    "/jenkins/build/*/src",
+    "c:\\Averhv\\src",
+    ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/Chrfinder"]
+packages = ["src/Chrfinder"]
```

### Comparing `chrfinder-0.0.1/PKG-INFO` & `chrfinder-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Chrfinder
-Version: 0.0.1
+Version: 0.0.2
 Summary: The package find the best chromatography based on properties of the mixture
 Project-URL: source, https://github.com/Averhv/Chrfinder
 Project-URL: tracker, https://github.com/Averhv/Chrfinder/issues
 Author-email: Anthony Verhoeven <anthony.verhoeven@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Diogo Santos Martins <diogo.santosmartins@epfl.ch>
@@ -59,80 +59,75 @@
   <img src="assets/Image_Chrfinder.webp" alt="Project Logo" width="650"/>
 </p>
 
 # Chrfinder
 
 ## <ins>Project overview</ins>
 
-[![PyPI version](http://img.shields.io/pypi/v/PubChemPy.svg?style=flat)](https://pypi.python.org/pypi/Chrfinder)
-
-[![License](http://img.shields.io/pypi/l/PubChemPy.svg?style=flat)](https://github.com/Averhv/Chrfinder/blob/master/LICENSE)
-
-
-
+<h1 align="center">
+    
+[![PyPI version](https://img.shields.io/pypi/v/Chrfinder?style=plastic&color=blue)](https://pypi.python.org/pypi/Chrfinder) [![License](https://img.shields.io/github/license/Averhv/Chrfinder?style=plastic&color=Orange)](https://github.com/Averhv/Chrfinder/blob/master/LICENSE) <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/Chrfinder?style=plastic" />
+</h1>
 
 Welcome to **Chrfinder**! This project **automates the selection of the most suitable chromatography** technique . By simply providing the **names** of the molecules in the mixture, the code retrieves their physicochemical properties from **PubChem** (web source) and determines the optimal chromatography method based on these properties. It also gives the optimal conditions.
 
 ## ✅ <ins>Benefits</ins>
 
 - **🚀 Efficiency**: Automates the property retrieval and decision-making process, saving time and reducing manual effort.
 - **🎯 Accuracy**: Utilizes precise physicochemical data to ensure the most suitable chromatography technique is chosen.
 - **🌐 Versatility**: Supports a wide range of organic compounds and chromatography methods (PubChem database).
 
 
 ## ⚙ <ins>Installation</ins>
 
 Create a new environment, you may also give the environment a different name. 
 
-```
+```bash
 conda create -n chrfinder python=3.10 
 ```
 
-```
+```bash
 conda activate chrfinder
-pip install .
+pip install Chrfinder
 ```
 
-If you need jupyter lab, install it 
+## 🛠️ <ins>Installation for Development</ins>
 
-```
+To get started with Chrfinder, you can follow these steps:
+```bash
+git clone https://github.com/Averhv/Chrfinder.git
+cd Chrfinder
+pip install .
 pip install jupyterlab
+jupyter lab
 ```
-
-## 🛠️ <ins>Development installation</ins>
-
-Initialize Git (only for the first time). 
-
-Note: You should have create an empty repository on `https://github.com:Averhv/Chrfinder`.
-
-```
-git init
-git add * 
-git add .*
-git commit -m "Initial commit" 
-git branch -M main
-git remote add origin git@github.com:Averhv/Chrfinder.git 
-git push -u origin main
-```
-
-Then add and commit changes as usual. 
-
-To install the package, run
-
-```
+#### Optional: Installing for Development and Testing
+If you want to contribute to Chrfinder or run the tests and get coverage, you can install the package in editable mode along with the necessary dependencies for testing and documentation:
+```bash
+git clone https://github.com/Averhv/Chrfinder.git
+cd Chrfinder
 pip install -e ".[test,doc]"
+pip install jupyterlab
+jupyter lab
 ```
 
-#### Run tests and get coverage
-
-```
+Then you need to run the tests as follow in your terminal:
+```bash
 pip install tox
 tox
 ```
-
+One can also run the following to get better **readability**:
+- runs tests for the Chrfinder.py file
+- measures code coverage
+- generates coverage reports in both XML and terminal formats
+- provides verbose output during test execution.
+```bash
+pytest --cov=src/Chrfinder.py --cov-report xml:.tox/coverage.xml --cov-report term -vv
+```
+Test result: 15 passed in ~20s
 ## 📒 <ins>Features</ins>
 
 ```python
 from chrfinder import main
 
 # Running the whole file ask for molecules through Tkinter and returns the best chromatography
 main()
```


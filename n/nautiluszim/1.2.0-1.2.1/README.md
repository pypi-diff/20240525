# Comparing `tmp/nautiluszim-1.2.0.tar.gz` & `tmp/nautiluszim-1.2.1.tar.gz`

## Comparing `nautiluszim-1.2.0.tar` & `nautiluszim-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/Dockerfile
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/openzim.toml
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/tasks.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/VERSION
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/__init__.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/constants.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/entrypoint.py
--rw-r--r--   0        0        0    20684 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/scraper.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/locale/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/database.js
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/display_rows.handlebars
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/favicon.png
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/home.html
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/info-circle-solid.svg
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/init.js
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/main-logo.png
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/media_player.handlebars
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/modal_empty_body.handlebars
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/modal_title.handlebars
--rw-r--r--   0        0        0    19903 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/nautilus.js
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/styles.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/tests/test_stub.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/LICENSE
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/README.md
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/Dockerfile
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/openzim.toml
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/tasks.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/VERSION
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/constants.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/entrypoint.py
+-rw-r--r--   0        0        0    20684 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/scraper.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/locale/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/database.js
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/display_rows.handlebars
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/favicon.png
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/home.html
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/info-circle-solid.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/init.js
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/main-logo.png
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/media_player.handlebars
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/modal_empty_body.handlebars
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/modal_title.handlebars
+-rw-r--r--   0        0        0    19903 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/nautilus.js
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/src/nautiluszim/templates/styles.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/tests/test_stub.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/README.md
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 nautiluszim-1.2.1/PKG-INFO
```

### Comparing `nautiluszim-1.2.0/.pre-commit-config.yaml` & `nautiluszim-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/CHANGELOG.md` & `nautiluszim-1.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.1]
+
+### Fixed
+
+- Missing libmagic in docker image
+
 ## [1.2.0]
 
 ### Added
 
 - Add urls support to collections. (#59)
 - Add archiveless collection.json support. (#60)
```

### Comparing `nautiluszim-1.2.0/Dockerfile` & `nautiluszim-1.2.1/Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LABEL org.opencontainers.image.source https://github.com/openzim/nautilus
 
 # Install necessary packages
 RUN apt-get update \
  && apt-get install -y --no-install-recommends \
       # locales required if tool has any i18n support
       locales-all wget \
+      libmagic1 \
  && rm -rf /var/lib/apt/lists/* \
  && python -m pip install --no-cache-dir -U \
       pip \
 && wget -nv -L https://nodejs.org/dist/v12.16.3/node-v12.16.3-linux-x64.tar.gz \
 && tar -C /usr/local --strip-components 1 -xf node-v12.16.3-linux-x64.tar.gz \
 && rm node-v12.16.3-linux-x64.tar.gz \
 && npm install -g handlebars
```

### Comparing `nautiluszim-1.2.0/openzim.toml` & `nautiluszim-1.2.1/openzim.toml`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/tasks.py` & `nautiluszim-1.2.1/tasks.py`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/constants.py` & `nautiluszim-1.2.1/src/nautiluszim/constants.py`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/entrypoint.py` & `nautiluszim-1.2.1/src/nautiluszim/entrypoint.py`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/scraper.py` & `nautiluszim-1.2.1/src/nautiluszim/scraper.py`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/locale/fr/LC_MESSAGES/messages.po` & `nautiluszim-1.2.1/src/nautiluszim/locale/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/favicon.png` & `nautiluszim-1.2.1/src/nautiluszim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/home.html` & `nautiluszim-1.2.1/src/nautiluszim/templates/home.html`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/info-circle-solid.svg` & `nautiluszim-1.2.1/src/nautiluszim/templates/info-circle-solid.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/init.js` & `nautiluszim-1.2.1/src/nautiluszim/templates/init.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/main-logo.png` & `nautiluszim-1.2.1/src/nautiluszim/templates/main-logo.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/nautilus.js` & `nautiluszim-1.2.1/src/nautiluszim/templates/nautilus.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/src/nautiluszim/templates/styles.css` & `nautiluszim-1.2.1/src/nautiluszim/templates/styles.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/.gitignore` & `nautiluszim-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/LICENSE` & `nautiluszim-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/README.md` & `nautiluszim-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/pyproject.toml` & `nautiluszim-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.2.0/PKG-INFO` & `nautiluszim-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautiluszim
-Version: 1.2.0
+Version: 1.2.1
 Summary: turns a collection of documents into a browsable ZIM file
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Project-URL: Homepage, https://github.com/openzim/nautilus
 Author-email: openZIM <dev@openzim.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offline,openzim,zim
```

